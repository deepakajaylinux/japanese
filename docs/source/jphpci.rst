===============
Phpci
===============

あらすじ
--------------

PHPCI は、ptconfigure に適したオープン ソース継続的な統合ツールです。ユーザーが念頭に置いてシンプルに構築してので、セットアップして使用する微風であるジェンキンスを行うことができますすべてはしない、しながら。これは Ubuntu とセントと使いやすさです OS。

ヘルプ コマンド
-----------------------

このコマンドのヘルプガイド Phpci モジュールに関する特定の操作を実行するユーザー。これは、企業のユーザーのすべてのタイプに適しています。

.. code-block:: bash
   
                ptconfigure PHPCI help

ヘルプ コマンド Phpci モジュールに組み込まれたコマンドの短いリストが表示されます。次のスクリーン ショットはそれを視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCI help
 ******************************


  This command allows you to install PHPCI, the popular Build Server.

  PHPCI, phpci

        - install
        Installs PHPCI through git, with its dependencies
        example: ptconfigure phpci install

        - config-default, default-config
        Installs a default config.yml file for PHPCI
        example: ptconfigure phpci config-default --yes --guess

        - install-default-database
        Installs a default database and user for PHPCI
        example: ptconfigure phpci install-default-database --yes --guess
            --mysql-admin-user="root" # guess will provide root
            --mysql-admin-pass="some-pass" # guess will provide ptconfigure

  You can install a complete local version of PHPCI with the following:

  sudo ptconfigure phpci install --yes --guess
  sudo ptconfigure phpci install-default-database --yes --guess
  sudo ptconfigure phpci config-default --yes --guess

 ------------------------------
 End Help
 ******************************


インストール
-----------------

このモジュールは phpci をインストールするのに役立ちます。このモジュールは作曲家を点検しなければならない最初のステップは、システムかどうか。それがない場合、システムで自動的に、それをインストールします。


.. code-block:: bash

                   ptconfigure Phpci install



上記のコマンドを入力した後、次のプロセス関与しているインストールのプロセス中に表形式で示されています。

.. cssclass:: table-bordered

 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+
 | パラメーター        | 代替パラメーター                          | オプション | コメント                                              |
 +=====================+===========================================+============+=======================================================+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci      | Y(Yes)     | ユーザーは、Yと入力することができ、インストールプ     |
 |                     | 使用することができます                    |            | ロセスを続行したい場合                                |
 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci      | N(No)      | ユーザーは、Nと入力することができ、インストールプ     |
 |                     | 使用することができます                    |            | ロセスを終了したい場合は|                             |
 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+


場合はインストールを続行すると、インストールの処理中に、次の手順、

* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウト、余分なパッケージを自動的にインストールされます。
* リスト アウトは、インストールする提案のパッケージ。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



表形式で表した、ユーザーからの入力が要求されます。



.. cssclass:: table-bordered

 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 | パラメーター       | パス                     | オプション            | コメント                                                       |
 +====================+==========================+=======================+================================================================+
 |Program data        | “/opt/phpunit(対応す     | Yes                   | ユーザーがデフォルトのプログラムのデータディレクトリを使用     |
 |directory (Default) | るモジュール)”           |                       | してインストールを続行する場合、それらはYESと入力をするこ      |
 |                    |                          |                       | とができます                                                   |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program data        | User Specific            | No(エンドスラッシュ)  | ユーザーが自分自身のプログラムデータディレクトリを続行したい   |
 |directory           |                          |                       | 場合は、入力Nとして、そして手に、彼らは場所を所有指定するこ    |
 |                    |                          |                       | とができます。                                                 |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program executor    | “/usr/bin”               | Yes                   | ユーザーがデフォルトのプログラム実行ディレクトリを使用         |
 |directory (Default) |                          |                       | してインストールを続行する場合、それらはYESと入力をすることが  |
 |                    |                          |                       | できます                                                       |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program executor    | User specific            | No(エンドスラッシュ)  | ユーザーが独自のプログラム実行ディレクトリを続行したい場合は、 |
 |directory           |                          |                       | 入力Nとして、そして手に、彼らは場所を所有指定すること          |
 |                    |                          |                       | ができます。|                                                  |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。


.. code-block:: bash

 kevell@corp:/#ptconfigure PHPCI install
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 [Pharaoh Logging] Packages php5-mcrypt, curl from the Packager Apt are already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-45785693692.sh
 chmod 755 /tmp/ptconfigure-temp-script-45785693692.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45785693692.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45785693692.sh
 Temp File /tmp/ptconfigure-temp-script-45785693692.sh Removed
 Creating /tmp/ptconfigure-temp-script-47686609771.sh
 chmod 755 /tmp/ptconfigure-temp-script-47686609771.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47686609771.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47686609771.sh
 Module rewrite already enabled
 Temp File /tmp/ptconfigure-temp-script-47686609771.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Composer reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-71236381661.sh
 chmod 755 /tmp/ptconfigure-temp-script-71236381661.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71236381661.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71236381661.sh
 Installing block8/phpci (1.6.0)
   - Installing block8/phpci (1.6.0)
    Loading from cache

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
  - Installing symfony/yaml (v2.6.4)
    Loading from cache

  - Installing block8/b8framework (1.1.9)
    Loading from cache

  - Installing ircmaxell/password-compat (v1.0.4)
    Loading from cache

  - Installing psr/log (1.0.0)
    Loading from cache

  - Installing monolog/monolog (1.12.0)
    Loading from cache

  - Installing pimple/pimple (v1.1.1)
    Loading from cache

  - Installing symfony/console (v2.6.4)
    Loading from cache

  - Installing symfony/filesystem (v2.6.4)
    Loading from cache

  - Installing symfony/config (v2.6.4)
    Loading from cache

  - Installing robmorgan/phinx (v0.4.2.1)
    Loading from cache

  - Installing swiftmailer/swiftmailer (v5.3.1)
    Loading from cache

 Generating autoload files
 Temp File /tmp/ptconfigure-temp-script-42085224634.sh Removed
 Creating /tmp/ptconfigure-temp-script-47565859655.sh
 chmod 755 /tmp/ptconfigure-temp-script-47565859655.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47565859655.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47565859655.sh
 [Pharaoh Logging] Lets begin Configuration of a Web Server for PHPCI
 [Pharaoh Logging] Lets Add our Apache VHost
 [Pharaoh Logging] Now lets restart Apache so we are serving our new application 

 Logging Starting
 Logging Complete
 Logging Starting
 Logging Complete
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.phpci.local
	DocumentRoot /opt/phpci/phpci/public/
	<Directory /opt/phpci/phpci/public/>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Require all granted

        <IfModule mod_rewrite.c>
          RewriteEngine On
          RewriteBase /opt/phpci/phpci/public/
          RewriteCond %{REQUEST_FILENAME} !-f
          RewriteCond %{REQUEST_FILENAME} !-d
          RewriteRule . /index.php [L]
        </IfModule>

	</Directory>

 </VirtualHost>

 Assuming Okay due to yes parameter
 Site www.phpci.local already enabled
 a2ensite www.phpci.local done
 Logging Starting
 Logging Complete
 Temp File /tmp/ptconfigure-temp-script-47565859655.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCI: Success
 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash

 kevell@corp:/#ptconfigure PHPCI config-default

 Install PHP CI Default Configuration? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPCI Defaults        *
 *******************************
 Set non-default value for db_read_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_write_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_name? Default is phpci (Y/N) 
 n
 Set non-default value for db_username? Default is phpci (Y/N) 
 n
 Set non-default value for db_pass? Default is phpci_pass (Y/N) 
 n
 Set non-default value for phpci_url? Default is http://www.phpci.local (Y/N) 
 n
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ****************************** 

.. code-block:: bash


 kevell@corp:/#ptconfigure phpci install-default-database
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 Database script executed
 ******************************  

 Seems Fine...Database Actions Finished
 ******************************

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ******************************



利点
--------

* PHPCI の構成とデータベース ファイルをインストールするために使用します。一方、既存の任意のファイルがある場合、インストール内容を上書きします。
* 新しいバージョンを自動的に更新することができます。
* それはユーザーのデータベース インストール願いごとを受け入れることができます。
* 継続的な統合が可能です。
* 複数の環境
* PDO、mysql、sqlite のような別の亜種と php の構築、debug... など。
* 自動フィーチャ検知。
 

