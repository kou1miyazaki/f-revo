# F-RevoCRM 6.5 patch2

F-RevoCRM は、世界中で活用されている VtigerCRM をベースに、
日本の企業文化に合わせてシンキングリードが独自のカスタマイズを行った、
フリー＆オープンな高機能CRMアプリケーションです。

## 動作要件
* Apache 2.4以上
* PHP 5.4以上（7.x非対応）
* MySQL 5.5以上

## パッチ適用方法
F-RevoCRM 6.5 patch2 の適用方法になります。

### 前提条件
F-RevoCRM 6.5 がインストールされ、ソースコードの変更がされていないことを確認してください。
ソースコードの変更がある場合は、本パッチファイルに含まれるファイルとの差分を確認して変更箇所に影響が出ないように作業をしてください。

### 1. ファイルの上書き
下記ディレクトリをF-RevoCRMがインストールされているディレクトリに上書きしてください。
* layouts
* libraries
* modules
* resources

## F-RevoCRM6.5 patch2の変更点
* 機能改善
  - フィールドの編集からラベル名を変更できるように改善（多言語は不可）
  - 管理者権限を持っている場合は「すべて」が付くフィルタが編集できるように改善
  - 予定表を見やすいように改善
  - 予定表で予定をマウスオーバーした際に「場所」項目が表示されるように改善
  - IEの互換表示モードにならないようにmetaタグを追加
* 不具合修正
  - vtigercrm.logが利用PHPバージョン等よって1世代しか残らない不具合を修正
  - 複数選択可能な選択肢の名称を変更した際に、対象の選択肢が選択されているデータの名称が変わるように修正
  - IEでドキュメントのファイルをダウンロードすると文字化けしないように修正
  - IEで金額を入力した後、他の入力欄にカーソルが当たらなくなる現象を修正
  - ワークフローでメール送信時に「担当者」を本文等に挿入してもメールに記載されない問題を修正
  - レポートで日付型の項目を出力すると「-」しか出力されない問題を修正
  - 各モジュールのエクスポートで大量のデータを出力した際にエラーになる問題を修正
  - ユーザ管理で「アクティブ」「非アクティブ」の切り替えやアルファベット検索が正しく動作しない問題を修正

以上