======
HHVM
======

あらすじ
------------

このモジュールは、インストールを容易に、国連 HHVM 人気ビルド サーバー コンピューターをインストールします。ヒップホップ仮想マシン （HHVM） は、ジャスト イン タイム (JIT) コンパイルに基づいてプロセス仮想マシン ハックと PHP のプログラミング言語のための実行エンジンを務めています。JIT コンパイルの原則を使用して、実行される PHP やハックのコード最初であり動的に x 86 64 マシン コードに変換して、最適化されたネイティブで実行される中間のヒップホップ バイト コード (HHBC) に変換されます。今後のテーマで HHVM モジュールについてみてみましょう。

ヘルプ コマンド
------------------

Help コマンドと同様、目的に関するユーザー ガイドとして HHVM モジュールに含まれているオプションについて。それは HHVM モジュールの代替パラメーターが一覧表示されます。また、HHVM モジュールをインストールするための構文について説明します。HHVM モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		ptconfigure HHVM help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、HHVM の下で help コマンドについて視覚化します。


.. code-block:: bash


 kevell@corp:/# ptconfigure HHVM help
 ******************************


  This command allows you to install HHVM, the popular Build Server.

  HHVM, hhvm

        - install
        Installs HHVM through package manager
        example: ptconfigure hhvm install

        - uninstall
        Uninstalls HHVM through package manager
        example: ptconfigure hhvm uninstall

 ------------------------------
 End Help
 ******************************



インストール
----------------

ユーザーのマシンに HHVM をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

                ptconfigure HHVM install

上記のコマンドを入力した後、次のプロセスが発生します表形式で表示されます。


.. cssclass:: table-bordered


 +-----------------------+-----------------------------------------+------------+------------------------------------------------------+
 | パラメータ            | 代替パラメータ                          | オプション | 注釈                                                 |
 +=======================+=========================================+============+======================================================+
 |Install HHVM? (Y/N)    | 代わりにHHVMの我々はまた、hhvm使用する  | Y(Yes)     | ユーザーは、Yと入力することができ、                  |
 |                       | ことができます。                        |            | インストールプロセスを続行したい場合                 |
 +-----------------------+-----------------------------------------+------------+------------------------------------------------------+
 |Install HHVM? (Y/N)    | 代わりにHHVMの我々はまた、hhvm使用する  | N(No)      | ユーザーは、Nと入力することができ、                  |
 |                       | ことができます。                        |            | インストールプロセスを終了したい場合は|              |
 +-----------------------+-----------------------------------------+------------+------------------------------------------------------+



最後に、インストール プロセスを完了を取得します。次のスクリーン ショットは、絵 HHVM をインストールするプロセスを表します。

.. code-block:: bash

 kevell@corp:/# ptconfigure HHVM install
 Install HHVM? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! HHVM !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-41870275104.sh
 chmod 755 /tmp/ptconfigure-temp-script-41870275104.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-41870275104.sh Permissions
 Executing /tmp/ptconfigure-temp-script-41870275104.sh
 --2015-01-16 14:19:14--  http://dl.hhvm.com/conf/hhvm.gpg.key
 Resolving dl.hhvm.com (dl.hhvm.com)... 140.211.166.134
 Connecting to dl.hhvm.com (dl.hhvm.com)|140.211.166.134|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 1707 (1.7K) [application/pgp-keys]
 Saving to: ‘STDOUT’

 100%[=====================================================================================================>] 1,707       --.-K/s   in 0.001s  

 2015-01-16 14:19:16 (1.68 MB/s) - written to stdout [1707/1707]

 OK
 deb http://dl.hhvm.com/ubuntu trusty main
 Get:1 http://dl.hhvm.com trusty InRelease [2,104 B]
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Get:2 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Get:3 http://dl.hhvm.com trusty/main amd64 Packages [1,669 B]
 Hit http://extras.ubuntu.com trusty Release.gpg
 Get:4 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Get:5 http://dl.hhvm.com trusty/main i386 Packages [20 B]
 Hit http://extras.ubuntu.com trusty Release
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Get:6 http://security.ubuntu.com trusty-security/main Sources [63.1 kB]
 Get:7 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Get:8 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Hit http://in.archive.ubuntu.com trusty Release
 Get:9 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB]
 Get:10 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Get:11 http://security.ubuntu.com trusty-security/multiverse Sources [716 B]
 Get:12 http://security.ubuntu.com trusty-security/main amd64 Packages [196 kB]
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://downloads.hipchat.com stable/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Ign http://dl.hhvm.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Get:13 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:14 http://security.ubuntu.com trusty-security/universe amd64 Packages [84.2 kB]
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Get:15 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1,166 B]
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Get:16 http://security.ubuntu.com trusty-security/main i386 Packages [187 kB]
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Get:17 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Get:18 http://security.ubuntu.com trusty-security/universe i386 Packages [84.2 kB]
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Get:19 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1,412 B]
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:20 http://in.archive.ubuntu.com trusty-updates/main Sources [155 kB]
 Get:21 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,061 B]
 Get:22 http://in.archive.ubuntu.com trusty-updates/universe Sources [97.6 kB]
 Get:23 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [3,550 B]
 Get:24 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [398 kB]
 Get:25 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8,875 B]
 Get:26 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [239 kB]
 Get:27 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [9,373 B]
 Get:28 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [390 kB]
 Get:29 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [8,846 B]
 Get:30 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [240 kB]
 Get:31 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [9,567 B]
 Hit http://in.archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/main Sources
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Sources
 Hit http://in.archive.ubuntu.com trusty-backports/universe Sources
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://in.archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 2,347 kB in 42s (55.6 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-41870275104.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libboost-filesystem1.54.0 libboost-program-options1.54.0
  libboost-regex1.54.0 libboost-thread1.54.0 libgflags2 libgoogle-glog0
  libjemalloc1 libmemcached10 libonig2 libtbb2 libunwind8
 The following NEW packages will be installed:
  hhvm libboost-filesystem1.54.0 libboost-program-options1.54.0
  libboost-regex1.54.0 libboost-thread1.54.0 libgflags2 libgoogle-glog0
  libjemalloc1 libmemcached10 libonig2 libtbb2 libunwind8
 0 upgraded, 12 newly installed, 0 to remove and 228 not upgraded.
 Need to get 13.8 MB of archives.
 After this operation, 4,036 kB of additional disk space will be used.
 Get:1 http://dl.hhvm.com/ubuntu/ trusty/main hhvm amd64 3.4.2~trusty [12.9 MB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-filesystem1.54.0 amd64 1.54.0-4ubuntu3.1 [34.2 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-program-options1.54.0 amd64 1.54.0-4ubuntu3.1 [115 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-regex1.54.0 amd64 1.54.0-4ubuntu3.1 [261 kB]
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-thread1.54.0 amd64 1.54.0-4ubuntu3.1 [26.5 kB]
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgflags2 amd64 2.0-1.1ubuntu1 [65.9 kB]
 Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/main libunwind8 amd64 1.1-2.2ubuntu3 [48.3 kB]
 Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgoogle-glog0 amd64 0.3.3-1 [61.3 kB]
 Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/main libmemcached10 amd64 1.0.8-1ubuntu2 [83.4 kB]
 Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjemalloc1 amd64 3.5.1-2 [76.8 kB]
 Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libonig2 amd64 5.9.1-1ubuntu1 [89.1 kB]
 Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libtbb2 amd64 4.2~20130725-1.1ubuntu1 [94.7 kB]
 Fetched 13.8 MB in 4min 15s (54.2 kB/s)
 Selecting previously unselected package libboost-filesystem1.54.0:amd64.
 (Reading database ... 180191 files and directories currently installed.)
 Preparing to unpack .../libboost-filesystem1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
 Unpacking libboost-filesystem1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Selecting previously unselected package libboost-program-options1.54.0:amd64.
 Preparing to unpack .../libboost-program-options1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
 Unpacking libboost-program-options1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Selecting previously unselected package libboost-regex1.54.0:amd64.
 Preparing to unpack .../libboost-regex1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
 Unpacking libboost-regex1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Selecting previously unselected package libboost-thread1.54.0:amd64.
 Preparing to unpack .../libboost-thread1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
 Unpacking libboost-thread1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Selecting previously unselected package libgflags2.
 Preparing to unpack .../libgflags2_2.0-1.1ubuntu1_amd64.deb ...
 Unpacking libgflags2 (2.0-1.1ubuntu1) ...
 Selecting previously unselected package libunwind8.
 Preparing to unpack .../libunwind8_1.1-2.2ubuntu3_amd64.deb ...
 Unpacking libunwind8 (1.1-2.2ubuntu3) ...
 Selecting previously unselected package libgoogle-glog0.
 Preparing to unpack .../libgoogle-glog0_0.3.3-1_amd64.deb ...
 Unpacking libgoogle-glog0 (0.3.3-1) ...
 Selecting previously unselected package libmemcached10:amd64.
 Preparing to unpack .../libmemcached10_1.0.8-1ubuntu2_amd64.deb ...
 Unpacking libmemcached10:amd64 (1.0.8-1ubuntu2) ...
 Selecting previously unselected package libjemalloc1.
 Preparing to unpack .../libjemalloc1_3.5.1-2_amd64.deb ...
 Unpacking libjemalloc1 (3.5.1-2) ...
 Selecting previously unselected package libonig2.
 Preparing to unpack .../libonig2_5.9.1-1ubuntu1_amd64.deb ...
 Unpacking libonig2 (5.9.1-1ubuntu1) ...
 Selecting previously unselected package libtbb2.
 Preparing to unpack .../libtbb2_4.2~20130725-1.1ubuntu1_amd64.deb ...
 Unpacking libtbb2 (4.2~20130725-1.1ubuntu1) ...
 Selecting previously unselected package hhvm.
 Preparing to unpack .../hhvm_3.4.2~trusty_amd64.deb ...
 Unpacking hhvm (3.4.2~trusty) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up libboost-filesystem1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Setting up libboost-program-options1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Setting up libboost-regex1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Setting up libboost-thread1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
 Setting up libgflags2 (2.0-1.1ubuntu1) ...
 Setting up libunwind8 (1.1-2.2ubuntu3) ...
 Setting up libgoogle-glog0 (0.3.3-1) ...
 Setting up libmemcached10:amd64 (1.0.8-1ubuntu2) ...
 Setting up libjemalloc1 (3.5.1-2) ...
 Setting up libonig2 (5.9.1-1ubuntu1) ...
 Setting up libtbb2 (4.2~20130725-1.1ubuntu1) ...
 Setting up hhvm (3.4.2~trusty) ...
 ********************************************************************
 * HHVM is installed.
 * 
 * Running PHP web scripts with HHVM is done by having your webserver talk to HHVM
 * over FastCGI. Install nginx or Apache, and then:
 * $ sudo /usr/share/hhvm/install_fastcgi.sh
 * $ sudo /etc/init.d/hhvm restart
 * (if using nginx)  $ sudo /etc/init.d/nginx restart
 * (if using apache) $ sudo /etc/init.d/apache restart
 * 
 * Detailed FastCGI directions are online at:
 * https://github.com/facebook/hhvm/wiki/FastCGI
 * 
 * If you're using HHVM to run web scripts, you probably want it to start at boot:
 * $ sudo update-rc.d hhvm defaults
 * 
 * Running command-line scripts with HHVM requires no special setup:
 * $ hhvm whatever.php
 * 
 * You can use HHVM for /usr/bin/php even if you have php-cli installed:
 * $ sudo /usr/bin/update-alternatives --install /usr/bin/php php /usr/bin/hhvm 60
 ********************************************************************
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package hhvm from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 HHVM: Success
 ------------------------------
 Installer Finished
 ******************************


国連のインストール
--------------------

国連は hhvm をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure HHVM uninstall


上記のコマンドのスクリーン ショットは以下します。



.. code-block:: bash


 kevell@corp:/# ptconfigure hhvm uninstall
 Uninstall HHVM? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! HHVM !        *
 *******************************
 [Pharaoh Logging] Removing Package hhvm
 update-alternatives: warning: alternative /usr/bin/hhvm (part of link group php) doesn't exist; removing from list of alternatives
 update-alternatives: warning: forcing reinstallation of alternative /usr/bin/php5 because link group php is broken
 update-alternatives: warning: not replacing /usr/bin/php with a link
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  libboost-context1.54.0 libboost-filesystem1.54.0
  libboost-program-options1.54.0 libboost-regex1.54.0 libboost-thread1.54.0
  libc-client2007e libgflags2 libgoogle-glog0 libjemalloc1 libonig2 libtbb2
  libunwind8 mlock
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  hhvm
 0 upgraded, 0 newly installed, 1 to remove and 13 not upgraded.
 After this operation, 0 B of additional disk space will be used.
 (Reading database ... 401748 files and directories currently installed.)
 Removing hhvm (3.6.1~trusty) ...
 ********************************************************************
 * HHVM is being removed. You can remove it from your webserver with:
 * 
 * $ sudo /usr/share/hhvm/uninstall_fastcgi.sh
 * $ sudo /etc/init.d/nginx restart
 * $ sudo /etc/init.d/apache restart
 ********************************************************************
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ...
 [Pharaoh Logging] Removed Package hhvm from the Packager Apt
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Uninstaller:
 ------------------------------
 HHVM: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* パラメーターにおいてヘルプおよびインストール ＆ アンインストール操作されている大文字小文字を区別しながらも有利です
  他の人をに比べてください。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* HHVM は web サーバーのスループットにつながるライブの型情報を使用してより効率的なネイティブ コードを生成する能力を持っていて、
  低待機時間です。
