# 使い方

<p class="description">Material-UIとReactを今すぐ始めましょう。</p>

Material-UIコンポーネントは独立して機能します。 **これらは自立しており**、表示するのに必要なスタイルだけを加えます。 それらは[normalize.css](https://github.com/necolas/normalize.css/)のようなグローバルのスタイルシートには依存しません。

You can use any of the components as demonstrated in the documentation. どのようにインポートされるか確認する為にそれぞれのコンポーネントの[デモページ](/components/buttons/)を参照してください。

## 今すぐ始める

以下に簡単な例を示します。 **文字通り必要なものすべてです**:

```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import Button from '@material-ui/core/Button';

function App() {
  return (
    <Button variant="contained" color="primary">
      Hello World
    </Button>
  );
}

ReactDOM.render(<App />, document.querySelector('#app'));
```

そうです。 これは本当に始めるのに必要な全てです。 この編集可能なデモで確認できるように:

{{"demo": "pages/getting-started/usage/Usage.js", "hideToolbar": true, "bg": true}}

## Globals

知っておく必要のあるいくつかの重要なことで、Material-UIの使い易さは改善されます。

### Responsive meta tag

Material-UI is developed mobile-first, a strategy in which we first write code for mobile devices, and then scale up components as necessary using CSS media queries. To ensure proper rendering and touch zooming for all devices, add the responsive viewport meta tag to your `<head>` element.

```html
<meta
  name="viewport"
  content="minimum-scale=1, initial-scale=1, width=device-width"
/>
```

### CssBaseline

Material-UIはオプションで[CssBaseline](/components/css-baseline/)コンポーネントを提供しています。 It fixes some inconsistencies across browsers and devices while providing slightly more opinionated resets to common HTML elements.

## バージョン管理されたドキュメント

This documentation always reflects the latest stable version of Material-UI. You can find older versions of the documentation on a [separate page](https://material-ui.com/versions/).

## 次のステップ

これで基本的なセットアップがわかったので、次の項目について詳しく学びましょう。

- [Material Designフォントとタイポグラフィ](/components/typography/)を導入する方法
- [テーマソリューションを活用する方法](/customization/theming/) 。
- コンポーネントの見た目を[上書き](/customization/components/)する方法
