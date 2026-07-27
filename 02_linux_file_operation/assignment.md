# トレーニングコース第２回課題
## 課題１：ファイルとディレクトリの作成
以下のようなファイル・ディレクトリ構成を Linux コマンドを用いて作成してください。 ファイルの中身は空で構いません


以下に実行コマンドとその出力を示す。

1. 大元のディレクトリとその中身のディレクトリを作成
`$mkdir linux_practice`
`$ mkdir linux_practice/memo`
`$ mkdir linux_practice/data`

2. memo ディレクトリ内に空ファイルを作成
`$touch linux_practice/memo/note1.txt$ touch linux_practice/memo/note2.txt`

3. data ディレクトリ内に空ファイルを作成
`$ touch linux_practice/data/sample1.txt`
`$ touch linux_practice/data/sample2.txt`
`$ touch linux_practice/data/sample3.txt`

5. 構成の確認
`$ ls -R linux_practice`


出力：
`linux_practice:
data  memo

linux_practice/data:
sample1.txt  sample2.txt  sample3.txt

linux_practice/memo:
note1.txt  note2.txt`


主要な利用コマンドの簡単な説明

mkdir：新しいディレクトリを作成するコマンド

ls -R：ls はディレクトリの中身を一覧表示するコマンドであり、 -R オプションをつけることで、指定したディレクトリの中身だけでなくその中にあるディレクトリの中身まで、すべて表示。


## 課題２


## 課題３


## 課題４


