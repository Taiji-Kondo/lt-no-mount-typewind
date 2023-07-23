---
layout: default
---

# Modifiers

- `hover`、`before`等の疑似要素、擬似クラス
- `tw.hover(...)`という関数実行で指定

```tsx
const Normal = () => {
  return (
    <button
      className={tw.bg_blue_500.hover(tw.bg_blue_600).first_letter(tw.text_red_500.font_bold)}
    >
      Click Me
    </button>
  );
};
```