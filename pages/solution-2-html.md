# Search Question - HTML Solution

```jsx
export default function SearchPage({ searchParams }) {
  const { q } = searchParams;
  return (
    <>
      <form>
        <input type="text" name="q" placeholder="Search..." required />
        <button type="submit">Submit</button>
      </form>
      {q && <>Some Results...</>}
    </>
  );
}
```
