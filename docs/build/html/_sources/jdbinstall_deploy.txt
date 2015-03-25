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







インストール
----------------

インストールする必要があるとき、ユーザーは DBIstall のため、次のコマンドを発行できます。システムがインストールの手順を実行します。


.. code-block:: bash
	
		 ptdeploy dbinstall install


システムの既定のホストを使用して Enter キーを押して、Mysql のホストを求めます。


.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1


システムを求める Mysql 管理者ユーザー ユーザー名は"root"となりますと、Mysql の管理者パスワードです。


.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
その後、システムを求めるアプリケーション DB ユーザー既存ユーザーを続行または新しいユーザーを作成することができます。一度提供するオプションの '0' で新しいユーザー、システム、新しいユーザー名やアプリケーション DB パスワード アプリケーション DB 名を求めるため。


.. code-block:: bash






一度上記記載システム確認を求めます。確認の後、システムは、プロセスを実行します。


.. code-block:: bash











Save
----------------

ユーザーはプロジェクトのデータベースを保存する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
		ptdeploy dbinstall save	

処刑の前に、システムを求める続行、続行する場合は、'Y' を入力する確認場合ない enter ' ñ '。


.. code-block:: bash









システムの既定のホストを使用して Enter キーを押して、Mysql のホストを求めます。

.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1


システムを求める Mysql 管理者ユーザー ユーザー名は"root"となりますと、Mysql の管理者パスワードです。


.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
その後、システムは、アプリケーションDBユーザーをお願いいたします。

.. code-block:: bash


Drop
----------------

ユーザーはプロジェクトのデータベースを削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
		ptdeploy dbinstall drop      

処刑の前に、システムを求める続行、続行する場合は、'Y' を入力する確認場合ない enter ' ñ '。                   

.. code-block:: bash








システムの既定のホストを使用して Enter キーを押して、Mysql のホストを求めます。


.. code-block:: bash

 What's the Mysql Host? Enter for 127.0.0.1

システムを求める Mysql 管理者ユーザー ユーザー名は"root"となりますと、Mysql の管理者パスワードです。

.. code-block:: bash

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 123456

 
その後、システムは、アプリケーションDBユーザーをお願いいたします。

.. code-block:: bash



代替パラメータ
-----------------------------

3 つの代替のパラメーターのいずれかのコマンド dbinstall、DBInstall、db インストールで使用できます。

eg: ptdeploy DBInstall help/  ptdeploy db-install help                 

メリット
--------------

* それをチェックし、それはインストールするパッケージのすべての依存関係を確認してください 
* このシステムは既にそれらを持っていない限りユーザーを設定する最初の dbconfigure が実行されます 
* dbinstall 特定のデータベース サーバーのホーム ディレクトリにすべてのシステムのデータバンクを作成します


