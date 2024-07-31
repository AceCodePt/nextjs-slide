# Buttons Question - CSS Solution

```jsx
export default function ButtonsGroup() {
  return (
    <div class="button-container">
      <button>1</button>
      <button>2</button>
      <button>3</button>
      <button>4</button>
      <button>5</button>
    </div>
  );
}
```

```css
.button-container:has(button:hover) button:not(:hover) {
  scale: 0.5;
}
```
