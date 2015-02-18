===========
Cleopatra
===========

あらすじ
-----------

このモジュールは、更新されたバージョンにインストールを持ち上げます。自動化が可能です。このモジュールのインストール中はデータ ディレクトリと遺言執行者のディレクトリの場所を指定できます。それはあなたの環境の構成を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
------------------

このコマンドのヘルプガイド クレオパトラについてユーザー。ユーザーのすべてのタイプに適しています。代替パラメーターとインストール用のコマンドを示しています。次のヘルプ コマンドとスクリーン ショットの使用に関するユーザーに役立ちます。


.. code-block:: bash

		cleopatra Cleopatra help

.. code-block:: bash
 
	kevell@corp:/# cleopatra Cleopatra help
	******************************


	This command allows you to update Cleopatra.

	Cleopatra, cleo, cleopatra

        - install
        Installs the latest version of cleopatra
        example: cleopatra cleopatra install

	------------------------------
	End Help
	******************************



インストール
---------------

それはちょうど、下記のコマンドを使用してクレオパトラ モジュールをインストールする簡単なプロセスです。


.. code-block:: bash

  cleopatra Cleopatra install


コマンドを与えた後クレオパトラは、新しい更新プログラムでインストールされます。

ユーザー入力が経過した後かどうか任意のファイルが存在しないと手に、それは自動的にインストールされますがチェックされます。

次のスクリーン ショットは、それを列挙します。


.. code-block:: bash

 kevell@corp:/# cleopatra cleopatra install

 Install Cleopatra - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          Cleopatra!         *
 *******************************
 What is the program data directory? Found "/opt/cleopatra" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/cleopatra.git'  /tmp/cleopatra/cleopatraCloning into '/tmp/cleopatra/cleopatra'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/cleopatra Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Cleopatra: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
------------

.. cssclass:: table-bordered

 +-----------------------------+-----------------------------------------------+------------+--------------------------------------------+
 | パラメータ                  | 代替パラメータ                                | オプション | コメント                                   |
 +=============================+===============================================+============+============================================+
 |Install cleopatra cleopatra  | 使用できる3つのパラメータがある。             | Y(Yes)     | これは、クレオパトラがインストールされます |
 |Update to latest             | Cleopatra, cleo, Cleopatra                    |            | クレオパトラの下で                         |
 |version? (Y/N)               | 例: cleopatra cleopatra install/              |            |                                            |
 |                             |     cleopatra cleo install                    |            |                                            | 	
 +-----------------------------+-----------------------------------------------+------------+--------------------------------------------+
 |Install cleopatra cleopatra  | 使用できる3つのパラメータがある。             | N(No)      | これは、インストールを終了します           |
 |Update to latest             | Cleopatra, cleo, Cleopatra                    |            |                                            |
 |version? (Y/N)               | 例: cleopatra cleopatra install/              |            |                                            |
 |                             |     cleopatra cleo install|                   |            |                                            |
 +-----------------------------+-----------------------------------------------+------------+--------------------------------------------+


利点
--------

* クレオパトラは、構成ファイルをインストールする使用されます。中に既存の任意のファイルがある場合、インストール内容を上書きします。
* 新しいバージョンを自動的に更新することができます。
* 更新は、web 検索なしこのモジュールで実行できます。


 
