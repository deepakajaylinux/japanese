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

        - install
        Install
        example: ptconfigure pear pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure pear pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure pear pkg-ensure --package-name="somename"
        
 ------------------------------
 End Help


Install
----------


ユーザーが梨をインストールする必要がある場合は、以下のコマンドは、プロセスを実行します。

.. code-block:: bash

	ptconfigure pear pkg-install --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-install --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************



Remove
------------


ユーザがシステム梨を除去する必要がある場合、下記のコマンドは、プロセスを実行する。

.. code-block:: bash

	ptconfigure pear pkg-remove --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-remove --package-name="file"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_CSV"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_Util"
 pear/File cannot be uninstalled, other installed packages depend on this package
 [Pharaoh Logging] Removing Package file from the Packager Pear did not execute correctly
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Failure

 ------------------------------
 Pear Mods Finished
 ******************************



Ensure
---------

ユーザーが梨を確保する必要がある場合、下記のコマンドは、プロセスを実行します


.. code-block:: bash

	ptconfigure pear pkg-ensure --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-ensure --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************






代替パラメータ
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
 

