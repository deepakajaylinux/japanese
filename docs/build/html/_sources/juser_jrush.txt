==============
JUser
==============

概要
-------------

ユーザーは、コンピューターまたはネットワークのサービスを使用する人です。ユーザーは一般的に完全に理解するために必要な技術的な知識がなくても、システムまたはソフトウェア製品を使用してください。

ユーザー多くの場合ユーザー アカウントがあり、システムには、ユーザー名 (またはユーザー名) によって識別されます。ユーザー名の他の条項ログイン名を含める、画面名。

ユーザーのアカウント、システムへの認証と承認によって提供される、またはそのシステムに接続されているリソースへのアクセスを許可するユーザーことができます。ただし、認証は承認を含意しません。アカウントにログインするには、ユーザー通常必要とされる会計、セキュリティ、ログ記録、およびリソース管理の目的のため、パスワードまたは他の資格情報で自分自身を認証します。

Helpコマンド
----------------------

このコマンドは、Juser モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
        
	        jrush juser help

.. code-block:: bash

 kevell@corp:/# jrush juser help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update JUser.

  JUser, juser

        - delete
        Deletes a user
        example: jrush juser delete

        - info
        Display the details of a user
        example: jrush juser info

        - change the password of a user
        Change a users password
        example: jrush juser password

 ------------------------------
 End Help
 ****************************************




Delete
----------------

ユーザー マシンでユーザーを削除する必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush juser delete ..config file=”bootstrap file path”

上記のコマンドの絵の表現は以下します。


.. code-block:: bash

 kevell@corp:/# jrush juser delete --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Delete:
 -------------------------

 The following user has been deleted:

 User ID: 0
 Name: 
 User Name: 
 Email: 
 ------------------------------
 JUser Delete Finished
 ****************************************


Info
----------------

ユーザーはマシンでのユーザーの詳細を表示する必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush juser info ..config file=”bootstrap file path”

上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# jrush juser info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Info:
 -------------------------
 
 User ID: 
 Name: 
 User Name: 
 Email: 

 ------------------------------
 JUser Info Finished
 ****************************************

Password
----------------

ユーザーのマシンで、ユーザーのパスワードを変更する必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush juser password ..config file=”bootstrap file path”


代替パラメータ
-----------------------------

2 つの代替のパラメーターのいずれかのコマンドで使用できます。

juser and JUser

eg: jrush juser info ..config file=”bootstrap file path” / jrush JUser info ..config file=”bootstrap file path”                            

.. code-block:: bash

 kevell@corp:/# jrush juser password --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 5
 Enter a new Password. To enter as parameter use --password 
 12345
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Password:
 -------------------------

 User ID: 0
 Name: 
 User Name: 
 Email: 
 User Password: NOT SET

 ------------------------------
 JUser Password Finished
 ****************************************


メリット
--------------

* 簡単な単一コマンドを使用してユーザーに関する情報を取得する 
* 簡単に 1 つのコマンドを使用してバック エンドからユーザーのパスワードを変更する 
* をユーザー アカウントに取り扱いが容易

