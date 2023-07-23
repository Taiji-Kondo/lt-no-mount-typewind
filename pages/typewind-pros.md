---
layout: default
---

# Typewindを使うと何が嬉しいか

<ul>
    <li>Tailwindのデメリットで挙がった「<span class="underline decoration-red-500">Tailwindのクラス名を覚える必要がある</span>」を（少し）解決してくれる</li>
    <li>型のおかげでclass名の補完が出るのでタイポしなくなる</li>
    <li>IDEのTailwindプラグインに頼らなくて良くなる</li>
</ul>

```tsx
// 🤔
const TailWindButton = () => {
  return (
    <button className="bg-blue-500 text-white text-lg font-bold py-2 px-4 rounded shadow-sm hover:bg-blue-700">
      Click me
    </button>
  );
};

// 😎
const TypeWindButton = () => {
  return (
    <button className={tw.bg_blue_500.text_white.text_lg.font_bold.py_2.px_4.rounded.shadow_sm.hover(bg_blue_700)}>
      Click me
    </button>
  );
};
```