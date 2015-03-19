=============
PTVirtualize
=============

概要
-----------

 Ptvirtualize VirtualBoxを管理することが実現する。このモジュールは、ptconfigureの下にインストールすることができます。このモジュールでのインストール中にデータディレクトリとエグゼディレクトリが指定することができます。このモジュールは、UbuntuとセントのOSと最も快適です。

Helpコマンド
--------------------

このhelpコマンドはptvirtualizeモジュールに関するユーザーをガイドする。これは、ビジネスの人々のすべての種類に適しています。 helpコマンドは、ptvirtualizeモジュールに内蔵されたコマンドの短いリストを示しています。

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize help
	******************************


	This command allows you to install or update ptvirtualize.

	ptvirtualize, ptvirtualize

        - install
        Installs the latest version of ptvirtualize
        example: ptconfigure ptvirtualize install

	------------------------------
	End Help
	******************************

インストール
----------------------

ptvirtualizeモジュールのインストールは、デバイスドライバやプラグイン、実行のためのプログラムが準備させる行為を含むです。このモジュールをインストールする際に次のコマンドを実行すると、渡されます。

.. code-block:: bash

	ptconfigure ptvirtualize install

コマンドを入力した後にシステムが尋ねることができます

Install ptvirtualize?(Y/N)

ユーザーは、Yを与えた場合、ptvirtualizeがインストールされます。次のスクリーンショットは、それを証明する。

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ptvirtualize         *
	*******************************
	What is the program data directory? Found "/opt/ptvirtualize" - use this? (Enter nothing for yes, no end slash)

	What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

	git clone 'https://github.com/PharaohTools/ptvirtualize.git'  /tmp/ptvirtualize/ptvirtualizeCloning into '/tmp/ptvirtualize/ptvirtualize'...
	remote: Counting objects: 4063, done.
	remote: Total 4063 (delta 0), reused 0 (delta 0)
	Receiving objects: 100% (4063/4063), 2.13 MiB | 393.00 KiB/s, done.
	Resolving deltas: 100% (2530/2530), done.
	Checking connectivity... done.
	Program Data folder populated
	Program Executor Deleted if existed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	ptvirtualize: Success
	------------------------------
	Installer Finished
	******************************

ユーザーは、Nを与えた場合、それは画面を終了します。次のスクリーンショットは、それを証明する。

.. code-block:: bash

	kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	ptvirtualize: Failure
	------------------------------
	Installer Finished
	******************************

オプション
--------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+-----------------------------+----------------------------------------------------------+
 | パラメータ               | オプション      | ディレクトリ                | コメント                                                 |
 +==========================+=================+=============================+==========================================================+
 |Data directory(DEFAULT)   | YES             | “/opt/ptvirtualize”         | それはptconfigureの下ptvirtualizeをインストールします    |
 +--------------------------+-----------------+-----------------------------+----------------------------------------------------------+
 |Data directory            | No              | End slash                   | ユーザーがパスを指定する必要があります。                 |
 +--------------------------+-----------------+-----------------------------+----------------------------------------------------------+
 |Executor directory        | Yes             | “/usr/bin”                  | それは、エグゼディレクトリにインストールされます         |
 |(Default)                 |                 |                             |                                                          |
 +--------------------------+-----------------+-----------------------------+----------------------------------------------------------+
 |Executor directory        | No              | No trailing slash           | ユーザーは、ディレクトリ名などの入力を提供します|        |
 +--------------------------+-----------------+-----------------------------+----------------------------------------------------------+
         

メリット
-------------

* Ubuntuユーザは単にリポジトリからptvirtualizeをインストールすることができます。
* ptvirtualizeの本当の利点は、その性能にあります。
* ホストOSとの統合。
* 高速アクセス可能性。
* 仮想ボックスを管理します。
