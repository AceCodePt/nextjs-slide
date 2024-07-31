# Search Question - Server Side Solution

```jsx{all|5-9|all}
import { redirect } from 'next/navigation'

export default function SearchPage({ searchParams }) {
  const { q } = searchParams;
  function handleSearch(formData) {
      'use server';
      const query = formData.get('q');
      redirect(`/search?q=${query}`);
  }
  return (
    <>
      <form action={handleSearch}>
        <input type="text" name="q" placeholder="Search..." required />
        <button type="submit">Submit</button>
      </form>
      {q && <>Some Results...</>}
    </>
  );
}
```
