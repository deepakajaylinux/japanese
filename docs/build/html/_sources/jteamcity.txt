====================
Teamcity モジュール
====================

あらすじ
---------

Teamcity は、Java ベースのビルドの管理と継続的な統合サーバーです。このモジュールは Teamcity server の最新バージョンとその依存関係をインストールすることを目指しています。

ヘルプ コマンド
----------------

ヘルプ コマンドはタスクを達成するために必要を提供するためにユーザーをガイドします。確認するコマンド、ターミナルの下でのヘルプの使用を次のように与えられる

.. code-block:: bash

	ptconfigure Teamcity help


下のスナップショットは、help コマンドの絵の表現を与えるし、Teamcity と teamcity として 2 つのパラメーターを一覧表示します。(パラメーターは大文字と小文字)


.. code-block:: bash

	kevell@copy:/# ptconfigure teamcity help
	******************************


	This command allows you to install Teamcity, the popular Build Server.

	Teamcity, teamcity

        - install
        Installs Teamcity from the Jetbrains distributed native package
        example: ptconfigure teamcity install

	------------------------------
	End Help
	******************************


インストール
---------------

Teamcity モジュールをインストールするために使用されるコマンドは下記します。


.. code-block:: bash

	ptconfigure Teamcity install



下のスクリーン ショットでは、teamcity モジュールをインストールする方法について説明します。

.. code-block:: bash


	kevell@corp:/# ptconfigure Teamcity install
	Install Teamcity? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Teamcity !        *
	*******************************
	PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/Teamcity/Model/TeamcityUbuntu.php on line 42
	[Pharaoh Logging] Ensure module install is not checking versions
	[Pharaoh Logging] Module Java reports itself as Installed
	[Pharaoh Logging] Not installing as already installed
	Creating /tmp/ptconfigure-temp-script-82478215982.sh
	chmod 755 /tmp/ptconfigure-temp-script-82478215982.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-82478215982.sh Permissions
	Executing /tmp/ptconfigure-temp-script-82478215982.sh
	--2015-01-08 14:42:15--  http://download.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download.jetbrains.com (download.jetbrains.com)... 54.217.236.18
	Connecting to download.jetbrains.com (download.jetbrains.com)|54.217.236.18|:80... connected.
	HTTP request sent, awaiting response... 302 Moved Temporarily
	Location: http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz [following]
	--2015-01-08 14:42:16--  http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download-cf.jetbrains.com (download-cf.jetbrains.com)... 54.230.190.208, 54.230.190.220, 54.230.190.210, ...
	Connecting to download-cf.jetbrains.com (download-cf.jetbrains.com)|54.230.190.208|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 551078596 (526M) [application/x-tar]
	Saving to: ‘TeamCity-8.1.3.tar.gz’
		
	 99% [                                                                                                   >  ] 60,46,771   63.3KB/s 	



オプション
------------


.. cssclass:: table-bordered


 +----------------------+-----------+------------------------------------------------------------------------------------------------+
 | パラメーター         | 必要な    | コメント                                                                                       |
 +======================+===========+================================================================================================+
 |ptconfigure Teamcity  | Y(Yes)    | このコマンドは、チームシティー·モジュールをインストールします                                  |
 |install               |           |                                                                                                |
 +----------------------+-----------+------------------------------------------------------------------------------------------------+
 |Install Teamcity      | Y         | ユーザーは、Y、出口が、それは、新しいバージョンを更新あるいはそれがサポートする要件を持つ      |
 |( Y/N)                |           | 新鮮なパッケージをインストールする場合は、チームシティ>ーするための要件をサポートするため、    |
 |                      |           | このモジュールのチェックを入力すると。                                                         |
 +----------------------+-----------+------------------------------------------------------------------------------------------------+
 |Install Teamcity      | N         | ユーザーは、Nを入力すると、インストールが中止された。                                          |
 |( Y/N)|               |           |                                                                                                |
 +----------------------+-----------+------------------------------------------------------------------------------------------------+
  

ユーザーのメリット
-----------------------

Teamcity サーバーを効率的に実行するすべてのサポート要件をインストールします。

* アクセス、インストールの使いやす
* コーディングは大文字小文字を区別です。

 

