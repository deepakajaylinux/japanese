================
MysqlAdmins
================

あらすじ
---------

このモジュール アシスト、インストールも mysql の管理者ユーザとして管理ルート ユーザーを使用せず。これを使用して、ユーザーの管理機能を管理できます。

ヘルプ コマンド
----------------------

ヘルプ コマンドは mysql 管理者とその利点をインストールするために使用されるコマンドに関するユーザーをガイドします。この mysql 管理者] のヘルプ オプションを使用するコマンドを次に示します。

.. code-block:: bash

	ptconfigure MysqlAdmins help


スクリーン ショットの下に与えられたとして mysql 管理者のヘルプ コマンドの処理でユーザー可能性があります。


.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlAdmins help
 ******************************


  This command allows you to install admin users for MySQL so that MySQL can
  be managed without using the Root User.

  MysqlAdmins, mysql-admins, mysqladmins

        - install
        Installs Mysql Admin Users.
        example: ptconfigure mysql-admins install

 ------------------------------
 End Help
 ******************************


インストール
-------------

Mysql 管理者コンピューターにインストールする、指定および彼らの管理の操作を管理するユーザーを容易にします。Mysql 管理者をインストールするために使用されるコマンドは、下記マークされます。


.. code-block:: bash

	ptconfigure MysqlAdmins install


さらに、表形式で表示されます、次の操作が発生します。

.. cssclass:: table-bordered

 +---------------------------+-----------------------------------------------+------------+----------------------------------------------+
 | パラメーター              | 代替パラメーター                              | オプション | コメント                                     |
 +===========================+===============================================+============+==============================================+
 |Install Admin User for     | MysqlAdminsの代わりに、                       | Y(Yes)     | ユーザーは、Yと入力することができ、          |
 |MySQL? (Y/N)               | これらの代替名を使用することができる:         |            | インストールプロセスを続行したい場合         |
 |                           | mysql-admins, mysqladmins.                    |            |                                              |
 +---------------------------+-----------------------------------------------+------------+----------------------------------------------+
 |Install MySQL Server?      | MysqlAdminsの代わりに、                       | N(No)      | ユーザーは、Nとして入力することができ、      |
 |(Y/N)                      | これらの代替名を使用することができる:         |            | インストールプロセスを終了したい場合は       |
 |                           | mysql-admins, mysqladmins.|                   |            |                                              |
 +---------------------------+-----------------------------------------------+------------+----------------------------------------------+



場合は、インストール プロセスを続行すると、次の制約を指定しての管理機能をフレーム彼らすることができます。

* MySQL Root User
* MySQL Root Pass
* MySQL New Admin User
* MySQL New Admin Pass

リモート システムで mysql の管理者のインストールを処理する場合は、ユーザーを指定できます。

* MySQL Host.

次のスクリーン ショットは、上記のインストールのプロセスについての絵の表現を与えます。


.. code-block:: bash


 kevell@corp:/# ptconfigure mysql-admins install 
 Install Admin User for MySQL? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Admins!        * 
 ******************************* 
 Enter MySQL Root User: 
 root 
 Enter MySQL Root Pass: 
 root123 
 Enter MySQL New Admin User: 
 kevells 
 Enter MySQL New Admin Pass: 
 kevells
 Enter MySQL Host: Enter nothing for 127.0.0.1 
 127.0.0.1   
 Creating /tmp/ptconfigure-temp-script-4745646149.sh 
 chmod 755 /tmp/ptconfigure-temp-script-4745646149.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-4745646149.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-4745646149.sh 
 Warning: Using a password on the command line interface can be insecure. 
 Temp File /tmp/ptconfigure-temp-script-4745646149.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 MysqlAdmins: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  



利点
----------

* Mysql の場合管理者は、ユーザーのコンピューターに既にインストールされてし、メッセージをユーザーに通知する、それが既に表示されます。
  インストールされています。
* このモジュールを使用して、管理者は要件に従って彼らの管理の操作を管理できます。
* リモート システムにおいても、インストール処理を実行できます。
* ルート ユーザーを使用して、ユーザーことができますがインストール mysql 管理者。
 

