===============
JArticle
===============

概要
-------------

それは jarticle の詳細を管理します。これは、記事をモジュールとして使用することができます。Joomla は、異なる種類のコンテンツを作成するため、あなたのウェブサイトを構築するためのオプションの広い範囲を提供します。

Joomla、アーティクルはおそらくその他のリソース (画像など) へのリンクとテキストで構成されるコンテンツの一部です。記事コンテンツ システムとコンテンツの階層の最下位レベルでの情報の基本的単位であります。各記事は正確に 1 つのカテゴリです。カテゴリ別のカテゴリ、サブ カテゴリを作ることができます。未分類の記事を持って可能です。これらの記事がなければ任意のカテゴリに関連付けられています。


Helpコマンド
----------------------

このコマンドは、jarticle モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        jrush  jarticle help


.. code-block:: bash

 kevell@corp:/# jrush  jarticle help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla JArticles (Component, Module or Plugin).

  JArticle, jarticle

        - disable
        Deletes a jarticle
        example: jrush jarticle disable

        - enable
        Enables a jarticle
        example: jrush jarticle enable

        - info
        Display the details of a jarticle
        example: jrush jarticle info


 ------------------------------
 End Help
 ****************************************



Enable
----------------

ユーザーは、特定の記事を有効にする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush jarticle enable ..config file=”bootstrap file path”

Info
------

ユーザーは記事の情報を知る必要がある場合。下コマンドを考えるに役立つ

.. code-block:: bash
        
	        jrush jarticle info ..config file=”bootstrap file path”


上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# jrush jarticle info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JArticle ID. To enter title/alias/asset-id use --jarticle-title, --jarticle-alias or --jarticle-asset-id parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JArticle Information:
 -------------------------

 Article ID: 2
 Asset ID: 35
 Alias: about-us
 Title: About Us
 Created By: 825
 Created By Alias: Joomla
 State: 1
 ------------------------------
 JArticle Manage Finished
 ****************************************


Disable
----------------

ユーザーは特定の記事を無効にする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush jarticle disable ..config file=”bootstrap file path”

代替パラメータ
----------------------------

2 つの代替のパラメーターのいずれかのコマンドで使用できます。

jarticle, JArticle

eg:  jrush jarticle disable/ jrush JArticle disable                                 




メリット
--------------

* あなたの記事を整理するためのオプションの方法を提供するため 
* いくつかのテキストが含まれていて、写真や他のコンテンツ タイプに含めることができます * 簡単な方法でアーティクルに関する情報を取得する
  ことができます 
* を有効にして 1 つのステップで記事を無効にすることができます


