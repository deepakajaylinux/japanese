=========
Node-JS
=========

あらすじ
-------------

このモジュールは、サーバー側の JS 言語ノード JS をインストールするユーザーを支援します。Node.js は、オープン ソースは、サーバー側とネットワー キング アプリケーションのクロスプラット フォーム ランタイム環境です。Node.js アプリケーション、JavaScript で記述されているし、OS X、Microsoft Windows、Linux および FreeBSD 上 Node.js ランタイム内で実行することができます。ここでは、私たちを見てみましょうどのようにこのモジュールをインストールすると、ノード JS を使用して容易します。

ヘルプ コマンド
---------------------

ヘルプ コマンド同様目的に関してユーザーをリードとしてノード-JS のモジュールに含まれているオプションについて。ヘルプ コマンド ノード-JS のモジュールの代替パラメーターが一覧表示されます。また、ノード-JS のモジュールをインストールするための構文について説明します。ノード-JS のモジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash

		ptconfigure NodeJS help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、ノードの JS 下 help コマンドについて視覚化します。


.. code-block:: bash
		


 kevell@corp:/# ptconfigure NodeJS help
 ******************************


  This command allows you to install Node JS, The Server Side JS Language

  NodeJS, node-js, nodejs

        - install
        Installs NodeJS through apt-get.
        example: ptconfigure node-js install

 ------------------------------
 End Help
 ******************************



インストール
----------------

ノード JS をインストールするコンピューターに、ように、次のコマンドを使用するだけで実行できます。

.. code-block:: bash

		ptconfigure node-js install

上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +----------------------+---------------------------------------------+--------------+-------------------------------------------------+
 | パラメータ           | 代替パラメータ                              | オプション   | 注釈                                            |
 +======================+=============================================+==============+=================================================+
 |Install Node JS?      | の代わりに NodeJS, node-js, nodejs          | Y(Yes)       | ユーザーは、Yと入力することができ、             |
 |(Y/N)                 | また、使用することができる.                 |              | インストールプロセスを続行したい場合            |
 +----------------------+---------------------------------------------+--------------+-------------------------------------------------+
 |Install Node JS?      | の代わりに NodeJS, node-js, nodejs          | N(No)        | ユーザーは、Nと入力することができ、             |
 |(Y/N)                 | また、使用することができる.                 |              | インストールプロセスを続行したい場合|           |
 +----------------------+---------------------------------------------+--------------+-------------------------------------------------+



インストール プロセスを続行すると、インストールの実行中に、次のプロセスが発生します。

* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 読み取り状態情報。
* 自動的にインストールされるパッケージのリスト。
* インストールされている新しいパッケージのリスト。
* リストをアップグレードすると、新しくインストールされたファイルの数を削除、アップグレードされません。

最後に、レポートと状態明確に報告されます。また、正常に実行パッケージ nodejs パッケー ジャー Apt から追加します。次のスクリーン ショットの説明に従ってインストールの全体のプロセスを示しています。

ノード-js のモジュールがユーザーのコンピューターに既に存在する場合に、Apt が既にインストールされているパッケー ジャーからパッケージ ノード js として、メッセージが表示されます。スクリーン ショットを次のようにメッセージのこれらのタイプの良い例です。


.. code-block:: bash

 kevell@corp:/# ptconfigure node-js install
 Install Node JS? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Node JS!        *
 *******************************
	Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  ax25-node libax25 openbsd-inetd
 The following NEW packages will be installed:
  ax25-node libax25 node openbsd-inetd
 0 upgraded, 4 newly installed, 0 to remove and 17 not upgraded.
 Need to get 110 kB of archives.
 After this operation, 465 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libax25 amd64 0.0.12-rc2+cvs20120204-2ubuntu2 [22.7 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main openbsd-inetd amd64 0.20091229-2ubuntu3 [30.8 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/universe ax25-node amd64 0.3.2-7.4 [54.8 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/universe node all 0.3.2-7.4 [1,284 B]
 Fetched 110 kB in 2s (39.1 kB/s)
 Selecting previously unselected package libax25.
 (Reading database ... 237551 files and directories currently installed.)
 Preparing to unpack .../libax25_0.0.12-rc2+cvs20120204-2ubuntu2_amd64.deb ...
 Unpacking libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Selecting previously unselected package openbsd-inetd.
 Preparing to unpack .../openbsd-inetd_0.20091229-2ubuntu3_amd64.deb ...
 Unpacking openbsd-inetd (0.20091229-2ubuntu3) ...
 Selecting previously unselected package ax25-node.
 Preparing to unpack .../ax25-node_0.3.2-7.4_amd64.deb ...
 Unpacking ax25-node (0.3.2-7.4) ...
 Selecting previously unselected package node.
 Preparing to unpack .../node_0.3.2-7.4_all.deb ...
 Unpacking node (0.3.2-7.4) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Setting up openbsd-inetd (0.20091229-2ubuntu3) ...
 * Stopping internet superserver inetd
   ...done.
 * Not starting internet superserver: no services enabled
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up ax25-node (0.3.2-7.4) ...
 Setting up node (0.3.2-7.4) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package node from the Packager Apt executed correctly
            
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libv8-3.14.5
 The following NEW packages will be installed:
  libv8-3.14.5 nodejs
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 1,873 kB of archives.
 After this operation, 7,429 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libv8-3.14.5 amd64 3.14.5.8-5ubuntu2 [1,189 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe nodejs amd64 0.10.25~dfsg2-2ubuntu1 [684 kB]
 Fetched 1,873 kB in 14s (126 kB/s)
 Selecting previously unselected package libv8-3.14.5.
 (Reading database ... 237621 files and directories currently installed.)
 Preparing to unpack .../libv8-3.14.5_3.14.5.8-5ubuntu2_amd64.deb ...
 Unpacking libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Selecting previously unselected package nodejs.
 Preparing to unpack .../nodejs_0.10.25~dfsg2-2ubuntu1_amd64.deb ...
 Unpacking nodejs (0.10.25~dfsg2-2ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Setting up nodejs (0.10.25~dfsg2-2ubuntu1) ...
 update-alternatives: using /usr/bin/nodejs to provide /usr/bin/js (js) in auto mode
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package nodejs from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NodeJS: Success
 ------------------------------
 Installer Finished


利点
------------

* ヘルプ コマンドを宣言するために使用されるパラメーター、インストールしない大文字と小文字は他と比較される間、加えられた利点であります。
* それは裕福な両方セント OS とも Ubuntu のように。
* 場合はノード js パッケージをユーザーのコンピューターに存在上書きされません、代わりにそのそれメッセージが表示されますすでに
  存在しています。
* Node.js Google V8 JavaScript エンジンを使用して、コードを実行して基本的なモジュールの大きな割合を JavaScript で書かれています。
  Node.js には Apache HTTP サーバーや IIS などのソフトウェアを使用せず Web サーバーとして動作するアプリケーションをできるようにする組み込みのラ   イブラリが含まれています。
 

