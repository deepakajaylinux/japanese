===============
Mysqlserver
===============


あらすじ
------------

このモジュールは、apt-get 経由で更新されたバージョンの mysql サーバをインストールするためにファシリテーターとして機能します。あなたのマシンで mysql サーバーが既に存在する場合それは新しく更新されたモジュールの空室状況をチェックします。

ヘルプ コマンド
----------------

このモジュールの下で実行できるアクションについても使用方法に関するユーザー ヘルプ コマンドについて説明します。また、mysql サーバの代替名をについて説明します。ヘルプ オプションを使用するためのコマンドを以下に

.. code-block:: bash

	ptconfigure mysql-server help

このコマンドにより、ユーザーをその目的と mysql サーバのインストールに使用するコマンドについても注意してください。
下記のスクリーン ショットは、help コマンドについて絵画表現を示しています。


.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************


インストール
----------------

Mysql サーバをインストールするために使用されるコマンドは以下の通りです。


.. code-block:: bash

	ptconfigure mysql-server install

インストール中には、次のプロセスが発生します。
--------------------------------------------------------

* Apt-get 経由で mysql サーバーのいくつかのツールをインストールするこのモジュールを支援します。
* 最初に root のパスワードが設定されます。
* インストール中に、--mysql ルート パスのパラメーターになります。
* --Mysql ルート パスが使用できない場合は mysql 既定ルート パスの設定のための ptconfigure 設定を検索します。
* 両方手順を上記の取得が失敗した場合にそれは ptconfigure に root パスワードの設定して続行されます。

追加オプション:
--------------------
詳細については、mysql サーバのインストールに関連する追加オプションを参照してくださいみましょう。

.. cssclass:: table-bordered

 +------------------+--------------------------------------------------------------+------------+--------------------------------------------+
 | パラメーター     | ディレクトリ（デフォルト）                                   | オプション | コメント                                   |
 +==================+==============================================================+============+============================================+
 |Install MySQL     | MySQLサーバの代わりに、これらの代替名を使用することができる: | Y(Yes)     | ユーザーは、Yと入力することができ、        |
 |Server? (Y/N)     | MysqlServer,mysql-server, mysqlserver.                       |            | インストールプロセスを続行したい場合       |
 +------------------+--------------------------------------------------------------+------------+--------------------------------------------+
 |Install MySQL     | MySQLサーバの代わりに、これらの代替名を使用することができる: | N(No)      | ユーザーは、Nとして入力することができ、    |
 |Server? (Y/N)     | MysqlServer,mysql-server, mysqlserver.                       |            | インストールプロセスを終了したい場合は|    |
 +------------------+--------------------------------------------------------------+------------+--------------------------------------------+


次のスクリーン ショットは、インストール プロセスに関してグラフィカルなプレゼンテーションを与えます。

Mysql サーバーが既にある場合が既にインストールされているユーザーに、メッセージがスローされ、あなたのマシンに存在します。次のスクリーン ショットを確認するプロセスを表します。



利点
----------

* インストール中に mysql サーバ、更新されたバージョンをインストールします。
* インストール、およびモジュールの空室状況をチェックする前に保証します。
* 新しいモジュールは、更新されたバージョンに含まれている、すべての場合、不足しているモジュールを個別にインストールされます。
* Mysql サーバでライブラリ関数の可用性を確認します。
 


