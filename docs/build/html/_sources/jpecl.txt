=====
PECL
=====

あらすじ
----------------

PECL 正エミッタ結合論理」の略です。Pecl は差動ロジック出力高速クロック分配回路でよく使用されます。このコマンドは、作成、削除、setpassward、ユーザーが存在します。グループの活動はこのコマンドを使っても可能。このコマンドの主な機能は、システムに基づいています。Ubuntu や CentOS を適しています。

ヘルプ コマンド
----------------------

Pecl パッケージの開発は非常に簡単になります: それはで動作が存在する、修正、作成、システム pecl の設定パスワードをサポートします。Pecl、パッケージの変更されるユーザーの既定のレイアウトするたびに、ユーザーが大量のコードを書いたはそう簡単になります。

.. code-block:: bash

		ptconfigure pecl help


次のスクリーン ショットでは、その機能について説明します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PECL help

 ******************************


  This command allows you to modify create or modify pecls

  PECL, pecl

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************



作成します。
------------

このコマンドを使用すると新しいシステム pecl を作成することができます。上書きが存在場合可能です。新しい pecl 名前は単一コマンド自体に言及することができます。

作成するために使用されるコマンドのとおりです。


.. code-block:: bash

		ptconfigure pecl create 

上記のコマンドとして入力後、それ pecl の作成を開始します。ファイルの場合既存の指示メッセージが表示されます。スクリーン ショットは、コマンドとその機能について説明します。


.. code-block:: bash

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"


削除
------------

このコマンドを使用すると、pecl を削除することができます。リムーバブル pecl 名前は単一コマンドライン自体に言及することができます。
作成するために使用されるコマンドのとおりです。


.. code-block:: bash

		ptconfigure pecl remove 



開始後の上記のコマンドとして入力、pecl の取り外し。ファイル、pecl から既に削除した場合を示すメッセージが表示されます。スクリーン ショットは、コマンドとその機能について説明します。


.. code-block:: bash

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"



設定するパスワード
--------------------

Setpassward は、モジュールを pecl で root 権限で特定のコマンドを実行に使用されます。興味深いは、ユーザー パスワードを使用して、特定のコマンドと、システムの現在のユーザーのパスワードをユーザーを要求します。作成するために使用されるコマンドのとおりです。


.. code-block:: bash

	ptconfigure pecl  set-passward


Pecl 名と新しいパスワードが同じコマンド行に言及も。これにより、このモジュールの別の利点。次のスクリーン ショットは、その機能を視覚化します。


.. code-block:: bash

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"



存在します。
-------------

このコマンドは、pecl の存在を確認するために使用します。単純なコマンドは、このコマンドが正常に動作します。まずそれシステム pecl 名をチェックし、それかどうか既存かどうかを示します。次のコマンドはこの機能を実行するために使用


.. code-block:: bash

		ptconfigure pecl Exists


次のスクリーン ショットは、その機能を視覚化します。

.. code-block:: bash

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"


グループを表示します。
------------------------

このコマンドは、pecl の作業グループをチェックするために使用します。単純なコマンドは、このコマンドが正常に動作します。まずグループ名 pecl 名の順にチェックイン システム、pecl が属しているグループ名を示していて、。次のコマンドはこの機能を実行するために使用します。


.. code-block:: bash

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"


グループへの追加
------------------------

これは、pecl をグループに追加するユーザーを容易にします。追加するときそれは pecl 名とグループ名を要求することができます。よると、ユーザーが入力できる彼らの願いを。


.. code-block:: bash
   
		ptconfigure pecl add-to-group



コマンドの入力後それはグループでは pecl を追加します。


.. code-block:: bash

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"


グループからの削除
----------------------------

このコマンドを使用すると、pecl グループから削除することができます。リムーバブル pecl 名前は単一コマンドライン自体に言及することができます。
作成するために使用されるコマンドのとおりです。


.. code-block:: bash

		ptconfigure pecl remove-from-group 



開始後の上記のコマンドとして入力、pecl グループから削除します。ファイル、pecl から既に削除した場合を示すメッセージが表示されます。スクリーン ショットは、コマンドとその機能について説明します。


.. code-block:: bash

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"


利点
----------------

* 非大文字小文字を区別します。
* Ubuntu や CentOS で裕福な。
* 低消費電力。
* 新しいシステム pecl を作成します。
* 削除、pecl
* 追加のグループ化が可能です。
* 削除グループが可能です。
* ショー グループが可能です。

 
