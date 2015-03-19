============
DBConfigure
============

概要
-------------

これはモニカのデータベース機能モジュール。このデータベースに由来することができる構成がアプリケーションにEntity Frameworkの構成を定義するDbContextから派生データベースと同じアセンブリ内に配置することができる。コンフィギュレーションは、保護されたメソッドを呼び出すと、ユーザの派生型のコンストラクタで、このデータベースの保護されたプロパティを設定することで設定されています。使用するタイプは、アプリケーションの設定ファイルに登録することができる。これはUbuntuとCentOSのに十分である。


Helpコマンド
-----------------------

helpコマンドはptdeployでデータベースを処理するユーザーをガイドします。このhelpコマンドは、confのを作成するためのユーザーをガイドします。これは、現在のデータベースをリセットします。データベースは、組織の内部動作をサポートし、顧客やサプライヤーとのオンライン相互作用を支えるために使用されます。 dbconfigureためのhelpコマンドを以下に示します。


.. code-block:: bash
	
	ptdeploy  DBConfigure help

後に上記のコマンドを入力すると、データベースを処理するために機能を開始する。これは、スクリーンショットで関数を教理。

 次のスクリーンショットは、DBConfigureについて示しています。

.. code-block:: bash

 kevell@corp:/# ptdeploy DBConfigure help
 ******************************


  This command is part of Default Modules and handles Databasing Functions.

  DBConfigure, db-configure, dbconfigure, db-conf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --mysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30

代替パラメータ
-----------------------------------

利用可能な4代わりのパラメータがあります。

DBConfigure, db-configure, dbconfigure, db-conf.

を設定し、confの
-----------------------

このプロセスは、プロジェクトのために、データベース·ユーザーとpasswardを設定します。また、彼らが必要とする場合は、新しいリソースを作成するには、adminを使用しています。次のスクリーンショットは、その機能を示しています。

.. code-block:: bash

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --m	     ysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"

次のコマンドは、設定するために使用。

.. code-block:: bash

	ptdeploy  db-conf Conf

上記のキーでコマンドと述べた後、次のプロセスが機能させることができる。これは、スクリーンショットに示されている。

'' Y "として入力した後、これは、MySQLの管理者ユーザは、MySQLのホスト、アプリケーションDBユーザー、およびアプリケーションDBパスワード、DB名を尋ねます。これらのこのプロセスは、その機能を起動するためにユーザーが入力を入力する

リセット
----------

このプロセスは、一般的な値に現在のデータベースをリセットするために使用。このような場合にはptdeployは、実行データベース構成の前に書くことができます。データベースの名前は、同じコマンドライン自体に入力することができる。

次のコマンドを実行すると、リセットするために使用される。

.. code-block:: bash

	ptdeploy  db-conf reset

次のスクリーンショットは、このプロセスの機能を示しています。

.. code-block:: bash

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30

オプション
---------------
.. cssclass:: table-bordered


 +--------------------------------------+------------------+---------------------------------------------------------+
 | パラメータ                           | オプション       | コメント                                                |
 +======================================+==================+=========================================================+
 |Do you want to configure a database?  | Yes              | ptdeploy undderデータベースを構成しました。             |
 +--------------------------------------+------------------+---------------------------------------------------------+
 |Do you want to configure a database?  | No               | 設定画面を終了します|                                   |
 +--------------------------------------+------------------+---------------------------------------------------------+


メリット
--------------

* アドバンテージデータベースの設定を簡単に構築し、ユーザーを許可し、高性能、低メンテナンス、リモートデータベースの設定です
  クライアント/サーバー·アプリケーションとWebベースのアプリケーションを配備する。
* これは、ユーザーUbuntuとCentOSのとの友好です。
* 非大文字と小文字の区別は、このモジュールの大きなメリットです。
* これは、PHPなどの標準インターフェースをサポート
* これは、データベース機能を処理することは容易である
