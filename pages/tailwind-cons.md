---
layout: bullets
---

# デメリット

- Tailwindのクラス名を覚える必要がある
- class名の記述が長くなりがちで可読性が落ちる

```tsx
const Button = () => {
  return (
    <button className="bg-blue-500 text-white text-lg font-bold py-2 px-4 rounded shadow-sm hover:bg-blue-700">
      Click me
    </button>
  );
};
```