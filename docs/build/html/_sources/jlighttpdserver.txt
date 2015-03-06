========================
LigHTTPDServer module
========================


あらすじ
----------

Lighttpd は標準に準拠した、安全かつ柔軟なままスピードが重大な環境用に最適化された web サーバーです。Apache の代替 web サーバーです。

Lighttpd Auth、外部プログラムを FastCGI、SCGI および CGI インターフェイス出力圧縮、URL の書き換え、許可する web アプリケーションをサポートする任意のプログラミング言語で書かれたサーバーと共に使用するにはLighttpd は、最もよく知られた非同期サーバーです。非同期アプローチの主な利点はスケーラビリティです。

このモジュールは Lighttpd はサーバーの最新バージョンとその依存関係をインストールすることを目指しています。


ヘルプ コマンド
------------------

ヘルプ コマンドはタスクを達成するために必要を提供するためにユーザーをガイドします。確認するコマンド、ターミナルの下でのヘルプの使用を次のように与えられる

.. code-block:: bash

	ptconfigure lighttpdserver help


下のスナップショットは、help コマンドの絵の表現を与えるし、LigHTTPDServer、lighttpd サーバー、lighttpdserver として 3 つのパラメーターを一覧表示します。(パラメーターは大文字と小文字)


.. code-block:: bash

	 Kevell@corp:/# ptconfigure LigHTTPDServer help

	 ******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

  	LigHTTPDServer, lighttpd-server, lighttpdserver

        - install
        Installs LigHTTPD HTTP Server
        example: ptconfigure lighttpd-server install

	------------------------------
	End Help
	******************************


インストール
------------------

Lighttpd のモジュールをインストールするために使用されるコマンドは下記します。


.. code-block:: bash

	ptconfigure lighttpd-server  install



.. code-block:: bash

	Kevell@corp:/# ptconfigure lighttpd-server install

	Install LigHTTPD Server? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         LigHTTPD Server!        *
	*******************************
	update-alternatives: warning: not replacing /usr/share/man/man1/spawn-fcgi.1.gz with a link
	2015-01-09 14:45:09: (network.c.405) can't bind to port:  80 Address already in use 
	invoke-rc.d: initscript lighttpd, action "start" failed.
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        gamin libgamin0 libterm-readkey-perl libterm-readline-perl-perl spawn-fcgi
	Suggested packages:
	rrdtool apache2-utils
	The following NEW packages will be installed:
        gamin libgamin0 libterm-readkey-perl libterm-readline-perl-perl lighttpd
        spawn-fcgi
	0 upgraded, 6 newly installed, 0 to remove and 280 not upgraded.
	Need to get 378 kB of archives.
	After this operation, 1,622 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgamin0 amd64 0.1.10-4.1ubuntu1 [16.4 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe gamin amd64 0.1.10-4.1ubuntu1 [41.1 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main libterm-readkey-perl amd64 2.31-1 [27.4 kB]
	Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libterm-readline-perl-perl all 1.0303-1 [51.9 kB]
	Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe lighttpd amd64 1.4.33-1+nmu2ubuntu2 [227 kB]
	Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/universe spawn-fcgi amd64 1.6.3-1 [14.0 kB]
	Fetched 378 kB in 24s (15.2 kB/s)
	Selecting previously unselected package libgamin0.
	(Reading database ... 171800 files and directories currently installed.)
	Preparing to unpack .../libgamin0_0.1.10-4.1ubuntu1_amd64.deb ...
	Unpacking libgamin0 (0.1.10-4.1ubuntu1) ...
	Selecting previously unselected package gamin.
	Preparing to unpack .../gamin_0.1.10-4.1ubuntu1_amd64.deb ...
	Unpacking gamin (0.1.10-4.1ubuntu1) ...
	Selecting previously unselected package libterm-readkey-perl.
	Preparing to unpack .../libterm-readkey-perl_2.31-1_amd64.deb ...
	Unpacking libterm-readkey-perl (2.31-1) ...
	Selecting previously unselected package libterm-readline-perl-perl.
	Preparing to unpack .../libterm-readline-perl-perl_1.0303-1_all.deb ...
	Unpacking libterm-readline-perl-perl (1.0303-1) ...
	Selecting previously unselected package lighttpd.
	Preparing to unpack .../lighttpd_1.4.33-1+nmu2ubuntu2_amd64.deb ...
	Unpacking lighttpd (1.4.33-1+nmu2ubuntu2) ...
	Selecting previously unselected package spawn-fcgi.
	Preparing to unpack .../spawn-fcgi_1.6.3-1_amd64.deb ...
	Unpacking spawn-fcgi (1.6.3-1) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libterm-readkey-perl (2.31-1) ...
	Setting up libterm-readline-perl-perl (1.0303-1) ...
	Setting up spawn-fcgi (1.6.3-1) ...
	update-alternatives: using /usr/bin/spawn-fcgi.standalone to provide /usr/bin/spawn-fcgi (spawn-fcgi) in auto mode
	Setting up gamin (0.1.10-4.1ubuntu1) ...
	Setting up libgamin0 (0.1.10-4.1ubuntu1) ...
	Setting up lighttpd (1.4.33-1+nmu2ubuntu2) ...
	 * Starting web server lighttpd
	   ...fail!
	Processing triggers for libc-bin (2.19-0ubuntu6) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	[Pharaoh Logging] Adding Package lighttpd from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	LigHTTPDServer: Success
	------------------------------
	Installer Finished
	******************************

オプション
-----------


.. cssclass:: table-bordered



 +----------------------------+-----------------------------------+------------+-----------------------------------------------------------+
 | パラメーター               | 代替パラメータ                    | 必須       | 注釈                                                      |
 +============================+===================================+============+===========================================================+
 |ptconfigure lighttpd-server | LigHTTPDServer, lighttpd-server,  | Yes        | Lighttpdのモジュールをインストールします。このコマンド    |
 |install                     | lighttpdserver                    |            |                                                           |
 +----------------------------+-----------------------------------+------------+-----------------------------------------------------------+
 |Install lighttpd-server     | LigHTTPDServer, lighttpd-server,  | Y          | ユーザーは、Yを入力すると、以前にインストールしたバージョ |
 |(Y/N)                       | lighttpdserver                    |            | ンのために、このモジュールのチェックは、                  |
 |                            |                                   |            | 終了した場合には、最新バージョンに更新されたか、          |
 |                            |                                   |            | そうでなければ、新鮮なパッケージをインストールします。    |
 +----------------------------+-----------------------------------+------------+-----------------------------------------------------------+
 |Install lighttpd-server     | LigHTTPDServer, lighttpd-server,  | N          | ユーザーは、Nを入力すると、インストールが中止された。     |
 |(Y/N)                       | lighttpdserver|                   |            |                                                           |
 +----------------------------+-----------------------------------+------------+-----------------------------------------------------------+

ユーザーのメリット
-----------------------

* 任意のブラウザーのない単一の環境で LigHTTPDServer をインストールします。
* アクセス、インストールの使いやす
* コーディングは大文字小文字を区別です。
* 非大文字小文字の区別
* Ubuntu や CentOS で裕福な。
 

