============
NetBeans
============

概要
-------------

NetBeansはJavaをするだけでなく、他の言語、特にPHP、C / C ++、およびHTMLで主に開発するための統合開発環境（IDE）である。また、Javaデスクトップアプリケーションなどのためのアプリケーション·プラットフォーム·フレームワークです。

NetBeans IDEは、Javaで書かれているし、Windows、OS X、Linuxの、Solarisおよび互換性のあるJVMをサポートしている他のプラットフォーム上で実行することができます。 NetBeans IDEは、Javaプログラミング言語のためのビルトインサポートとクロスプラットフォームIDEです。

NetBeansプラットフォームは、アプリケーションがモジュールと呼ばれるモジュール式のソフトウェアコンポーネントのセットから開発することができます。 （NetBeans IDEの自身を含む）NetBeansプラットフォームに基づくアプリケーションは、サードパーティの開発者によって拡張することができます。

helpコマンド
----------------------

このコマンドは、NetBeansモジュールの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash
        
        ptconfigure Netbeans help


.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans help
 ******************************


  This command allows you to install and uninstall NetBeans - IDE.

  NetBeans, Netbeans, netbeans

        - install
        Installs a version of NetBeans.
        example: ptconfigure netbeans install
	
	- uninstall
        Uninstalls a version of NetBeans.
        example: ptconfigure netbeans uninstall
 ------------------------------
 End Help
 ******************************



インストール
----------------

このコマンドは、システム内のNetbeansのをインストールするのに役立ちます。以下のコマンドは、インストールのプロセスを実行します。

.. code-block:: bash
        
        ptconfigure netbeans install


.. code-block:: bash


 kevell@corp:/# ptconfigure netbeans install
 Install NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed

 Enter (1) to Install NetBeans in Silent:
 Enter (2) to install NetBeans in UserFriendly:
 1
 Creating /tmp/ptconfigure-temp-script-53829501149.sh
 chmod 755 /tmp/ptconfigure-temp-script-53829501149.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-53829501149.sh Permissions
 Executing /tmp/ptconfigure-temp-script-53829501149.sh
 --2015-04-01 11:42:15--  http://download.netbeans.org/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving download.netbeans.org (download.netbeans.org)... 137.254.120.26
 Connecting to download.netbeans.org (download.netbeans.org)|137.254.120.26|:80... connected.
 HTTP request sent, awaiting response... 302 Moved Temporarily
 Location: http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh [following]
 --2015-04-01 11:42:16--  http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving dlc-cdn.sun.com (dlc-cdn.sun.com)... 23.205.118.80, 23.205.118.73
 Connecting to dlc-cdn.sun.com (dlc-cdn.sun.com)|23.205.118.80|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 212403200 (203M) [application/x-sh]
 Saving to: â€˜netbeans-8.0-linux.shâ€™ 

 100%[===========================================================================================>] 21,24,03,200 78.0KB/s   in 78m 40s

 2015-04-01 13:00:58 (43.9 KB/s) - â€˜netbeans-8.0-linux.shâ€™ saved [212403200/212403200]

 Temp File /tmp/ptconfigure-temp-script-53829501149.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ****************************** 


アンインストール
-------------------

このコマンドは、システム内のNetbeansのをアンインストールするのに役立ちます。以下のコマンドは、インストールのプロセスを実行します。


.. code-block:: bash

	ptconfigure netbeans uninstall

.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans uninstall

 Uninstall NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80402838784.sh
 chmod 755 /tmp/ptconfigure-temp-script-80402838784.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80402838784.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80402838784.sh
 Configuring the installer...
 Searching for JVM on the system...
 Extracting installation data...
 Running the installer wizard...
 Temp File /tmp/ptconfigure-temp-script-80402838784.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ******************************




オプション
-----------

.. cssclass:: table-bordered

 +----------------------+-------------------------------------------------------+--------------+----------------------------------------+
 | パラメーター         | 代替パラメータ                                        | オプション   | コメント                               |
 +======================+=======================================================+==============+========================================+
 |Install Netbeans?     | コマンドラインで使用することができる三つの別のパラメ  | Y            | システムは、インストールプロセスを     |
 |                      | ーターが存在する。 Netbeans , NetBeans , netbeans     |              | 開始します                             |
 |                      | 例えば： ptconfigure NetBeans install,                |              |                                        |
 |                      | ptconfigure netbeans install                          |              |                                        |
 +----------------------+-------------------------------------------------------+--------------+----------------------------------------+
 |Install Netbeans?     | コマンドラインで使用することができる三つの別のパラメ  | N            | システムは、インストール·              |
 |                      | ーターが存在する。 Netbeans , NetBeans , netbeans     |              | プロセスを停止し、                     |
 |                      | 例えば： ptconfigure NetBeans install,                |              |                                        |
 |                      | ptconfigure netbeans install|                         |              |                                        |
 +----------------------+-------------------------------------------------------+--------------+----------------------------------------+


メリット
--------------

* ユーザーインターフェース管理（例えばメニューとツールバー）
* ユーザー設定管理
* ストレージ管理（あらゆる種類のデータを保存と読み込み）
* ウィンドウ管理
* ウィザードフレームワークは、（ステップ·バイ·ステップのダイアログをサポートしています）
* NetBeansのビジュアルライブラリ
* 統合された開発ツール
