============
Rackspace
============

概要
-------------

ラック スペース雲で成功するために高パフォーマンスで信頼性の高いインフラストラクチャを提供します。フル機能、最適化されたプラットフォームとワークロードを実行する専門家のチームがかかります。

Rackspace は 2 つの主な基幹業務のクラウド サーバーと専用サーバー。ラック スペースを設計、構築、お客様の個々 のニーズに応じて両方の環境にわたってワークロードを動作ことができます。

クラウド サーバー - 管理インフラストラクチャ サービス レベルは、クラウドでは、アーキテクチャのアドバイス、安全保障の支援を通じて Api と Sdk) コード開発支援など顧客をセットアップに必要なサービスのコア セットを提供します。管理操作のサポートのレベルはすべて管理インフラストラクチャ サービスに加えて、追加のプロアクティブ ・ サポートを提供します。

プロアクティブなサービスは提供されるオン デマンド サポートの専用サーバ - 管理されたサービス レベルで構成されます。



Helpコマンド
----------------------

This command helps to determine the usage of Rackspace. The user will come to know about the different way/format to execute this module. This command guides the end user to know the purpose of this command. Below given are the command and the screenshot of the same. 

.. code-block:: bash


 kevell@corp:/# ptconfigure Rackspace help

 ******************************


    This is an extension provided for Handling Servers on Rackspace.

    Rackspace, rackspace

        - box-add
        Lets you add boxes to Rackspace, and adds them to your papyrusfile
        example: ptconfigure rackspace box-add
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your Rackspace account - Careful - its irreversible
        example: ptconfigure rackspace box-destroy-all --yes --guess

        - save-ssh-key, sshkey, ssh-key
        Will let you save a local ssh key to your Rackspace account, so you can ssh in to your nodes with it
        securely and without a password
        example: ptconfigure rackspace save-ssh-key
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - list
        Will display data about your Rackspace account
        example: ptconfigure rackspace list
        example: ptconfigure rackspace list --yes
                    --guess # use project saved connection details if possible
                    --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

        - list-containers
        Will display Container data about your Rackspace account
        example: ptconfigure rackspace list-containers
        example: ptconfigure rackspace list-containers --yes
                    --guess # use project saved connection details if possible

        - list-objects
        Will display object of Containers data about your Rackspace account
        example: ptconfigure rackspace list-objects
        example: ptconfigure rackspace list-objects --yes
                    --guess # use project saved connection details if possible

 ------------------------------
 End Help
 ******************************


Box-add
----------------

このコマンドは、ラック スペースにボックスを追加することができ、パピルス ファイルに追加します。特定のコマンドの下、プロセスが実行されます。
.. code-block:: bash

 ptconfigure rackspace box-add --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box-destroy 
-------------------

このコマンドは、ボックス/es で環境を破壊してパピルス ファイルからそれらを削除に役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash

 ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box-destroy-all
---------------------

このコマンドは、Rackspace アカウントにすべての箱を破壊するのに役立ちます。最も重要な部分はリバーシブルではないです。

.. code-block:: bash     

 ptconfigure rackspace box-destroy-all --yes --guess

Save-ssh-key 
---------------------

このコマンドは、ローカル ssh キー保存、Rackspace アカウントにすることができます ssh でそれをあなたのノードをしっかりとパスワードなしに役立ちます。-Ssh キーから、ssh キーはこの特定のコマンドを使用する 3 つの代替パラメーターがあります。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     
	
	ptconfigure rackspace save-ssh-key --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"


List 
---------------------

このコマンドは、Rackspace アカウントに関するデータに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 
	
	ptconfigure rackspace list
        
.. code-block:: bash 

	ptconfigure rackspace list --yes --guess # use project saved connection details if possible --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

List-containers 
---------------------

このコマンドは、コンテナー、Rackspace アカウントに関するデータを表示するのに役立ちます。特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash 
	
 	ptconfigure rackspace list-containers

.. code-block:: bash 

	ptconfigure rackspace list-containers --yes --guess # use project saved connection details if possible


List-objects
---------------------

このコマンドは、Rackspace アカウントについてコンテナー データ オブジェクトを表示するのに役立ちます。特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash 

 	ptconfigure rackspace list-objects

.. code-block:: bash 

	ptconfigure rackspace list-objects --yes --guess # use project saved connection details if possible

代替パラメータ
------------------------------       

2 つの代替パラメーターをコマンドラインで使用することができますがあります。

Rackspace, rackspace


メリット
--------------

Rackspace はバックアップおよび MySQL のワークロードに特化したエンジニアによってサポートされているリレーショナル データベース用に設計された高性能、特化したインフラストラクチャ要求の厳しい顧客のための完全なソリューションを提供します。Rackspace は、アプリケーションの開発に焦点を当てるし、基盤となるインフラストラクチャについて心配しないでを希望お客様のため完全に管理されたサービスです。オン デマンド ・ バックアップとリストアに関するサービス提供しています統合監視、冗長ストレージ成長するスケーラビリティに基づいてアプリケーションのニーズとあなたのデータベースに対するフル コントロール。
