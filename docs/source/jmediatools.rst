============
Media Tools
============


あらすじ
------------

このモジュール インストール メディア ツールがユーザーのシステムの生産性を高める VLC メディア プレーヤーとして推奨 GC を目指します。VLC メディア プレーヤーでは、多くのオーディオおよびビデオの圧縮方法やファイルを含むフォーマット DVD ビデオ ビデオ CD、ストリーミング プロトコル サポートします。（通称 VLC) VLC メディア プレーヤーはポータブル無料とオープン ソース、クロスプラット フォームのメディア プレーヤーとストリーミング メディア サーバー VideoLAN のプロジェクトによって書かれました。私たちを見てみましょうどのようにこのモジュール アシスト VLC をインストールするについて。

ヘルプ コマンド
--------------------

ヘルプ コマンド同様目的に関してユーザーを導くようにメディア ツール モジュールに含まれているオプションについて。ヘルプ コマンドはメディア ツールの代替パラメーターが一覧表示されます。また、VLC をインストールするための構文について説明します。メディア ツール モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash
  
 ptconfigure mediatools help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、[メディア ツール ヘルプ コマンドについて視覚化します。


.. code-block:: bash


	Kevell@corp:/# ptconfigure MediaTools help
	******************************


	This command allows you to install a few GC recommended Media Tools
        for productivity in your system. Currently, we're only including
        VLC Media Player

         MediaTools, media-tools, mediatools, mediatools, media-tools

        - install
        Installs some media tools
        example: ptconfigure mediatools install

	------------------------------
	End Help


インストール
---------------


次のコマンドは、メディアのツールをインストールするために使用します。


.. code-block:: bash

	ptconfigure mediatools install



スクリーン ショットは、その機能を視覚化します。



.. code-block:: bash


        - install
        Installs some media tools
        example: ptconfigure mediatools install

        ------------------------------
        End Help

インストール プロセスを続行すると、インストール中に、次のプロセスが発生します。

* パッケージからテンプレートを抽出します。
* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* 自動的にインストールされているパッケージを一覧表示します。
* インストールされている余分なパッケージを一覧表示します。
* 推奨パッケージを一覧表示します。
* インストールされている新しいパッケージを一覧表示します。
* 最後に、レポートは、ステータスと結果を明確に表示されます。
* 次のスクリーン ショットは絵上記のプロセスについて説明します。



.. code-block:: bash



 kevell@corp:/# ptconfigure mediatools install 
 Install Media Tools? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Media Tools!        * 
 ******************************* 
 [Pharaoh Logging] Packages vlc, libdvdread4 from the Packager Apt are already installed, so not installing 
 Creating /tmp/ptconfigure-temp-script-57996813529.sh 
 chmod 755 /tmp/ptconfigure-temp-script-57996813529.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-57996813529.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-57996813529.sh 
 --2015-03-27 13:21:10--  http://download.videolan.org/pub/debian/stable//Packages 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 3520 (3.4K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ 

 100%[=======================================================================================================>] 3,520       --.-K/s   in 0s      

 2015-03-27 13:21:11 (77.0 MB/s) - â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ saved [3520/3520] 

 --2015-03-27 13:21:12--  http://download.videolan.org/pub/debian/stable/stable/libdvdcss2_1.2.13-0_amd64.deb 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 44462 (43K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ 

 100%[=======================================================================================================>] 44,462      65.6KB/s   in 0.7s   

 2015-03-27 13:21:13 (65.6 KB/s) - â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ saved [44462/44462] 

 Selecting previously unselected package libdvdcss2. 
 (Reading database ... 362949 files and directories currently installed.) 
 Preparing to unpack .../dvdcss-2TJ4IX/libdvdcss.deb ... 
 Unpacking libdvdcss2 (1.2.13-0) ... 
 Setting up libdvdcss2 (1.2.13-0) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-57996813529.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 
 Single App Installer: 
 -------------------------------------------- 
 MediaTools: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 





オプション
----------


.. cssclass:: table-bordered

 +---------------------------+--------------------------------------------+--------------+---------------------------------------------+
 | パラメーター              | 代替パラメーター                           | オプション   | コメント                                    |
 +===========================+============================================+==============+=============================================+
 |Install Media Tools? (Y/N) | その代わりMediaToolsのの、次の代替を使用   | Y(Yes)       | ユーザーは、Yとして入力することができ、     |
 |                           | することもできる media-tools, mediatools.  |              | インストールプロセスを続行したい場合        |
 +---------------------------+--------------------------------------------+--------------+---------------------------------------------+
 |Install Media Tools? (Y/N) | その代わりMediaToolsのの、次の代替を使用   | N(No)        | ユーザーは、Nと入力することができ、         |
 |                           | することもできる media-tools, mediatools.  |              | インストールプロセスを終了したい場合は|     |
 +---------------------------+--------------------------------------------+--------------+---------------------------------------------+


   
利点
------------


* ヘルプおよびインストール操作で使用されるパラメーター大文字小文字が区別されません中に他の人に比べて利点であります。
  このモジュールは、システムの生産性の使用を強化することができます。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* このモジュール GC 推奨メディア ツールのインストールを容易にします。
 

