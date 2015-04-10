==============
DBInstall
==============


概要
-------------

Dbinstall モジュール データベース インストール機能を処理するのに役立ちます。このコマンドは、新しいデータベースをインストールするために使用します。インストールに sudo アクセスする必要があります。 または root として実行する必要があります。これは、rpm コマンドまたは tar パッケージの miminstall コマンドの実行が含まれますとも初期データベースを作成する dbinstall コマンドを使用する場合。

初期データベースを作成中に dbinstall コマンドを使用して Mimer SQL データベースを構築することができますソフトウェアをインストールしました。

私たち Linux (CentOS) サーバーで新しいデータベースをインストールし、接続文字列にデータベース名が必要です (サーバー) から、データベースに接続するとき。前に述べたように、dbinstall コマンド sudo アクセス必要があります。 または root で実行する必要があります。特権シェルの sudo パスワードから開始されていない場合になります。

Dbinstall セッション、データベース名、データベースの場所と、データベースのパスワードの中には (つまり管理者) の管理者を指定してください。インストール環境の例等のオプションもあります。セッションが完了したら、完全に運用データベースが - TCP 経由の再起動時の自動起動クライアント/サーバーへのアクセスを有効になっています。


Helpコマンド
----------------------

このコマンドは、DBinstall モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
	
		ptdeploy DBInstall help
       
上記のコマンドの絵画表現は、次に示す


.. code-block:: bash

 kevell@corp:/# ptdeploy DBInstall help
 ******************************


  This command is part of Default Modules and handles Database Installation Functions.

  DBInstall, db-install, dbinstall

          - install
          install the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install install

          - save
          save the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install save

          - drop
          drop the database for a project.
          example: ptdeploy db-install drop

      
 --------------
  Wordpress Module:

  The Wordpress module extends DBInstall by adding wordpress-install

  Wordpress module adds the actions wordpress-install and wp-install to DBInstall, requiresd to allow the Post DB
  Install hooks for Wordpress, the DB restore won't work correctly without at least the url.

  ptdeploy dbinstall wordpress-install --yes --guess --hook-url=www.site.env
 ------------------------------
 End Help
 ******************************







Installation
----------------

インストールする必要があるとき、ユーザーは DBIstall のため、次のコマンドを発行できます。システムがインストールの手順を実行します。


.. code-block:: bash
	
		 ptdeploy dbinstall install


.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall install
 Do you want to install a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User? 

 You must enter a value. Please try again.
 What's the MySQL Admin User?

 You must enter a value. Please try again.
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB User?
 (0) **CREATE NEW USER** 
 (1) phpci 
 (2) debian-sys-maint 
 (3) phpci 
 (4) phpmyadmin 
 1
 What's the application DB Password?
 phpci_pass
 What's the application DB Name?
 Current Db's are:
 hps
 phpci
 phpmyadmin

 phpci
 Database script executed
 **************************************
 Seems Fine...Database Actions Finished
 **************************************




Save
----------------

ユーザーはプロジェクトのデータベースを保存する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
		ptdeploy dbinstall save	

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall save
 Do you want to save a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB Name?
 Current Db's are:
 asdf
 hps
 phpci 

 asdf
 Cannot connect with these details. Sure you want to continue? (Y/N) 
 y
 Exporting DB to /opt/db/database.sql 
 Database Dumping...
 **************************************
 Seems Fine...Database Actions Finished
 ************************************** 




Drop
----------------

ユーザーはプロジェクトのデータベースを削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
		ptdeploy dbinstall drop      


.. code-block:: bash


 kevell@corp:/# ptdeploy db-install drop 

 Do you want to perform drop actions (user/db)? (Y/N) 
 y
 Do you want to drop a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root123
 What's the application DB Name?
 (0) karuna 
 (1) test1 
 (2) test2 
 2
 Database test2 dropped
 **************************************
 Seems Fine...Database Actions Finished
 **************************************




代替パラメータ
-----------------------------

3 つの代替のパラメーターのいずれかのコマンド dbinstall、DBInstall、db インストールで使用できます。

eg: ptdeploy DBInstall help/  ptdeploy db-install help                 

メリット
--------------

* それをチェックし、それはインストールするパッケージのすべての依存関係を確認してください 
* このシステムは既にそれらを持っていない限りユーザーを設定する最初の dbconfigure が実行されます 
* dbinstall 特定のデータベース サーバーのホーム ディレクトリにすべてのシステムのデータバンクを作成します


