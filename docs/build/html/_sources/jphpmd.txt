=========
PHPMD
=========

あらすじ
----------------

PHP MessDeductor PHP の依存のスピンオフであり、よく知られている Java ツール PMD の PHP と同等であることを目指しています。PHPMD は、PHP の依存によって測定される未フォーマット ストリームのユーザー フレンドリーなフロント エンド アプリケーションとして見なすことができます。一般担保または GC が受け入れられ、市場仲介者の過半数でレポ市場で担保としてその特定の瞬間と非常によく似たはレポ ・ レートで資産の範囲です。これは Ubuntu とセントに適した OS。

ヘルプ コマンド
----------------------

与えられた PHPMD のソースコードをベースにかかるし、そのソース内のいくつかの潜在的な問題します。PHPMD は若いプロジェクトとコードのにおいと分析のソース コード内のエラーを検出する PMD と比較して、事前に定義された規則の限られたセットだけを提供できるようにします。Allimplemented ルールの詳細について学ぶためにルールのセクションをチェック アウト。次のヘルプ コマンドは phpmd モジュールをインストールするユーザーをガイドします。


.. code-block:: bash

		ptconfigure PHPMD help

次のスクリーン ショット取り出したその機能。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPMD help
 ******************************


  This command allows you to install PHPMD from a GC Repo.

  PHPMD

        - install
        Installs the latest GC Repo version of PHPMD
        example: ptconfigure phpmd install

 ------------------------------
 End Help
 ******************************



インストール
-------------------------

現時点で PHPMD は次の 3 つのレンダラーが付属しています：

* xml, XML としてレポートの書式を設定します。
* text, シンプルなテキスト形式。
* html、可能性のある問題を持つ単一の HTML ファイル。

ユーザーのマシンに PHPMD をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure PHPMD install

上記のコマンドを入力した後、次のプロセスが発生しますスクリーン ショット形式で表示されます。


.. code-block:: bash

 kevell@corp:/# ptconfigure phpmd install
 Install PHP Mess Detector ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mess Dt.        *
 *******************************
 What is the program data directory? Found "/opt/phpmd" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpmd.git'  /tmp/phpmd/phpmdCloning into '/tmp/phpmd/phpmd'...
 remote: Counting objects: 356, done.
 remote: Total 356 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (356/356), 306.45 KiB | 9.00 KiB/s, done.
 Resolving deltas: 100% (239/239), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 PHPMD: Success
 ------------------------------
 Installer Finished
 ******************************



オプション
------------

.. cssclass:: tabe-bordered

  +-------------------------------+----------------------------+------------+---------------------------------------------------------+
  | パラメータ                    | ディレクトリ (デフォルト)  | オプション | 注釈                                                    |
  +===============================+============================+============+=========================================================+
  |Data directory (デフォルト)    | “/opt/PHPMD”               | Yes        | それはptconfigure下PHPMDモジュールをインストールします  |
  +-------------------------------+----------------------------+------------+---------------------------------------------------------+
  |Data directory                 | エンドスラッシュ           | No         | ユーザーがパスを指定する必要があります。                |
  +-------------------------------+----------------------------+------------+---------------------------------------------------------+
  |Executor directory             | “/usr/bin”                 | Yes        | それは、エグゼディレクトリにインストールされます        |
  |(デフォルト)                   |                            |            |                                                         |
  +-------------------------------+----------------------------+------------+---------------------------------------------------------+
  |Executor directory             | No trailing slash          | No         | ユーザーは、ディレクトリ名などの入力を提供します|       |
  +-------------------------------+----------------------------+------------+---------------------------------------------------------+

 

利点
------------------

過度の公共カウント:
 
パブリック メソッドと、クラスで宣言されている属性の数が多いクラス分割されるように増加の努力をする必要がありますを示すことができます。
徹底的にテストする必要あります。


過度のパラメータ一覧:

長いパラメーター リストは、多数のパラメーターをラップする新しいオブジェクトを作成することを指定できます。基本的に、パラメーターを一緒にグループ化してください。


循環的複雑度:

複雑さはメソッドに加えて、メソッド エントリの 1 つの意思決定ポイントの数によって決まります。


スーパーグローバル:

スーパー グローバル変数への直接アクセスは悪い練習と見なされます。これらの変数が用意されているオブジェクトにカプセル化する必要があります。
フレームワークによって例えば。


ショート変数:

非常に短い名前を持つフィールド、ローカル、またはパラメーターを検出します。


長い変数:

長い名前を持つフィールド、正式なまたはローカル変数が宣言されているときに検出します。


 
