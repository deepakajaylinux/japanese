==============
VMWarePlayer
==============

概要
----------------

VMPlayerは、既存の仮想アプライアンスを実行し、（機能的であるように、インストールするオペレーティングシステムが必要です）独自の仮想マシンを作成することができます。これは、VMware Workstationの、より多くの機能ではなく、無償で同様のプログラムと同じ仮想化コアを使用しています。 VMware Playerはptconfigureで利用可能です。これは、UbuntuとCentOSので適しています。

Helpコマンド
-----------------------

このヘルプコマンドは、仮想マシンのプレイヤーを作成するためのユーザーをガイドします。 ptconfigureに特化した。また、仮想マシンの機能を提供します
プレイヤー。Vmplayerためのhelpコマンドを以下に示します。

.. code-block:: bash
		
	ptconfigure VMWarePlayer help


後に上記のコマンドを入力すると、プレーヤ設定を作成する機能を開始する。これは、スクリーンショットでvmplayerの機能を教理。

インストール
-----------------

vmplayerのインストールが更新されたバージョンでインストールを行うために必要。それは、単に以下のコマンドを使用して、ptconfigure下vmplayerモジュールをインストールするためのマニフェストプロセスであり、

.. code-block:: bash

	ptconfigure VMWarePlayer install


コマンドを活性化した後、入力をcatechizeます。

はい自動的にシステムからのチェックでvmplayerをインストールするようにすると、ユーザー入力。インストールを終了しない場合。以下のスクリーンショットは、vmplayerとその機能を発揮。


オプション
------------

.. cssclass:: table-bordered

 +-----------------------+------------------------------------+--------------+-----------------------------------------------+
 | パラメータ            | 代替パラメータ                     | オプション   | コメント                                      |
 +=======================+====================================+==============+===============================================+
 |Install vmplayer?(Y/N) | vmplayer, VMPlayer, VM-player      | Y            | それはファラオのツールでptconfigure下に       |
 |                       |                                    |              | vmplayerインストールされます                  |
 +-----------------------+------------------------------------+--------------+-----------------------------------------------+
 |Install vmplayer?(Y/N) | vmplayer, VMPlayer, VM-player      | N            | システム出口インストール|                     |
 +-----------------------+------------------------------------+--------------+-----------------------------------------------+

.. code-block:: bash

 kevell@corp:/# ptconfigure VMWarePlayer install
 Install VMWarePlayer? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! VMWare Player !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-7944529549.sh
 chmod 755 /tmp/ptconfigure-temp-script-7944529549.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-7944529549.sh Permissions
 Executing /tmp/ptconfigure-temp-script-7944529549.sh
 --2015-03-26 10:24:11--  https://download3.vmware.com/software/player/file/VMware-Player-7.0.0-2305329.x86_64.bundle
 Resolving download3.vmware.com (download3.vmware.com)... 23.65.99.51, 2600:1411:0:193::2ef, 2600:1411:0:1a0::2ef, ...
 Connecting to download3.vmware.com (download3.vmware.com)|23.65.99.51|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 210911382 (201M) [application/x-octet-stream]
 Saving to: â€˜VMware-Player-7.0.0-2305329.x86_64.bundleâ€™ 

 100%[======================================================================================================>] 21,09,11,382 44.1KB/s   in 2h
 36m 

 2015-03-26 13:01:08 (21.9 KB/s) - â€˜VMware-Player-7.0.0-2305329.x86_64.bundleâ€™ saved [210911382/210911382]


 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine", 

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:25874): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",
 Gtk-Message: Failed to load module "canberra-gtk-module": libcanberra-gtk-module.so: cannot open shared object file: No such file or directory
 Extracting VMware Installer...done.
 Temp File /tmp/ptconfigure-temp-script-7944529549.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VMWarePlayer: Success
 ------------------------------
 Installer Finished
 ******************************



メリット
----------------

* 既存の仮想appliencesを実行して、仮想マシンを作成する
* 大文字小文字を区別
* UbuntuとセントOSに適し
* 専門家のすべての種類のために使用される
