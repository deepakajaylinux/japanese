============
VNCPasswd
============

あらすじ
----------------

Vncpasswd ユーティリティを使用して、作成および VNC サーバー認証用のパスワードを変更する必要があります。Vncserver スクリプトから起動すると、ローカル デスクトップ マネージャーで起動したときにこのようなパスワードを使用します。vncpasswd は、1 つまたは 2 つのパスワードを入力することができます。Vncpasswd ユーティリティ尋ねる対話的にかどうかそれは 2 番目のパスワードを設定する必要があります。これは ubunt と centos 最も快適です。

ヘルプ コマンド
----------------------

Help コマンドは、Ubuntu の man ページを連想させる、コンソール ベースの広範なヘルプ システムに含まれています。ヘルプ トピックは、リモートまたはローカル エリアのためのパスワードをインストールするためのヘルプがあります。引数を指定しないでコマンドを記述する簡単です。

.. code-block:: bash

                ptconfigure  VNC-passwd help

次のスクリーン ショットは、それを視覚化できます。


.. code-block:: bash

 kevell@corp:/# ptconfigure VNCPasswd help

 ******************************


  This command allows you to install VNCPasswd, the popular Remote/Local Desktop Manager Solution.

  VNCPasswd, vncpasswd, vnc-passwd

        - install
        Installs VNCPasswd through a package manager
        example: ptconfigure vnc install

 ------------------------------
 End Help
 ******************************

インストール
-----------------

インストールは vncpassward をインストールすることができます。リモートまたはローカルのデスクトップで非常に人気です。Vnc passwd パッケージ マネージャーを介してインストールします。最初のパスワードは、プライマリ 1 つは、2 番目のパスワードは表示のみの認証に使用できます。Ubuntu や centos で快適です。
 

.. code-block:: bash

                ptconfigure  VNC-passwd install

後コマンド、システム内のキーはユーザーの入力を求めることができます。ユーザー入力がある場合 Y として他の VNCpassward をインストール可能性があります終了することができます。次のスクリーン ショットはそれを視覚化できます。



.. code-block:: bash

 kevell@corp:/# ptconfigure VNC-passwd install

 Install VNCPasswd? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNCPasswd !        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following NEW packages will be installed:
  expect
 0 upgraded, 1 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package expect from the Packager Apt did not execute correctly
 Enter VNC User:

 Enter VNC Pass:

 Creating /tmp/ptconfigure-temp-script-40114506906.sh
 chmod 755 /tmp/ptconfigure-temp-script-40114506906.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-40114506906.sh Permissions
 Executing /tmp/ptconfigure-temp-script-40114506906.sh
 sudo: unknown user: /usr/bin/expect
 sudo: unable to initialize policy plugin
 Temp File /tmp/ptconfigure-temp-script-40114506906.sh Removed
 [Pharaoh Logging] Removing Package expect
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'expect' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 0 upgraded, 0 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Package expect from the Packager Apt is not installed, so not removed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNCPasswd: Success
 ------------------------------
 Installer Finished
 ******************************








オプション
---------------


.. cssclass:: table-bordered

 +----------------------------+--------------------------------------+-------------+-------------------------------------------------------+
 | パラメーター               | パラメーターの代替                   | オプション  | コメント                                              |
 +============================+======================================+=============+=======================================================+
 |Install VNCpasswd?(Y/N)     | 我々は使用することができます         | Y           | それはptconfigureの下VNCPasswardをインストールします  |
 |                            | VNCPasswd, vncpasswd, vnc-passwd     |             |                                                       |
 +----------------------------+--------------------------------------+-------------+-------------------------------------------------------+
 |Install VNCpasswd?(Y/N)     | 我々は使用することができます         | N           | システム出口インストール                              |
 |                            | VNCPasswd, vncpasswd, vnc-passwd|    |             |                                                       |
 +----------------------------+--------------------------------------+-------------+-------------------------------------------------------+


利点
-----------------

* 多言語サポート
* VNC 認証
* 最適化されたパフォーマンス
* ファイルの転送が可能
* 強力な導入戦略
 

