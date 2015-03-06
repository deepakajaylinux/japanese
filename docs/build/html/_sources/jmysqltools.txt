================
MysqlTools
================

あらすじ
-----------

このモジュール MySQL サーバーを支援するいくつかのツールをインストールすることを目的します。それはまた MySQL ワークベンチ GUI をインストールしてとして容易に mytop コマンド ライン ツールと同様です。

ヘルプ コマンド
-----------------

ヘルプ コマンドはこのモジュールの処理にユーザーを指示します。これに加えて、それはまた代替パラメーターを指定します。ヘルプ オプションを使用するコマンドは次のとおりです。


.. code-block:: bash

	ptconfigure MysqlTools help


Help コマンドは、またこの mysqltools モジュールをインストールするために使用されるコマンドを指定します。スクリーン ショットの下に与えられた見てください。



.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools help

 ******************************


  This command allows you to install some tools to help with MySQL Server. Installs the MySQL
  Workbench GUI and also the mytop Command Line Tool.

  MysqlTools, mysql-tools, mysqltools

        - install
        Installs Mysql Tools through apt-get.
        example: ptconfigure mysql-tools install

 ------------------------------
 End Help
 ******************************


インストール
---------------

このモジュールは、apt-get の助けを借りて、mysql サーバをサポートする mysql のツールをインストールします。あなたのマシンに mysqltools をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

	ptconfigure MysqlTools install


.. cssclass:: table-bordered


 +---------------------+--------------------------------------------------------------+------------+----------------------------------------+
 | パラメーター        | 代替パラメーター                                             | オプション | コメント                               |
 +=====================+==============================================================+============+========================================+
 |Install MySqlTools?  | 代わりに Mysql Toolsこれらの代替名を使用することができます:  | Y(Yes)     | ユーザーは、Yと入力することができ、    |
 |(Y/N)                | MysqlTools,mysql-tools                                       |            | インストールプロセスを続行したい場合   |  
 +---------------------+--------------------------------------------------------------+------------+----------------------------------------+
 |Install MySqlTools?  | 代わりに Mysql Toolsこれらの代替名を使用することができます:  | N(No)      | ユーザーは、Nと入力することができ、    |
 |(Y/N)                | MysqlTools,mysql-tools                                       |            | インストールプロセスを続行したい場合|  |
 +---------------------+--------------------------------------------------------------+------------+----------------------------------------+



場合は、ユーザーを続行 mysql ツールをインストールする、次の操作は実行されますインストール中


* パッケージ リストを読み取ります。
* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* 必要な余分なパッケージをインストールします。
* 推奨パッケージをインストールします。
* 新しいパッケージをインストールします。
* は、アップグレード、新たにインストール、削除され、アップグレードされていないファイルの数が表示されます。

スクリーン ショット以下のようには上記のようなグラフィカルなプレゼンテーションの手順についてを与えます。



.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools install

 Install MySQL Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Tools!        *
 *******************************
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 mysql-workbench : Depends: libmysqlcppconn7 (>= 1.1.3) but it is not installabl                                                                                        e
                   Recommends: ttf-bitstream-vera but it is not going to be inst                                                                                        alled
                   Recommends: mysql-utilities but it is not going to be install                                                                                        ed
 [Pharaoh Logging] Adding Package mysql-workbench from the Packager Apt did not e                                                                                        xecute correctly
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libconfig-inifiles-perl
 The following NEW packages will be installed:
  libconfig-inifiles-perl mytop
 0 upgraded, 2 newly installed, 0 to remove and 13 not upgraded.
 Need to get 73.8 kB of archives.
 After this operation, 288 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main libconfig-inifiles-perl                                                                                         all 2.68-1 [39.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mytop all 1.9.1-1 [34                                                                                        .1 kB]
 Fetched 73.8 kB in 7s (10.5 kB/s)
 Selecting previously unselected package libconfig-inifiles-perl.
 (Reading database ... 254866 files and directories currently installed.)
 Preparing to unpack .../libconfig-inifiles-perl_2.68-1_all.deb ...
 Unpacking libconfig-inifiles-perl (2.68-1) ...
 Selecting previously unselected package mytop.
 Preparing to unpack .../archives/mytop_1.9.1-1_all.deb ...
 Unpacking mytop (1.9.1-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libconfig-inifiles-perl (2.68-1) ...
 Setting up mytop (1.9.1-1) ...
 [Pharaoh Logging] Adding Package mytop from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlTools: Success
 ------------------------------
 Installer Finished
 ******************************
 

それはまたたとえばインストールされているツールの名前を指定します


.. code-block:: bash


 .. rubric:: mysql-server-core-5.5:amd64, mysql-server-5.5: amd64, libaio1:amd64, mysql-server:amd64.

利点
----------

* ユーザーは、mysql サーバをサポートする、必要なツールをインストールできます。
* それが容易になります MySQL のワークベンチ GUI をインストールしてとしても mytop コマンド ライン ツールとして。
* インストールの完了後は新たにインストールされているツールのリストが表示されます。
 
