==============
Jenkins
==============

あらすじ
-------------

ジェンキンスさんはビルド サーバーに人気です。ジェンキンスさんは Java で書かれたオープン ソースの継続的な統合ツールです。ジェンキンスさんはソフトウェア開発のための継続的な統合サービスを提供します。例えば Apache Tomcat サーブレット コンテナーで実行しているサーバー ベースのシステムです。
ジェンキンスのコア機能と柔軟性に合わせて、さまざまな環境で、すべての利害関係者のための開発プロセスを合理化することができます。

ヘルプ コマンド
----------------------

このコマンドは、ジェンキンス モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。



.. code-block:: bash
             
		ptconfigure jenkins help


上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash

 
 kevell@corp:/# ptconfigure jenkins help
 ******************************


 This command allows you to install Jenkins, the popular Build Server.

 Jenkins, jenkins

 - install
 Installs Jenkins through apt-get
 example: ptconfigure jenkins install

 ------------------------------
 End Help
 ******************************




インストール
----------------

ユーザーのマシンでジェンキンス モジュールをインストールする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
              
	        ptconfigure jenkins install



上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins install
 Install Jenkins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Jenkins !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-14615194352.sh
 chmod 755 /tmp/ptconfigure-temp-script-14615194352.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-14615194352.sh Permissions
 Executing /tmp/ptconfigure-temp-script-14615194352.sh
 E: Could not get lock /var/lib/apt/lists/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/lib/apt/lists/
 OK
 Temp File /tmp/ptconfigure-temp-script-14615194352.sh Removed
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
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
 jenkins : Depends: daemon but it is not installable
           Depends: default-jre-headless but it is not installable or
                    java-runtime-headless
 [Pharaoh Logging] Adding Package jenkins from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jenkins: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
-----------                               

.. cssclass:: table-bordered

 +-----------------------+--------------------------------------------+-------------+----------------------------------------------+
 | パラメーター          | 代替パラメーター                           | オプション  | コメント                                     |
 +=======================+============================================+=============+==============================================+
 |ptconfigure Jenkins    | 代わりに使用したの Jenkins, ユーザーが追   | Y(Yes)      | ユーザがオプションを提供すると、             |
 |Install                | 加することができますjenkins                |             | システムはインストールプロセスを開始します   |
 +-----------------------+--------------------------------------------+-------------+----------------------------------------------+
 |ptconfigure Jenkins    | 代わりに使用したの Jenkins, ユーザーが追   | N(No)       | ユーザがオプションを提供すると、             |
 |Install                | 加することができますjenkins                |             | システムはインストールプロセスを停止します|  |
 +-----------------------+--------------------------------------------+-------------+----------------------------------------------+


利点
--------------

* 即時バグ検出
* いいえインテグレーション ステップのライフ サイクル
* 任意の時点で展開可能なシステム
* プロジェクトの進化の記録
 
