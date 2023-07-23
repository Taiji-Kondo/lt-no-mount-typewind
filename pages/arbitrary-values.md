---
layout: default
---

# Arbitrary Values

- `text-[20px]`のようなTailwindで定義されていない値を使いたい場合の記述
- `tw.text_[20px]`のように書ける

```tsx
const Normal = () => {
  return (
    <button className={tw.text_['20px'].py_3.px_4.bg_blue_500}>Click Me</button>
  );
};
```