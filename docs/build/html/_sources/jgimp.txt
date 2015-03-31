=======
GIMP
=======

概要
-----------

このモジュールは、ユーザーが一般的なイメージエディタですGIMPをインストールすることができます。

GIMPは、GNU画像処理プログラムの頭字語）は、画像レタッチや編集、自由形式の描画、サイズ変更、トリミング、フォトモンタージュ、異なる画像フォーマット間の変換、および、より特殊なタスクに使用されます。

GIMPは自由に誰にも（とによって）分配され、誰もがその内容とそのソースコードを見ることができ、問題を機能を追加したり、修正することができます。それはLGPLv3のとGPLv3の+ライセンスの下でリリースされています。 GIMPは2大学生の学校のプロジェクトとして1995年に始まった。今GIMPは、GNU / LinuxのすべてのディストリビューションおよびMicrosoft WindowsとMac OS Xの最近のバージョンで利用可能な本格的なアプリケーションです

私たちは、このモジュールは、今後のトピックからGIMPをインストールして容易に方法を見てみましょう。

helpコマンド
-------------------

helpコマンドは、このモジュールの目的に関するユーザーを表す簡潔なユーザーマニュアル、そのリストアウトのapt-getを通じてGIMPをインストールするための構文と一緒に、宣言で使用することができ、その代わりのパラメータである。このモジュールの下にヘルプオプションを使用するための構文を以下に示します、

.. code-block:: bash

	ptconfigure GIMP help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、GIMPの下に、helpコマンドについてあなたを視覚化。

.. code-block::  bash

 kevell@corp:/# ptconfigure GIMP help 
 ******************************** 

  This command allows you to install GIMP, the popular Image Editor 
  GIMP, gimp 

        - install 
        Installs GIMP through apt-get 
        example: ptconfigure gimp install 

 ------------------------------ 
 End Help 
 ****************************** 


インストール
------------------

このモジュールを使用してapt-getを通ってGIMPをインストールするために使用されるコマンドは、単に以下のコマンドを使用して簡単です、

.. code-block:: bash

	ptconfigure GIMP install

テーブルから描かれているように上記のコマンドを入力した後、以下のステップが実行される、

.. cssclass:: table-bordered

 +--------------------------+-------------------+------------+--------------------------------------------------------------------------+
 | パラメーター             | 代替パラメータ    | オプション | コメント                                                                 |
 +==========================+===================+============+==========================================================================+
 |GIMP Install? (Y/N)       | GIMP, gimp        | Y(Yes)     | ユーザーがインストールを続行したい場合は、Yと入力することができます      |
 +--------------------------+-------------------+------------+--------------------------------------------------------------------------+
 |GIMP Install? (Y/N)       | GIMP, gimp        | N(No)      | ユーザーがインストールを終了したい場合は、Nとして入力することができます| |  
 +--------------------------+-------------------+------------+--------------------------------------------------------------------------+
 

以下のスクリーンショットは、インストールのプロセスについて視覚的に示している。


.. code-block:: bash

 kevell@corp:/# ptconfigure gimp install 
 Install GIMP? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *          ! GIMP !        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-67656420389.sh 
 chmod 755 /tmp/ptconfigure-temp-script-67656420389.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-67656420389.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-67656420389.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following package was automatically installed and is no longer required: 
  libjemalloc1 
 Use 'apt-get autoremove' to remove it. 
 The following extra packages will be installed: 
  gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 libccolamd2.8.0 
  libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 libilmbase6 
  libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 libumfpack5.6.2 
  libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 Suggested packages: 
  gimp-help-en gimp-help gimp-data-extras 
 The following NEW packages will be installed: 
  gimp gimp-data libamd2.3.1 libbabl-0.1-0 libblas3 libcamd2.3.1 
  libccolamd2.8.0 libcholmod2.1.2 libgegl-0.2-0 libgfortran3 libgimp2.0 
  libilmbase6 libjavascriptcoregtk-1.0-0 liblapack3 libmng2 libopenexr6 
  libumfpack5.6.2 libwebkitgtk-1.0-0 libwebkitgtk-1.0-common 
 0 upgraded, 19 newly installed, 0 to remove and 6 not upgraded. 
 Need to get 14.2 MB/19.7 MB of archives. 
 After this operation, 87.2 MB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty-proposed/main libwebkitgtk-1.0-0 amd64 2.4.8-1ubuntu1/ubuntu14.04.1 [7,224 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main libgimp2.0 amd64 2.8.10-0ubuntu1 [484 kB] 
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main gimp-data all 2.8.10-0ubuntu1 [3,068 kB] 
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main gimp amd64 2.8.10-0ubuntu1 [3,411 kB] 
 Fetched 9,355 kB in 18min 31s (8,412 B/s) 
 Selecting previously unselected package libamd2.3.1:amd64. 
 (Reading database ... 381874 files and directories currently installed.) 
 Preparing to unpack .../libamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libbabl-0.1-0:amd64. 
 Preparing to unpack .../libbabl-0.1-0_0.1.10-1ubuntu2_amd64.deb ... 
 Unpacking libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Selecting previously unselected package libcamd2.3.1:amd64. 
 Preparing to unpack .../libcamd2.3.1_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libccolamd2.8.0:amd64. 
 Preparing to unpack .../libccolamd2.8.0_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libblas3. 
 Preparing to unpack .../libblas3_1.2.20110419-7_amd64.deb ... 
 Unpacking libblas3 (1.2.20110419-7) ... 
 Selecting previously unselected package libgfortran3:amd64. 
 Preparing to unpack .../libgfortran3_4.8.2-19ubuntu1_amd64.deb ... 
 Unpacking libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Selecting previously unselected package liblapack3. 
 Preparing to unpack .../liblapack3_3.5.0-2ubuntu1_amd64.deb ... 
 Unpacking liblapack3 (3.5.0-2ubuntu1) ... 
 Selecting previously unselected package libcholmod2.1.2:amd64. 
 Preparing to unpack .../libcholmod2.1.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libilmbase6:amd64. 
 Preparing to unpack .../libilmbase6_1.0.1-6ubuntu1_amd64.deb ... 
 Unpacking libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Selecting previously unselected package libopenexr6:amd64. 
 Preparing to unpack .../libopenexr6_1.6.1-7ubuntu1_amd64.deb ... 
 Unpacking libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Selecting previously unselected package libumfpack5.6.2:amd64. 
 Preparing to unpack .../libumfpack5.6.2_1%3a4.2.1-3ubuntu1_amd64.deb ... 
 Unpacking libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Selecting previously unselected package libgegl-0.2-0:amd64. 
 Preparing to unpack .../libgegl-0.2-0_0.2.0-4ubuntu1_amd64.deb ... 
 Unpacking libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Selecting previously unselected package libjavascriptcoregtk-1.0-0:amd64. 
 Preparing to unpack .../libjavascriptcoregtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libmng2:amd64. 
 Preparing to unpack .../libmng2_2.0.2-0ubuntu3_amd64.deb ... 
 Unpacking libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Selecting previously unselected package libwebkitgtk-1.0-common. 
 Preparing to unpack .../libwebkitgtk-1.0-common_2.4.8-1ubuntu1/ubuntu14.04.1_all.deb ... 
 Unpacking libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libwebkitgtk-1.0-0:amd64. 
 Preparing to unpack .../libwebkitgtk-1.0-0_2.4.8-1ubuntu1/ubuntu14.04.1_amd64.deb ... 
 Unpacking libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Selecting previously unselected package libgimp2.0. 
 Preparing to unpack .../libgimp2.0_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking libgimp2.0 (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp-data. 
 Preparing to unpack .../gimp-data_2.8.10-0ubuntu1_all.deb ... 
 Unpacking gimp-data (2.8.10-0ubuntu1) ... 
 Selecting previously unselected package gimp. 
 Preparing to unpack .../gimp_2.8.10-0ubuntu1_amd64.deb ... 
 Unpacking gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for hicolor-icon-theme (0.13-1) ... 
 Processing triggers for mime-support (3.54ubuntu1.1) ... 
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ... 
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ... 
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ... 
 Rebuilding /usr/share/applications/bamf-2.index... 
 Setting up libamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libbabl-0.1-0:amd64 (0.1.10-1ubuntu2) ... 
 Setting up libcamd2.3.1:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libccolamd2.8.0:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libblas3 (1.2.20110419-7) ... 
 update-alternatives: using /usr/lib/libblas/libblas.so.3 to provide /usr/lib/libblas.so.3 (libblas.so.3) in auto mode 
 Setting up libgfortran3:amd64 (4.8.2-19ubuntu1) ... 
 Setting up liblapack3 (3.5.0-2ubuntu1) ... 
 update-alternatives: using /usr/lib/lapack/liblapack.so.3 to provide /usr/lib/liblapack.so.3 (liblapack.so.3) in auto mode 
 Setting up libcholmod2.1.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libilmbase6:amd64 (1.0.1-6ubuntu1) ... 
 Setting up libopenexr6:amd64 (1.6.1-7ubuntu1) ... 
 Setting up libumfpack5.6.2:amd64 (1:4.2.1-3ubuntu1) ... 
 Setting up libgegl-0.2-0:amd64 (0.2.0-4ubuntu1) ... 
 Setting up libjavascriptcoregtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libmng2:amd64 (2.0.2-0ubuntu3) ... 
 Setting up libwebkitgtk-1.0-common (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libwebkitgtk-1.0-0:amd64 (2.4.8-1ubuntu1/ubuntu14.04.1) ... 
 Setting up libgimp2.0 (2.8.10-0ubuntu1) ... 
 Setting up gimp-data (2.8.10-0ubuntu1) ... 
 Setting up gimp (2.8.10-0ubuntu1) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-67656420389.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 GIMP: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  



メリット
------------

* ヘルプとのaptの他のさまざまな機能を宣言に使用されるパラメータは、大文字と小文字は区別されません。
* これは、裕福な両方セントOSのと同様にUbuntuののようである。


GIMPはまたそうでなければ、時間がかかる、または不可能であることを行うために、より複雑なアルゴリズムを使用する「スマート」なツールを提供しています。これらを含める：

* クローンツール、ブラシを使用してコピーピクセル
* ヒーリングブラシ、エリアからコピーピクセルとトーンと色を補正し

クローンツールのように動作しますが、距離の変化を補正する*パースペクティブクローンツール、

* ぼかしツールをシャープは、ぼかしやブラシを使ってシャープ
* ダッジと火傷ツール（火傷）対象画素が（ドッジ）明るくしたり、暗くしたりしたブラシです


GIMP変換ツールが含まれます：

* 揃え
* 移動
* トリミング
* 回転させて
* スケール
* せん断
* の視点
* フリップ
