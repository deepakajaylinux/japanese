==========
Composer
==========

あらすじ
---------

作曲家は、PHP のプログラミング言語 PHP ソフトウェアと必要なライブラリの依存関係を管理するための標準フォーマットを提供するためのアプリケーション レベルの依存関係マネージャーです。

それはそれらをインストール、プロジェクトとプロジェクトに必要な依存ライブラリを宣言することができます。作曲家はマルチプラット フォームと努めていますそれ Windows、Linux、OSX にも同じように実行します。

ヘルプ コマンド
-----------------

このコマンドは、作曲家モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドは代替パラメーターとインストール用のコマンドについて、エンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
              
		 ptconfigure composer help


.. code-block:: bash

 kevell@corp:/# ptconfigure composer help
 ******************************


  This command allows you to update Composer.

  Composer, composer

        - install
        Installs the latest version of composer
        example: ptconfigure composer install

 ------------------------------
 End Help
 ******************************

インストール
--------------

ユーザー マシンで作曲家のモジュールをインストールする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
               
		 ptconfigure composer install


インストール中に、システムを求める、ディレクトリ名、あなたのパスを設定したい場合はあなたのパスを定義できます。定義によって続いた '/' のシンボルをあなたのパスには。既定のパスを使用して Enter キーを押します。

"What is the program data directory? "/opt/composer" - use this?


インストール中に、システムを求める実行ディレクトリ名、あなたのパスを設定したい場合はあなたのパスを定義できます。定義によって続いた '/' のシンボルをあなたのパスには。既定のパスを使用して Enter キーを押します。


"What is the program executer directory? Found "/usr/bin" - Use this? "
                              


.. cssclass:: table-bordered

 +--------------------------+-----------------------------------------------+------------+------------------------------------------------+
 | パラメーター             | 代替パラメーター                              | オプション | コメント                                       |
 +==========================+===============================================+============+================================================+
 |ptconfigure composer      | 使用できる2つの別のパラメータがある。         | Y          | システムは、インストールプロセスを開始します   |
 |Install? (Y/N)            | Composer , composer                           |            |                                                |
 +--------------------------+-----------------------------------------------+------------+------------------------------------------------+
 |ptconfigure composer      | 使用できる2つの別のパラメータがある。         | N          | システムは、インストール·プロセスを停止し、    |
 |Install? (Y/N)            | Composer , composer|                          |            |                                                |
 +--------------------------+-----------------------------------------------+------------+------------------------------------------------+



インストール コマンドのスクリーン ショットは以下します。


.. code-block:: bash


 kevell@corp:/$ ptconfigure composer install
 Install Composer - Update to latest version ? (Y/N) 
 Y
 ******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash) 
  
 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...
  
 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 6
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data Folder /opt/composer Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Composer: Success
 ------------------------------

 Installer Finished
 ******************************

利点
--------

* それは、アプリケーションの依存関係 (例えばライブラリ) をインストールします。
* それはまたユーザーは、その主な"Packagist"で利用可能な PHP アプリケーションをインストールすることができます利用可能なパッケージが含まれているリ  ポジトリ。
* それもサードパーティ製のコードの使用を容易にする自動負荷情報を指定するライブラリ自動ロード機能を提供します。
 

