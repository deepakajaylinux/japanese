============
Pear
============

あらすじ
-------------

梨は、略して「PHP 拡張子とアプリケーション リポジトリ」と、フルーツのようなちょうど発音されます。PEAR の目的は提供します。

* PHP のユーザ用のオープン ソース コードの構造化されたライブラリ
* コード配布およびパッケージ管理システム
* ここで指定した PHP で書かれたコードの標準スタイル
* PHP 拡張コミュニティ ライブラリ (PECL)


PEAR のミッションは、再利用可能なコンポーネントを提供する、PHP の技術革新をリード、PHP 開発のためのベスト プラクティスを提供する、開発者を教育します。

PEAR のコードは、「パッケージ」に分割されます。各パッケージは、開発チーム、バージョン番号、リリース サイクル、マニュアル、(依存関係を含む） その他のパッケージに定義された関係を持つ別のプロジェクトです。パッケージ内に、記述ファイルを gzip 圧縮された tar ファイルとして配布され、PEAR インストーラーを用いてローカル システムにインストールされています。

ヘルプ コマンド
----------------------

このコマンドは、PEAR モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure pear help

上記のコマンドの絵の表現は以下します。


.. code-block:: bash


 kevell@corp:/# ptconfigure pear help
 ******************************


  This command allows you to modify create or modify pears

  Pear, pear

        - create
        Create a new system pear, overwriting if it exists
        example: ptconfigure pear create --pearname="somename"

        - remove
        Remove a system pear
        example: ptconfigure pear remove --pearname="somename"

        - set-password
        Set the password of a system pear
        example: ptconfigure pear set-password --pearname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pear
        example: ptconfigure pear exists --pearname="somename"

        - show-groups
        Show groups to which a pear belongs
        example: ptconfigure pear show-groups --pearname="somename"

        - add-to-group
        Add pear to a group
        example: ptconfigure pear add-to-group --pearname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pear from a group
        example: ptconfigure pear remove-from-group --pearname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************


作成します。
------------


ユーザーは新しいシステム ナシまたは既存のものを上書きする必要があります作成する必要がある場合、特定のコマンドの下、プロセスが実行されます。



.. code-block:: bash
	
	ptconfigure pear create --pearname=”somename”

削除
------------

ユーザー システム梨を削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash

	ptconfigure pear remove --pearname=”somename”

パスワードの設定
---------------------

ユーザー システム pear のパスワードを設定する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
	ptconfigure pear setpassword --pearname=”somename”-- new-password=”somepassword”


存在します。
---------------------

ユーザーは、pear の存在を知る必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
	ptconfigure pear exists --pearname=”somename”


グループ表示
---------------------

ユーザーは、pear が属するグループを知る必要がある場合、特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
	ptconfigure pear show-groups --pearname=”somename”


グループを追加します。
-----------------------

ユーザーはナシ、特定のグループに割り当てる必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
 	ptconfigure pear add-to-group --pearname=”somename” -- groupname=”somegroupname”


グループから削除します。
----------------------------

Pear をグループから削除する必要があるとき、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
 		ptconfigure pear remove-from-group --pearname=”name” --groupname=”groupname”




代替パラメーター
--------------------

2 つの代替パラメーターをコマンドラインで使用することができますがあります。


Pear, pear


.. code-block:: bash

 Eg: ptconfigure pear create --pearname=”somename”/ ptconfigure Pear create --pearname=”somename”

利点
--------------
 
Pear.php.net は pear.php.net から利用可能なパッケージに、人にやさしい (HTML) とマシン向け (現在残り) インターフェイスを提供します。すべての通信に HTTP プロトコルで発生します。Pear.php.net サイト提供するその他の機能は次のとおりです。


* ユーザ アカウント管理 (SVN サーバーの独立した)
* パッケージの管理
* 管理をリリースします。
* Ubuntu セントの OS で裕福な
* 非大文字小文字の区別
 

