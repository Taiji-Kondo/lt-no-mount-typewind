---
layout: default
---

# Important

- `important`をつけたい場合は`tw.important()`として引数に当てたいクラスを渡す

```tsx
const Normal = () => {
  return (
    <button
      className={tw.important(tw.text_red_500).hover(tw.important(tw.text_red_600))}
    >
      Click Me
    </button>
  );
};
```