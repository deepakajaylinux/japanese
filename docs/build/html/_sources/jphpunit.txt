==========
PHP Unit
==========

あらすじ
--------------

このモジュールは PHPUnit GC レポからインストールするユーザーを容易にします。PHP 単体テスト フレームワークは、単体テスト フレームワーク開発者のバグを発見し、順番に PHP ソフトウェアの開発に関連付けられているコストを削減することが可能です。PHP 単体テスト フレームワークは、XML、XHTML、または ASCII でレポートを生成します。このモジュールにより PHP ユニットをインストールするのにはどのように見てみましょう。

ヘルプ コマンド
--------------------

ヘルプ コマンド同様目的に関してユーザーを導くように PHP ユニット モジュールに含まれているオプションについて。また、PHP ユニットをインストールするための構文について説明します。PHP 単位モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		ptconfigure PHPUnit help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、PHP の単位の下のヘルプ コマンドについて視覚化します。




.. code-block:: bash

 kevell@corp:/# ptconfigure PHPUnit help
 ******************************

  This command allows you to install PHPUnit from a GC Repo.

  PHPUnit

        - install
        Installs the latest GC Repo version of PHPUnit
        example: ptconfigure phpunit install

 ------------------------------
 End Help
 ******************************

インストール
---------------

PHP ユニット、ユーザーのコンピューターにインストールするために使用するコマンドを次に示します。


.. code-block:: bash

		ptconfigure PHPUnit install

上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +------------------------+---------------+-------------------------------------------------------------------------------------+
 | パラメーター           | オプション    | コメント                                                                            |
 +========================+===============+=====================================================================================+
 |Install PHP Unit? (Y/N) | Y(Yes)        | ユーザーは、Yと入力することができ、インストールプロセスを続行したい場合             |
 +------------------------+---------------+-------------------------------------------------------------------------------------+
 |Install PHP Unit? (Y/N) | N(No)         | ユーザーは、Nと入力することができ、インストールプロセスを終了したい場合は|          |
 +------------------------+---------------+-------------------------------------------------------------------------------------+



ユーザー インストール プロセスの進行を表形式で示すように、次の操作が発生します。

.. cssclass:: table-bordered

 +------------------------+-----------------------+-------------------+--------------------------------------------------------------+
 | パラメーター           | パス                  | オプション        | コメント                                                     |
 +========================+=======================+===================+==============================================================+
 |Program data directory  | “/opt/phpunit (対応   | Yes               | ユーザーがデフォルトのプログラムのデータディレクトリを使用   |
 |                        | するモジュール)”      |                   | してインストールを続行する場合、それらはYESと入力をするこ    |
 |                        |                       |                   | とができます                                                 |
 +------------------------+-----------------------+-------------------+--------------------------------------------------------------+
 |Program data directory  | User specific         | No(エンドスラ     | ユーザーが自分自身のプログラムデータディレクトリを続行し     |
 |                        |                       | ッシュ)           | たい場合は、Nとして、手入力は、自分の場所を指定することが    |
 |                        |                       |                   | できます                                                     |
 +------------------------+-----------------------+-------------------+--------------------------------------------------------------+
 |Program executor        | “/usr/bin”            | Yes               | ユーザーがデフォルトのプログラム実行ディレクトリを使用       |
 |directory (デフォルト)  |                       |                   | してインストールを続行する場合、それらはYESと                |
 |                        |                       |                   | 入力をすることができます                                     |
 +------------------------+-----------------------+-------------------+--------------------------------------------------------------+
 |Program executor        | User specific         | No(エンドスラ     | ユーザーが独自のプログラム実行ディレクトリを続行したい場     |
 |directory               |                       | ッシュ)           | 合は、入力Nとして、そして手に、彼らは場所を所有指定          |
 |                        |                       |                   | することができます。|                                        |
 +------------------------+-----------------------+-------------------+--------------------------------------------------------------+


最後に、PHP ユニットのインストールを完了します。次のスクリーン ショットは、インストールのプロセスについて視覚的に示しています。



.. code-block:: bash

 kevell@corp:/# ptconfigure phpunit install
 Install PHP Unit ? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          PHP Unit !         *
 *******************************
 What is the program data directory? Found "/opt/phpunit" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone -b 3.5 'https://github.com/sebastianbergmann/phpunit.git'  /tmp/phpunit/phpunitCloning into '/tmp/phpunit/phpunit'...

 remote: Counting objects: 50529, done.
 Receiving objects:  71% (35876/50529), 12.02 MiB | 41.00 KiB/s
 Receiving objects:  95% (48003/50529), 16.82 MiB | 38.00 KiB/s
 Receiving objects:  95% (48254/50529), 16.86 MiB | 40.00 KiB/s
 Receiving objects:  96% (48508/50529), 16.95 MiB | 43.00 KiB/s



 remote: Total 50529 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (50529/50529), 17.91 MiB | 36.00 KiB/s, done.
 Resolving deltas: 100% (26834/26834), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/dbunit.git'  /tmp/phpunit/dbunitCloning into '/tmp/phpunit/dbunit'...
 remote: Counting objects: 4596, done.
 remote: Total 4596 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4596/4596), 1.04 MiB | 31.00 KiB/s, done.
 Resolving deltas: 100% (3183/3183), done.
 Checking connectivity... done.
 git clone -b 1.2 'https://github.com/sebastianbergmann/php-file-iterator.git'  /tmp/phpunit/php-file-iteratorCloning into '/tmp/phpunit/php-file-iterator'...
 remote: Counting objects: 453, done.
 remote: Total 453 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (453/453), 60.66 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (188/188), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-code-coverage.git'  /tmp/phpunit/php-code-coverageCloning into '/tmp/phpunit/php-code-coverage'...
 remote: Counting objects: 7650, done.
 remote: Total 7650 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (7650/7650), 2.77 MiB | 17.00 KiB/s, done.
 Resolving deltas: 100% (3671/3671), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-token-stream.git'  /tmp/phpunit/php-token-streamCloning into '/tmp/phpunit/php-token-stream'...
 remote: Counting objects: 1234, done.
 remote: Total 1234 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1234/1234), 201.76 KiB | 41.00 KiB/s, done.
 Resolving deltas: 100% (565/565), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-mock-objects.git'  /tmp/phpunit/phpunit-mock-objectsCloning into '/tmp/phpunit/phpunit-mock-objects'...
 remote: Counting objects: 4703, done.
 remote: Total 4703 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4703/4703), 837.24 KiB | 104.00 KiB/s, done.
 Resolving deltas: 100% (2910/2910), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-selenium.git'  /tmp/phpunit/phpunit-seleniumCloning into '/tmp/phpunit/phpunit-selenium'...
 remote: Counting objects: 8115, done.
 remote: Total 8115 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (8115/8115), 2.07 MiB | 28.00 KiB/s, done.
 Resolving deltas: 100% (4762/4762), done.
 Checking connectivity... done.
 git clone 'https://github.com/phpengine/ptconfigure-phpunit-php-timer'  /tmp/phpunit/php-timerCloning into '/tmp/phpunit/php-timer'...
 remote: Counting objects: 253, done.
 remote: Total 253 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (253/253), 31.55 KiB | 12.00 KiB/s, done.
 Resolving deltas: 100% (126/126), done.
 Checking connectivity... done.
 git clone 'https://github.com/sebastianbergmann/php-text-template.git'  /tmp/phpunit/php-text-templateCloning into '/tmp/phpunit/php-text-template'...
 remote: Counting objects: 209, done.
 remote: Total 209 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (209/209), 33.69 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (92/92), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPUnit35: Success
 ------------------------------
 Installer Finished
 ******************************

利点
------------

* このモジュール レポ バージョンから PHP ユニットをインストールするユーザーを容易にします。
* ユーザーは、プログラムのデータ ディレクトリと遺言執行者のための独自のパスを選択できます。
* ヘルプとインストールの宣言で使用されるパラメーターは大文字と小文字を区別しながら他の人に比べての利点を追加する必要があります。
* それは裕福な両方セント OS とも ubuntu のように。
 

