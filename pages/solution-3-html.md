# Interactivity Question - HTML + CSS Solution

```jsx
export default function CheckboxComponent() {
  return (
    <>
      <input type="checkbox" />
      <span class="not-checked">I'm not checked</span>
      <span class="checked">I'm checked!</span>
    </>
  );
}
```

```css
span {
  display: none;
}

input:not(:checked) ~ .not-checked {
  display: block;
}

input:checked ~ .checked {
  display: block;
}
```
