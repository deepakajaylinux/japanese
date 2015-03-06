==============
Phake
==============

あらすじ
-------------

Phake は PHP のモック作成用フレームワークです。予測可能で制御された方法で、実際のオブジェクトを模倣するオブジェクトを作成できます。テスト (SUT) の下でお使いのシステムによって外部メソッドの呼び出しからの入力の SUT を出力、SUT のちょうど別のフォームとして扱うことができます。これはテストに間接的な入力メソッドのスタブとテストから間接的な出力を受け取るメソッドへのパラメーターを検証することによって行われます。

ヘルプ コマンド
----------------------

このコマンドは、Phake モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
        
	        ptconfigure Phake help


 kevell@corp:/# ptconfigure Phake help
 ******************************


  This command allows you to install or update Phake.

  Phake, phake

        - install
        Installs the latest version of phake
        example: ptconfigure phake install

        - ensure
        Installs the latest version of phake, only if a version is not installed
        example: ptconfigure phake ensure

 ------------------------------
 End Help
 ******************************


インストール
----------------

ユーザーのマシンに Phake をインストールする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
         
   	        ptconfigure Phake install
 


システムを求める、ディレクトリ名、あなたのパスを設定したい場合はあなたのパスを定義できます。定義に続くパス '/' 記号。行われる変更がない場合は、Enter キーを押します。


"What is the program data directory? Found "/opt/phake" - use this?


システムを求める実行ディレクトリ名、あなたのパスを設定したい場合はあなたのパスを定義できます。定義に続くパス '/' 記号。行われる変更がない場合は、Enter キーを押します

"What is the program executer directory? Found "/usr/bin" - Use this? "


下のスクリーン ショットを示します。


.. code-block:: bash

 kevell@corp:/# ptconfigure Phake install
 Install Phake ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Phake         *
 *******************************
 What is the program data directory? Found "/opt/phake" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'http://github.com/jaz303/phake.git'  /tmp/phake/phakeCloning into '/tmp/phake/phake'...
 remote: Counting objects: 552, done.
 remote: Total 552 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (552/552), 91.36 KiB | 76.00 KiB/s, done.
 Resolving deltas: 100% (314/314), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Phake: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
-----------                               


.. cssclass:: table-bordered

 +------------------------+----------------------------------------------+----------------+---------------------------------------------+
 | パラメータ             | 代替パラメータ                               | オプション     | 注釈                                        |
 +========================+==============================================+================+=============================================+
 |ptconfigure Phake       | 2代替パラメータのいずれかがコマンド -        | Y              | ユーザがオプションを提供すると、            |
 |Install                 | で使用することができます Phake, phake        |                | システムはインストールプロセスを開始します  |
 |                        | eg: ptconfigure phake Install                |                |                                             |
 +------------------------+----------------------------------------------+----------------+---------------------------------------------+
 |ptconfigure Phake       | 2代替パラメータのいずれかがコマンド -        | N              | ユーザがオプションを提供すると、            |
 |Install                 | で使用することができます Phake, phake        |                | システムはインストールプロセスを停止します  |
 |                        | eg: ptconfigure phake Install|               |                |                                             |
 +------------------------+----------------------------------------------+----------------+---------------------------------------------+


利点
--------------

* Phake は、偉大なモック ライブラリと PHPUnit に簡単に統合することができます。
* プロトタイプ モックやスタブやスタブと検証フェーズ間の分離への新しいアプローチはとてもさわやかで簡単に
  使用します。
 

