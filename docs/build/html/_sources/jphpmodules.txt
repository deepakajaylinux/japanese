===========
PHPModules
===========

あらすじ
-------------

このモジュールを目指してのインストールといくつかの一般的なと役立つサポート Php モジュールを包みます。いくつかの例は： php5 gd イメージ ライブラリ、php5 imagick イメージ libs、php5 カール リモート ファイル処理 libs、php5 mysql の mysql 接続を処理するためのライブラリ。今後のテーマでのインストールのプロセスはこのモジュールを使用する方法を見てみましょう。

ヘルプ コマンド
----------------------

Help コマンドと同様、目的に関するユーザー ガイドとして Php モジュールとして含まれているオプションについて。それは Php モジュールの代替パラメーターが一覧表示されます。また、Php モジュールをインストールするための構文について説明します。Php モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash
	
		ptconfigure PHPModules help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、Php モジュールの下に、help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************



インストール
--------------

ユーザーのコンピューターで php モジュールをインストールするために使用するコマンドを次に示します。

.. code-block:: bash

		ptconfigure phpmods install

上記のコマンドを入力した後、次のプロセスが発生します表形式で表示されます。


.. cssclass:: table-bordered

 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+
 | パラメーター           | 代替パラメーター                              | オプション    | コメント                                       |
 +========================+===============================================+===============+================================================+
 |Install PHP Modules?    | の代わりに phpmods, 我々は使用することがで    | Y(Yes)        | ユーザーは、Yと入力することができ、            |
 |(Y/N)                   | きますPHPModules, php-mods, php-modules,      |               | インストールプロセスを続行したい場合           |
 |                        | phpmodules.                                   |               |                                                |
 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+
 |Install PHP Modules?    | の代わりに phpmods, 我々は使用することがで    | N(No)         | ユーザーは、Nと入力することができ、            |
 |(Y/N)                   | きますPHPModules, php-mods, php-modules,      |               | インストールプロセスを終了したい場合は         |
 |                        | phpmodules.|                                  |               |                                                |
 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+


場合は、インストールを続行すると、インストールのプロセス中に記載されて、リストの下：


* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウトは自動的にインストールされているパッケージ。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。

.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install
 
 Install PHP Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mysql from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* ヘルプとインストールで使用されるパラメーター大文字小文字が区別されません中に他の人に比べて、追加の利点は。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* すべての頻繁に使用する php モジュールのインストールを取得する単一のプロセスの下で包まれていた。
 

