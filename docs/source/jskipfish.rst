=============
Skipfish
=============


概要
------------

skipfishをインストールするために使用skipfishモジュール。 SkipfishはアクティブなWebアプリケーションのセキュリティ偵察ツールです。これは、再帰的なクロールと辞書ベースのプローブを行うことにより、標的部位のためのインタラクティブなサイトマップを準備します。結果のマップは、その後アクティブなセキュリティチェックの数からの出力と注釈されている。ツールによって生成された最終報告書は、プロのWebアプリケーションセキュリティ評価のための基盤となることを意味している。このモジュールは、UbuntuとセントOSに強化する。

Helpコマンド
----------------------

helpコマンドは、とだけでなく、Skipfishモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それはSkipfishモジュールの別のパラメータを示しています。また、Skipfishモジュールをインストールするための構文について説明します。 Skipfishモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash	 

	ptconfigure Skipfish help 

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、Skipfish下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash 

 kevell@corp:/# ptconfigure Skipfish help 

 ****************************** 


  This command allows you to install Skipfish. 
  Skipfish, skipfish 

        - install 
        Installs Skipfish. 
        example: ptconfigure skipfish install 

 ------------------------------ 
 End Help 
 ****************************** 


 
インストール
-----------------

このコマンドは、対話型のサイトマップとskipfishをインストールするには許可する。ユーザーは、次のコマンドskipfishインストールしたいときにインストールするには、ユーザーをガイドします。

.. code-block:: bash 

	ptconfigure skipfish install 

このコマンドを入力した後、システムは、ユーザーが望む尋ねます。他のプロセスは、スクリーンショットを経て、インストールを説明しています。

.. code-block:: bash 


 kevell@corp:/# ptconfigure Skipfish install 
 Install  Skipfish? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *          Skipfish !        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
  skipfish 
 0 upgraded, 1 newly installed, 0 to remove and 15 not upgraded. 
 Need to get 233 kB of archives. 
 After this operation, 574 kB of additional disk space will be used. 
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty/universe skipfish amd64 2.10b-1 [233 kB] 
 Fetched 233 kB in 29s (7,910 B/s) 
 Selecting previously unselected package skipfish. 
 (Reading database ... 199429 files and directories currently installed.) 
 Preparing to unpack .../skipfish_2.10b-1_amd64.deb ... 
 Unpacking skipfish (2.10b-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up skipfish (2.10b-1) ... 
 [Pharaoh Logging] Adding Package skipfish from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Skipfish: Success 
 ------------------------------ 
 Installer Finished 

 ****************************** 


オプション
-----------

.. cssclass:: table-bordered 

 +-------------------------+------------------------------+---------------+--------------------------------------------------+
 | パラメーター            | 代替パラメータ               | オプション    | コメント                                         |
 +=========================+==============================+===============+==================================================+
 |Install Skipfish? (Y/N)  | Skipfish, skipfish           | Y(Yes)        | ユーザーは、Yと入力することができ、              |
 |                         |                              |               | インストールプロセスを続行したい場合             |
 +-------------------------+------------------------------+---------------+--------------------------------------------------+
 |Install Skipfish? (Y/N)  | Skipfish, skipfish           | N(No)         | ユーザーは、Nと入力することができ、              |
 |                         |                              |               | インストールプロセスを終了したい場合は|          |
 +-------------------------+------------------------------+---------------+--------------------------------------------------+



メリット
--------------

* skipfishは、高度に適応性と信頼性です。
* 適切に設計されたセキュリティチェック。
* マルチフレームワークサイトの優雅な取り扱い
* 自動更新されたバージョンのインストール
* 高速アクセス可能。
* 非大文字と小文字の区別。
* UbuntuとセントOSの観光も。

