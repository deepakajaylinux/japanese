==================
RubySystem
==================

あらすじ
------------

Ruby のシステムは、動的な反射、高度なスクリプト言語です。Ruby システムは Ruby RVM を扱う Web アプリケーション開発のためだけです。強力なスクリプト言語として通常のシェル スクリプトで、システム管理のスクリプト処理のニーズを達成するために使用される一般的には非常に良い選択肢として使用することもできます。組み込みモジュールのセットといくつかの外部ライブラリ、Ruby のシステムのシステム管理を効率化できます。Ruby のシステムは非常に便利で強力なツールがありますすべてのシステム管理者のツールボックスで持っています。それは、Ubuntu とセント OS と快適です。

ヘルプ コマンド
--------------------

このコマンドは目標と Ruby のシステム モジュールの下に利用可能なコマンドについて機能することができます。また、Ruby のシステムをインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。


.. code-block:: bash
        
		ptconfigure RubySystem help



次のイメージはまた、このモジュールを明確に理解することができます。


.. code-block:: bash

 kevell@corp:/# ptconfigure RubySystem help
 ******************************


  This command allows you to install Ruby RVM, the system wide version.

  RubySystem, rubysystem, ruby-system, rubysys

        - install
        Installs Ruby a System Wide version of Ruby for you
        example: ptconfigure ruby-rvm install

  Ruby is installed the recommended per-user way. To use ruby after the install
  first run "source ~/.rvm/scripts/rvm" to get access to the Ruby install for
  your user, then "rvm install 1.9.3" (to install, specify version as needed)
  then "rvm use 1.9.3" (to select your default version for the session)

 ------------------------------
 End Help
 ******************************


インストール
-------------------

それはモジュールをインストールする Ruby システム ptconfigure の下でちょうど、下記のコマンドを使用して明白なプロセス


.. code-block:: bash
        
                ptconfigure rubysystem install

コマンド キーの後に求めることができます。

Install Ruby, system wide?(Y/N)

場合に、ユーザー入力の Y として、Rubysystem パッケージからインストールします。その他に、それは、画面を終了できます。次のスクリーン ショットを説明することができます。
それは。


.. code-block:: bash


 kevell@corp:/# ptconfigure RubySystem install
 
 Install Ruby, System Wide? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Ruby System!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  ruby1.9.1-examples ri1.9.1 graphviz ruby1.9.1-dev
 The following NEW packages will be installed:
  ruby1.9.1
 0 upgraded, 1 newly installed, 0 to remove and 12 not upgraded.
 1 not fully installed or removed.
 Need to get 37.5 kB of archives.
 After this operation, 240 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main ruby1.9.1 amd64 1.9.3.0-1ubuntu1 [37.5 kB]
 Fetched 37.5 kB in 7s (5232 B/s)
 Selecting previously unselected package ruby1.9.1.
 (Reading database ... 282890 files and directories currently installed.)
 Preparing to unpack .../ruby1.9.1_1.9.3.0-1ubuntu1_amd64.deb ...
 Unpacking ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up zend-server-php-5.3 (6.1.0+b1177) ...
 Module php5 already enabled
 Module rewrite already enabled
 Site zendserver_gui already enabled
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0
 Content-type: text/html

 Setting up ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 update-alternatives: using /usr/bin/gem1.9.1 to provide /usr/bin/gem (gem) in auto mode
 [Pharaoh Logging] Adding Package ruby1.9.1 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 RubySystem: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
--------------


.. cssclass:: table-bordered


 +---------------------+--------------------------------------------------+------------+------------------------------------------------+
 | パラメータ          | 代替パラメータ                                   | オプション | 注釈                                           |
 +=====================+==================================================+============+================================================+
 |ptconfigure          | 我々は使用することができますRubySystem,          | Y          | システムは、インストールプロセスを開始します   |  
 |Rubysystem Install   | rubysystem, ruby-system, rubysys.                |            |                                                |
 +---------------------+--------------------------------------------------+------------+------------------------------------------------+
 |ptconfigure          | 我々は使用することができますRubySystem,          | N          | システムは、インストール·プロセスを停止し、    |
 |Rubysystem Install   | rubysystem, ruby-system, rubysys.|               |            |                                                |
 +---------------------+--------------------------------------------------+------------+------------------------------------------------+


利点
---------

* Ruby のシステムは、迅速かつ簡単なオブジェクト指向プログラミングの動的な反射、高度なスクリプト言語です。
* システムでは Ruby、便利で楽しいツールです。展開プロセスで使用されているツールを含みます。
* Ruby のシステムは既にウェブ開発、一般的なソフトウェア エンジニア リングの極端な知識を持つ経験豊富な専門家スキル。
* Ruby プログラミング言語 Ruby システムの主な利点は、開発のスピードと見なされます。
 

