---
layout: default
---

# 簡単な使い方

通常のJavaScript

```js
const addNumbers = (a, b) => {
    return a + b;
}

// この処理はエラーにならずに結果として文字列の`57`が出力される 😇
const result = addNumbers(5, "7")
```

<p class="text-lg font-bold text-center my-10!">↓</p>

TypeScript

```ts
const addNumbers = (a: number, b: number) => {
    return a + b;
}

// Compile Error!! 😊
const result = addNumbers(5, "7")
```