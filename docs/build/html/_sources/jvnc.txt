===========
VNC
===========

あらすじ
-------------

このモジュールは VNC4server の apt 経由でインストールするための支援を提供します。仮想マシン接続を使用できます。インストールの前に保証を促進します。

ヘルプ コマンド
-----------------

Help コマンドは、VNC モジュールに関する意識を提供します。また、この VNC モジュールの下に実行可能なオプションについて説明します。
この VNC モジュールのヘルプ コマンドは下記します。

.. code-block:: bash

	ptconfigure vnc help

スクリーン ショットの下に与えられた VNC モジュールの下に help コマンドの使用に関する表現を示します。


.. code-block:: bash

 Kevell@corp:/# ptconfigure vnc help
 ******************************


        This command allows you to install VNC, the popular Virtual Machine Solution.

	 VNC, vnc

        - install
        Installs VNC through apt-get
        example: ptconfigure vnc install

	------------------------------
	End Help
	******************************


インストール
------------------



.. code-block:: bash
	
		ptconfigure vnc install

上記のようにコマンドを入力した後、次の操作の場所をかかります。


.. cssclass:: table-bordered

 +----------------------+-------------------+-------------+------------------------------------------------------------------+
 | パラメータ           | 別のパラメータ    | オプション  | コメント                                                         |
 +======================+===================+=============+==================================================================+
 |Install VNC? (Y/N)    | VNC, vnc          | Y(Yes)      | Y.Parametersとして、ユーザは、インストールプロセスを続行した     |
 |                      |                   |             | い場合は、彼らが入力できる                                       |
 +----------------------+-------------------+-------------+------------------------------------------------------------------+
 | Install VNC? (Y/N)   | VNC, vnc          | N(No)       | ユーザーがインストールプロセスを終了したい場合は、 Nを使用し     |
 |                      |                   |             | て簡単に終了することができます|                                  |
 +----------------------+-------------------+-------------+------------------------------------------------------------------+




VNC サーバーのインストール中は下与えられる次操作を実行します。

* パッケージ リスト、状態情報を読み取ります
* 依存関係ツリーを構築します。
* 余分なパッケージを提案パッケージとして vnc java として xbase クライアントをインストールします。
* 新しいパッケージとして vnc4server xbase クライアントをインストールします。
* それもアップグレードすると、ファイルの数が表示されます新しくインストール、削除、アップグレードされません。

スクリーン ショットは、以下に示すインストールのプロセスに関してグラフィカル ユーザーについて説明します。


.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  xbase-clients
 Suggested packages:
  vnc-java
 The following NEW packages will be installed:
  vnc4server xbase-clients
 0 upgraded, 2 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,579 kB of archives.
 After this operation, 5,418 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe xbase-clients all 1:7.7+1ubuntu8 [2,752 B]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vnc4server amd64 4.1.1+xorg4.3.0-37ubuntu5.0.1 [1,577 kB]
 Fetched 1,579 kB in 33s (46.6 kB/s)
 Selecting previously unselected package xbase-clients.
 (Reading database ... 211210 files and directories currently installed.)
 Preparing to unpack .../xbase-clients_1%3a7.7+1ubuntu8_all.deb ...
 Unpacking xbase-clients (1:7.7+1ubuntu8) ...
 Selecting previously unselected package vnc4server.
 Preparing to unpack .../vnc4server_4.1.1+xorg4.3.0-37ubuntu5.0.1_amd64.deb ...
 Unpacking vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xbase-clients (1:7.7+1ubuntu8) ...
 Setting up vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 update-alternatives: using /usr/bin/vnc4server to provide /usr/bin/vncserver (vncserver) in auto mode
 update-alternatives: using /usr/bin/Xvnc4 to provide /usr/bin/Xvnc (Xvnc) in auto mode
 update-alternatives: using /usr/bin/x0vnc4server to provide /usr/bin/x0vncserver (x0vncserver) in auto mode
 update-alternatives: using /usr/bin/vnc4passwd to provide /usr/bin/vncpasswd (vncpasswd) in auto mode
 update-alternatives: using /usr/bin/vnc4config to provide /usr/bin/vncconfig (vncconfig) in auto mode
 [Pharaoh Logging] Adding Package vnc4server from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************



ユーザーのコンピューターに、vnc サーバーが既に存在する場合それはスローします例外メッセージ vnc サーバーが既にインストールされています。次のスクリーン ショットは、例外メッセージに関する表現を与えます。

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 [Pharaoh Logging] Package vnc4server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************



利点
---------------

* インストールの前に保証するプロセスことができます。
* それは apt 経由でのインストールを容易にします。
* それは仮想マシン接続を使用できます。
* の VNC サーバーは既に存在する場合に確保のプロセス中に例外メッセージがスローされます。
 

