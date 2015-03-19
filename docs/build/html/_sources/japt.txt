====
Apt
====

概要
-----------

この傾向モジュールの主な目的は、新しいAPTSを作成することですし、同様に既存のAPTSを修正することを目的としている。このモジュールは、ユーザの要件に基づいて、APTSにアクセスして変更するためのさまざまな機能の集合を有している。
今後のトピックにaptアクセスする際の、このモジュールの異なる側面についても、このモジュールを使用する方法を扱っています。

helpコマンド
-------------------

helpコマンドは、ユーザーが使用に関する意識し取得することが容易に簡単なユーザーマニュアルは、このモジュールを取り扱うの方法論は、異なる機能を実行することです。また、アウト宣言で使用できる代替パラメータを示します。それは、アプトの下で異なる機能を使用すると、アクセスするための構文の例を強調しています。

アプトの下のヘルプオプションの宣言に使用されるコマンドは、以下の通りです

.. code-block:: bash

	ptconfigure Apt help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、がち下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash

 kevell@corp:/# ptconfigure apt help
 ******************************


  This command allows you to modify create or modify apts

  Apt, apt

        - create
        Create a new system apt, overwriting if it exists
        example: ptconfigure apt create --aptname="somename"

        - remove
        Remove a system apt
        example: ptconfigure apt remove --aptname="somename"

        - set-password
        Set the password of a system apt
        example: ptconfigure apt set-password --aptname="somename" --new-password="somepassword"

        - exists
        Check the existence of a apt
        example: ptconfigure apt exists --aptname="somename"

        - show-groups
        Show groups to which a apt belongs
        example: ptconfigure apt show-groups --aptname="somename"

        - add-to-group
        Add apt to a group
        example: ptconfigure apt add-to-group --aptname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove apt from a group
        example: ptconfigure apt remove-from-group --aptname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

アプトの異なる特徴
---------------------------------

このトピックでは、このモジュールの下のaptの異なる特徴、そしてまた、これらのさまざまな機能を使用するには、可能な方法を扱っています。

傾向の下で、このモジュールの様々な態様は、以下に記載されている

* Create
* Remove
* set-password
* exists
* show-groups
* add-to-group
* remove-from-group


CREATE
-------------
この関数は、新しいシステムがやすい作成を目指し、そしてだけでなく、既存の例で上書きされます。このモジュールを使用しやすくするこの機能は、次の構文によって達成することができる

.. code-block:: bash

	ptconfigure apt create --aptname="somename"

aptnameの代わりに、ユーザは、作成される傾向の名前を指定することができる。上記の指定されたコマンドを入力した後は、apt新システムは、指定した名前で作成されます。

REMOVE
-----------

この機能は、既存のaptの除去を目的としています。このモジュールを使用しやすくするこの機能は、次の構文によって達成することができる

.. code-block:: bash

	ptconfigure apt remove --aptname="somename"

aptnameの代わりに、ユーザーが削除するのaptの名前を指定することができます。上記の指定されたコマンドを入力した後、指定されやすいが削除されます。


SET PASSWORD
--------------------

この関数は、要件に従ってやすいシステムに新しいパスワードを設定することが容易になります。これは、特定のコマンドを適用することによって行うことができる
以下に、

.. code-block:: bash

	ptconfigure apt set-password --aptname="somename" --new-password="somepassword"



この機能を実現するために、ユーザは、2つのフィールドを指定する必要があり、

* Apt name
* New password

上記のコマンドの形式で2つのフィールドが指定した後、指定されがちの新しいパスワードが作成されます。


EXISTS
-----------

この関数は、のaptの存在を確認することを目的としている。これは、以下のコマンドを使用して、簡単に行うことができる

.. code-block:: bash

	ptconfigure apt exists --aptname="somename"

上記のようにコマンドを適用した後、前述のaptの存在が結果と確保することとしております。

SHOWのグループ
--------------------

この機能により、ユーザーはグループがし易い属しないものにについて知って支援しています。これは、単純に以下のコマンドを使用することによって達成することができる

.. code-block:: bash

	ptconfigure apt show-groups --aptname="somename"

ユーザは、そのグループの詳細を知るために、aptname分野においてやすいの名前を指定する必要がある。

ADD _TO_GROUP
-----------------------

この機能の主な目的は、下記のように単純にコマンドを適用することによって、必要なグループに必要な傾向を追加することで、

.. code-block:: bash

	ptconfigure apt add-to-group --aptname="somename" --groupname="somegroupname"

この機能を実現するために、ユーザは、上記のコマンドの形式で自分のニーズに従って以下の二つのフィールドを指定する必要があり、

* Aptname
* group name

REMOVE_FROM_GROUP
--------------------------------

この機能の主な目的は、下記のように単純にコマンドを適用することによってグループからやすくを除去することで、

.. code-block:: bash

	ptconfigure apt remove-from-group --aptname="somename" --groupname="somegroupname"

この機能を実現するために、ユーザは、上記のコマンドの形式で自分のニーズに従って以下の二つのフィールドを指定する必要があり、

* Aptname
* group name

別のパラメータ
-----------------------------

宣言で使用することができるいずれかがこのモジュールの別のパラメータであり、

* Apt
* apt

メリット
-----------

* ヘルプとのaptの他のさまざまな機能を宣言に使用されるパラメータは、大文字と小文字は区別されません。
* これは、裕福な両方セントOSのと同様にUbuntuののようである。
* このモジュールを使用すると、ユーザーが作成し、同様に彼らのニーズに従ってがちを変更することができます。
* 傾向の存在は、このモジュールの下に確保することができる。
