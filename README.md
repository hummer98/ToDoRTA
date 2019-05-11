# ToDoRTA
ToDoアプリRTA用

# レギュレーション

## 計測開始の前提条件
* homebrewインストール済
* anyenv > rbenv環境構築済
* direnv環境構築済
* Xcodeインストール済
* iOS12~向け
* 検証端末はiPhone XS Plus
* README.md, .gitignore, LICENSE.md以外のファイルがディレクトリ内に存在しないこと

## コーディングにおける成約
* cocoapodsライブラリは自由に使うことができる
* gistにて公開されているextensionは使用可能とする。ただし、classやModelなどこのプロジェクトの仕様専用とみなされるものは不可。
* ブラウザ等でサンプルコードを参照するのは良いが、コピペは禁止する。打鍵して写経するのはOK。
  * 例外としてAppleのドキュメント内に存在するコードはコピペしてもかまわない。

## Definition of Done (完了の定義)
* testFlightにデプロイされること
* testFlightより実機にインストールした端末でテスト項目がすべて完了していること
* ソースコードがgithubにpushされていること
* 上記を満たした時点でタイマーストップ

## 仕様書
* いわゆるToDoアプリ
* タスクの付属情報はタスクタイトル(テキスト)のみ。
* タスクを新規に追加できること
* 記録したタスクを一覧できること
* 記録したタスクを編集できること
* タスクを削除できること
* タスクすべてを永続化できること

## テストシナリオ
0. アプリタップで起動
1. 何もタスクが表示されていないこと
2. タスクを追加する
3. >追加したタスクが一覧に表示されていること
4. タスクを追加する
5. >2と4で追加したタスクが一覧表示されていること
6. 2で追加したタスクを削除する
7. >4で追加したタスクだけが一覧で表示されていること
8. 4で追加したタスクを削除する
