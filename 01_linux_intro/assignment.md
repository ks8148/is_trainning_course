# トレーニングコース第1回課題
## 課題1
利用したショートカットとその説明を記述してください。




まず1行目を普通に実行

`$ echo "This is a very very long command for practice"`




次にCtrl+Pで直前の実行履歴を呼び戻す。

Alt+Bを何回か押すことで何単語か左に移動し「a」と「very」の間に移動

Ctrl+Wを1回押して「a」を消去

「yet another」と書き加えて実行

`$ echo "This is yet another very very long command for practice"`



Ctrl+Pを2回押して1行目を呼び戻す。

Alt+Bを何回か押して「long」と「command」の間に移動

Ctrl+Wを5回押して単語を削除

「a」を付け加えて実行

`$ echo "This is a command for practice"`



## 課題2
1. bash コマンドのファイル名を確認してください。

2. 1の場所に bash というファイルが存在することを確認してください。

3. 1の場所が環境変数 PATH に含まれていることを確認してください。

利用したコマンドとその説明を記述してください。

1.ファイル名確認手順

`$ which bash`

上のコードの実行により、ファイル名は「`/usr/bin/bash`」と分かった。


2.ファイルの存在確認

`$ ls -l /usr/bin/bash`

上のコードの実行結果として、「`-rwxr-xr-x 1 root root 1396520 Mar 14  2024 /usr/bin/bash`」と表示されたため、存在することが確認できた。


3.環境変数に含まれているかの確認

`echo $PATH`

上のコードの実行結果として、「`/usr/bin`」が表示されたため、PATHに含まれていると確認できた。



## 課題3

1.コマンド ls は何を目的とするコマンドでしょうか。

ディレクトリの中身（ファイルやフォルダ）をリスト表示し、今自分がいる場所にどんなデータがあるかを確認することを目的としたコマンド


2.コマンド ls でファイルサイズを人間に読める単位 (human readable) で表示するには、どのオプションを使えばいいでしょうか。

`$ ls --help`

上のコードを実行することで、「`-h`」が`-h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.`と書かれているため、-hオプションを使えばよいことがわかる。



## 課題4

「`$ ls no_such_file.txt`」

エラー内容：`ls: cannot access 'no_such_file.txt': No such file or directory`

意味：no_such_file.txt という名前のファイルにアクセスしようとしたが、そのようなファイルは存在しない。


「`$ not_a_real_command`」

エラー内容：not_a_real_command: command not found

意味：not_a_real_command というコマンドを実行しようとしたが、コマンドが存在しない。


「`$ rm`」

エラー内容：rm: missing operand

意味：rmコマンドを実行したが、何を削除するのかが指定されていない。(引数不足)


「`$ cd /no/such/dir`」

エラー内容：-bash: cd: /no/such/dir: No such file or directory

意味：/no/such/dir というディレクトリに移動しようとしたが、そのような場所が存在しない。







