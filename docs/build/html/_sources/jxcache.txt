==========
Xcache
==========

概要
---------

XCache はフリー、オープン ソースの操作コード cacher、サーバー上の PHP スクリプトの実行のパフォーマンスを強化するために設計されています。コードのコンパイル済みバージョンがメモリにキャッシュすることで PHP コードのコンパイル時間を排除することによってパフォーマンスを最適化し、このようにコンパイル済みのバージョンは、メモリから直接 PHP スクリプトを読み込みます。

Helpコマンド
-------------

このコマンドは xcache の使用状況を判断するのに役立ちます。Xcache の代替パラメーターを示します。また、xcache モジュールの機能の構文について説明します。Xcache のヘルプ コマンドが表示されます以下の通りです。							 

.. code-block:: bash

	ptconfigure xcache help

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache help
 ******************************


  This command allows you to update Xcache.

  Xcache, xcache

        - install
        Installs the latest version of xcache
        example: ptconfigure xcache install

 ------------------------------
 End Help
 ******************************


インストール
----------------


端末上で xcache モジュールをインストールするために使用されるコマンドは以下します。

.. code-block:: bash

        ptconfigure xcache install

上記のコマンドは xcache とその依存関係の最新バージョンをインストールすることを目指しています.


上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache install
 Install Xcache? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Xcache!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-56147605410.sh
 chmod 755 /tmp/ptconfigure-temp-script-56147605410.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-56147605410.sh Permissions
 Executing /tmp/ptconfigure-temp-script-56147605410.sh
 --2015-03-20 17:05:11--  http://kr.archive.ubuntu.com/ubuntu/pool/universe/x/xcache/php5-xcache_3.1.0-2_amd64.deb
 Resolving kr.archive.ubuntu.com (kr.archive.ubuntu.com)... 103.22.220.133
 Connecting to kr.archive.ubuntu.com (kr.archive.ubuntu.com)|103.22.220.133|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 108582 (106K) [application/x-debian-package]
 Saving to: ‘php5-xcache_3.1.0-2_amd64.deb.1’

 100%[=======================================================================================================>] 1,08,582    36.1KB/s   in 2.9s   

 2015-03-20 17:05:15 (36.1 KB/s) - ‘php5-xcache_3.1.0-2_amd64.deb.1’ saved [108582/108582]

 php5_invoke xcache: already enabled for apache2 SAPI
 php5_invoke xcache: already enabled for cli SAPI
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 (Reading database ... 195553 files and directories currently installed.)
 Preparing to unpack php5-xcache_3.1.0-2_amd64.deb ...
 Unpacking php5-xcache (3.1.0-2) over (3.1.0-2) ...
 Setting up php5-xcache (3.1.0-2) ...
 * Restarting web server apache2
   ...done.
 Temp File /tmp/ptconfigure-temp-script-56147605410.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xcache: Success
 ------------------------------
 Installer Finished
 ******************************



代替パラメータ
-----------------------

2 つの代替パラメーターをコマンドラインで使用することができますがあります。

Xcache, xcache


メリット
-----------

* 安定した動作 
* 新しい PHP バージョンへの迅速な適応 
* 簡単なインストール









