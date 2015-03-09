=======
SVN
=======

あらすじ
------------

このモジュールは、Ubuntu で SVN の最新バージョンをインストールするユーザーを支援します。Apache Subversion (頻繁に短縮された SVN、コマンド svn の名の後) は、Apache ライセンスの下でフリー ソフトウェアとして配布ソフトウェア バージョンとリビジョン コントロール システムです。[1] 開発者はソース コード、web ページ、およびドキュメントなどのファイルの現在と過去のバージョンを維持するために Subversion を使用します。その目標は、広く使われている並行版システム (CVS) に大抵互換性がある後継者であります。このモジュールは、インストール、アンインストール、ubuntu で subversion を確実にどのように役立つかを見てみましょう。

ヘルプ コマンド
---------------------

Help コマンドと同様、目的に関するユーザー ガイドとして SVN で含まれているオプションについて。それは SVN の代替パラメーターが一覧表示されます。インストールするための構文についても説明します、アンインストール、SVN を確保します。SVN モジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash
	
		ptconfigure svn help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、SVN の下で help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure svn help
 ******************************


  This command allows you to install the latest available SVN in the Ubuntu
  repositories.

  SVN, svn

        - install
        Installs the latest available (In your package manager) version of SVN
        example: ptconfigure svn install

        - ensure
        Ensures SVN is installed
        example: ptconfigure svn ensure

        - uninstall
        Installs the latest version of SVN
        example: ptconfigure svn uninstall

 ------------------------------
 End Help
 ******************************



インストール
---------------

SVN の ubuntu をインストールするために使用するコマンドを次に示します。


.. code-block:: bash
		
		ptconfigure svn install


上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +---------------------+--------------------------------------+------------+-----------------------------------------------------+
 | パラメーター        | 代替パラメーター                     | オプション | コメント                                            |
 +=====================+======================================+============+=====================================================+
 |Install SVN? (Y/N)   | 代わりにSVNの、我々はまた、svn       | Y(Yes)     | ユーザーは、Yと入力することができ、                 |
 |                     | を使用することができます             |            | インストールプロセスを続行したい場合                |
 +---------------------+--------------------------------------+------------+-----------------------------------------------------+
 |Install SVN? (Y/N)   | 代わりにSVNの、我々はまた、svn       | N(No)      | ユーザーは、Nと入力することができ、                 |
 |                     | を使用することができます             |            | インストールプロセスを終了したい場合は|             |
 +---------------------+--------------------------------------+------------+-----------------------------------------------------+


インストール プロセスを続行すると、インストールの実行中に、次のプロセスが発生します。

* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 読み取り状態情報。
* インストールされた余分なパッケージを一覧表示します。
* インストールされている新しいパッケージを一覧表示します。
* アップグレード ファイルの数、新しくインストールされた、削除された、ないアップグレード。
* 最後に、SVN のインストールを完了を取得します。次のスクリーン ショットは、ubuntu での SVN のインストールのプロセスについて示しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure svn install
 Install SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libserf-1-1 libsvn1
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  libserf-1-1 libsvn1 subversion
 0 upgraded, 3 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,240 kB of archives.
 After this operation, 4,701 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libserf-1-1 amd64 1.3.3-1ubuntu0.1 [42.2 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libsvn1 amd64 1.8.8-1ubuntu3.1 [917 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main subversion amd64 1.8.8-1ubuntu3.1 [280 kB]
 Fetched 1,240 kB in 43s (28.3 kB/s)
 Selecting previously unselected package libserf-1-1:amd64.
 (Reading database ... 211229 files and directories currently installed.)
 Preparing to unpack .../libserf-1-1_1.3.3-1ubuntu0.1_amd64.deb ...
 Unpacking libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Selecting previously unselected package libsvn1:amd64.
 Preparing to unpack .../libsvn1_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Selecting previously unselected package subversion.
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Setting up libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************


国連のインストール
-----------------------

国連、SVN、ubuntu をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure svn uninstall


上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。



.. cssclass:: table-bordered

 +----------------------+------------------------------------+------------+--------------------------------------------------------------+
 | パラメーター         | 代替パラメーター                   | オプション | コメント                                                     |
 +======================+====================================+============+==============================================================+
 |Uninstall SVN? (Y/N)  | 代わりにSVNの、我々はまた、svn     | Y(Yes)     | ユーザーの願いはアンインストールプロセスを続行する場合、     |
 |                      | を使用することができます           |            | それらはYと入力をすることができます                          |
 +----------------------+------------------------------------+------------+--------------------------------------------------------------+
 |Uninstall SVN? (Y/N)  | 代わりにSVNの、我々はまた、svn     | N(No)      | ユーザーの願いはアンインストールプロセスを終了するには場合、 |
 |                      | を使用することができます           |            | それらはNとして入力をすることができます|                     |
 +----------------------+------------------------------------+------------+--------------------------------------------------------------+


国連のインストール プロセスを続行すると、国連のインストールの実行中に、次のプロセスが発生します。

* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 読み取り状態情報。
* 自動的にインストールされているパッケージを一覧表示します。
* 削除されるパッケージを一覧表示します。
* アップグレード ファイルの数、新しくインストールされた、削除された、ないアップグレード。

最後に、SVN の国連のインストールを完了を取得します。次のスクリーン ショットは、国連の ubuntu での SVN のインストールのプロセスについて示しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure svn uninstall
 Uninstall SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 [Pharaoh Logging] Removing Package subversion
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  libserf-1-1 libsvn1
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  subversion
 0 upgraded, 0 newly installed, 1 to remove and 8 not upgraded.
 After this operation, 1,425 kB disk space will be freed.
 (Reading database ... 211322 files and directories currently installed.)
 Removing subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package subversion from the Packager Apt
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

確保するため
-----------------

SVN を確保するために使用するコマンドを次に示します。

.. code-block:: bash

		ptconfigure svn ensure

確認プロセスは、次の関数を実行します。

* それは、モジュールがインストールされているかどうか、およびバージョンを確認していないかどうかを確認します。
* モジュールがすでにインストールされている場合は、既に存在していたように報告されます。
* モジュールがない場合、ユーザーのマシンで利用できる、インストールを続行します。

次のスクリーン ショットを確認するプロセスを示しています。



.. code-block:: bash

 kevell@corp:/# ptconfigure svn ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: svn: not found
 [Pharaoh Logging] Module SVN reports itself as Not Installed 
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  subversion
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 0 B/280 kB of archives.
 After this operation, 1,425 kB of additional disk space will be used.
 Selecting previously unselected package subversion.
 (Reading database ... 211282 files and directories currently installed.)
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


利点
-----------

* ヘルプとインストールでは、宣言で使用されるパラメーター、アンインストール中の利点を追加する必要がある大文字と小文字が区別されません確認します
  他の人をに比べてください。
* ユーザーは、インストールを実行する前に空室状況について確認できます。
* それは、パッケージを上書きしません、それゆえそれはより少なく時間のかかる。
 

