============
Gittools
============


あらすじ
------------

Gittools は、速度、データ整合性、および分散、非リニア ワークフローのサポートに重点を置いて分散リビジョン管理システムです。
このモジュールは、更新されたバージョンにインストールを持ち上げます。インストール中にそれはまた gitfrom、git コア、gitcole、ptconfigure の下で gitfrom をインストールできます。自動化が可能です。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
------------------

このコマンドのヘルプガイド ptconfigure についてユーザー。それ以下の時間がかかることができるので自動的にインストールされます。ユーザーのすべてのタイプに適しています。次のヘルプのコマンドは、gittools インストールのユーザーを支援します。このコマンドライン引数に関する情報が表示されるコマンドの名前を指定します。

.. code-block:: bash

		ptconfigure gittools help

コマンドの入力後は使い方を示しています。スクリーン ショットは、このコマンドの機能を表現できます。

Y
.. code-block:: bash

 kevell@corp:/# ptconfigure GitTools help
 ******************************


  This command allows you to install Git and a set of common Git Tools. These include
  Git - the distributed source control manager, git Core a supplement to Git, Gitk
  which is a GUI for git, and git-cola, which is also a Git GUI.

  GitTools, gittools, git-tools

        - install
        Installs the latest version of Git Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************


インストール
----------------

インストールには規定または操作の準備がインストールされている機器を作るに必要なサービスへの接続が含まれます。それはモジュールをインストールする gittools ptconfigure の下でちょうど、下記のコマンドを使用してマニフェスト プロセスです。


.. code-block:: bash 

		ptconfigure gittools install

それは質問攻めにコマンド入力活性化後。

ユーザーはい自動的にインストールされます gittools システムからのチェックを入力します。次のスクリーン ショットは、それを示しています。



.. code-block:: bash

 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 299 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 19s (6,077 B/s)
 Selecting previously unselected package gitk.
 (Reading database ... 176395 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 299 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 1min 3s (5,679 B/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 176413 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package libjs-underscore.
 Preparing to unpack .../libjs-underscore_1.4.4-2ubuntu1_all.deb ...
 Unpacking libjs-underscore (1.4.4-2ubuntu1) ...
 Selecting previously unselected package git-cola.
 Preparing to unpack .../git-cola_1.9.3-1_all.deb ...
 Unpacking git-cola (1.9.3-1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up libjs-underscore (1.4.4-2ubuntu1) ...
 Setting up git-cola (1.9.3-1) ...
 [Pharaoh Logging] Adding Package git-cola from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************

次の手順では、迅速な処理のインストール

ステップ 1: Install gittools ?(Y/N)
ステップ 2: の場合、ユーザーは、システム Y を与えることができますバージョンを確認し、インストール
N は、ユーザーがインストールを終了する場合は、ステップ 3 に。

オプション
---------------

.. cssclass:: table-bordered


 +----------------------+------------------------------------------------+------------+---------------------------------------------------+
 | パラメーター         | 代替パラメーター                               | オプション | コメント                                          |
 +======================+================================================+============+===================================================+
 |Install gittools?     | 代わりにgittoolsを使用するのでは、             | Y(Yes)     | それはgitのをインストールし、                     |
 |(Y/N)                 | 我々は使用することができます GitTools,         |            | ptconfigure下の共通gittoolsのセットになります。   |
 |                      | gittools, git-tools                            |            |                                                   |
 +----------------------+------------------------------------------------+------------+---------------------------------------------------+
 |Install gittools?     | 代わりにgittoolsを使用するのでは、             | N(No)      | システム出口インストール                          |
 |(Y/N)                 | 我々は使用することができます GitTools,         |            |                                                   |
 |                      | gittools, git-tools|                           |            |                                                   |
 +----------------------+------------------------------------------------+------------+---------------------------------------------------+


利点
-----------

* Gittools は、複雑なワークフローに関連付けられます。
* Gittools によって粒状コミットので簡単に他のバージョン コントロール システム （VCS） よりユーザーで決定できる正確
  次のコミットでなければなりません。
* ユーザー ワークフローの符号化を向上させる Gittools。
* git コーラは、高度な Git commit ツール、git gui に似ています。
* git コーラ グラフィカルなビューアー、簡単に、インタラクティブなステージング、inotify のサポートを備えています。

