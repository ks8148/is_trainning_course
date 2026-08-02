# トレーニングコース第２回課題
## 課題１：ファイルとディレクトリの作成
以下のようなファイル・ディレクトリ構成を Linux コマンドを用いて作成してください。 ファイルの中身は空で構いません


以下に実行コマンドとその出力を示す。

1. 大元のディレクトリとその中身のディレクトリを作成
`$ mkdir linux_practice`
`$ mkdir linux_practice/memo`
`$ mkdir linux_practice/data`

2. memo ディレクトリ内に空ファイルを作成
`$ touch linux_practice/memo/note1.txt$ touch linux_practice/memo/note2.txt`

3. data ディレクトリ内に空ファイルを作成
`$ touch linux_practice/data/sample1.txt`
`$ touch linux_practice/data/sample2.txt`
`$ touch linux_practice/data/sample3.txt`

5. 構成の確認
`$ ls -R linux_practice`


出力：
`linux_practice:`
`data  memo`

`linux_practice/data:`
`sample1.txt  sample2.txt  sample3.txt`

`linux_practice/memo:`
`note1.txt  note2.txt`


主要な利用コマンドの簡単な説明

mkdir：新しいディレクトリを作成するコマンド

ls -R：ls はディレクトリの中身を一覧表示するコマンドであり、 -R オプションをつけることで、指定したディレクトリの中身だけでなくその中にあるディレクトリの中身まで、すべて表示。


## 課題２　ファイルのコピー・移動・名前変更・検索
以下に実行したコマンドと出力を示す。

`$ cp linux_practice/data/sample1.txt linux_practice/memo/sample1_backup.txt`

`$ mv linux_practice/data/sample2.txt linux_practice/data/result.txt`

`$ mv linux_practice/data/sample3.txt linux_practice/memo/`

`$ ln -s ../memo/note1.txt linux_practice/data/link_to_note1.txt`

`$ cat linux_practice/data/link_to_note1.txt`

`$ find linux_practice -type f`

`linux_practice/memo/sample3.txt`

`linux_practice/memo/note1.txt`

`linux_practice/memo/note2.txt`

`linux_practice/memo/sample1_backup.txt`

`linux_practice/data/sample1.txt`

`linux_practice/data/result.txt`

`$ find linux_practice -type l`

`linux_practice/data/link_to_note1.txt`



コピー、移動、名前変更、シンボリックリンクの違いについての簡単な説明を以下に示す。

・コピー (cp)

ファイルの実体を複製し、別の場所に新しいファイルとして保存する

特徴: 操作後、元のファイルと新しいファイルという2つのファイルになる。それぞれの中身を後から編集しても、互いに影響を及ぼさないため、バックアップを取る際に使用する。


・移動 (mv)

ファイルの実体を、別のディレクトリへ移動させる。

特徴: 操作後、元の場所からはファイルが消滅し、ファイルが存在するのは移動先のみになる。


・名前変更 (mv)

コマンド自体は「移動」と同じ mv を使用し、同じディレクトリ内でファイル名を変更することを、「同じ場所への移動」として扱う。

特徴: ファイルの場所は変わらず、名前だけが変更され、ファイルは1つのままになる。


・シンボリックリンク (ln -s)

ファイルの実体は複製せず、元のファイルが存在する場所へのショートカットだけを別の場所に作成します。

特徴: リンクファイル自体の容量はほぼゼロで、リンク先を編集すると、元のファイルが編集される。また、大元のファイルを削除したり移動したりすると、リンクは「リンク切れ」となり機能しなくなる。ストレージ容量を圧迫する大容量データ等に別の場所からアクセスしたい場合などに重宝する。



## 課題３


## 課題４


