============
OpenOffice
============

概要
------------

このモジュールは、OpenOfficeの.Openオフィス、オフィス関連のソフトウェアの最初のオープンスイートですインストールするには、ファシリテーターとして機能します。私たちは今後のトピックで開いたオフィスを設置するの使用状況や方法論を見てみましょう。

helpコマンド
----------------------

helpコマンドは、とだけでなく、オープンオフィスモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それは、オープンオフィスモジュールの別のパラメータを示しています。また、オープンオフィスモジュールをインストールするための構文について説明します。オープンオフィスモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash 

	ptconfigure OpenOffice help 

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、オープンオフィスの下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash 

 kevell@corp:/# ptconfigure openoffice help
 ******************************


  This command allows you to install and uninstall OpenOffice.

  Openoffice, openoffice

        - install
        Installs OpenOffice.
        example: ptconfigure openoffice install
	
	- uninstall
        Uninstalls OpenOffice.
        example: ptconfigure openoffice uninstall

 ------------------------------
 End Help
 ******************************


インストール
--------------

ユーザーはマシンにオープンオフィスをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash 
 
	ptconfigure openoffice install 

表形式で示すように、上記のコマンドを入力した後、次の処理が発生します。

.. cssclass:: table-bordered 


 +-----------------------------+------------------------------+--------------+----------------------------------------------------+
 | パラメーター                | 代替パラメータ               | オプション   | コメント                                           |
 +=============================+==============================+==============+====================================================+
 |Install Open Office? (Y/N)   | openoffice, OpenOffice,      | Y(Yes)       | ユーザーは、Yと入力することができ、                |
 |                             | Openoffice                   |              | インストールプロセスを続行したい場合               |
 +-----------------------------+------------------------------+--------------+----------------------------------------------------+
 |Install Open Office? (Y/N)   | openoffice, OpenOffice,      | N(No)        | ユーザーは、Nと入力することができ、                |
 |                             | Openoffice                   |              | インストールプロセスを終了したい場合は|            |
 +-----------------------------+------------------------------+--------------+----------------------------------------------------+


ユーザーがインストールの処理中に、インストールを進行する場合は、次のリストで説明します。

* パッケージ一覧を読み込みます。
* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リストアウト自動的にインストールされたパッケージ。
* リストアウトインストールしている余分なパッケージ。
* リストのアウトを示唆したパッケージ。
* リストアウトインストールする新しいパッケージ。
* 、新しくインストールされ、アップグレードされた削除され、アップグレードされていないファイルの数に関する詳細。



最後に、インストールのプロセスが完了して取得します。次のスクリーンショットは、視覚的にインストールすると、彼は事務所を開いてアンインストールするプロセスを表す。

.. code-block:: bash 


 kevell@corp:/# ptconfigure openoffice install

 Install OpenOffice? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          OpenOffice !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-47988758288.sh
 chmod 755 /tmp/ptconfigure-temp-script-47988758288.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47988758288.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47988758288.sh
 --2015-04-07 10:55:59--  http://sourceforge.net/projects/openofficeorg.mirror/files/4.1.1/binaries/en-US/  
 Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gz
 Resolving sourceforge.net (sourceforge.net)... 216.34.181.60
 Connecting to sourceforge.net (sourceforge.net)|216.34.181.60|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://sourceforge.net/projects/openofficeorg.mirror/files/4.1.1/binaries/en-US/Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-  
 US.tar.gz/download [following] 
 --2015-04-07 10:56:00--  http://sourceforge.net/projects/openofficeorg.mirror/files/4.1.1/binaries/en-US/ 
 Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gz/download
 Connecting to sourceforge.net (sourceforge.net)|216.34.181.60|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://downloads.sourceforge.net/project/openofficeorg.mirror/4.1.1/binaries/en-US/Apache_OpenOffice_4.1.1_Linux_x86_install-
 deb_en- US.tar.gz?r=&ts=1428384361&use_mirror=softlayer-sng [following]
 --2015-04-07 10:56:01--  http://downloads.sourceforge.net/project/openofficeorg.mirror/4.1.1/binaries/en-US/ 
 Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gz?r=&ts=1428384361&use_mirror=softlayer-sng
 Resolving downloads.sourceforge.net (downloads.sourceforge.net)... 216.34.181.59
 Connecting to downloads.sourceforge.net (downloads.sourceforge.net)|216.34.181.59|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://softlayer-sng.dl.sourceforge.net/project/openofficeorg.mirror/4.1.1/binaries/en-US/
 Apache_OpenOffice_4.1.1_Linux_x86_install- deb_en-US.tar.gz [following]
 --2015-04-07 10:56:02--  http://softlayer-sng.dl.sourceforge.net/project/openofficeorg.mirror/4.1.1/binaries/en-US/ 
 Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gz
 Resolving softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)... 216.12.198.152
 Connecting to softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)|216.12.198.152|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 152829286 (146M) [application/x-gzip]
 Saving to: â€˜Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gzâ€™

 100%[======================================================================================================>] 15,28,29,286  356KB/s   in 11m  
 2s 
		
 2015-04-07 11:07:04 (226 KB/s) - â€˜Apache_OpenOffice_4.1.1_Linux_x86_install-deb_en-US.tar.gzâ€™ saved [152829286/152829286]

 gtk-update-icon-cache: Cache file created successfully.
 gtk-update-icon-cache: Cache file created successfully.
 gtk-update-icon-cache: Cache file created successfully.
 gtk-update-icon-cache: Cache file created successfully.
 en-US/
 en-US/DEBS/
 en-US/DEBS/openoffice-ooofonts_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-calc_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-writer_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-draw_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-javafilter_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core07_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-impress_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-impress_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core04_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-impress_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core01_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-graphicfilter_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-math_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-pyuno_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-writer_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-ure_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-res_4.1.1-6_i386.deb
 en-US/DEBS/openoffice_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-images_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-draw_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-base_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-draw_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core06_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-writer_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core02_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-math_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-base_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core05_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-onlineupdate_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-en-us_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-calc_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-xsltfilter_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-math_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-ooolinguistic_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-core03_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-en-us-help_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-gnome-integration_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-calc_4.1.1-6_i386.deb
 en-US/DEBS/desktop-integration/
 en-US/DEBS/desktop-integration/openoffice4.1-debian-menus_4.1.1-9775_all.deb
 en-US/DEBS/openoffice-ogltrans_4.1.1-6_i386.deb
 en-US/DEBS/openoffice-brand-base_4.1.1-6_i386.deb
 en-US/readmes/
 en-US/readmes/README_en-US
 en-US/readmes/README_en-US.html
 en-US/licenses/
 en-US/licenses/LICENSE
 en-US/licenses/NOTICE
 (Reading database ... 415747 files and directories currently installed.)
 Preparing to unpack .../openoffice-base_4.1.1-6_i386.deb ...
 Unpacking openoffice-base (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-base_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-base (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-calc_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-calc (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-draw_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-draw (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-en-us_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-en-us (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-impress_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-impress (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-math_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-math (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-brand-writer_4.1.1-6_i386.deb ...
 Unpacking openoffice-brand-writer (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-calc_4.1.1-6_i386.deb ...
 Unpacking openoffice-calc (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core01_4.1.1-6_i386.deb ...
 Unpacking openoffice-core01 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core02_4.1.1-6_i386.deb ...
 Unpacking openoffice-core02 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core03_4.1.1-6_i386.deb ...
 Unpacking openoffice-core03 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core04_4.1.1-6_i386.deb ...
 Unpacking openoffice-core04 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core05_4.1.1-6_i386.deb ...
 Unpacking openoffice-core05 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core06_4.1.1-6_i386.deb ...
 Unpacking openoffice-core06 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-core07_4.1.1-6_i386.deb ...
 Unpacking openoffice-core07 (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-draw_4.1.1-6_i386.deb ...
 Unpacking openoffice-draw (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-base_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-base (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-calc_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-calc (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-draw_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-draw (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-help_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-help (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-impress_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-impress (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-math_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-math (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-res_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-res (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us-writer_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us-writer (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-en-us_4.1.1-6_i386.deb ...
 Unpacking openoffice-en-us (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-gnome-integration_4.1.1-6_i386.deb ...
 Unpacking openoffice-gnome-integration (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-graphicfilter_4.1.1-6_i386.deb ...
 Unpacking openoffice-graphicfilter (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-images_4.1.1-6_i386.deb ...
 Unpacking openoffice-images (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-impress_4.1.1-6_i386.deb ...
 Unpacking openoffice-impress (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-javafilter_4.1.1-6_i386.deb ...
 Unpacking openoffice-javafilter (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-math_4.1.1-6_i386.deb ...
 Unpacking openoffice-math (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-ogltrans_4.1.1-6_i386.deb ...
 Unpacking openoffice-ogltrans (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-onlineupdate_4.1.1-6_i386.deb ...
 Unpacking openoffice-onlineupdate (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-ooofonts_4.1.1-6_i386.deb ...
 Unpacking openoffice-ooofonts (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-ooolinguistic_4.1.1-6_i386.deb ...
 Unpacking openoffice-ooolinguistic (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-pyuno_4.1.1-6_i386.deb ...
 Unpacking openoffice-pyuno (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-ure_4.1.1-6_i386.deb ...
 Unpacking openoffice-ure (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-writer_4.1.1-6_i386.deb ...
 Unpacking openoffice-writer (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice-xsltfilter_4.1.1-6_i386.deb ...
 Unpacking openoffice-xsltfilter (4.1.1-6) over (4.1.1-6) ...
 Preparing to unpack .../openoffice_4.1.1-6_i386.deb ...
 Unpacking openoffice (4.1.1-6) over (4.1.1-6) ...
 Setting up openoffice-ure (4.1.1-6) ...
 Setting up openoffice-core01 (4.1.1-6) ...
 Setting up openoffice-core02 (4.1.1-6) ...
 Setting up openoffice-core03 (4.1.1-6) ...
 Setting up openoffice-core04 (4.1.1-6) ...
 Setting up openoffice-core05 (4.1.1-6) ...
 Setting up openoffice-core06 (4.1.1-6) ...
 Setting up openoffice-core07 (4.1.1-6) ...
 Setting up openoffice-draw (4.1.1-6) ...
 Setting up openoffice-en-us (4.1.1-6) ...
 Setting up openoffice-gnome-integration (4.1.1-6) ...
 Setting up openoffice-graphicfilter (4.1.1-6) ...
 Setting up openoffice-images (4.1.1-6) ...
 Setting up openoffice-impress (4.1.1-6) ...
 Setting up openoffice-javafilter (4.1.1-6) ...
 Setting up openoffice-math (4.1.1-6) ...
 Setting up openoffice-ogltrans (4.1.1-6) ...
 Setting up openoffice-onlineupdate (4.1.1-6) ...
 Setting up openoffice-ooofonts (4.1.1-6) ...
 Setting up openoffice-ooolinguistic (4.1.1-6) ...
 Setting up openoffice-pyuno (4.1.1-6) ...
 Setting up openoffice-writer (4.1.1-6) ...
 Setting up openoffice-xsltfilter (4.1.1-6) ...
 Setting up openoffice (4.1.1-6) ...
 Setting up openoffice-base (4.1.1-6) ...
 Setting up openoffice-brand-base (4.1.1-6) ...
 Setting up openoffice-brand-draw (4.1.1-6) ...
 Setting up openoffice-brand-impress (4.1.1-6) ...
 Setting up openoffice-brand-math (4.1.1-6) ...
 Setting up openoffice-brand-writer (4.1.1-6) ...
 Setting up openoffice-calc (4.1.1-6) ...
 Setting up openoffice-en-us-base (4.1.1-6) ...
 Setting up openoffice-en-us-calc (4.1.1-6) ...
 Setting up openoffice-en-us-draw (4.1.1-6) ...
 Setting up openoffice-en-us-help (4.1.1-6) ...
 Setting up openoffice-en-us-impress (4.1.1-6) ...
 Setting up openoffice-en-us-math (4.1.1-6) ...
 Setting up openoffice-en-us-res (4.1.1-6) ...
 Setting up openoffice-en-us-writer (4.1.1-6) ...
 Setting up openoffice-brand-calc (4.1.1-6) ...
 Setting up openoffice-brand-en-us (4.1.1-6) ...
 (Reading database ... 415747 files and directories currently installed.)
 Preparing to unpack .../openoffice4.1-debian-menus_4.1.1-9775_all.deb ...
 Unpacking openoffice-debian-menus (4.1.1-9775) over (4.1.1-9775) ...
 /usr/bin/gtk-update-icon-cache
 /usr/bin/gtk-update-icon-cache
 Setting up openoffice-debian-menus (4.1.1-9775) ...
 /usr/bin/gtk-update-icon-cache
 /usr/bin/gtk-update-icon-cache
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for gnome-icon-theme (3.10.0-0ubuntu2) ...
 Temp File /tmp/ptconfigure-temp-script-47988758288.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 OpenOffice: Success
 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure openoffice uninstall

 Uninstall OpenOffice? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          OpenOffice !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-27028685322.sh
 chmod 755 /tmp/ptconfigure-temp-script-27028685322.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-27028685322.sh Permissions
 Executing /tmp/ptconfigure-temp-script-27028685322.sh
 gtk-update-icon-cache: Cache file created successfully.
 gtk-update-icon-cache: Cache file created successfully.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'openoffice.org-thesaurus-it' is not installed, so not removed
 Package 'openoffice.org-hunspell' is not installed, so not removed
 Package 'openoffice.org-core' is not installed, so not removed
 Package 'openoffice.org-spellcheck-en-us' is not installed, so not removed
 Package 'openoffice.org-dev-doc' is not installed, so not removed
 Package 'openoffice.org-bundled' is not installed, so not removed
 Package 'openoffice.org3' is not installed, so not removed
 Package 'openoffice.org3-dict-es' is not installed, so not removed
 Package 'openoffice.org3-dict-en' is not installed, so not removed
 Package 'openoffice.org3-dict-fr' is not installed, so not removed
 Package 'openoffice.org3-writer' is not installed, so not removed
 Package 'openofficeorg-desktop-integration' is not installed, so not removed
 Package 'openoffice.org-debian-menus' is not installed, so not removed
 Package 'openoffice.org3-en-us' is not installed, so not removed
 Package 'openoffice.org3-impress' is not installed, so not removed
 Package 'openoffice.org3-draw' is not installed, so not removed
 Package 'openoffice.org3-calc' is not installed, so not removed
 Package 'openoffice.org-ure' is not installed, so not removed
 Package 'openoffice.org3-math' is not installed, so not removed
 Package 'openoffice.org3-base' is not installed, so not removed
 Package 'openoffice.org' is not installed, so not removed
 Package 'openoffice.org-base' is not installed, so not removed
 Package 'openoffice.org-calc' is not installed, so not removed
 Package 'openoffice.org-common' is not installed, so not removed
 Package 'openoffice.org-draw' is not installed, so not removed
 Package 'openoffice.org-emailmerge' is not installed, so not removed
 Package 'openoffice.org-filter-binfilter' is not installed, so not removed
 Package 'openoffice.org-gnome' is not installed, so not removed
 Package 'openoffice.org-gtk' is not installed, so not removed
 Package 'openoffice.org-help-ca' is not installed, so not removed
 Package 'openoffice.org-help-cs' is not installed, so not removed
 Package 'openoffice.org-help-da' is not installed, so not removed
 Package 'openoffice.org-help-de' is not installed, so not removed
 Package 'openoffice.org-help-dz' is not installed, so not removed
 Package 'openoffice.org-help-el' is not installed, so not removed
 Package 'openoffice.org-help-en-gb' is not installed, so not removed
 Package 'openoffice.org-help-en-us' is not installed, so not removed
 Package 'openoffice.org-help-es' is not installed, so not removed
 Package 'openoffice.org-help-et' is not installed, so not removed
 Package 'openoffice.org-help-eu' is not installed, so not removed
 Package 'openoffice.org-help-fi' is not installed, so not removed
 Package 'openoffice.org-help-fr' is not installed, so not removed
 Package 'openoffice.org-help-gl' is not installed, so not removed
 Package 'openoffice.org-help-hi-in' is not installed, so not removed
 Package 'openoffice.org-help-hu' is not installed, so not removed
 Package 'openoffice.org-help-it' is not installed, so not removed
 Package 'openoffice.org-help-ja' is not installed, so not removed
 Package 'openoffice.org-help-km' is not installed, so not removed
 Package 'openoffice.org-help-ko' is not installed, so not removed
 Package 'openoffice.org-help-nl' is not installed, so not removed
 Package 'openoffice.org-help-om' is not installed, so not removed
 Package 'openoffice.org-help-pl' is not installed, so not removed
 Package 'openoffice.org-help-pt' is not installed, so not removed
 Package 'openoffice.org-help-pt-br' is not installed, so not removed
 Package 'openoffice.org-help-ru' is not installed, so not removed
 Package 'openoffice.org-help-sl' is not installed, so not removed
 Package 'openoffice.org-help-sv' is not installed, so not removed
 Package 'openoffice.org-help-zh-cn' is not installed, so not removed
 Package 'openoffice.org-help-zh-tw' is not installed, so not removed
 Package 'openoffice.org-hyphenation-af' is not installed, so not removed
 Package 'openoffice.org-hyphenation-ca' is not installed, so not removed
 Package 'openoffice.org-hyphenation-de' is not installed, so not removed
 Package 'openoffice.org-hyphenation-en-us' is not installed, so not removed
 Package 'openoffice.org-hyphenation-fr' is not installed, so not removed
 Package 'openoffice.org-hyphenation-hr' is not installed, so not removed
 Package 'openoffice.org-hyphenation-hu' is not installed, so not removed
 Package 'openoffice.org-hyphenation-it' is not installed, so not removed
 Package 'openoffice.org-hyphenation-ro' is not installed, so not removed
 Package 'openoffice.org-hyphenation-sh' is not installed, so not removed
 Package 'openoffice.org-hyphenation-sl' is not installed, so not removed
 Package 'openoffice.org-hyphenation-sr' is not installed, so not removed
 Package 'openoffice.org-hyphenation-zu' is not installed, so not removed
 Package 'openoffice.org-impress' is not installed, so not removed
 Package 'openoffice.org-java-common' is not installed, so not removed
 Package 'openoffice.org-kde' is not installed, so not removed
 Package 'openoffice.org-l10n-af' is not installed, so not removed
 Package 'openoffice.org-l10n-ar' is not installed, so not removed
 Package 'openoffice.org-l10n-as' is not installed, so not removed
 Package 'openoffice.org-l10n-ast' is not installed, so not removed
 Package 'openoffice.org-l10n-be-by' is not installed, so not removed
 Package 'openoffice.org-l10n-bg' is not installed, so not removed
 Package 'openoffice.org-l10n-bn' is not installed, so not removed
 Package 'openoffice.org-l10n-br' is not installed, so not removed
 Package 'openoffice.org-l10n-bs' is not installed, so not removed
 Package 'openoffice.org-l10n-ca' is not installed, so not removed
 Package 'openoffice.org-l10n-cs' is not installed, so not removed
 Package 'openoffice.org-l10n-cy' is not installed, so not removed
 Package 'openoffice.org-l10n-da' is not installed, so not removed
 Package 'openoffice.org-l10n-de' is not installed, so not removed
 Package 'openoffice.org-l10n-dz' is not installed, so not removed
 Package 'openoffice.org-l10n-el' is not installed, so not removed
 Package 'openoffice.org-l10n-en-gb' is not installed, so not removed
 Package 'openoffice.org-l10n-en-za' is not installed, so not removed
 Package 'openoffice.org-l10n-eo' is not installed, so not removed
 Package 'openoffice.org-l10n-es' is not installed, so not removed
 Package 'openoffice.org-l10n-et' is not installed, so not removed
 Package 'openoffice.org-l10n-eu' is not installed, so not removed
 Package 'openoffice.org-l10n-fa' is not installed, so not removed
 Package 'openoffice.org-l10n-fi' is not installed, so not removed
 Package 'openoffice.org-l10n-fr' is not installed, so not removed
 Package 'openoffice.org-l10n-ga' is not installed, so not removed
 Package 'openoffice.org-l10n-gl' is not installed, so not removed
 Package 'openoffice.org-l10n-gu' is not installed, so not removed
 Package 'openoffice.org-l10n-he' is not installed, so not removed
 Package 'openoffice.org-l10n-hi-in' is not installed, so not removed
 Package 'openoffice.org-l10n-hr' is not installed, so not removed
 Package 'openoffice.org-l10n-hu' is not installed, so not removed
 Package 'openoffice.org-l10n-id' is not installed, so not removed
 Package 'openoffice.org-l10n-in' is not installed, so not removed
 Package 'openoffice.org-l10n-it' is not installed, so not removed
 Package 'openoffice.org-l10n-ja' is not installed, so not removed
 Package 'openoffice.org-l10n-ka' is not installed, so not removed
 Package 'openoffice.org-l10n-km' is not installed, so not removed
 Package 'openoffice.org-l10n-ko' is not installed, so not removed
 Package 'openoffice.org-l10n-ku' is not installed, so not removed
 Package 'openoffice.org-l10n-lt' is not installed, so not removed
 Package 'openoffice.org-l10n-lv' is not installed, so not removed
 Package 'openoffice.org-l10n-mk' is not installed, so not removed
 Package 'openoffice.org-l10n-ml' is not installed, so not removed
 Package 'openoffice.org-l10n-mn' is not installed, so not removed
 Package 'openoffice.org-l10n-mr' is not installed, so not removed
 Package 'openoffice.org-l10n-nb' is not installed, so not removed
 Package 'openoffice.org-l10n-ne' is not installed, so not removed
 Package 'openoffice.org-l10n-nl' is not installed, so not removed
 Package 'openoffice.org-l10n-nn' is not installed, so not removed
 Package 'openoffice.org-l10n-nr' is not installed, so not removed
 Package 'openoffice.org-l10n-ns' is not installed, so not removed
 Package 'openoffice.org-l10n-oc' is not installed, so not removed
 Package 'openoffice.org-l10n-om' is not installed, so not removed
 Package 'openoffice.org-l10n-or' is not installed, so not removed
 Package 'openoffice.org-l10n-pa-in' is not installed, so not removed
 Package 'openoffice.org-l10n-pl' is not installed, so not removed
 Package 'openoffice.org-l10n-pt' is not installed, so not removed
 Package 'openoffice.org-l10n-pt-br' is not installed, so not removed
 Package 'openoffice.org-l10n-ro' is not installed, so not removed
 Package 'openoffice.org-l10n-ru' is not installed, so not removed
 Package 'openoffice.org-l10n-rw' is not installed, so not removed
 Package 'openoffice.org-l10n-si' is not installed, so not removed
 Package 'openoffice.org-l10n-sk' is not installed, so not removed
 Package 'openoffice.org-l10n-sl' is not installed, so not removed
 Package 'openoffice.org-l10n-sr' is not installed, so not removed
 Package 'openoffice.org-l10n-ss' is not installed, so not removed
 Package 'openoffice.org-l10n-st' is not installed, so not removed
 Package 'openoffice.org-l10n-sv' is not installed, so not removed
 Package 'openoffice.org-l10n-ta' is not installed, so not removed
 Package 'openoffice.org-l10n-te' is not installed, so not removed
 Package 'openoffice.org-l10n-tg' is not installed, so not removed
 Package 'openoffice.org-l10n-th' is not installed, so not removed
 Package 'openoffice.org-l10n-tn' is not installed, so not removed
 Package 'openoffice.org-l10n-tr' is not installed, so not removed
 Package 'openoffice.org-l10n-ts' is not installed, so not removed
 Package 'openoffice.org-l10n-ug' is not installed, so not removed
 Package 'openoffice.org-l10n-uk' is not installed, so not removed
 Package 'openoffice.org-l10n-uz' is not installed, so not removed
 Package 'openoffice.org-l10n-ve' is not installed, so not removed
 Package 'openoffice.org-l10n-vi' is not installed, so not removed
 Package 'openoffice.org-l10n-xh' is not installed, so not removed
 Package 'openoffice.org-l10n-za' is not installed, so not removed
 Package 'openoffice.org-l10n-zh-cn' is not installed, so not removed
 Package 'openoffice.org-l10n-zh-tw' is not installed, so not removed
 Package 'openoffice.org-l10n-zu' is not installed, so not removed
 Package 'openoffice.org-math' is not installed, so not removed
 Package 'openoffice.org-officebean' is not installed, so not removed
 Package 'openoffice.org-style-andromeda' is not installed, so not removed
 Package 'openoffice.org-style-oxygen' is not installed, so not removed
 Package 'openoffice.org-style-tango' is not installed, so not removed
 Package 'openoffice.org-thesaurus-ca' is not installed, so not removed
 Package 'openoffice.org-thesaurus-cs' is not installed, so not removed
 Package 'openoffice.org-thesaurus-de' is not installed, so not removed
 Package 'openoffice.org-thesaurus-de-ch' is not installed, so not removed
 Package 'openoffice.org-thesaurus-en-au' is not installed, so not removed
 Package 'openoffice.org-thesaurus-en-us' is not installed, so not removed
 Package 'openoffice.org-thesaurus-fr' is not installed, so not removed
 Package 'openoffice.org-thesaurus-hu' is not installed, so not removed
 Package 'openoffice.org-thesaurus-ne' is not installed, so not removed
 Package 'openoffice.org-thesaurus-ro' is not installed, so not removed
 Package 'openoffice.org-thesaurus-ru' is not installed, so not removed
 Package 'openoffice.org-thesaurus-sk' is not installed, so not removed
 Package 'openoffice.org-voikko' is not installed, so not removed
 Package 'openoffice.org-writer' is not installed, so not removed
 Package 'docvert-openoffice.org' is not installed, so not removed
 Package 'kde-thumbnailer-openoffice' is not installed, so not removed
 Package 'mozilla-openoffice.org' is not installed, so not removed
 Package 'openclipart-openoffice.org' is not installed, so not removed
 Package 'openoffice.org-dmaths' is not installed, so not removed
 Package 'openoffice.org-filter-mobiledev' is not installed, so not removed
 Package 'openoffice.org-mysql-connector' is not installed, so not removed
 Package 'openoffice.org-ogltrans' is not installed, so not removed
 Package 'openoffice.org-pdfimport' is not installed, so not removed
 Package 'openoffice.org-presentation-minimizer' is not installed, so not removed
 Package 'openoffice.org-presenter-console' is not installed, so not removed
 Package 'openoffice.org-report-builder' is not installed, so not removed
 Package 'openoffice.org-sdbc-postgresql' is not installed, so not removed
 Package 'openoffice.org-starter-guide' is not installed, so not removed
 Package 'openoffice.org-style-crystal' is not installed, so not removed
 Package 'openoffice.org-style-galaxy' is not installed, so not removed
 Package 'openoffice.org-style-hicontrast' is not installed, so not removed
 Package 'openoffice.org-wiki-publisher' is not installed, so not removed
 Package 'openoffice.org-writer2latex' is not installed, so not removed
 Package 'openoffice.org-writer2xhtml' is not installed, so not removed
 Package 'openoffice.org-zemberek' is not installed, so not removed
 Package 'python-openoffice' is not installed, so not removed
 Package 'libopenoffice-oodoc-perl' is not installed, so not removed
 Package 'openoffice.org-hyphenation-lt' is not installed, so not removed
 Package 'openoffice.org-hyphenation' is not installed, so not removed
 Package 'openoffice.org-dtd-officedocument1.0' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
  jsvc libcommons-daemon-java libjetty-java libslf4j-java
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
   openoffice-debian-menus*
 0 upgraded, 0 newly installed, 1 to remove and 8 not upgraded.
 After this operation, 2,224 kB disk space will be freed.
 (Reading database ... 415746 files and directories currently installed.)
 Removing openoffice-debian-menus (4.1.1-9775) ...
 /usr/bin/gtk-update-icon-cache
 /usr/bin/gtk-update-icon-cache
 Purging configuration files for openoffice-debian-menus (4.1.1-9775) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for gnome-icon-theme (3.10.0-0ubuntu2) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages will be REMOVED:
   jsvc libcommons-daemon-java libjetty-java libslf4j-java
 0 upgraded, 0 newly installed, 4 to remove and 8 not upgraded.
 After this operation, 1,844 kB disk space will be freed.
 (Reading database ... 415423 files and directories currently installed.)
 Removing jsvc (1.0.15-5ubuntu2) ...
 Removing libcommons-daemon-java (1.0.15-5ubuntu2) ...
 Removing libjetty-java (6.1.26-1ubuntu1) ...
 Removing libslf4j-java (1.7.5-2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 removed doc-base file...
 Temp File /tmp/ptconfigure-temp-script-27028685322.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Uninstaller:
 ------------------------------
 OpenOffice: Success
 ------------------------------
 Installer Finished
 ******************************




メリット
----------

* ヘルプとインストールで使用されるパラメータは、他の人に比べながら、追加的な利点である大文字と小文字を区別しません。
* これは、Ubuntuと同様にセントOSの両方に裕福なです。
* この意志モジュールが更新されたバージョンでは、PHPのAPCをインストールします。
* 生産性スイートとしてApache OpenOfficeのを使用する主な利点は、コストから来ている。これは、ワードプロセッサ、スプレッドシート、
  プレゼンテーション、ベクトルグラフィックの編集およびデータベース管理コンポーネントを含む。
* 初心者が使用することを学ぶことは簡単だが、それは経験豊富なユーザーが欲しい高度なタスクを実行するのに十分強力である。それは、
  そのように設計されています コマンドや関数は、あなたが全体のスイート全体のソフトウェアの仕事の1コンポーネントで実行します。

