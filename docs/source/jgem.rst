=====
Gem
=====

概要
-----------

このモジュールは、GEMを操作するためのユーザーのすべてのニーズを包み込む。これは、さまざまな機能をカバーし、手で実行される様々な機能を促進する。
RubyGemsのは、Rubyのプログラムとライブラリを配布するための標準フォーマットを提供するRubyプログラミング言語用のパッケージマネージャで、簡単に宝石のインストールを管理するように設計されたツール、およびサーバー用の（自己完結型の形式で「宝石」と呼ばれる）それらを配布。
私たちはさまざまな機能とどのように今後のトピックからこのモジュールを使用するを見てみましょう。

helpコマンド
-------------------

helpコマンドは、目的やさまざまな機能、およびそれらの様々な機能を実装するための構文についてユーザーに指示します。また、アウト宣言で使用できる代替パラメータを示します。このモジュールの下にヘルプオプションを適用するための構文形式は、以下に示す

.. code-block:: bash

	ptconfigure gem help

次のスクリーンショットは、このモジュールの下にヘルプオプションの出力と作業を視覚化する。

.. code-block:: bash


 kevell@corp:/# ptconfigure gem help
 ******************************


  This command allows you to modify create or modify gems

  Gem, gem

        - install
        Install
        example: ptconfigure gem pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure gem pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure gem pkg-ensure --package-name="somename"

        - update
        Update
        example: ptconfigure gem update



 ------------------------------
 End Help
 ******************************


宝石の異なる特徴
---------------------------------

上記のhelpコマンドから示されているように、宝石の様々な特徴は以下のように記載されている、

* Install
* Remove
* Ensure
* Update



私たちはこれらの機能について詳細に見てみましょう。

Install
-----------

この機能は、ユーザーが必要なパッケージをインストールすることができます。次のスクリーンショットは出力を視覚化する、


.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-install --package-name=cucumber
 Successfully installed cucumber-2.0.0
 1 gem installed
 Installing ri documentation for cucumber-2.0.0...
 Installing RDoc documentation for cucumber-2.0.0...
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


REMOVE
-------------

この関数は、既存の宝石を削除することを目指しています。このモジュールを使用して、宝石のこの機能は、次の構文によって達成することができる

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

gemnameの代わりに、ユーザーが削除する宝石の名前を指定することができます。上記の指定されたコマンドを入力した後、指定された宝石が削除されます。

.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-remove --package-name=cucumber
 Removing cucumber
 Successfully uninstalled cucumber-2.0.0
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Failure

 ------------------------------
 Gem Mods Finished
 ****************************** 



Ensure
---------


この関数は、パッケージが、マシンに正しくインストールされている保証します。

.. code-block:: bash

	ptconfigure gem pkg-ensure --package="ssh"

.. code-block:: bash


 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 true
 [Pharaoh Logging] Package cucumber from the Packager Gem is Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 false
 [Pharaoh Logging] Package cucumber from the Packager Gem is not Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************



別のパラメータ
-----------------------------

宣言で使用することができるいずれかがこのモジュールの別のパラメータであり、

* Gem
* gem

メリット
-------------

* ヘルプと宝石の他のさまざまな機能を宣言に使用されるパラメータは、大文字と小文字は区別されません。
* これは、裕福な両方セントOSのと同様にUbuntuののようである。
* ユーザーが作成し、同様に彼らのニーズに従って宝石を変更することができ、このモジュールを使用する。
* 宝石の存在は、このモジュールの下に確保することができる。
