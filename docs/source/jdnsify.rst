========
Dnsify
========

概要
-----------

これは封筒にDNSを管理するユーザのすべての主要なニーズをモジュール。このトピックでは、このモジュールを使用する方法について、およびdnsify使用する際のさまざまな機能について議論することです。

helpコマンド
-------------------

helpコマンドは、ハンドルとボックスの様々な機能を実行するために、このモジュールの取り扱いにユーザを導く。これは、別のパラメータアウトをリストし、使用してボックスを変更するさまざまな機能の構文を強調しています。 dnsifyモジュールの下のヘルプオプションの構文は次のようになり、

.. code-block:: bash

	ptconfigure DNSify help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、dnsify下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash


 kevell@corp:/# ptconfigure Dnsify help 
 ****************************** 


  This command provides a generic Box Management wrapper around all of the Box Providers (Cloud and Otherwise) so that we have a 
  generic way to create and destroy boxes. 

  DNSify, dnsify 

        - install-generic-autopilots 
        Install the generic Dnsify autopilot templates for a Tiny or Medium (Current Default) set of Environments 
        example: ptconfigure dnsify install-generic-autopilots 
        example: ptconfigure dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

        - box-add 
        Installs a Box through a cloud provider 
        example: ptconfigure dnsify box-add --environment-name="*environment*" 
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
        example: ptconfigure dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

        - box-destroy 
        Removes a Box from both papyrus and the cloud provider 
        example: ptconfigure dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy 

        - list-papyrus 
        List all servers in papyrus, or those of a particular environment 
        example: ptconfigure dnsify list-papyrus --yes 
        example: ptconfigure dnsify list-papyrus --yes --environment-name="staging" 


 ------------------------------ 
 End Help 
 ****************************** 

dnsifyの様々な機能
----------------------------------

以下に示すように、このトピックは、このモジュールの下dnsifyのさまざまな機能について説明します



* Install generic autopilots
* Adding box
* Removing box
* Destroying a box
* list

一般的なオートパイロットをインストール
----------------------------------------------------------------

この関数は、環境の小さなまたは中規模セットに適用可能なオートパイロットをインストールすることを目指しています。これは、下記のようにコマンドを適用することによって実現することができる

.. code-block:: bash
	
	ptconfigure dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

上記の構文に示すように、ユーザは、一般的なオートパイロットをインストールするために、次のフィールドを指定する必要があります。

* destination directory
* template-group

ボックスの追加
------------------------


この機能は、単に次のコマンドを使用して、クラウド·プロバイダーを通じてボックスを追加することを目的とし、

.. code-block:: bash

 example: ptconfigure dnsify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

ユーザーは、上記のコマンドに示すように、次のフィールドを指定する必要が

* environment name
* server prefix
* provider
* image id
* box amount（ボックスの数を表す整数値である必要があります追加する）
* Force name（ボックス名）
* parallax（それは、複数のボックスを追加する際に使用することができ、任意である。）


削除ボックス
------------------


この関数は、パピルスからボックスを削除することを目指しています。これは、以下のコマンドを使用して実施することができる

.. code-block:: bash

	ptconfigure dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

ユーザーは、上記のコマンドに示すように、次のフィールドを指定する必要が

* environment name
* environment version
* provider

ボックスの破棄
------------------------

この関数は、パピルスからボックスを削除することを目指しています。この関数は、次のコマンドを使用して簡単に実装することができ、

.. code-block:: bash

	ptconfigure dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy

上記のコマンドは、特定の環境のすべてのボックスを破壊するために使用される。

リスト
---------

この関数の主な目的は、特定のパピルスのか、環境内のすべてのサーバーをリストすることです。すべてのサーバをリストするための構文は、以下の通りである
.. code-block:: bash

	ptconfigure dnsify list-papyrus --yes --environment-name="staging"

上記のコマンドは、指定された環境のパピルスを一覧表示されます。

別のパラメータ
-----------------------------

宣言で使用することができるいずれかがこのモジュールの別のパラメータであり、

* DNSify
* dnsify

メリット
-----------

* ボックスのヘルプや他の操作で使用される構文は、大文字と小文字は区別されません。
* これは、裕福な両方セントOSで、同様のUbuntuのようです。
* DNS管理でボックスを管理するためのすべての主要な機能は、この単一のモジュールの下に包まれます。
