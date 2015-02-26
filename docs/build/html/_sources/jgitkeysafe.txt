============
GitKeySafe
============


あらすじ
------------------

Git のキーを安全にすることができます安全な Git キーをインストールします。これにより、セキュリティで保護された方法でアクセス許可。これらのシステムは、ファイルシステムのアクセス許可を表示するユーザーの能力を持っています。読み取りアクセス許可がファイルを読み取る権限が付与されます。書き込みアクセス許可は、ファイルを変更する権限を付与されます。実行権限は、ファイルを実行する権限を付与されます。Ubuntu で、セント快適 OS。

ヘルプ コマンド
----------------------

ヘルプ コマンド同様目的に関してユーザーを導くように Gitkeysafe モジュールに含まれているオプションについて。Help コマンドは、ptconfigure モジュールの下に Gitkeysafe の代替パラメーターを一覧表示されます。また、ユーザーのお電話くださいインストールするための構文について説明します。Gitkeysafe のヘルプ コマンドを以下に示します。

.. code-block:: bash

		ptconfigure GitkeySafe help


このモジュールのための利点を追加する非大文字小文字を区別ヘルプ コマンドの構文です。次のスクリーン ショットは help コマンド、ヘルプ コマンド非大文字小文字を区別このモジュールのための利点を追加するための構文の下についてユーザーを視覚化します。次のスクリーン ショットは gitkeysafe の下で help コマンドについてユーザーを視覚化します。



.. code-block:: bash

 kevell@corp:/# ptconfigure GitKeySafe help

 ******************************


  This module installs Git Key-Safe Server to the program git-key-safe

  GitKeySafe, git-key-safe, gitkeysafe

        - install
        Installs Git Key-Safe Server
        example: ptconfigure gitkeysafe install

        script example: git-safe-key -i /path/to/key clone http://git.com/repo.git

 ------------------------------
 End Help
 ******************************



インストール
-----------------

インストールには、通常オペレーティング システムで簡単にアクセス、ローカル コンピューター上の新しいファイルをインストール ファイルからコピー生成であるコードが含まれます.それらを使用して、ユーザーを確認し、ユーザー データを常に復元できるように、バックアップを持っています。次のコマンドで git 鍵保管ボックスをインストールするために使用します。

.. code-block:: bash

		ptconfigure gitkeysafe install

このモジュールのインストール中に次のスクリーン ショットが表示されます。


.. code-block:: bash

 kevell@corp:/# ptconfigure gitkeysafe install

 Install Git Key-Safe Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Git Key-Safe Server!        *
 *******************************
 Git Key-Safe script /usr/bin/git-key-safe added
 Git Key-Safe script /usr/bin/git-key-safe permissions changed to 775
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitKeySafe: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
------------


.. cssclass:: table-bordered


 +-----------------------+-------------------------------------------------------+------------+-----------------------------------------------+
 | パラメータ            | 代替パラメータ                                        | オプション | 注釈                                          |
 +=======================+=======================================================+============+===============================================+
 |Install gitkeysafe     | 代わりにgitkeysafeを使用するのでは、                  | Y(Yes)     | それはptconfigureの下gitkeysafeをインストール |
 |                       | 我々は使用することができます GitKeySafe,git-key-safe  |            |                                               |
 +-----------------------+-------------------------------------------------------+------------+-----------------------------------------------+
 |Install gitkeysafe     | 代わりにgitkeysafeを使用するのでは、                  | N(No)      | システム出口インストール                      |
 |                       | 我々は使用することができます GitKeySafe,git-key-safe| |            |                                               |
 +-----------------------+-------------------------------------------------------+------------+-----------------------------------------------+

利点
--------------

* 非大文字小文字の区別
* Git 鍵保管ボックスをインストールする使用します。
* ユーザーのアクセス許可を表示します。
* Ubuntu とセントが使用 OS
* セキュリティが可能です。
 

