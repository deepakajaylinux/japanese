=======
Boxify
=======


概要
-----------

このモジュールの封筒を作成してよくとして管理のボックスとしてユーザーのすべての主要な必要があります。このトピックでは、このモジュールを使用し、様々 な機能を使用して boxify する方法について議論します。


Helpコマンド
-------------------

Help コマンドを処理し、ボックスの様々 な機能を実行するためにこのモジュールを処理でユーザーをガイドします。アウト代替パラメーターを列挙し、様々 な機能を使用して、ボックスの変更の構文が強調表示されます。Boxify モジュールの下のヘルプ オプションの構文は、次に示す


.. code-block:: bash

	ptconfigure Boxify help


The syntax for declaring the help command is not case sensitive which is an added advantage. The following screenshot visualize you about the help command under boxify.

.. code-block:: bash


 kevell@corp:/# ptconfigure Boxify help 
 ****************************** 


  This command provides a generic Box Management wrapper around all of the Box Providers (Cloud and Otherwise) so that we have a 
  generic way to create and destroy boxes. 

  Boxify, boxify 

        - install-generic-autopilots 
        Install the generic Boxify autopilot templates for a Tiny or Medium (Current Default) set of Environments 
        example: ptconfigure boxify install-generic-autopilots 
        example: ptconfigure boxify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/boxify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

        - box-add 
        Installs a Box through a cloud provider 
        example: ptconfigure boxify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

        - box-remove 
        Removes a Box from the papyrus 
        example: ptconfigure boxify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

        - box-destroy 
        Removes a Box from both papyrus and the cloud provider 
        example: ptconfigure boxify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy 

        - list-papyrus 
        List all servers in papyrus, or those of a particular environment 
        example: ptconfigure boxify list-papyrus --yes 
        example: ptconfigure boxify list-papyrus --yes --environment-name="staging" 


 ------------------------------ 
 End Help 
 ****************************** 


boxifyの様々な機能
----------------------------------

このトピックについての様々 な機能について説明します下記のように、このモジュールの下に boxify

* ジェネリックのオート パイロットのインストール 
* 追加ボックス 
* 削除ボックス 
* 、ボックスを破棄する 
* リスト


一般的なオートパイロットをインストール
-------------------------------------------

この関数は、小さなまたは中程度の一連の環境に該当するオート パイロットのインストールが目指しています。これは、以下に示すようにコマンドを適用することによって実装できます。


.. code-block:: bash
	
	ptconfigure boxify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/boxify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 


上記の構文で示されているユーザーがある汎用のオート パイロットをインストールするために、次のフィールドを指定するには


* destination directory
* template-group


追加ボックス
--------------


単に次のコマンドを使用して、クラウド プロバイダーを通じてボックスを追加することを目的とするこの関数

.. code-block:: bash

	example: ptconfigure boxify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 


上記のコマンドで示されている次のフィールドを指定する必要があるユーザー


* environment name
* server prefix
* provider
* image id
* box amount （を追加するボックスの数を表す整数値をする必要があります)
* Force name (box name)
* parallax (それはオプションですが、1 つ以上のボックスを追加するときに使用することが
  できます)。


削除ボックス
------------------

この関数はパピルスから、ボックスを削除を目指します。これは、以下のコマンドを使用して実装することができます。


.. code-block:: bash

	ptconfigure boxify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

上記のコマンドで示されている次のフィールドを指定する必要があるユーザー


* environment name
* environment version
* provider

ボックスの破棄
---------------------

この関数はパピルスから、ボックスを削除を目指します。この関数は単に次のコマンドを使用して実装することができます。


.. code-block:: bash

	ptconfigure boxify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy

上記のコマンドは、特定の環境のすべてのボックスを破壊するために使用されます。


List
-------

この関数の主な目的は特定のパピルスまたは環境内のすべてのサーバーを外にリストアップします。すべてのサーバーをリストするための構文が表示されます、以下のよう


.. code-block:: bash

	ptconfigure boxify list-papyrus --yes --environment-name="staging"

上記のコマンドは、指定された環境のパピルスを一覧表示されます。


代替パラメータ
-----------------------------

これのいずれかの宣言で使用することができますこのモジュールの代替のパラメーターは、


* Boxify
* boxify


メリット
-----------

* ヘルプとボックスの他の操作で使用する構文の大文字と小文字は区別されません。
* それは裕福な両方セント OS とも Ubuntu のように。
* ボックスを管理するためのすべての主要な機能はこの単一モジュールの下にラップを取得します。

