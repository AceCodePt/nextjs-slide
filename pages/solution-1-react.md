# Buttons Question - React Solution

```tsx{all|5|11-12|13-18|all}
"use client";
import { useState } from "react";

export default function ButtonsGroup() {
  const [hoverIndex, setHoverIndex] = useState(null);

  return (
      {[...Array(5)].map((_, index) => (
        <button
          key={index}
          onMouseEnter={() => setHoverIndex(index)}
          onMouseLeave={() => setHoverIndex(null)}
          style={{
            scale:
              hoverIndex !== null && hoverIndex !== index
                ? 0.5
                : 1
          }}
        >
          Button {index + 1}
        </button>
      ))}
  );
}
```
