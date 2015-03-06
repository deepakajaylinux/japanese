=============
NginxServer
=============

あらすじ
---------

「エンジン X」発音される、Nginx は、高パフォーマンスの Web サーバー。Nginx Web サーバーは軽量化とは別のために構成できる汎用性の高いサーバー タスクは、多くの現代の web サイトの需要。Ngnix サーバーでアプリケーション設定を構成するユーザーにファシリテーターとして機能します。アプリケーションの設定のほとんどの例では、mysql 管理者ユーザー、ホスト、パスが含まれません。Nginx は多くのウェブ マスターのための選択の新しい Web サーバーとして見出しを作っています。その人気の一番の理由は、その速度です。Nginx は、Apache 以外のテスト環境でより速くそのアーキテクチャはイベント駆動型の Apache のプロセス駆動型ですのでです。Ptconfigure モジュールを通してこの Nginx のサーバーをインストールするための方法として機能します。

ヘルプ コマンド
-------------------

ヘルプ コマンド同様目的に関してユーザーを導くように Ngnix サーバー モジュールに含まれているオプションについて。ヘルプ コマンド Ngnix サーバーの代替パラメーターが一覧表示されます。また、Ngnix サーバーをインストールするための構文について説明します。ヘルプ コマンド Ngnix サーバーを以下のとおりです。

.. code-block:: bash

	ptconfigure nginx-server help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、Nginx のサーバーの下で help コマンドについて視覚化します。


.. code-block:: bash


	kevell@corp:/# ptconfigure NginxServer help
	******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

	NginxServer, nginx-server, nginxserver

        - install
        Installs Nginx HTTP Server
        example: ptconfigure nginx-server install

	------------------------------
	End Help
	******************************


インストール
--------------

Nginx のサーバーをインストールするように、次のコマンドを使用して簡単です：


.. code-block:: bash

	ptconfigure nginx-server install

次の操作上のコマンドを入力した後で示すように、表形式に発生します。

.. cssclass:: table-bordered

 +---------------------+--------------------------------------------------+------------+------------------------------------------------+
 | パラメーター        | 代替パラメーター                                 | オプション | コメント                                       |
 +=====================+==================================================+============+================================================+
 |Install NginxServer? | の代わりに Nginx Server, 以下の選択肢を使用す    | Y(Yes)     | ユーザーは、Yと入力することができ、            |
 |(Y/N)                | ることもできる: NginxServer, nginx-server,       |            | インストールプロセスを続行したい場合           |
 |                     | nginxserver.                                     |            |                                                |
 +---------------------+--------------------------------------------------+------------+------------------------------------------------+
 |Install NginxServer? | の代わりに Nginx Server, 以下の選択肢を使用す    | N(No)      | ユーザーは、Nと入力することができ、            |
 |(Y/N)                | ることもできる: NginxServer, nginx-server,       |            | インストールプロセスを終了したい場合は         |
 |                     | nginxserver.|                                    |            |                                                |
 +---------------------+--------------------------------------------------+------------+------------------------------------------------+

インストール プロセスを続行すると、Nginx の HTTP サーバーがインストールされます。Nginx のパッケージはすでにに存在する場合、ユーザーのコンピューターに、Nginx は既にそのマシンに存在するユーザーを指示するメッセージが表示されます。最終的に明確な結果とステータスのレポートが生成されます。次のスクリーン ショットは絵上記のプロセスについて説明します。

.. code-block:: bash
	

	Kevell@corp:/# ptconfigure nginx-server install
	
	Install Nginx Server? (Y/N) 
	y	
	*******************************
	*        Pharaoh Tools        *
	*         Nginx Server!       *
	*******************************
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	nginx-common nginx-core
	Suggested packages:
	fcgiwrap nginx-doc
	The following NEW packages will be installed:
	nginx nginx-common nginx-core
	0 upgraded, 3 newly installed, 0 to remove and 278 not upgraded.
	Need to get 347 kB of archives.
	After this operation, 1,295 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-common all 1.4.6-1ubuntu3.1 [17.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-core amd64 1.4.6-1ubuntu3.1 [324 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx all 1.4.6-1ubuntu3.1 [5,218 B]
	Fetched 347 kB in 3s (104 kB/s)
	Selecting previously unselected package nginx-common.
	(Reading database ... 168194 files and directories currently installed.)
	Preparing to unpack .../nginx-common_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx-common (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx-core.
	Preparing to unpack .../nginx-core_1.4.6-1ubuntu3.1_amd64.deb ...
	Unpacking nginx-core (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx.
	Preparing to unpack .../nginx_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	ureadahead will be reprofiled on next reboot
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Setting up nginx-common (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Setting up nginx-core (1.4.6-1ubuntu3.1) ...
	Setting up nginx (1.4.6-1ubuntu3.1) ...
	[Pharaoh Logging] Adding Package nginx from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	NginxServer: Success
	------------------------------
	Installer Finished
	******************************

利点
----------

* この Nginx のサーバーを使用して、ユーザーのアプリケーション設定を構成できます。
* ヘルプおよびインストール操作で使用されるパラメーター大文字小文字が区別されません中に他の人に比べて利点であります。
* Nginx は、それぞれの新しい要求のための新しいプロセスを作成する必要はありませんので高速です。
* Nginx は静的な Web ページのために特に非常に小さなメモリを使用します。
* Nginx はシステムの範囲で使用できます。
* Nginx は、拡張性とパフォーマンスはハードウェアに依存しません。
* Nginx は簡単にインストールおよび構成します。
* 、Apache のような Nginx をリードする Web サーバから期待するすべての機能があります。
* 静的ファイル サービング。
* /SSL/TLS をサポートします。
* 仮想ホスト。
* リバース プロキシ。
* 負荷分散します。
* 圧縮。
* アクセスを制御します。
* URL 書き換え。
* カスタムのログ記録。
* サーバー側が含まれています。
* WebDAV。
* ストリーミングの FLV.
* FastCGI。
 

