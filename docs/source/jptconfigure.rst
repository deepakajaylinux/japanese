=============
PTConfigure
=============

あらすじ
-----------

このモジュールは、更新されたバージョンにインストールを持ち上げます。自動化が可能です。このモジュールのインストール中はデータ ディレクトリと遺言執行者のディレクトリの場所を指定できます。それはあなたの環境の構成を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
------------------

このhelpコマンドはptconfigure約ユーザーを導く。ユーザーのすべてのタイプに適しています。これは、インストールのための代替パラメータとコマンドを示している。次のhelpコマンドとスクリーンショットは、使用状況に関するユーザを支援します。


.. code-block:: bash

		ptconfigure ptconfigure help

.. code-block:: bash
 
	kevell@corp:/# ptconfigure ptconfigure help
	******************************


	This command allows you to update ptconfigure.

	ptconfigure, cleo, ptconfigure

        - install
        Installs the latest version of ptconfigure
        example: ptconfigure ptconfigure install

	------------------------------
	End Help
	******************************



インストール
---------------

それはちょうど下記のコマンドを使用して、 ptconfigureモジュールをインストールするには、 simplierプロセスであり、


.. code-block:: bash

  ptconfigure ptconfigure install


コマンドを与えた後ptconfigureは新しい更新と一緒にインストールされます。

ユーザー入力が経過した後かどうか任意のファイルが存在しないと手に、それは自動的にインストールされますがチェックされます。

次のスクリーン ショットは、それを列挙します。


.. code-block:: bash

 kevell@corp:/# ptconfigure ptconfigure install

 Install ptconfigure - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          ptconfigure!         *
 *******************************
 What is the program data directory? Found "/opt/ptconfigure" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptconfigure.git'  /tmp/ptconfigure/ptconfigureCloning into '/tmp/ptconfigure/ptconfigure'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/ptconfigure Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptconfigure: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
------------

.. cssclass:: table-bordered

 +---------------------------------+-----------------------------------------------+------------+--------------------------------------------+
 | パラメータ                      | 代替パラメータ                                | オプション | コメント                                   |
 +=================================+===============================================+============+============================================+
 |Install ptconfigure ptconfigure  | 使用できる3つのパラメータがある。             | Y(Yes)     | それはptconfigureをインストールします      |
 |Update to latest                 | ptconfigure, cleo, ptconfigure                |            | クレオパトラの下で                         |
 |version? (Y/N)                   | 例: ptconfigure ptconfigure install/          |            |                                            |
 |                                 |     ptconfigure cleo install                  |            |                                            | 	
 +---------------------------------+-----------------------------------------------+------------+--------------------------------------------+
 |Install ptconfigure ptconfigure  | 使用できる3つのパラメータがある。             | N(No)      | これは、インストールを終了します           |
 |Update to latest                 | ptconfigure, cleo, ptconfigure                |            |                                            |
 |version? (Y/N)                   | 例: ptconfigure ptconfigure install/          |            |                                            |
 |                                 |     ptconfigure cleo install|                 |            |                                            |
 +---------------------------------+-----------------------------------------------+------------+--------------------------------------------+



利点
--------

* ptconfigureは、設定ファイルをインストールするために使用されます。がある場合、インストール中に任意のファイルは、内容に上書きされている既存の。
* 新しいバージョンを自動的に更新することができます。
* 更新は、web 検索なしこのモジュールで実行できます。


 
