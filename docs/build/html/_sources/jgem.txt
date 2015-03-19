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

        - create
        Create a new system gem, overwriting if it exists
        example: ptconfigure gem create --gemname="somename"

        - remove
        Remove a system gem
        example: ptconfigure gem remove --gemname="somename"

        - set-password
        Set the password of a system gem
        example: ptconfigure gem set-password --gemname="somename" --new-password=                                                                                        "somepassword"

        - exists
        Check the existence of a gem
        example: ptconfigure gem exists --gemname="somename"

        - show-groups
        Show groups to which a gem belongs
        example: ptconfigure gem show-groups --gemname="somename"

        - add-to-group
        Add gem to a group
        example: ptconfigure gem add-to-group --gemname="somename" --groupname="so                                                                                        megroupname"

        - remove-from-group
        Remove gem from a group
        example: ptconfigure gem remove-from-group --gemname="somename" --groupnam                                                                                        e="somegroupname"

 ------------------------------
 End Help
 ******************************

宝石の異なる特徴
---------------------------------

上記のhelpコマンドから示されているように、宝石の様々な特徴は以下のように記載されている、

* Create 
* Remove
* Set Password
* Exists
* Show_groups
* Add_to_group
* Remove_from_group

私たちはこれらの機能について詳細に見てみましょう。

作る
--------

この関数は、新しいシステムの宝石を作成することを目的、とだけでなく、既存の例で上書きされます。このモジュールを使用して、宝石のこの機能は、次の構文によって達成することができる

.. code-block:: bash

	ptconfigure gem create --gemname="somename"

gemnameの代わりに、ユーザーが作成される宝石の名前を指定することができます。上記の指定されたコマンドを入力した後、新たな宝石は、指定した名前で作成されます。

REMOVE
-------------

この関数は、既存の宝石を削除することを目指しています。このモジュールを使用して、宝石のこの機能は、次の構文によって達成することができる

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

gemnameの代わりに、ユーザーが削除する宝石の名前を指定することができます。上記の指定されたコマンドを入力した後、指定された宝石が削除されます。


SET PASSWORD
--------------------

この機能は、要件に応じて、システムの宝石に新しいパスワードを設定することが容易になります。これは、下記のようにコマンドを適用することによって行うことができる

.. code-block:: bash

	ptconfigure gem set-password --gemname="somename" --new-password="somepassword"

この機能を実現するために、ユーザは、2つのフィールドを指定する必要があり、

* Gem name
* New password

上記のコマンドの形式で2つのフィールドが指定した後、指定された宝石の新しいパスワードが作成されます。


EXISTS
--------

この関数は、宝石の存在を確認することを目的としている。これは、以下のコマンドを使用して、簡単に行うことができる

.. code-block:: bash

	ptconfigure gem exists --gemname="somename"

上記のようにコマンドを適用した後、前述の宝石の存在が結果と確保することとしております。

SHOWのグループ
------------------------

この機能により、ユーザーはへのグループについて知って支援する宝石が所属ん。これは、単純に以下のコマンドを使用することによって達成することができる

.. code-block:: bash

	ptconfigure gem show-groups --gemname="somename"

ユーザーは、そのグループの詳細を知るために、gemnameの分野で宝石の名前を指定する必要があります。

Add_TO_GROUP
-----------------------

この関数の主な目的は、下記のように単純にコマンドを適用することにより、必要なグループに必要な宝石を追加することです、

.. code-block:: bash

	ptconfigure gem add-to-group --gemname="somename" --groupname="somegroupname"

この機能を実現するために、ユーザは、上記のコマンドの形式で自分のニーズに従って以下の二つのフィールドを指定する必要があり、

* Gemname
* group name

REMOVE_FROM_GROUP
-------------------------------------

この機能の主な目的は、下記のように単純にコマンドを適用することによってグループから宝石を除去することで、

.. code-block:: bash

	ptconfigure gem remove-from-group --gemname="somename" --groupname="somegroupname"

この機能を実現するために、ユーザは、上記のコマンドの形式で自分のニーズに従って以下の二つのフィールドを指定する必要があり、

* Gemname
* group name

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
