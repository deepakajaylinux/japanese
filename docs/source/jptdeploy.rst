============
Ptdeploy
============

あらすじ
-------------

Ptdeploy は PHP のコードによって自動化された配置、ビルドやリリース機能、web アプリのバージョン管理およびインフラストラクチャとユーザーのアプリケーションを包みます。

よく展開を構築するために FTP または他アドホック ソリューションからコピーする多くのファイルが必要です。また、企業の自動化ツールの多くが欠落していた。ファラオのツールの下のこれらの不足 ptdeploy を克服するためにしたビルド。PHP は ptdeploy ルビー キャピストラーノでのギャップを埋めると同様。
このツールは、アプリケーションのプロビジョニングとあなたの箱をビルドします。ユーザーことができます 1 つまたは 2 つの PHP ファイルを自分のシステムにも単純または複雑なアプリケーション展開パターンを設定または、クラウド フレンドリーな展開パターンを速くセットアップします。

Ptdeploy はモジュラー、オブジェクト指向と拡張可能です。そして、ユーザーは任意の余分なモジュールが必要な場合彼らはすることができます作成要件に基づいて新しいモジュールを追加します。

この ptdeploy は、単一のファイルにユーザーの展開のすべてのステップをおおわラッパーとして機能します。これは 1 つのコマンドを使用して、アプリケーションのインスタンスを起動することができます。
 
ヘルプ コマンド
----------------------

このコマンドは、ptdeploy モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	ptconfigure ptdeploy help

 kevell@corp:/# ptconfigure Ptdeploy help
 ******************************


  This command allows you to update Ptdeploy.

  Ptdeploy, dapper, ptdeploy

        - install
        Installs the latest version of ptdeploy
        example: ptconfigure ptdeploy install

        - ensure
        Installs the latest version of ptdeploy, only if a version is not installed
        example: ptconfigure ptdeploy ensure

 ------------------------------
 End Help
 ******************************
 
インストール
----------------

このコマンドは私に役立ちますinstall ptdeploy の最新バージョン。特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
        ptconfigure ptdeploy install

上記のコマンドのスクリーンショットを以下にリストされている

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy install
 Install ptdeploy ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ptdeploy         *
 *******************************
 What is the program data directory? Found "/opt/ptdeploy" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptdeploy.git'  /tmp/ptdeploy/ptdeployCloning into '/tmp/ptdeploy/ptdeploy'...
 remote: Counting objects: 6989, done.
 remote: Total 6989 (delta 0), reused 0 (delta 0), pack-reused 6989
 Receiving objects: 100% (6989/6989), 2.61 MiB | 176.00 KiB/s, done.
 Resolving deltas: 100% (4335/4335), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************




確保するため
----------------

このコマンドは私に役立ちますinstall バージョンがインストールされていない場合にのみ ptdeploy の最新バージョン。特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash

	ptconfigure ptdeploy ensure

上記のコマンドのスクリーンショットを以下にリストされている

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************



オプション
----------- 


.. cssclass:: table-bordered

 +------------------------+------------------------------------------------------+-----------------+------------------------------------+
 | パラメーター           | 代替パラメーター                                     | オプション      | コメント                           |
 +========================+======================================================+=================+====================================+
 |ptconfigure ptdeploy    | コマンドラインで使用することができる3つの代替        | Y(Yes)          | システムは、インストール プロセス  |
 |install                 | のパラメータがある。                                 |                 | を開始します                       | 
 |                        | Ptdeploy, dapper, ptdeploy                           |                 |                                    |
 |                        | の例：ptconfigure ptdeploy install /                 |                 |                                    |
 |                        |       ptconfigure dapper install                     |                 |                                    |
 +------------------------+------------------------------------------------------+-----------------+------------------------------------+
 |ptconfigure ptdeploy    | コマンドラインで使用することができる3つの代替        | N(No)           | システムは、インストール プロセ    |
 |install                 | のパラメータがある。                                 |                 | スを停止します                     |
 |                        | Ptdeploy, dapper, ptdeploy                           |                 |                                    |
 |                        | の例：ptconfigure ptdeploy install /                 |                 |                                    |
 |                        |       ptconfigure dapper install|                    |                 |                                    |
 +------------------------+------------------------------------------------------+-----------------+------------------------------------+
 
 
利点
--------------

* ホスト ファイル、バーチャル ホスト ファイル、構成ファイルを編集して、データベースを更新しよりすべて自動化できますこれを使用します。
* リモート サーバー管理機能を使用して、ユーザーは任意のサイズのインフラストラクチャ全体にわたる展開を自動化できます。

