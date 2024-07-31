# Interactivity Question Advanced - Solution

my-script.js

```js
const btn = document.querySelector("button");
btn.addEventListener("click", async () => {
  const response = await fetch("/api/pressed");
  if (response.ok) {
    const text = await response.text();
    btn.innerHTML = text;
  }
});
```

