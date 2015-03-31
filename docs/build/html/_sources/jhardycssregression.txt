====================
HardyCssRegression
====================


概要
-----------

ハーディは、以前GhostStory 2として知られている： Ghostening 。ハーディは、キュウリを使ってCSSテストを簡素化し、あなたの自動ビルド·プロセスに組み込むことが簡単になり、コマンドラインツールです。テストケースを作る簡素化するChrome拡張もあります。それは、 Node.jsの上で動作し、セレンを使用しています。ハーディは、特に既存のビルドプロセスに統合、 CSSのテストを始めるためにできるだけ簡単にできるように設計されています。


テストは、キュウリで書かれており、セレンを使用している。ハーディは、 Node.jsの上で動作するため、すべての例のCSSテストヘルパーはJSで書かれています。その背後にある機能は、簡単にあなたのテストでは、Java 、 Rubyや他の何かで書かれているかどうか、任意のテスト·セットアップで再利用することができます。

helpコマンド
--------------

helpコマンドは、とだけでなく、 hardycssregressionモジュールに含まれているオプションについての目的について、ユーザーをガイドします。また、 hardycssregressionモジュールをインストールするための構文について説明します。 hardycssregressionモジュールのhelpコマンドは、以下のように示されている。


.. code-block:: bash

	ptconfigure HardyCssRegression help

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure HardyCssRegression help
 ********************************************


  This command allows you to install HardyCssRegression from a GC Repo.

  Hardy

        - install
        Installs the latest GC Repo version of Hardy
        example: ptconfigure HardyCssRegression install

 ------------------------------
 End Help
 ******************************


インストール
----------------

端末上hardycssregressionモジュールをインストールするために使用されるコマンドは、以下に記載されている

.. code-block:: bash

	ptconfigure HardyCssRegression install

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash


 kevell@corp:/# ptconfigure HardyCssRegression install
 Install Hardy? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          HARDY !         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-87533646787.sh
 chmod 755 /tmp/ptconfigure-temp-script-87533646787.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-87533646787.sh Permissions
 Executing /tmp/ptconfigure-temp-script-87533646787.sh
 Cloning into 'Hardy'...
 remote: Counting objects: 949, done.
 remote: Total 949 (delta 0), reused 0 (delta 0), pack-reused 949
 Receiving objects: 100% (949/949), 41.55 MiB | 242.00 KiB/s, done.
 Resolving deltas: 100% (425/425), done.
 Checking connectivity... done.
 Temp File /tmp/ptconfigure-temp-script-87533646787.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Hardy: Success
 ------------------------------
 Installer Finished
 ******************************



メリット
-----------

あなたの視覚的なレイアウトとして頑丈であることを確認するテスト。
