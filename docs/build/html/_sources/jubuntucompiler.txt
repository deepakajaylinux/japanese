================
Ubuntu Compiler
================

あらすじ
----------

このモジュールは、c プログラムを活性化します。Ubuntu や他の Linux ディストリビューションのコンパイルの問題からユーザーを救うために広範なパッケージのリポジトリがあります。1 つのコマンドは、プロのようなソースから構築できます。Ubuntu や centOS で快適です。

ヘルプ コマンド
-----------------

このコマンドのヘルプガイド Ubuntu コンパイラについてユーザー。それ以下の時間がかかることができるので自動的にインストールされます。C プログラムに適しています。

.. code-block:: bash

		ptconfigure Ubuntucompiler help


次のヘルプ コマンドは、インストールのユーザーを支援します。

.. code-block:: bash

	kevell@corp:/# ptconfigure UbuntuCompiler help
	******************************


         This allows you to Complie programs written in C Source

          UbuntuCompiler, ubuntu-compiler, ubuntucompiler

        - install
        Installs Ubuntu Compiling tools through apt-get.
        example: ptconfigure ubuntu-compiler install

	------------------------------
	End Help
	******************************

インストール
--------------

これはモジュールをインストールする Ubuntu コンパイラ ptconfigure の下でちょうど、下記のコマンドを使用して顕著なプロセス


.. code-block:: bash

  		ptconfigure Ubuntu-compiler install

コマンドを与えた後 Ubuntu コンパイラは新しい更新プログラムでインストールされます。

N を入力した場合、次の画面になります。


.. code-block:: bash

	Kevell@corp:/# ptconfigure UbuntuCompiler install
	Install Ubuntu Compiler? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	UbuntuCompiler: Failure
	------------------------------
	Installer Finished
	******************************



オプション
-----------


.. cssclass:: table-bordered

 +-----------------------+-----------------------------------------+----------------+------------------------------------------+
 | パラメーター          | 代替パラメータ                          | オプション     | 注釈                                     |
 +=======================+=========================================+================+==========================================+
 |Install Ubuntu         | UbuntuCompiler, ubuntu-compiler,        | Yes            | インストールプロセスを開始します         |
 |compiler? (Y/N)        | ubuntucompiler                          |                |                                          |
 +-----------------------+-----------------------------------------+----------------+------------------------------------------+
 |Install Ubuntu         | UbuntuCompiler, ubuntu-compiler,        | No             | インストールプロセスを終了します         |
 |compiler? (Y/N)        | ubuntucompiler|                         |                |                                          |
 +-----------------------+-----------------------------------------+----------------+------------------------------------------+

利点
-----------

* 高速ブート
* より良いセキュリティ
* コンパイル中を横取りするカーネルの変更
* C プログラムに適して

 
