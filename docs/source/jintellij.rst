==========
IntelliJ
==========


あらすじ
------------

このモジュールの最新バージョンとジェット脳 IDE である IntelliJ のインストールを促進します。IntelliJ プラットフォームは、包括的な一連のコンポーネント、仮想ファイル システム、UI フレームワーク、テキスト エディター、たとえば、解析を含む抽象構文木と他の言語に固有のインフラストラクチャ、ナビゲーション、コード補完、検査、意図、リファクタリング、バージョン管理の統合、スクリプトデバッガーのフレームワーク、グラフィカルなユニット テスト ランナーを実装するためのフレームワークとスマートな言語認識の Ide を構築するためのプラットフォームです。

IntelliJ プラットフォームのソース コードは Apache 2.0 ライセンスでカバーされます。つまり JetBrains にロイヤリティを支払うことがなくオープン ソースと商用の製品、プラットフォーム上に構築することができます。このモジュールの下に IntelliJ の機能についてみてみましょう。

ヘルプ コマンド
-----------------

Help コマンドと同様、目的に関するユーザー ガイドとして IntelliJ モジュールに含まれているオプションについて。それは、IntelliJ モジュールの代替パラメーターを一覧表示されます。また、IntelliJ モジュールをインストールするための構文について説明します。IntelliJ モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

 		ptconfigure IntelliJ help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、IntelliJ 下 help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure IntelliJ help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  IntelliJ, intellij

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************



インストール
---------------

ユーザーのマシンに JRush をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure IntelliJ install

上記のコマンドを入力した後、次の操作が発生します。

* IntelliJ バージョンの入力をユーザーに要求します。
* モジュールの可用性を確保し、ないバージョンをチェックします。
* 場合は、モジュールがユーザーのコンピューターに存在しません、インストールを開始します。
* インストール中に Java のインストール ディレクトリを入力するユーザーを要求します。

最後に、IntelliJ のインストールを完了を取得します。以下のようにスクリーン ショットは、IntelliJ をインストールするプロセスを示しています。



.. code-block:: bash

 kevells@corp:/# ptconfigure IntelliJ install
 Install IntelliJ IDE? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         IntelliJ IDE        *
 *******************************
 Enter IntelliJ Version
 PHP Notice:  Undefined offset: 0 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (0)  
 PHP Notice:  Undefined offset: 1 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (1)  

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-98824051629.sh
 chmod 755 /tmp/ptconfigure-temp-script-98824051629.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-98824051629.sh Permissions
 Executing /tmp/ptconfigure-temp-script-98824051629.sh
 Cloning into 'intellij'...
 remote: Counting objects: 1026, done.
 remote: Total 1026 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1026/1026), 205.06 MiB | 410.00 KiB/s, done.
 Resolving deltas: 100% (60/60), done.
 Checking connectivity... done.
 Checking out files: 100% (744/744), done.
 Temp File /tmp/ptconfigure-temp-script-98824051629.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 IntelliJ: Success
 ------------------------------
 Installer Finished
 ******************************

パラメーター
----------------------------

我々 が使用することができます IntelliJ intellij の代わりに

利点
------------


* このモジュール IntelliJ 最新版をインストールするユーザーを容易にします。
* ヘルプとインストールの宣言で使用されるパラメーターは大文字と小文字を区別しながら他の人に比べての利点を追加する必要があります。
* それは裕福な両方セント OS とも ubuntu のように。必要なステータスは、インストール中に明確に監視されます。
* インストール時にユーザーが必要なバージョンを入力できる、Java インストール ディレクトリだけでなく。
 

