=================
PackageManager
=================

あらすじ
----------------

このコマンドは、パッケージ管理をラップするために使用します。それは 3 つのオプションを有しています。彼らは pkg pkg インストール-pkg 削除を確認します。これは任意のシステムにインストールするユーザーを許可します。パッケージ マネージャーの機能を管理します。それは、Ubuntu や centos 関連の作業に最適。

ヘルプ コマンド
-----------------------

このヘルプ コマンドはインストール、確認、パッケージ管理を削除するユーザーをガイドします。これにより、インストール、確認、削除します。パッケージ マネージャーのヘルプ コマンドを以下に示します。

.. code-block:: bash

		ptconfigure packagemanager help

開始後の入力上記のコマンドをラップする機能します。それの教理のスクリーン ショットで機能します。



.. code-block:: bash

 kevell@corp:/# ptconfigure PackageManager help 

 ****************************** 


  This command allows you to use a Package Management wrapper. 

  PackageManager, package-manager, packagemanager, package-mgr, pkgmgr 

        - pkg-install 
        Installs a Package through a Package Manager 
        example: ptconfigure package-manager pkg-install --package-name="mysql" --packager-name="apt" 

        - pkg-ensure 
        Installs a Package through a Package Manager 
        example: ptconfigure package-manager pkg-ensure --package-name="mysql" --packager-name="apt" 
 
        - pkg-remove 
        Removes a Package through a Package Manager 
        example: ptconfigure package-manager pkg-remove --package-name="mysql" --packager-name="apt" 

  A package manager wrapper that will allow you to install packages on any system 

 ------------------------------ 
 End Help 
 ****************************** 



代替パラメーター
--------------------------------

宣言で定義することができます、代替パラメーターを次に示します。

PackageManager, package-manager, packagemanager, pkgmgr, package-mgr.


Pkg インストール
-----------------

インストールには、更新されたバージョンで、インストールを行うために必要な PackageManager のインストールが含まれます。それは ptconfigure の下で PackageManager モジュールをインストールするマニフェスト プロセスです。ちょうど、下記のコマンドを使用して PackageManager

.. Code-block:: bash

	ptconfigure PackageManager Install

それは質問攻めにコマンド入力活性化後。

ユーザーが [はい] を入力するときに自動的にシステムからのチェックと PackageManager がインストールされます。ない場合、インストールを終了します。次のスクリーン ショットは、PackageManager とその機能を示しています。


.. code-block:: bash


 kevell@corp:/# ptconfigure package-manager pkg-install --package-name="ssh" --packager-name="apt" 

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
   ssh 
 0 upgraded, 1 newly installed, 0 to remove and 87 not upgraded. 
 Need to get 0 B/1,106 B of archives. 
 After this operation, 29.7 kB of additional disk space will be used. 
 Selecting previously unselected package ssh. 
 (Reading database ... 198126 files and directories currently installed.) 
 Preparing to unpack .../ssh_1%3a6.6p1-2ubuntu2_all.deb ... 
 Unpacking ssh (1:6.6p1-2ubuntu2) ... 
 Setting up ssh (1:6.6p1-2ubuntu2) ... 
 [Pharaoh Logging] Adding Package ssh from the Packager Apt executed correctly 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 


Pkg 確保
-----------------

Pkg は、システム サービスが実行されているか確認します。実行開始しない場合それ以外のしないでください。このコマンドによって、ユーザーは、システムが働くか、またはアイドル状態かどうかを識別できます。簡単なコマンドは扱い易いです。次のコマンドは、パッケージ マネージャーを介して確保するために使用されます。


.. code-block:: bash
    
	ptconfigure PackageManager ensure



 kevell@corp:/# ptconfigure package-manager pkg-ensure --package-name="mysql" --packager-name="apt" 


 [Pharaoh Logging] Package mysql from the Packager apt is already installed, so not installing 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptconfigure package-manager pkg-ensure --package-name="ssh" --packager-name="apt" 

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
  ssh 
 0 upgraded, 1 newly installed, 0 to remove and 87 not upgraded. 
 Need to get 0 B/1,106 B of archives. 
 After this operation, 29.7 kB of additional disk space will be used. 
 Selecting previously unselected package ssh. 
 (Reading database ... 198126 files and directories currently installed.) 
 Preparing to unpack .../ssh_1%3a6.6p1-2ubuntu2_all.deb ... 
 Unpacking ssh (1:6.6p1-2ubuntu2) ... 
 Setting up ssh (1:6.6p1-2ubuntu2) ... 
 [Pharaoh Logging] Adding Package ssh from the Packager Apt executed correctly 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 



Pkg 削除
-----------------

Pkg は、パッケージ マネージャーからパッケージを削除するコマンドを削除します。パッケージ マネージャーは、まずパッケージ マネージャーから削除したいパッケージを確認します。確認を求めます。[削除] オプションを使用しています。

.. code-block:: bash

 		ptconfigure PackageManager remove


利点
-------------

* 非大文字小文字を区別します。
* Ubuntu や CentOS で裕福な。
* パッケージの削除が可能です。
* パッケージ マネージャーをラップします。
* コマンドは簡単に使用

 

