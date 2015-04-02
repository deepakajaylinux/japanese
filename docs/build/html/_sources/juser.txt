=======
User
=======

概要
-------------

ユーザーは、コンピューターを使用して誰です。コンピューターに作成すると、各アカウントの名前があり、この名前が、人の上昇、コンピューターへのアクセス。一部のシステム サービスも制限された、または特権を持つユーザー アカウントを使用して実行します。


ユーザーの管理は、ある特定の方法でアクセスを制限することによってセキュリティを目的として行われます。スーパー ユーザー (root) は、オペレーティング システムとその構成へのアクセスを完了管理目的使用のみのものです。特権を持たないユーザー制御特権エスカレーションの su と sudo のプログラムを使用できます。

システム管理の基本的な部分は構成およびユーザーとグループの管理します。このタスクの一部には、すべてのシステム エンティティの機能・ ログの監視が含まれます。

私たちは、Ubuntu の 12.04 VPS にこれらの概念が模索されますが、必須の最新の Linux ディストリビューションにたどることができます。


Helpコマンド
----------------------

このコマンドは、ユーザー モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
        
        ptconfigure user help


上記のコマンドのためのスクリーンショットは、以下に記載されている

.. code-block:: bash



 kevell@corp:/# ptconfigure user help
 ******************************
  
 This command allows you to modify create or modify users
 
 User, user

        - create
        Create a new system user, overwriting if it exists
        example: ptconfigure user create --username="somename"

        - remove
        Remove a system user
        example: ptconfigure user remove --username="somename"

        - set-password
        Set the password of a system user
        example: ptconfigure user set-password --username="somename" --new-password="somepassword"

        - exists
        Check the existence of a user
        example: ptconfigure user exists --username="somename"

        - show-groups
        Show groups to which a user belongs
        example: ptconfigure user show-groups --username="somename"

        - add-to-group
        Add user to a group
        example: ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

        - remove-from-group
        Remove user from a group
        example: ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

Create 
--------

ユーザーは新しいシステム ユーザー アカウントを作成する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
        
        ptconfigure user create --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user create
 
 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************

Remove
------------

ユーザーはシステムのユーザー アカウントを削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
  	
 	ptconfigure user remove --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user remove

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Set-password
--------------------

ユーザーはシステムのユーザーのパスワードを設定する必要がある場合、特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
  	
	ptconfigure user set-password --username="somename" --new-password="somepassword"

.. code-block:: bash

 kevell@corp:/# ptconfigure user set-password

 Enter Username:
 kevell
 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************


Exists
--------------------

ユーザー、ユーザーの存在を確認する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
        
        ptconfigure user exists --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user exists

 Enter Username:
 kevell
 ****************************** 


 User Modifications:
 --------------------------------------------

 User: Success = User Exists
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure user exists

 Enter Username:
 karuna
 ******************************


 User Modifications:
 --------------------------------------------

 User: Failure - User Does Not Exist
 User Name: 

 ------------------------------
 User Mods Finished
 ******************************

Show-groups 
--------------------

ユーザー、ユーザーが属するグループを表示する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash    

	ptconfigure user show-groups --username="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure user show-groups

 Enter Username:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: kevell


 ------------------------------
 User Mods Finished
 ******************************


Add-to-group 
--------------------

ユーザーは、グループにユーザーを追加する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash    
 	
	ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

.. code-block:: bash

 kevell@corp:/# ptconfigure user add-to-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell
 ******************************


 User Modifications:
 --------------------------------------------

 User: 1

 ------------------------------
 User Mods Finished
 ******************************


Remove-from-group 
-------------------------

ユーザー、グループからユーザーを削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash    
 	
	ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

.. code-block:: bash

 kevell@corp:/# ptconfigure user remove-from-group --username="kevell" --groupname="kumar"

 Enter New Password:
 kevell

 /usr/sbin/deluser: You may not remove the user from their primary group.
 [Pharaoh Logging] [User] Removing User kevell from the Group kevell did not execute correctly
 ******************************


 User Modifications:
 --------------------------------------------

 User: 

 ------------------------------
 User Mods Finished
 ******************************


代替パラメータ
--------------------------------

2 つの代替パラメーターをコマンドラインで使用することができますがあります。

User, user 

例: ptconfigure User help /ptconfigure user help


メリット
--------------

Linux 上でユーザ認証はシステム管理の比較的柔軟な領域です。非常に単純なツールと同じ目的を達成する多くの方法があります。



