---
layout: default
---

# Normal Usage

- Typewindから提供される`tw`オブジェクトにアクセス、チェーンすることでTailwindのクラスを呼び出せる
- `tw`は`tailwind.config.js`の設定を元にしているので独自で定義したカラーパレット等も呼び出し可能
- Typewindのクラス名はTailwindのクラスのハイフン(`-`)をアンダースコア(`_`)に変えたもの
- `-mt-1`のような負の値(ハイフン始まり)のクラスは、`tw._mt_1`のように指定する
- `inset-1/2`のような/が含まれるクラスは、`tw.inset_["1/2"]`のように指定する
- 色の不透明度は、`tw.bg_blue_500$["25"]`のように指定する

```tsx {5,6,7|3|4|5}
const Normal = () => {
  return (
    <div className={tw._mt_1}>
        <div className={tw.inset_["1/2"]}>
            <button className={tw.bg_blue_500.text_white.text_lg.font_bold.py_2.px_4.rounded.shadow_sm.hover(bg_blue_700$["25"])}>
              Click me
            </button>
        </div>
    </div>
  );
};
```