=======================
ApacheReverseProxy
=======================

あらすじ
-----------

このモジュール ライブラリ関数のインストールを目指します。インストール中に、ライブラリ関数、それは既存の空室状況をチェックはライブラリ関数。それの管理とアプリケーション設定を構成するのに役立ちます。ユーザーは、アプリケーション設定の既定値を指定できます。

ヘルプ コマンド
----------------

Help コマンドの使用、またとオプションのアクションを実行することができます注意してくださいユーザー取得について説明します。アウトが表示されます、代替
ようにコーディング Apache がリバース プロキシ モジュールの下に help コマンドの使用、次のように与えられる

.. code-block:: bash

	cleopatra ApacheReverseProxyModules help

以下に示す撮影画面ヘルプ コマンドの使用方法の絵の表現を与えます。



.. code-block:: bash

          Kevell@corp/# cleopatra ApacheReverseProxyModules help
	  ******************************


	  This command is part of Core and provides you  with a method by which you can configure Application Settings.
	  You can configure default application settings, ie: mysql admin user, host, pass

	  ApacheReverseProxyModules, apache-reverse-proxy-modules, apache-proxy-mods, apacheproxymodules, apache-lb-mods,
	  apache-load-balancer-modules

          - install
	        Installs Load Balancer/Reverse Proxy Apache Modules
        	example: cleopatra apache-lb-mods install

	  ------------------------------
          End Help
	  ****************************


インストール
---------------

以下に、コマンドを入力することができる場合は、apache をインストールするユーザーの願いリバース プロキシ モジュール システムに

.. code-block:: bash

		cleopatra ApacheReverseProxyModules install


オプション
------------

.. cssclass:: table-bordered


 +-----------------------+---------------------------------------------------+--------------+-------------------------------------+
 | パラメーター          | 代替パラメーター                                  | 必要な       | コメント                            |
 +=======================+===================================================+==============+=====================================+
 |Install ReverseProxy   | 代わりにReverseProxy ApacheModulesのユーザーは、  | Y(Yes)       | Yのようなユーザ入力は、             |
 |ApacheModules (Y/N)    | 次のパラメータを指定することができます。          |              | Apacheのリバースプロキシモジュール  |
 |                       | ApacheReverseProxyModules,                        |              | がインストールされます場合は        |
 |                       | apache-reverse-proxy-modules, apache- proxy-mods, |              |                                     |
 |                       | apacheproxymodules, apache-lb-mods,               |              |                                     |
 |                       | apache-load-balancer, modules                     |              |                                     |
 +-----------------------+---------------------------------------------------+--------------+-------------------------------------+
 |Install ReverseProxy   | 代わりにReverseProxy ApacheModulesのユーザーは、  | N(No)        | N等のユーザ入力した場合、           |
 |ApacheModules (Y/N)    | 次のパラメータを指定することができます。          |              | プロセスの意志がインストールから突  |
 |                       | ApacheReverseProxyModules,                        |              | 然終了を取得します。                |
 |                       | apache-reverse-proxy-modules, apache- proxy-mods, |              |                                     |
 |                       | apacheproxymodules, apache-lb-mods,               |              |                                     |
 |                       | apache-load-balancer, modules|                    |              |                                     |
 +-----------------------+---------------------------------------------------+--------------+-------------------------------------+


インストール中に、リバース プロキシ モジュール、状態情報、パッケージ一覧のビルド依存関係ツリーは読み取ります。すべてのパッケージがない場合は、新しいパッケージがインストールされます。スクリーン ショットは以下に示すグラフィカル インストールのプロセスについて説明します。

.. code-block:: bash


 kevell@corp:/#: cleopatra ApacheReverseProxyModules install
 Install Apache Rev. Proxy Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Proxy Mods!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libapache2-mod-proxy-html
 0 upgraded, 1 newly installed, 0 to remove and 229 not upgraded.
 Need to get 1,464 B of archives.
 After this operation, 22.5 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libapache2-mod-proxy-html amd64 1:2.4.7-1ubuntu4.1 [1,464 B]
 Fetched 1,464 B in 1s (1,323 B/s)
 Selecting previously unselected package libapache2-mod-proxy-html.
 (Reading database ... 181545 files and directories currently installed.)
 Preparing to unpack .../libapache2-mod-proxy-html_1%3a2.4.7-1ubuntu4.1_amd64.deb ...
 Unpacking libapache2-mod-proxy-html (1:2.4.7-1ubuntu4.1) ...
 Setting up libapache2-mod-proxy-html (1:2.4.7-1ubuntu4.1) ...
 [Pharaoh Logging] Adding Package libapache2-mod-proxy-html from the Packager Apt executed correctly
 [Pharaoh Logging] Package libxml2-dev from the Packager Apt is already installed, so not installing
 Creating /tmp/cleopatra-temp-script-49127207421.sh
 chmod 755 /tmp/cleopatra-temp-script-49127207421.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-49127207421.sh Permissions
 Executing /tmp/cleopatra-temp-script-49127207421.sh
 Considering dependency proxy_balancer for lbmethod_byrequests:
 Considering dependency proxy for proxy_balancer:
 Enabling module proxy.
 Considering dependency alias for proxy_balancer:
 Module alias already enabled
 Considering dependency slotmem_shm for proxy_balancer:
 Enabling module slotmem_shm.
 Enabling module proxy_balancer.
 Enabling module lbmethod_byrequests.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-49127207421.sh Removed
 Creating /tmp/cleopatra-temp-script-12740464083.sh
 chmod 755 /tmp/cleopatra-temp-script-12740464083.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-12740464083.sh Permissions
 Executing /tmp/cleopatra-temp-script-12740464083.sh
 Module proxy already enabled
 Temp File /tmp/cleopatra-temp-script-12740464083.sh Removed
 Creating /tmp/cleopatra-temp-script-61839737362.sh
 chmod 755 /tmp/cleopatra-temp-script-61839737362.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-61839737362.sh Permissions
 Executing /tmp/cleopatra-temp-script-61839737362.sh
 Considering dependency proxy for proxy_http:
 Module proxy already enabled
 Enabling module proxy_http.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-61839737362.sh Removed
 Creating /tmp/cleopatra-temp-script-22752304452.sh
 chmod 755 /tmp/cleopatra-temp-script-22752304452.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-22752304452.sh Permissions
 Executing /tmp/cleopatra-temp-script-22752304452.sh
 ERROR: Module mod_proxy_http does not exist!
 Temp File /tmp/cleopatra-temp-script-22752304452.sh Removed
 Creating /tmp/cleopatra-temp-script-19250932602.sh
 chmod 755 /tmp/cleopatra-temp-script-19250932602.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-19250932602.sh Permissions
 Executing /tmp/cleopatra-temp-script-19250932602.sh
 Considering dependency proxy for proxy_ftp:
 Module proxy already enabled
 Enabling module proxy_ftp.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-19250932602.sh Removed
 Creating /tmp/cleopatra-temp-script-38556602379.sh
 chmod 755 /tmp/cleopatra-temp-script-38556602379.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-38556602379.sh Permissions
 Executing /tmp/cleopatra-temp-script-38556602379.sh
 Considering dependency proxy for proxy_connect:
 Module proxy already enabled
 Enabling module proxy_connect.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-38556602379.sh Removed
 Creating /tmp/cleopatra-temp-script-85272088847.sh
 chmod 755 /tmp/cleopatra-temp-script-85272088847.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-85272088847.sh Permissions
 Executing /tmp/cleopatra-temp-script-85272088847.sh
 Considering dependency proxy for proxy_ajp:
 Module proxy already enabled
 Enabling module proxy_ajp.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-85272088847.sh Removed
 Creating /tmp/cleopatra-temp-script-31029043648.sh
 chmod 755 /tmp/cleopatra-temp-script-31029043648.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-31029043648.sh Permissions
 Executing /tmp/cleopatra-temp-script-31029043648.sh
 Considering dependency proxy for proxy_wstunnel:
 Module proxy already enabled
 Enabling module proxy_wstunnel.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-31029043648.sh Removed
 Creating /tmp/cleopatra-temp-script-2400353229.sh
 chmod 755 /tmp/cleopatra-temp-script-2400353229.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-2400353229.sh Permissions
 Executing /tmp/cleopatra-temp-script-2400353229.sh
 Considering dependency proxy for proxy_balancer:
 Module proxy already enabled
 Considering dependency alias for proxy_balancer:
 Module alias already enabled
 Considering dependency slotmem_shm for proxy_balancer:
 Module slotmem_shm already enabled
 Module proxy_balancer already enabled
 Temp File /tmp/cleopatra-temp-script-2400353229.sh Removed
 Creating /tmp/cleopatra-temp-script-88564779807.sh
 chmod 755 /tmp/cleopatra-temp-script-88564779807.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-88564779807.sh Permissions
 Executing /tmp/cleopatra-temp-script-88564779807.sh
 Enabling module cache.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-88564779807.sh Removed
 Creating /tmp/cleopatra-temp-script-68936090528.sh
 chmod 755 /tmp/cleopatra-temp-script-68936090528.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-68936090528.sh Permissions
 Executing /tmp/cleopatra-temp-script-68936090528.sh
 Enabling module headers.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-68936090528.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 Output of config test was:
 apache2: Syntax error on line 214 of /etc/apache2/apache2.conf: Could not open configuration file /etc/apache2/httpd.conf: No such file or dir ectory.
 Action 'configtest' failed.
 The Apache error log may have more information.
 * Restarting web server apache2
   ...fail!
 * The apache2 configtest failed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 ApacheReverseProxyModules: Success
 ------------------------------
 Installer Finished
 ******************************


ユーザーのメリット
----------------------

* 利用可能なパッケージ リストを表示し、順番に不足していると必要なパッケージをインストールします。
  逆のプロキシは、任意のクライアントに代わっての固定のリンク先に転送します。
* それは 1 つのサーバーから大規模なウェブサイトにホストされているコンテンツが組み込まれています。
* それは、アプリケーション設定を構成するのに役立ちます。
* それは裕福なセント OS とも ubuntu のように。
* 宣言で使用されるパラメーターは大文字と小文字を区別する加えられた利点であります。

