=========
PHPEdit
=========

概要
------------

PHPEditモジュールは、PHPのための完全な統合開発環境です。シンプルなPHPの編集よりもはるかに、それは、ユーザーが自分の展開に、プロジェクトの設計、彼らのドキュメントから必要なすべての機能を統合し、単一のツールで、フレンドリーで効率的な方法で彼らのプロジェクトを実施するために、ユーザーに役立ちます。これは、UbuntuとCentOSの適切な。

Helpコマンド
-----------------------

helpコマンドは、とだけでなく、Phpeditモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それはPhpeditモジュールの別のパラメータを示しています。また、Phpeditモジュールをインストールするための構文について説明します。 Phpeditモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash 

	ptconfigure Phpedit help 

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、Phpedit下に、helpコマンドについてあなたを視覚化。


.. code-block:: bash 

 kevell@corp:/# ptconfigure PHPEdit help 

 ****************************** 


  This command allows you to update PHPEdit. 

  PHP-Edit, phpedit, PHPEdit 

        - install 
        Installs the latest version of PHPEdit 
        example: ptconfigure phpedit install 

 ------------------------------ 
 End Help 
 ****************************** 

インストール
----------------

そ れはPHPEditは常に、新しい機能やメンテナンスの修正で、自動更新を進化されているため、ユーザneeds.Howeverスーツに合わせてカスタ マイズすることができるインストーラに同梱されているので、PHPEditは、ファイルとツールを助け、フレームワーク、拡張機能の多くが付属していますシステムは難なくPHPEditの最新のリリースに追いつく助けるために、も利用可能です。次のようにコマンドは、このモジュールのインストールに使用、

.. code-block:: bash 

	ptconfigure Phpedit install 

スクリーンショットは、このモジュールについて明らかにしている。


.. code-block:: bash 


 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************

アンインストール
------------------

モジュールのアンインストールに使用するコマンドは、以下に記載されている


.. code-block:: bash


 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
-----------

.. cssclass:: table-bordered 


 +----------------------------+-------------------------------------+------------+---------------------------------------------------+
 | パラメーター               | 代替パラメータ                      | オプション | コメント                                          |
 +============================+=====================================+============+===================================================+
 |Install phpedit? (Y/N)      | PHP-Edit, phpedit, PHPEdit          | Y          | ユーザーがインストールプロセスを続行します。      |
 +----------------------------+-------------------------------------+------------+---------------------------------------------------+
 |Install phpedit? (Y/N)      | PHP-Edit, phpedit, PHPEdit          | N          | ユーザーは、インストール·プロセスを終了したい。|  | 
 +----------------------------+-------------------------------------+------------+---------------------------------------------------+




メリット
---------------

* すべての利用可能なコードアシスタントとコードジェネレータで高速なユーザーコードを記述します。
* 統合デバッガを使用して、プロジェクトの品質、及びユニットテストモジュールを改善
* ユーザー·プロジェクトをクリックし、単一で簡単に展開し、リモートファイルに透過的に動作
* 自分の好きなフレームワークとユーザーの生産性を向上
* コード·インテリジェンスが可能です。
* デバッガとプロファイラも利用できる。
* 非大文字と小文字の区別は、このモジュールに重要な役割を機能する

