===========
Varnish
===========

概要
--------------

このモジュールは、ユーザーのマシンにニスをインストールするのに役立つ。ニスは、Webサーバの負荷を低減しながら、大幅にWebサイトを高速化することができるプログラムです。ニスの公式サイトによると、ニス」も、キャッシュのHTTPリバースプロキシとして知られているWebアプリケーションアクセラレータ」です。私たちは、このモジュールは、apt-getはのワニスのインストールを実行しないかについて、こちらを見てみましょう。

helpコマンド
------------------

helpコマンドは、とだけでなく、ワニスモジュールに含まれているオプションについての目的について、ユーザーをガイドします。 helpコマンドは、ワニスの別のパラメータを示しています。また、ワニスをインストールするための構文について説明します。ワニスモジュールの下のhelpコマンドは以下の通りである：
.. code-block:: bash

	ptconfigure varnish help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、ワニスモジュールの下helpコマンドについてご描く。

.. code-block:: bash

	kevell@corp:/# ptconfigure Varnish help
	******************************


        This command allows you to install Varnish, the popular HTTP Cache

        Varnish, varnish

        - install
        Installs Varnish through apt-get
        example: ptconfigure varnish install

	------------------------------
	End Help
	******************************

インストール
---------------------

ユーザーがマシンにニスをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash

	ptconfigure varnish install

表形式で示すように、上記のコマンドを入力した後、次の操作が発生します。

.. cssclass:: table-bordered


 +---------------------------+---------------------+------------------+-----------------------------------------------------------+
 | パラメーター              | 代替パラメータ      | オプション       | コメント                                                  |
 +===========================+=====================+==================+===========================================================+
 |Install Varnish? (Y/N)     | Varnish, varnish    | Y(Yes)           | ユーザーは、Yと入力することができ、インストールプロ       |
 |                           |                     |                  | セスを続行したい場合                                      |
 +---------------------------+---------------------+------------------+-----------------------------------------------------------+
 |Install Varnish? (Y/N)     | Varnish, varnish    | N(No)            | ユーザーは、Nと入力することができ、インストールプロセ     |
 |                           |                     |                  | スを終了したい場合は|                                     |
 +---------------------------+---------------------+------------------+-----------------------------------------------------------+


ユーザーがインストールプロセスを進行する場合は、インストールの実行中に次の処理が行われます。

* パッケージ一覧を読み込みます。
* 依存関係ツリーを構築します。
* 状態情報を読み取ります。
* インストールされているパッケージの一覧。
* インストールされて余分なパッケージのリスト。
* インストールされた新しいパッケージのリスト。
* アップグレードされたファイルの数、新しくインストールされ、削除、アップグレードされません。
* 最後に、ニスのHTTPアクセラレータを開始する。
* 以下のスクリーンショットは、上記のプロセスを示している。


.. code-block:: bash
   
	Kevell@corp:/# ptconfigure varnish install
	Install Varnish? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Varnish !        *
	*******************************
	Creating /tmp/ptconfigure-temp-script-95745650915.sh
	chmod 755 /tmp/ptconfigure-temp-script-95745650915.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-95745650915.sh Permissions
	Executing /tmp/ptconfigure-temp-script-95745650915.sh
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        libjemalloc1 libvarnishapi1
	Suggested packages:
	varnish-doc
	The following NEW packages will be installed:
	libjemalloc1 libvarnishapi1 varnish
	0 upgraded, 3 newly installed, 0 to remove and 6 not upgraded.
	Need to get 518 kB of archives.
	After this operation, 1,653 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libvarnishapi1 amd64 3.0.5-2 [29.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjemalloc1 amd64 3.5.1-2 [76.8 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe varnish amd64 3.0.5-2 [411 kB]
	Fetched 518 kB in 3s (152 kB/s)
	Selecting previously unselected package libvarnishapi1.
	(Reading database ... 201582 files and directories currently installed.)
	Preparing to unpack .../libvarnishapi1_3.0.5-2_amd64.deb ...
	Unpacking libvarnishapi1 (3.0.5-2) ...
	Selecting previously unselected package libjemalloc1.
	Preparing to unpack .../libjemalloc1_3.5.1-2_amd64.deb ...
	Unpacking libjemalloc1 (3.5.1-2) ...
	Selecting previously unselected package varnish.
	Preparing to unpack .../varnish_3.0.5-2_amd64.deb ...
	Unpacking varnish (3.0.5-2) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libvarnishapi1 (3.0.5-2) ...
	Setting up libjemalloc1 (3.5.1-2) ...
	Setting up varnish (3.0.5-2) ...
	 * Starting HTTP accelerator varnishd
	   ...done.
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Temp File /tmp/ptconfigure-temp-script-95745650915.sh Removed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	Varnish: Success
	------------------------------
	Installer Finished
	******************************

メリット
-----------------

* ワニスは、リバースHTTPプロキシの実装をキャッシュする近代的な、高パフォーマンス、オープンソースです。
* helpコマンドを宣言するために使用されるパラメータは、インストールが他の人に比べながら、追加的な利点である大文字と小文字を区別しません。
* これは、裕福な両方セントOSで、同様のUbuntuのようです。
