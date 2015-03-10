=========
PHPSSH 
=========

あらすじ
-----------

PhpSSH がそれを取得し、実行するも容易になりました。リモート シェルを取って PhpSSH を介して自動アップグレード ptconfigure をやすく
さまざまなタスクを遂行するためは、規範ユーザー インフラストラクチャで複数のサーバー マシンを持って場合です。

Helpコマンド
--------------------

helpコマンドは、とだけでなく、PHPのSSHに含まれているオプションについての目的について、ユーザーをガイドします。これは、PHPのSSHの別のパラメータを示しています。また、PHPのSSHモジュールの構文について説明します。 PHPのSSHモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash

                ptconfigure PHPSSH help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、help コマンドの下で PHP SSH について視覚化します。



.. code-block:: bash

 kevell@corp:/# ptconfigure PHPSSH help
 ******************************


  This command allows you to install the PHP SSH default Module

  PHPSSH, php-ssh, phpssh

        - install
        Installs the PECL PHP SSH Extension.
        example: ptconfigure phpssh install

 ------------------------------
 End Help
 ******************************



インストール
---------------------

これはモジュールをインストールする Phpssh ptconfigure の下でちょうど、下記のコマンドを使用して顕著なプロセス


.. code-block:: bash
         
                ptconfigure phpssh install

上記のコマンドを入力した後、次の手順インストールの処理中に、表で説明されているよう



.. cssclass:: table-bordered

 +----------------------+----------------------------------------------------+---------------+---------------------------------------------+
 | パラメーター         | 代替パラメーター                                   | オプション    | コメント                                    |
 +======================+====================================================+===============+=============================================+
 |Install PHPSSH? (Y/N) | 代わりに使用したの PHPSSH我々は使用することがで    | Y(Yes)        | ユーザーは、Yと入力することができ、         |
 |                      | きますphpssh, php-ssh                              |               | インストールプロセスを続行したい場合        |
 +----------------------+----------------------------------------------------+---------------+---------------------------------------------+
 |Install PHPSSH? (Y/N) | 代わりに使用したの PHPSSH我々は使用することがで    | N(No)         | ユーザーは、Nと入力することができ、         | 
 |                      | きますphpssh,php-ssh                               |               | インストールプロセスを終了したい場合は|     |
 +----------------------+----------------------------------------------------+---------------+---------------------------------------------+


場合は、インストールを続行すると、インストールのプロセス中に記載されて、リストの下：


* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウト、余分なパッケージをインストールします。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。


.. code-block:: bash


 kevell@corp:/# ptconfigure phpssh install
 Install PHP SSH? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP SSH!        *
 *******************************
 
 Creating config file /etc/php5/mods-available/ssh2.ini with new version
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libssh2-1
 The following NEW packages will be installed:
  libssh2-1 libssh2-php
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 91.0 kB of archives.
 After this operation, 389 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-1 amd64 1.4.3-2 [66.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-php amd64 0.12-1build1 [24.7 kB]
 Fetched 91.0 kB in 4s (19.8 kB/s)
 Selecting previously unselected package libssh2-1:amd64.
 (Reading database ... 183000 files and directories currently installed.)
 Preparing to unpack .../libssh2-1_1.4.3-2_amd64.deb ...
 Unpacking libssh2-1:amd64 (1.4.3-2) ...
 Selecting previously unselected package libssh2-php.
 Preparing to unpack .../libssh2-php_0.12-1build1_amd64.deb ...
 Unpacking libssh2-php (0.12-1build1) ...
 Setting up libssh2-1:amd64 (1.4.3-2) ...
 Setting up libssh2-php (0.12-1build1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package libssh2-php from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPSSH: Success
 ------------------------------
 Installer Finished
 ******************************		     


利点
-----------------

* 最初の第一の通信のプライバシーです。つまり、リモート シェルのログインを提供する接続する必要があります。
  盗聴を防ぐために暗号化されます。
* いずれかの当事者によるデータ送信がいない変更、または改ざんかどうかを確認するメカニズムがある必要があります。整合性チェックは、一言で言えば、
  必要であります。
* 適切な認証を確立するために、お互いに、サーバーとクライアントの両方の id を指定しなければなりません。
* PhpSSH によって提供される暗号化と認証メカニズムは大きい程度にセキュリティを強化できます。
 

