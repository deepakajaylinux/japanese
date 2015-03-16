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

.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-46222435876.sh
 chmod 755 /tmp/ptconfigure-temp-script-46222435876.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-46222435876.sh Permissions
 Executing /tmp/ptconfigure-temp-script-46222435876.sh
 Temp File /tmp/ptconfigure-temp-script-46222435876.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libdbd-mysql-perl libdbi-perl libterm-readkey-perl mysql-client-5.5
  mysql-client-core-5.5
 Suggested packages:
  libclone-perl libmldbm-perl libnet-daemon-perl libplrpc-perl
  libsql-statement-perl
 The following NEW packages will be installed:
  libdbd-mysql-perl libdbi-perl libterm-readkey-perl mysql-client
  mysql-client-5.5 mysql-client-core-5.5
 0 upgraded, 6 newly installed, 0 to remove and 172 not upgraded.
 Need to get 2,315 kB/3,321 kB of archives.
 After this operation, 40.1 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client-core-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [710 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [1,592 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-client all 5.5.41-0ubuntu0.14.04.1 [12.3 kB]
 Fetched 2,315 kB in 44s (51.7 kB/s)
 Selecting previously unselected package libdbi-perl.
 (Reading database ... 232987 files and directories currently installed.)
 Preparing to unpack .../libdbi-perl_1.630-1_amd64.deb ...
 Unpacking libdbi-perl (1.630-1) ...
 Selecting previously unselected package libdbd-mysql-perl.
 Preparing to unpack .../libdbd-mysql-perl_4.025-1_amd64.deb ...
 Unpacking libdbd-mysql-perl (4.025-1) ...
 Selecting previously unselected package libterm-readkey-perl.
 Preparing to unpack .../libterm-readkey-perl_2.31-1_amd64.deb ...
 Unpacking libterm-readkey-perl (2.31-1) ...
 Selecting previously unselected package mysql-client-core-5.5.
 Preparing to unpack .../mysql-client-core-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-client-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-client-5.5.
 Preparing to unpack .../mysql-client-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-client-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-client.
 Preparing to unpack .../mysql-client_5.5.41-0ubuntu0.14.04.1_all.deb ...
 Unpacking mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libdbi-perl (1.630-1) ...
 Setting up libdbd-mysql-perl (4.025-1) ...
 Setting up libterm-readkey-perl (2.31-1) ...
 Setting up mysql-client-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Setting up mysql-client-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Setting up mysql-client (5.5.41-0ubuntu0.14.04.1) ...
 [Pharaoh Logging] Adding Package mysql-client from the Packager Apt executed correctly
 Aborting downgrade from (at least) 5.6 to 5.5.
 If are sure you want to downgrade to 5.5, remove the file
 /var/lib/mysql/debian-*.flag and try installing again.
 dpkg: error processing archive /var/cache/apt/archives/mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb (--unpack):
  subprocess new pre-installation script returned error exit status 1
 Errors were encountered while processing:
  /var/cache/apt/archives/mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb
 E: Sub-process /usr/bin/dpkg returned an error code (1)
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   libaio1 libhtml-template-perl mysql-server-5.5 mysql-server-core-5.5
 Suggested packages:
   libipc-sharedcache-perl tinyca mailx
 The following NEW packages will be installed:
  libaio1 libhtml-template-perl mysql-server mysql-server-5.5
  mysql-server-core-5.5
 0 upgraded, 5 newly installed, 0 to remove and 172 not upgraded.
 Need to get 4,964 kB/5,036 kB of archives.
 After this operation, 53.0 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server-core-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [3,207 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server-5.5 amd64 5.5.41-0ubuntu0.14.04.1 [1,744 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main mysql-server all 5.5.41-0ubuntu0.14.04.1 [12.4 kB]
 Preconfiguring packages ...
 Fetched 4,964 kB in 1min 5s (75.8 kB/s)
 Selecting previously unselected package libaio1:amd64.
 (Reading database ... 233242 files and directories currently installed.)
 Preparing to unpack .../libaio1_0.3.109-4_amd64.deb ...
 Unpacking libaio1:amd64 (0.3.109-4) ...
 Selecting previously unselected package mysql-server-core-5.5.
 Preparing to unpack .../mysql-server-core-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking mysql-server-core-5.5 (5.5.41-0ubuntu0.14.04.1) ...
 Selecting previously unselected package mysql-server-5.5.
 Preparing to unpack .../mysql-server-5.5_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Selecting previously unselected package libhtml-template-perl.
 Preparing to unpack .../libhtml-template-perl_2.95-1_all.deb ...
 Unpacking libhtml-template-perl (2.95-1) ...
 Selecting previously unselected package mysql-server.
 Preparing to unpack .../mysql-server_5.5.41-0ubuntu0.14.04.1_all.deb ...
 Unpacking mysql-server (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package mysql-server from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************



Mysql サーバーが既にある場合が既にインストールされているユーザーに、メッセージがスローされ、あなたのマシンに存在します。次のスクリーン ショットを確認するプロセスを表します。


.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-23889189196.sh
 chmod 755 /tmp/ptconfigure-temp-script-23889189196.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23889189196.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23889189196.sh
 Temp File /tmp/ptconfigure-temp-script-23889189196.sh Removed
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************




利点
----------

* インストール中に mysql サーバ、更新されたバージョンをインストールします。
* インストール、およびモジュールの空室状況をチェックする前に保証します。
* 新しいモジュールは、更新されたバージョンに含まれている、すべての場合、不足しているモジュールを個別にインストールされます。
* Mysql サーバでライブラリ関数の可用性を確認します。
 


