# Interactivity Question Advanced - Solution

app/layout.tsx

```tsx
import Script from "next/script";

export default function RootLayout({
  children,
}: {
  children: React.ReactNode;
}) {
  return (
    <html lang="en">
      <body>
        {children}
        <Script src="./my-script.js" strategy="beforeInteractive" />
      </body>
    </html>
  );
}
```
