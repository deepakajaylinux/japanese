===============
Jasmine
===============

概要
---------

ジャスミンは、JavaScript コードをテストするためのビヘイビアー駆動開発フレームワークです。ジャスミンは、opean ソースの javascript フレームワークのテストです。ブラウザー、DOM、または任意の JavaScript フレームワークには依存しません。このように Node.js プロジェクトの web サイトに適しています。 またはどこでもその java スクリプトの設定を実行できます。

Helpコマンド
--------------

このコマンドは、ジャスミンのモジュールの使用状況を判断するのに役立ちます。それはジャスミンの代替パラメーターが一覧表示されます。また、ジャスミンのモジュールの機能の構文について説明します。ジャスミンのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

        ptconfigure Jasmine  help

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptconfigure Jasmine help
 ******************************


  This command allows you to install Jasmine from a GC Repo.

  Jasmine

        - install
        Installs the latest GC Repo version of Jasmine.
        example: ptconfigure Jasmine install

 ------------------------------
 End Help
 ******************************


インストール
---------------

端末上でジャスミンのモジュールをインストールするために使用されるコマンドは以下します。

.. code-block:: bash

        ptconfigure Jasmine install

上記のコマンドはジャスミンとその依存関係の最新バージョンをインストールすることを目指しています.

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptconfigure jasmine install
 Install Jasmine? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jasmine        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79546324044.sh
 chmod 755 /tmp/ptconfigure-temp-script-79546324044.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79546324044.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79546324044.sh
 Cloning into 'jasmine'...
 remote: Counting objects: 12178, done.
 remote: Total 12178 (delta 0), reused 0 (delta 0), pack-reused 12178
 Receiving objects: 100% (12178/12178), 6.60 MiB | 8.00 KiB/s, done.
 Resolving deltas: 100% (7866/7866), done.
 Checking connectivity... done.
 Archive:  jasmine-standalone-2.0.0.zip
  inflating: MIT.LICENSE             
  inflating: lib/jasmine-2.0.0/jasmine_favicon.png  
  inflating: lib/jasmine-2.0.0/jasmine.js  
  inflating: lib/jasmine-2.0.0/jasmine-html.js  
  inflating: lib/jasmine-2.0.0/jasmine.css  
  inflating: lib/jasmine-2.0.0/console.js  
  inflating: lib/jasmine-2.0.0/boot.js  
  inflating: SpecRunner.html         
  inflating: src/Player.js           
  inflating: src/Song.js             
  inflating: spec/PlayerSpec.js      
  inflating: spec/SpecHelper.js      
 Temp File /tmp/ptconfigure-temp-script-79546324044.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jasmine: Success
 ------------------------------
 Installer Finished
 ******************************


目標
-----------

* 良いテストの実践を奨励すべき 
* スタートを切ることを簡単にする必要があります 
* 継続的なビルド システムと簡単に統合する必要があります




