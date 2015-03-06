=======
PHPAPC
=======

あらすじ
-------------

このモジュールは、ユーザーのコンピューターにすべての可能な方法で、PHP の APC をインストールする目指します。

APC は PHP の op コード キャッシングの最も人気のあるキャッシュ メカニズムの 1 つです。アクティブ キャッシュの PHP コードを自動的に開始します。W3 を合計キャッシュ プラグイン オブジェクトを格納するためにうまく動作も ＆ MySQL をキャッシュします。

今後のテーマはガイドで完全にあなたのすべての側面、PHP の APC のインストールにかかわる。



ヘルプ コマンド
---------------------

ヘルプ コマンド同様目的に関してユーザーのガイドとして、Php の APC モジュールに含まれているオプションについて。それは Php の APC モジュールの代替パラメーターが一覧表示されます。また、Php の APC モジュールをインストールするための構文について説明します。Php の APC モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash
	
		ptconfigure PHPAPC help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、Php の APC の下で help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPAPC help

 ******************************


  This command allows you to install some common and helpful PHP APC.

  PHPAPC, php-apc, phpapc, phpapc

        - install
        Install PHP APC.
        example: ptconfigure phpapc install

 ------------------------------
 End Help
 ******************************




インストール
----------------

ユーザーのコンピューターで、Php の APC をインストールするために使用するコマンドを次に示します。


.. code-block:: bash
	
		ptconfigure phpapc install


上記のコマンドを入力した後、次のプロセスが発生します表形式で表示されます。


.. cssclass:: table-bordered

 +--------------------+-------------------------------------------+------------+----------------------------------------------+
 | パラメーター       | 代替パラメーター                          | オプション | コメント                                     |
 +====================+===========================================+============+==============================================+
 |Install PHP APC?    | の代わりに phpapc, 我々は使用することが   | Y(Yes)     | ユーザーは、Yと入力することができ、          |
 |(Y/N)               | できますPHPAPC, php-apc.                  |            | インストールプロセスを続行したい場合         |
 +--------------------+-------------------------------------------+------------+----------------------------------------------+
 |Install PHP APC?    | の代わりに phpapc, 我々は使用することが   | N(No)      | ユーザーは、Nと入力することができ、          |
 |(Y/N)               | できますPHPAPC, php-apc.                  |            | インストールプロセスを終了したい場合は|      |
 +--------------------+-------------------------------------------+------------+----------------------------------------------+



場合は、インストールを続行すると、インストールのプロセス中に記載されて、リストの下：


* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 読み取り状態情報。
* リスト アウトは自動的にインストールされているパッケージ。
* リスト アウト、余分なパッケージをインストールしています。
* リスト アウト提案パッケージ。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。


最後に、インストールが完了を取得します。次のスクリーン ショットは、PHP の APC をインストールするプロセスを視覚的に表します。


.. code-block:: bash

 kevell@corp:/# ptconfigure phpapc install

 Install PHP APC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP APC!        *
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
 The following extra packages will be installed:
  php5-apcu
 The following packages will be REMOVED:
  php5-xcache
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 1 to remove and 78 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPAPC: Success
 ------------------------------
 Installer Finished
 ******************************

APC 関数
------------------


このサブ トピックを扱う最もしばしば使われた APC の下で機能します。Php の APC での作業中、ユーザーは APC のこれらの関数を参照できます。

* apc_add — 新しい変数にキャッシュするデータ ストア
* apc_bin_dump — 指定したファイルおよびユーザー変数のバイナリ ダンプの取得
* apc_bin_dumpfile —  キャッシュされたファイルと、ファイルにユーザー変数のバイナリ ダンプを出力
* apc_bin_load-バイナリ ダンプを APC のファイル/ユーザ キャッシュに読み込む
* apc_bin_loadfile-バイナリ ダンプを APC のファイル/ユーザ キャッシュにファイルからロード
* apc_cache_info-キャッシュされた apc のデータから情報を取得
* apc_cas-新しい値と古い値を更新
* apc_clear_cache-APC キャッシュをクリアします。
* apc_compile_file-ファイルをバイトコード キャッシュに保存すべてフィルターをバイパスします。
* apc_dec-ストアドの数を減らす
* apc_define_constants-検索と一括定義する定数のセットを定義
* apc_delete_file-opcode キャッシュからファイルを削除します。
* apc_delete-格納されている変数をキャッシュから削除
* apc_exists-APC キーが存在するかどうかはチェック
* apc_fetch-格納されている変数をキャッシュから取得
* apc_inc-ストアド数を増やします。
* apc_load_constants-定数のセットをキャッシュから読み込みます
* apc_sma_info-取得 APC の共有メモリ割り当てに関する情報
* apc_store-キャッシュ データ ストア内の変数



利点
-----------

* ヘルプとインストールで使用されるパラメーター大文字小文字が区別されません中に他の人に比べて、追加の利点は。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* この意志モジュール更新版で、php の apc をインストールします。
* モジュールがユーザーのマシンで既に存在する場合それが既に存在するようにメッセージが表示されます。
* APC apc.php を使って、シンプルな web ベースのインターフェイスを提供するという名前のファイルが付属します。
 

