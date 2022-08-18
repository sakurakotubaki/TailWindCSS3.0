# 環境構築の仕方

**公式ドキュメント**
https://tailwindcss.com/docs/installation

## TailWindCLEで環境構築を行う

## プロジェクトフォルダでコマンドを順番に実行する

1. package.jsonを生成
```
npm install -D tailwindcss
```

2. tailwindの設定に必要なファイルを生成
```
npx tailwindcss init
```
3. CSS に Tailwind ディレクティブを追加する
- srcフォルダを作成して、input.cssファイルを作成して、
  ドキュメントのコードをコピーして使う

4. Tailwind CLI ビルド プロセスを開始する
```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```
5. buildを簡単に行えるように設定をする。package.jsonを生成するファイルを入力する
   既に存在するファイルに設定が追加される
- 毎回、4番のコマンドを打ち込むのはめんどくさい!
```
npm init -y
```
6. buildできる設定をpackage.jsonに追加したら、こちらのコマンドを実行する。
```
npm run build
```
7. srcフォルダに、index.htmlファイルを用意する
