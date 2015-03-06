=============
NetworkTools
=============

あらすじ
----------

ネットワーク ツールは、分析およびコンピュータ ネットワークのさまざまな側面を構成するように設計ソフトウェア ユーティリティです。ほとんどのオペレーティング システムで検出された最も一般的なネットワーク ツールには Traceroute、Netstat、Ping が含まれています。各ネットワーク ツールは独自の機能を持っています。

たとえば。

Ping を使用してチェック接続

Netstat は着信および発信の両方のネットワーク接続を表示するために使用します。

ヘルプ コマンド
------------------

このコマンドは、ネットワーク用ツール] モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドは、エンド ユーザー ガイドをいつ、どのように知っているに使用されるコマンドです。以下に、コマンドと同じのスクリーン ショット。



.. code-block:: bash

		ptconfigure networktools help



上記のコマンドの絵の表現は以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools help
 ******************************


  This command allows you to install a set of common Network Tools. These include
  traceroute, netstat, lsof, telnet and ps.

  NetworkTools, networktools, network-tools

        - install
        Installs the latest version of Network Tools
        example: ptconfigure networktools install

 ------------------------------
 End Help
 ******************************

インストール
---------------

とき、ユーザーはマシンで任意のネットワーク ツールをインストールする必要があります。特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash


 	ptconfigure networktool install



.. cssclass:: table-bordered


 +-----------------------+-------------------------------------------------------+------------+---------------------------------------------+
 | パラメータ            | 別のパラメータ                                        | オプション | 注釈                                        |
 +=======================+=======================================================+============+=============================================+
 |Install Network Tools? | の代わりに NetworkTools, 我々は使用することができます | Y(Yes)     | ユーザーは、Yと入力することができ、         |  
 |(Y/N)                  | networktools, network-tools.                          |            | インストールプロセスを続行したい場合        |
 +-----------------------+-------------------------------------------------------+------------+---------------------------------------------+
 |Install Network Tools? | の代わりに NetworkTools, 我々は使用することができます | N(No)      | ユーザーは、Nと入力することができ、         |
 |(Y/N)                  | networktools, network-tools.                          |            | インストールプロセスを終了したい場合は|     |
 +-----------------------+-------------------------------------------------------+------------+---------------------------------------------+


場合はインストールを続行すると、インストールの処理中に、次の手順、

* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools install
 Install Network Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Network Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  traceroute
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 45.0 kB of archives.
 After this operation, 176 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe traceroute amd64 1:2.0.20-0ubuntu0.1 [45.0 kB]
 Fetched 45.0 kB in 4s (10.0 kB/s)
 Selecting previously unselected package traceroute.
 (Reading database ... 182980 files and directories currently installed.)
 Preparing to unpack .../traceroute_1%3a2.0.20-0ubuntu0.1_amd64.deb ...
 Unpacking traceroute (1:2.0.20-0ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up traceroute (1:2.0.20-0ubuntu0.1) ...
 update-alternatives: using /usr/bin/traceroute.db to provide /usr/bin/traceroute (traceroute) in auto mode
 update-alternatives: using /usr/bin/lft.db to provide /usr/bin/lft (lft) in auto mode
 update-alternatives: using /usr/bin/traceproto.db to provide /usr/bin/traceproto (traceproto) in auto mode
 update-alternatives: using /usr/sbin/tcptraceroute.db to provide /usr/sbin/tcptraceroute (tcptraceroute) in auto mode
 [Pharaoh Logging] Adding Package traceroute from the Packager Apt executed correctly
 [Pharaoh Logging] Package netstat from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package lsof from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package telnet from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package ps from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetworkTools: Success
 ------------------------------
 Installer Finished
 ******************************


利点
-----------

このモジュールは、一般的なネットワーク ツールのセットをインストールするに役立ちます。これは、サービスが役に立つ場合ネットワーク内やインターネット上の他のコンピューターとのネットワー キングのさまざまなツールをインストールするユーザー。これにより、リモート マシンで作業しているユーザー。
 

