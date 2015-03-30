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
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Server!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libboost-filesystem1.54.0 libboost-program-options1.54.0 
  libboost-thread1.54.0 libgoogle-perftools4 libpcrecpp0 libsnappy1 
  libtcmalloc-minimal4 libunwind8 mongodb-clients 
 Use 'apt-get autoremove' to remove them. 
 The following NEW packages will be installed: 
  debconf-utils 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 57.4 kB of archives. 
 After this operation, 157 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main debconf-utils all 1.5.51ubuntu2 [57.4 kB] 
 Fetched 57.4 kB in 14s (4,097 B/s) 
 Selecting previously unselected package debconf-utils. 
 (Reading database ... 380784 files and directories currently installed.) 
 Preparing to unpack .../debconf-utils_1.5.51ubuntu2_all.deb ... 
 Unpacking debconf-utils (1.5.51ubuntu2) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up debconf-utils (1.5.51ubuntu2) ... 
 [Pharaoh Logging] Adding Package debconf-utils from the Packager Apt executed correctly 
 Creating /tmp/ptconfigure-temp-script-12002365099.sh 
 chmod 755 /tmp/ptconfigure-temp-script-12002365099.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-12002365099.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-12002365099.sh 
 Temp File /tmp/ptconfigure-temp-script-12002365099.sh Removed 
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
 


