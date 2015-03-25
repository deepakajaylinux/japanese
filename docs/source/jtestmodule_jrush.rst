=============
Test module
=============

概要
--------------

テストケースはテスト モジュールのファイル拡張子についてこのチェックとして、最も人気のある jrush のそれを使用します。テストケースのフレームワークでは、テストの他の記事と組み合わせて使用することができます。この結果、テストケースのみ残してより具体的かつ高度な機能を実装する他のライブラリ関数のテスト ベースラインを提供します。現在のアクションが表示されます。これは、Ubuntu や centOS で快適です。

Helpコマンド
-----------------------

ヘルプ コマンド同様目的に関してユーザーのガイドとして、テストケースに含まれているオプションについて。テストケースの代替パラメーターを示します。また、Jrush モジュールの機能の構文について説明します。テストケースのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		jrush testmodules help

コマンドの入力後それとしてアクション オプションを示します。次のイメージは、明らかにそれを視覚化します。

.. code-block:: bash

 kevell@corp:/# jrush TestModule help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update TestModule.

  TestModule, testmodule, test-module

        - action-one
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-one

        - action-two
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-two

 ------------------------------
 End Help
 ****************************************



代替パラメータ
--------------------------------

またユーザーのテストケースを使用して、次のオプションを利用できます。

Test Module, testmodule, test-module.

オプション
-------------

2 つのオプションが利用できます。彼らの次のとおりです。

* Action-one
* Action-two

Action-one
-----------------

記事の現在のタイトルが表示されます。1 つのアクションを行うに使用するコマンドは次のように、

.. code-block:: bash

		jrush test-module action-one

与えるコマンドは、それを示して後現在の詳細と記事のタイトル。スクリーン ショットは、同じを表します。

.. code-block:: bash

 kevell@corp:/# jrush test-module action-one --config-file="/var/www/html/joomla/configuration.php"
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 TestModule Action One:
 -------------------------
 array(6) {
  [0]=>
  string(8) "About Us"
  [1]=>
  string(15) "Article 1 Title"
  [2]=>
  string(18) "Creating Your Site"
  [3]=>
  string(9) "article-1"
  [4]=>
  string(9) "article-2"
  [5]=>
  string(9) "article-3"
 }

 ------------------------------
 TestModule Action One Finished
 ****************************************



Action-two
-----------------

記事の現在のタイトルが表示されます。1 つのアクションを行うに使用するコマンドは次のように、

.. code-block:: bash

		jrush testmodule action-two

与えるコマンドは、それを示して後現在の詳細と記事のタイトル。


メリット
----------------

* 正しい方法で、モジュールを確認してください。
* 非大文字小文字を区別します。
* より時間がかかる。
* 簡単にサイトをアップグレードするより安い。
* 最新アップデートが利用可能 
* Ubuntu や centOS を使用するに適しています。


