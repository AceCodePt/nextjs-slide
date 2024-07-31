# Search Question - Client Side Solution

```tsx{all|6-8,18|10-13|21|all}
"use client";
import { useRouter } from "next/router";
import { useState } from "react";

export default function SearchPage() {
  const router = useRouter();
  const { q } = router.query;
  const [query, setQuery] = useState(q || "");

  const handleSubmit = (e) => {
    e.preventDefault();
    router.push(`/search?q=${query}`);
  };

  return (
    <>
      <form onSubmit={handleSubmit}>
        <input type="text" value={query} onChange={(e) => setQuery(e.target.value)} />
        <button type="submit">Submit</button>
      </form>
      {query && <>Some Results...</>}
    </>
  );
}
```
