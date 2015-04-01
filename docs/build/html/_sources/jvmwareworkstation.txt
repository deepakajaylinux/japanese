===================
VMwareWorkstation
===================

概要
----------------

VMwareWorkステーションは、技術的な専門家を設定し、仮想マシンと対話する方法をより強力なコントロールを提供します。 ptconfigure下に貴重な時間を節約するために、仮想マシンを共有し、閲覧、接続、保護、インストールするためのオプションの様々なから選択してください。暗号化されている仮想マシンを作成し、パスワードの変更を必要とし、事前に定義された日時に満了する。これは、UbuntuとCentOSのをサポートしています。

Helpコマンド
------------------------

このヘルプコマンドは、仮想マシンと対話するユーザーをガイドします。それは、オプションのインストール、保護、接続、共有しptconfigureで利用可能表示しているパーソナライズされています。また、パスワード有効を提供します。 VMworkstationためのhelpコマンドを以下に示します。

.. code-block:: bash

	ptconfigure VMWareworkstation help

後、上記のコマンドを入力し、それがに機能して開始します。ユーザーはいつでもそこに戻ることができるように、VMwareのワークステーションの状態を保存するスナップショット機能を活用。

.. code-block:: bash

 kevell@corp:/# ptconfigure VMWareWorkstation help
 ******************************


  This command allows you to install Logstash.

  VMWareWorkstation

        - install
        Installs VMWareWorkstation
        example: ptconfigure VMWareWorkstation install

 ------------------------------
 End Help
 ******************************


インストール
-----------------

インストールが更新されたバージョンでインストールを行うために必要なVMwareWork局の設置が含まれています。それはちょうど下記のコマンドを使用して、ptconfigure Oracleの下にVMwareWorkステーションモジュールをインストールするには、マニフェストプロセスであり、

.. code-block:: bash

	ptconfigure VMwareWorkstation Install

コマンドを活性化した後、入力をcatechizeます。

はい自動的にシステムから確認するとVMwareWork駅をインストールするようにすると、ユーザー入力。インストールを終了しない場合。次のスクリーンショットVMwareWorkステーションとその機能を発揮。


.. code-block:: bash



 kevell@corp:/# ptconfigure VMWareWorkstation install
 Install VMWareWorkstation? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! VMWare Workstation !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-59050143457.sh
 chmod 755 /tmp/ptconfigure-temp-script-59050143457.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-59050143457.sh Permissions
 Executing /tmp/ptconfigure-temp-script-59050143457.sh
 --2015-03-26 11:33:55--  https://download3.vmware.com/software/wkst/file/VMware-Workstation-Full-11.0.0-2305329.x86_64.bundle
 Resolving download3.vmware.com (download3.vmware.com)... 23.65.99.51, 2600:1411:0:1a0::2ef, 2600:1411:0:193::2ef, ...
 Connecting to download3.vmware.com (download3.vmware.com)|23.65.99.51|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 438023042 (418M) [application/x-octet-stream]
 Saving to: Ã¢â‚¬ËœVMware-Workstation-Full-11.0.0-2305329.x86_64.bundleÃ¢â‚¬â„¢

 100%[======================================================================================================>] 43,80,23,042  197KB/s   in 37m 
 57s

 2015-03-26 12:11:53 (188 KB/s) - Ã¢â‚¬ËœVMware-Workstation-Full-11.0.0-2305329.x86_64.bundleÃ¢â‚¬â„¢ saved [438023042/438023042]


 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",

 (vmware-installer.py:6280): Gtk-WARNING **: Unable to locate theme engine in module_path: "murrine",
 Gtk-Message: Failed to load module "canberra-gtk-module": libcanberra-gtk-module.so: cannot open shared object file: No such file or directory
 Extracting VMware Installer...done.
 Temp File /tmp/ptconfigure-temp-script-59050143457.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VMWareWorkstation: Success
 ------------------------------
 Installer Finished
 ******************************




オプション
---------------
.. cssclass:: table-bordered

 +---------------------+-----------------------------------+------------+--------------------------------------------------+
 | パラメータ          | 代替パラメータ                    | オプション | コメント                                         |
 +=====================+===================================+============+==================================================+
 |Install VMwareWork   | VMwareWork station,               | Y          | それはファラオのツールでptconfigure              |
 |station? (Y/N)       | VMware-Workstation                |            | 下VMwareWorkstationをインストールします          |
 +---------------------+-----------------------------------+------------+--------------------------------------------------+
 |Install VMwareWork   | VMwareWork station,               | N          | システム出口インストール                         |
 |station?(Y/N)        | VMware-Workstation|               |            |                                                  |
 +---------------------+-----------------------------------+------------+--------------------------------------------------+


メリット
-------------

* 大文字小文字を区別
* UbuntuとセントOSに適し
* 仮想マシンとの対話が可能です
* オプションのVerityがご利用いただけます
* パスワードの変更が可能です
