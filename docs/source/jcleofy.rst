=======
Cleofy
=======

概要
-----------

このモジュールは、彼らのプロジェクトのためにオートパイロットファイルの標準セットを作成する際に、ユーザーが容易にすることを目的。私たちは今後の話題からcleofyの関数についても、このモジュールを使用し、方法を見てみましょう。

helpコマンド
--------------------

helpコマンドは、ユーザーが使用に関する意識し取得することが容易に簡単なユーザーマニュアルは、このモジュールを取り扱うの方法論は、異なる機能を実行することです。また、アウト宣言で使用できる代替パラメータを示します。それはcleofy下に異なる機能を使用すると、アクセスするための構文の例を強調しています。

cleofy下のヘルプオプションの宣言に使用されるコマンドは、以下の通りです

.. code-block:: bash

	ptconfigure cleofy help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、cleofy下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/ptconfigure/autopilots        
	example: ptconfigure cleofy list        

 - standard        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
	example: ptconfigure cleofy standard        

 - tiny        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "tiny" style infrastructure.        	example: ptconfigure cleofy tiny        

 - medium        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure.        	example: ptconfigure cleofy medium        

 - medium-web        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: ptconfigure cleofy medium-web        

 - db-cluster        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
 	example: ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: ptconfigure cleofy install-generic-autopilots        
	example: ptconfigure cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    

 ------------------------------
 End Help
 ******************************



cleofyの機能
------------------------

以下に示すようにこのトピックでは、このモジュールの下cleofyのさまざまな機能について示している

* List
* Standard
* Tiny
* Medium
* Medium-web
* DB-cluster
* Install_generic_autopilots

リスト
-----------

この関数は、指定した場所（ビルド/設定/ ptconfigure /オートパイロット）内のすべての自動操縦のファイルをリストすることを目的。この機能を適用するための構文は、以下に示す

.. code-block:: bash

	ptconfigure cleofy list

スタンダード
---------------------

ユーザのプロジェクトのために（ビルド/設定/ ptconfigure /オートパイロットで）ptconfigureのオートパイロットのデフォルトセットを作成する際にこの機能を支援。この機能は、単に以下のコマンドを使用して適用することができる

.. code-block:: bash

	ptconfigure cleofy standard

.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy standard

 Cleofy This? (Y/N) 
 y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 test1
 Value for: Default Temp Dir (should usually be /tmp/)

 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-cleo-dapper.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-new.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-update.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-any-box.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-ubuntu.php
 ******************************


 Success
 In Cleofy
 ******************************





小さな
----------

この関数は、小さなインフラのプロジェクトのために（ビルド/設定/ ptconfigure /オートパイロットで）ptconfigureのオートパイロットのデフォルトセットを作成することを目指しています。この機能を実装するには、以下のように次のコマンドを使用し、

.. code-block:: bash

	ptconfigure cleofy tiny

メディア
-----------

この機能は、メディアインフラのプロジェクトのために（ビルド/設定/ ptconfigure /オートパイロットで）ptconfigureのオートパイロットのデフォルトセットを作成することを目指しています。この機能を実装するには、以下のように次のコマンドを使用し、

.. code-block:: bash

	ptconfigure cleofy medium

Medium_Web
-------------------

この機能は、メディアウェブとインフラではなく、データベースとのプロジェクトのために（ビルド/設定/ ptconfigure /オートパイロットで）ptconfigureのオートパイロットのデフォルトセットを作成することを目指しています。この機能を実装するには、以下のように次のコマンドを使用し、

.. code-block:: bash

	ptconfigure cleofy medium-web

DB_cluster
---------------

この機能は、ユーザーがプロジェクトのptconfigureのオートパイロットのデフォルトセット（ビルドで/ configに/ ptconfigure /オートパイロット）を作成することを目指しています。

この機能を実装するには、以下のように次のコマンドを使用し、

.. code-block:: bash

	ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

Install_generic_autopilots
--------------------------------

与えられたように、この関数は単にコマンドを使用して、環境の小さなまたは媒体セットの汎用オートパイロットテンプレートをインストールするのに役立つ
以下に、

.. code-block:: bash
	
	ptconfigure cleofy install-generic-autopilots        
Or  

.. code-block:: bash

	ptconfigure cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    

上記のようにコマンドを実装するには、ユーザーは、リストされているとして、次のフィールドを指定する必要が

* destination dir
* template group

別のパラメータ
-----------------------------

宣言で使用することができるいずれかがこのモジュールの別のパラメータであり、

* Cleofy, 
* cleofy

メリット
-------------

* ヘルプとのaptの他のさまざまな機能を宣言に使用されるパラメータは、大文字と小文字は区別されません。
* これは、裕福な両方セントOSのと同様にUbuntuののようである。
* このモジュールは、オートパイロットの標準セットを作成する際に、プロジェクトのすべてのニーズを包み込む。
