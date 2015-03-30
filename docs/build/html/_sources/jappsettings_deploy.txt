===============
Appsettings
===============

概要
-----------------

それをappSettingがすることは、私たちは、アプリケーションが適切にタスクを実行するために必要で、設定とアプリケーション全体の設定を維持することができます。これは、アプリケーションの容易なメンテナンスと展開するのに役立ちます。のAppSettingを使用することにより、我々は、ユーザー定義の値を定義することができます。

Helpコマンド
------------------

このコマンドは、AppSettingsの使用状況を判断するのに役立ちます。それは、AppSettingsの機能のために別のパラメータと構文を示しています
モジュール。のAppSettingsためのhelpコマンドは以下の通りである。

.. code-block:: bash

	ptdeploy appsettings help

helpコマンドの絵画表現は、以下のとおりである


.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings help

 ******************************


  This command is part of Default Modules and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  AppSettings, appsettings
	
        - set
        Set a configuration value
        example: ptdeploy appsettings set

        - get
        Get the value of a setting you have configured
        example: ptdeploy appsettings get

        - delete
        Delete a setting you have configured
        example: ptdeploy appsettings delete

        - list
        Display a list of all default available settings
        example: ptdeploy appsettings list

 ------------------------------
 End Help
 ******************************


Set
---------

設定コマンドは、構成値を設定するのに役立つ。以下のコマンドは、プロセスを実行します。


.. code-block:: bash

	ptdeploy appsettings set

helpコマンドの絵画表現は、以下のとおりである


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings set

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 What Value do you want to give this variable?
 /tmp/
 ******************************

 Seems Fine...
 In Application Config
 ******************************


Get
--------

Getコマンドを使用すると、すでに設定した設定の値を取得するのに役立ちます。以下のコマンドは、プロセスを実行します。


.. code-block:: bash

	ptdeploy appsettings get


helpコマンドの絵画表現は、以下のとおりである

.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings get

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 4
 ******************************


 Variable Name: linux-user
 Variable Value: karuna
 
 In Application Config
 ******************************


Delete
--------

deleteコマンドは、設定した設定を削除するのに役立ちます。以下のコマンドは、プロセスを実行します。


.. code-block:: bash

	ptdeploy appsettings delete

helpコマンドの絵画表現は、以下のとおりである

.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings delete

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 ******************************


 Seems Fine...
 In Application Config
 ******************************



List
-------

listコマンドでは、すべてのデフォルト使用可能な設定の一覧を表示するのに役立ちます。下のcommadは、プロセスが実行されます。


.. code-block:: bash

	ptdeploy appsettings list

helpコマンドの絵画表現は、以下のとおりである


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings list

 Do you want to Configure Application Settings? (Y/N) 
 y
 ******************************


 Variable Type is: allSet 
   linux-user is: karuna 
   mysql-admin-user is: mani 
 Variable Type is: allTotal 
   mysql-admin-user 
   mysql-admin-host 
   mysql-admin-pass 
   linux-user 
   linux-user-dir 
   program-dir 
   temp-base-dir 
   distro 
   op-sys 
   linux-type 

 In Application Config
 ******************************



別のパラメータ
--------------------------

コマンドラインで使用することができる2つの別のパラメータがある。

AppSettings, appsettings


メリット
-----------

* 強く型付けされたアクセス
* 非大文字と小文字の区別


