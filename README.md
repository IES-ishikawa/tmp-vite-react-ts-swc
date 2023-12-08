## 概要

このリポジトリは React + Typescript + Vite + Swc の環境を Visual Studio Code の Dev Container を使用して迅速にスタートアップするためのテンプレートリポジトリです。

## 前提

以下がローカル環境にインストールされていること。  
拡張機能はインストールされていない場合、Visual Studio Code で開いたタイミングでインストールするか聞かれるので、インストールしてください。

- [Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code)
  - [Dev Container](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)拡張機能(または[ExtensionPacks](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack))
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)

## 使用方法

1.Docker Desktop を起動します。  
2.このリポジトリを Visual Studio Code で開きます。  
3.画面右下の「コンテナーで再度開く」を選択します。(Dev Container 拡張機能がないと出てきません)  
![image1](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image1.png)

または画面左下のリモートウィンドウを開き「コンテナーで再度開く」を選択します。  
![image2](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image2.png)  
![image3](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image3.png)

4.右下にスナックバーが表示され、Docker コンテナの構築が始まりますのでしばらく待ちます。  
![image4](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image4.png)  
![image5](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image5.png)

5.ターミナルに下図のような表示がされればコンテナの構築は完了です。  
![image6](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image6.png)

6.「F5」キーを押すとポート 5173(Vite のデフォルト)でデバッグサーバーが立ち、Chrome が自動的に立ち上がってデバッグ出来ます。  
![image7](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image7.png)

「タスク'vite start'を追跡できません。問題マッチャーが定義されていることを確認してください。」と表示された場合には  
「このタスクの選択内容を保存する」にチェックを入れて、このままデバッグを選択してください。  
(問題マッチャーは定義してあり、正常に動作していますがなぜか表示されます。)  
![image8](https://github.com/IES-ishikawa/assets/blob/main/vite-react-ts-swc-template/image8.png)

7.開発コンテナー名を変える場合は[devcontainer.json](.devcontainer/devcontainer.json) 2 行目の"name"の値を変えてください。  
モジュール名を変更する場合には[package.json](package.json)2 行目の"name"の値を変えてください。(これは必ず行って下さい。)

8.Let's Hack!

## 注意点

- [このリポジトリ](https://github.com/IES-ishikawa/vite-react-ts-swc-template.git)にはプッシュしないでください
