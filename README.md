## 概要

このリポジトリは React + Typescript + Vite + Swc の環境を Visual Studio Code の Dev Container を使用して迅速にスタートアップするためのテンプレートリポジトリです。

## 前提

以下がローカル環境にインストールされていること

- [Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code)
  - [Dev Container](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)拡張機能(または[ExtensionPacks](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack))
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)

## 使用方法

1.このリポジトリを Visual Studio Code(以下 VSCode)で開きます。  
2.

```js
export default {
	// other rules...
	parserOptions: {
		ecmaVersion: 'latest',
		sourceType: 'module',
		project: ['./tsconfig.json', './tsconfig.node.json'],
		tsconfigRootDir: __dirname
	}
};
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
