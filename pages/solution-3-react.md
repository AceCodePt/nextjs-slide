# Interactivity Question - Client Side Solution

```tsx
"use client";
import { useState } from "react";

export default function CheckboxComponent() {
  const [checked, setChecked] = useState(false);

  return (
    <>
      <input type="checkbox" checked={checked} />
      {checked ? "I'm checked!" : "I'm not checked"}
    </>
  );
}
```
