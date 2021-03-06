========
Awstats
========

概要
------------

このモジュールは、最新のバージョンで、AWStatsはの設置を促進する。 AWStatsは、そのようなウェブ、ストリーミングメディア、メール、FTPサーバなどのインターネットサービスからのデータを分析するのに適したツールを報告するオープンソースのWeb分析、である。 AWStatsのは、HTMLレポートを生成する、サーバーのログファイルを解析し、解析する。

訪問者、ページ、ヒット、時間、検索エンジン、あなたのサイトを見つけるために使用されるキーワード、壊れたリンク、ロボットや多：AWStatsの（高度なWeb統計）を使用すると、すべてのWeb統計を含めて示している強力な、フル機能を備えたWebサーバのログファイルアナライザですもっと。

私たちは、このAWStatsは、特徴や今後のトピックでAWStatsはの要件をインストールする方法の詳細を見てみましょう。

helpコマンド
---------------------

helpコマンドは、とだけでなく、AWStatsのモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それは、AWStatsのモジュールの別のパラメータを示しています。また、AWStatsのモジュールをインストールするための構文について説明します。 AWStatsのモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash	
	
	ptconfigure AWStats help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、AWStatsの下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWStats help
 ******************************


  This command allows you to update AWStats.

  AWStats, Awstats, awstats

        - install
        Installs the latest version of awstats
        example: ptconfigure awstats install

 ------------------------------
 End Help
 ******************************

インストール
----------------

ユーザーがマシンにAWStatsのをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash

	ptconfigure AWStats install

表形式で示すように、上記のコマンドを入力した後、次の処理が発生します。

.. cssclass:: table-bordered

 +-----------------------+--------------------------------+----------------+----------------------------------------------------+
 | パラメーター          | 代替パラメータ                 | オプション     | コメント                                           |
 +=======================+================================+================+====================================================+
 |Install AWStats? (Y/N) | AWStats, Awstats, awstats      | Y(Yes)         | ユーザーは、Yと入力することができ、                |
 |                       |                                |                | インストールプロセスを続行したい場合               |
 +-----------------------+--------------------------------+----------------+----------------------------------------------------+
 |Install AWStats? (Y/N) | AWStats, Awstats, awstats      | N(No)          | ユーザーは、Nと入力することができ、                |
 |                       |                                |                | インストールプロセスを終了したい場合は|            |
 +-----------------------+--------------------------------+----------------+----------------------------------------------------+


ユーザーがインストールを進行する場合は、以下の処理がインストール中に関与している：

* パッケージ一覧を読み込みます。
* 依存関係ツリーを構築します。
* 必要な追加パッケージをインストールします
* 提案されたパッケージをインストールします。
* 新しいパッケージをインストールします。

以下のスクリーンショットに示すように、最後に、日本語化を目指して修正のインストールが正常に完了されます：

.. code-block:: bash

 kevell@corp:/# ptconfigure awstats install
 Install AWStats? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         AWStats!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libnet-xwhois-perl
 Suggested packages:
  libgeo-ipfree-perl
 The following NEW packages will be installed:
  awstats libnet-xwhois-perl
 0 upgraded, 2 newly installed, 0 to remove and 182 not upgraded.
 Need to get 799 kB of archives.
 After this operation, 3,311 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main awstats all 7.2+dfsg-1 [778 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libnet-xwhois-perl all 0.90-4 [21.0 kB]
 Fetched 799 kB in 12s (65.2 kB/s)
 Selecting previously unselected package awstats.
 (Reading database ... 199987 files and directories currently installed.)
 Preparing to unpack .../awstats_7.2+dfsg-1_all.deb ...
 Unpacking awstats (7.2+dfsg-1) ...
 Selecting previously unselected package libnet-xwhois-perl.
 Preparing to unpack .../libnet-xwhois-perl_0.90-4_all.deb ...
 Unpacking libnet-xwhois-perl (0.90-4) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Setting up awstats (7.2+dfsg-1) ...
 Setting up libnet-xwhois-perl (0.90-4) ...
 [Pharaoh Logging] Adding Package awstats from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 AWStats: Success
 ------------------------------
 Installer Finished
 ******************************



日本語化を目指して修正の特長
----------------------------------------------

完全なログ解析は、あなたに以下の情報を表示するようにAWStatsのが可能になります。

* 訪問やユニーク訪問者数
* 訪問期間と最後の訪問
* 認証されたユーザー、そして最後に認証されたの訪問
* 週とラッシュ時間の日数（ページ、ヒット、毎日、1時間KB）
* ホストのドメイン/国の訪問者（ページ、ヒット、KB）
* ホストリスト、最後の訪問や、未解決のIPアドレスリスト
* 閲覧最多、入口と出口ページ
* ファイルタイプ（mod_gzipのかmod_deflateがための）*ウェブ圧縮統計
* 使用ブラウザ（ページ、ヒット、各ブラウザ用KB）使用
* OS（ページ、ヒット、各OS用KB）
* ロボットの訪問
* ワーム攻撃
* ダウンロードと継続検出 あなたのサイトを見つけるために使用される*検索エンジン、キーフレーズとキーワード
* HTTPエラー（ページ最後のリファラにはない、など、）
* 画面サイズレポート
* 回数は、あなたのサイトは「お気に入りのブックマークに追加」されているサポートするブラウザの
* 比：ジャワ、フラッシュ、RealG2リーダー、QuickTimeのリーダー、WMAリーダー、PDFリーダー負荷分散サーバー比について*クラスタレポート
* その他のパーソナライズされた報告書...



それだけでなく、次の機能をサポートします。

* すべてのログ形式を分析することができます
* ダイナミックで（CGIとして、コマンドラインから、ブラウザから作品
  いくつかのチャートのフィルタ機能）
* 統計の更新は、Webインターフェイスからオンデマンドで行うことができ、
  あなたのスケジューラからだけでなく、

* 無制限のログファイルのサイズ、サポート分割ログファイル（負荷分散システム）でも、
  入口と出口のページのためのログファイルを「ほぼソート」*サポート
* 前または分析中にDNSルックアップを逆に、DNSキャッシュファイルをサポートしています
  IPロケーションまたはドメイン名から*カントリー検出
* WHOISリンク
* オプション/フィルタやプラグインの多くは、使用することができます
  サポートされている*マルチという名前のWebサイト（仮想サーバー）
* クロスサイトスクリプティング攻撃の保護
* いくつかの言語
* まれなPerlのライブラリの必要はありません
* 動的CGI出力として報告する
* 静的HTMLまたはXHTMLページを1でレポートまたはフレーム
* 実験PDFエクスポート
* 見て、色があなたのサイトのデザイン（CSS）を一致させることができます
* HTMLのヘルプとツールチップがページを報告した
* 簡単（編集するだけで1コンフィギュレーション·ファイル）を使用する
* 分析データベースはXML形式で保存することができる（XSLT処理用、...）
* Webminのモジュール
* ソースとフリー（GNU GPL）（Perlスクリプト）
* すべてのプラットフォーム上で利用可能

日本語化を目指して修正の必要条件
-------------------------------------------------------

AWStatsのCGIスクリプトを使用するには、次の要件が必要になります。

* あなたのサーバーは、あなたが読むことができるログファイルにウェブアクセスをログインする必要があります。
* AWStatsはを実行するには、コマンドラインから、ご使用のオペレーティング·システムができなければなりません
  Perlスクリプト（.plのファイル）を実行する。
* Perlモジュール「エンコード」に、利用可能でなければなりません。

（リアルタイムの統計のための）CGIとしてAWStatsはを実行するには、Webサーバーは、そのようなスクリプトを実行することができなければならない。

  そうでない場合は、最後のPerlのバージョンをダウンロードすることによりこの問題を解決することができます。

  http://www.activestate.com/ActivePerl/（Windowsの場合）

  http://www.perl.com/pub/language/info/software.html（すべてのOS）

メリット
-----------


* 追加された利点の一方である大文字と小文字を区別しませんヘルプとインストールとアンインストールの操作で使用されるパラメータ
  他の人に比べ。
* これは、Ubuntuと同様にセントOSの両方に裕福なです。
* この意志モジュールが更新されたバージョンで日本語化を目指して修正をインストールします。
* モジュールがすでにユーザマシン内に存在されている場合は、それがすでに存在しているようにメッセージが表示されます。
* AWStatsのは、Apacheの（NCSA組み合わせ/ XLF / ELFログ形式または共通ログ形式（CLF））を含むほとんどの主要なWebサーバログファイル形式をサポート   しています  WebSTARの、IIS（W3Cログ形式）、および他の多くの一般的なWebサーバのログ形式。
* 開発者は、SourceForge.netを通じてAWStatsのプロジェクトに貢献することができます。
* Perlで書かれ、AWStatsは、ほぼすべてのオペレーティングシステム上に展開することができます
* これは、ほとんどのLinuxディストリビューションで利用可能なパッケージを使用して、サーバー管理ツールです。
* AWStatsは、ログファイルは、リモートからダウンロードすることができます状況でローカルな使用のために、そのようなMS Windowsのように、ワークステー  ションにインストールすることができます サーバー。
