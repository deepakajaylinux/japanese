======
Jrush
======

あらすじ
------------

このモジュールは、jrush あなたのマシンにインストールするのに役立ちます。また、最新バージョンの更新を容易にします。私たちを見てみましょうどのようにこのモジュール、jrush をインストールするのに役立ちます。

ヘルプ コマンド
--------------------

Help コマンドと同様、目的に関するユーザー ガイドとして Jrush モジュールに含まれているオプションについて。それは Jrush モジュールの代替パラメーターが一覧表示されます。また、Jrush モジュールをインストールするための構文について説明します。Jrush モジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash

		ptconfigure JRush help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、JRush の下で help コマンドについて視覚化します。



.. code-block:: bash

 kevell@corp:/# ptconfigure JRush help
 ******************************


  This command allows you to install or Update JRush.

  JRush, jrush, Jrush, jRush

        - install
        Installs the latest version of jRush
        example: ptconfigure jRush install

 ------------------------------
 End Help
 ******************************




インストール
----------------

ユーザーのマシンに JRush をインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure JRush install




オプション
----------------

上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +---------------------------+------------------------------------------------+--------------+----------------------------------------------+
 | パラメーター              | 代替パラメーター                               | オプション   | コメント                                     |
 +===========================+================================================+==============+==============================================+
 |Install JRush - Joomla     | 代わりにJRushの我々は使用することができます:   | Y(Yes)       | ユーザーは、Yと入力することができ、          |
 |Command Line ? (Y/N)       | jrush, Jrush.                                  |              | インストールプロセスを続行したい場合         |
 +---------------------------+------------------------------------------------+--------------+----------------------------------------------+
 |Install JRush - Joomla     | 代わりにJRushの我々は使用することができます:   | N(No)        | ユーザーは、Nと入力することができ、          |
 |Command Line ? (Y/N)       | jrush, Jrush.                                  |              | インストールプロセスを終了したい場合は|      |
 +---------------------------+------------------------------------------------+--------------+----------------------------------------------+


ユーザー インストール プロセスの進行を表形式で示すように、次の操作が発生します。


.. cssclass:: table-bordered

 
 +------------------------+-----------------------------------+------------+----------------------------------------------------------------+
 | パラメーター           | パス                              | オプション | コメント                                                       |
 +========================+===================================+============+================================================================+
 |Program data directory  | “/opt/jrush (corresponding        | Yes        | ユーザーがデフォルトのプログラムのデータディレクトリを使用     |
 |(デフォルト)            | module)                           |            | してインストールを続行する場合、それらはYESと入力をすること    |
 |                        |                                   |            | ができます                                                     |
 +------------------------+-----------------------------------+------------+----------------------------------------------------------------+
 |Program data directory  | User specific                     | No(End     | ユーザーが自分自身のプログラムデータディレクトリを続行したい   |
 |                        |                                   | slash)     | 場合は、Nとして、手入力は、自分の場所を指定することができます  |
 +------------------------+-----------------------------------+------------+----------------------------------------------------------------+
 |Program executor        | “/usr/bin”                        | Yes        | ユーザーがデフォルトのプログラム実行ディレクトリを使用してイ   |
 |directory (デフォルト)  |                                   |            | ンストールを続行する場合、それらはYESと入力をする              |
 |                        |                                   |            | ことができます                                                 |
 +------------------------+-----------------------------------+------------+----------------------------------------------------------------+
 |Program executor        | User Specific                     | N0(End     | ユーザーが独自のプログラム実行ディレクトリを続行したい場       |
 |directory               |                                   | slash)     | 合は、入力Nとして、そして手に、彼らは場所を所                  |
 |                        |                                   |            | 有指定することができます。|                                    |
 +------------------------+-----------------------------------+------------+----------------------------------------------------------------+


インストール中には、次のプロセスが発生します。

* 受信オブジェクトのステータスが表示されます。
* デルタの解決の状態が表示されます。
* 接続をチェックします。
* 設定プログラムのデータ フォルダーとして表示されます。
* 既に存在していた場合に、プログラム エグゼキュータを削除します。

最後に、 Jrushのインストールが完了します。以下のスクリーンショットは、インストールしてJRushあなたのマシンをアンインストールするプロセスを示している。

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush install
 Install JRush - Joomla Command Line ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/jrush.git'  /tmp/jrush/jrushCloning into '/tmp/jrush/jrush'...
 remote: Counting objects: 3452, done.
 remote: Total 3452 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (3452/3452), 2.04 MiB | 50.00 KiB/s, done.
 Resolving deltas: 100% (2097/2097), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash

.. code-block:: bash

 kevell@corp:/# ptconfigure jRush uninstall
 Un Install JRush - Joomla Command Line ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)
 
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* このモジュールを最新のバージョン JRush をインストールするユーザーを容易にします。
* ユーザーは、プログラムのデータ ディレクトリと遺言執行者の独自のパスを選択できます。
* ヘルプとインストールの宣言で使用されるパラメーターは大文字と小文字を区別しながら他の人に比べての利点を追加する必要があります。
* それは裕福な両方セント OS とも ubuntu のように。必要なステータスは、インストール中に明確に監視されます。
 

