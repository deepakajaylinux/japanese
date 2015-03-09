======
Xvfb
======

あらすじ
------------

このモジュールは、人気の高いバーチャル マシン ソリューションとして知られている xvfb をインストールするのに容易にします。モジュールは、仮想マシンで作業するため、ソリューションを提供します。仮想フレームバッファー X として知られている xvfb は X 11 表示サーバー プロトコルを実装するディスプレイ サーバーです。表示の他のサーバーと対照をなして Xvfb 操作を実行しますすべてグラフィカル メモリに任意の画面の出力を表示せず。私たちを見てみましょう、どのようにこのモジュール xvfb apt-get 経由でインストールするのに役立ちます。

ヘルプ コマンド
--------------------

Help コマンドと同様、目的に関するユーザー ガイドとして xvfb モジュールに含まれているオプションについて。ヘルプ コマンド xvfb モジュールの代替パラメーターが一覧表示されます。それはまた xvfb モジュールを示しています xvfb モジュール ヘルプ コマンドをインストールするための構文について説明します以下の通りです。

.. code-block:: bash

		ptconfigure Xvfb help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、xvfb モジュールの下に、help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure Xvfb help
 ******************************


  This command allows you to install Xvfb, the popular Virtual Machine Solution.

  Xvfb, xvfb

        - install
        Installs Xvfb through apt-get
        example: ptconfigure xvfb install

 ------------------------------
 End Help
 ******************************



インストール
----------------

ユーザーのコンピューターに、xvfb をインストールするために使用されるコマンドを次に示します。


.. code-block:: bash

		ptconfigure xvfb install

上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +----------------------+-------------------------+---------------+--------------------------------------------------+
 | パラメーター         | 代替パラメーター        | オプション    | コメント                                         |
 +======================+=========================+===============+==================================================+
 |Install Xvfb? (Y/N)   | Xvfb, xvfb              | Y(Yes)        | ユーザーは、Yと入力することができ、              |
 |                      |                         |               | インストールプロセスを続行したい場合             |
 +----------------------+-------------------------+---------------+--------------------------------------------------+
 |Install Xvfb? (Y/N)   | Xvfb, xvfb              | N(No)         | ユーザーは、Nと入力することができ、              |
 |                      |                         |               | インストールプロセスを終了したい場合は|          |
 +----------------------+-------------------------+---------------+--------------------------------------------------+
             

インストール プロセスを続行すると、インストールの実行中に、次のプロセスが発生します。

* 読み取りパッケージのリスト。
* 依存関係ツリーを構築します。
* 読み取り状態情報。
* インストールされている新しいパッケージのリスト。
* アップグレード ファイルの数、新しくインストールされた、削除された、ないアップグレード。

最後に、ステータスが明確に報告され、Apt パッケージ xvfb を追加する、パッケー ジャーから正しく実行されます。次のスクリーン ショットは、xvfb をインストールするプロセスについて示しています。

Xvfb モジュールがユーザーのコンピューターに既に存在する場合に、Apt が既にインストールされているパッケー ジャーからパッケージ xvfb として、メッセージが表示されます。スクリーン ショットを次のようにメッセージのこれらのタイプの良い例です。



.. code-block:: bash

 kevell@corp:/# ptconfigure xvfb install
 Install Xvfb? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! Xvfb !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  xvfb
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 747 kB of archives.
 After this operation, 2,191 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main xvfb amd64 2:1.15.1-0ubuntu2.6 [747 kB]
 Fetched 747 kB in 36s (20.6 kB/s)
 Selecting previously unselected package xvfb.
 (Reading database ... 211203 files and directories currently installed.)
 Preparing to unpack .../xvfb_2%3a1.15.1-0ubuntu2.6_amd64.deb ...
 Unpacking xvfb (2:1.15.1-0ubuntu2.6) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xvfb (2:1.15.1-0ubuntu2.6) ...
 [Pharaoh Logging] Adding Package xvfb from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xvfb: Success
 ------------------------------
 Installer Finished
 ******************************


利点
-----------

* ヘルプ コマンドを宣言するために使用されるパラメーター、インストールしない大文字と小文字は他と比較される間、加えられた利点であります。
* それは裕福な両方セント OS とも Ubuntu のように。
* 場合 xvfb パッケージをユーザーのコンピューターに存在上書きされません、代わりにそのメッセージが既に存在すると表示されます。

Xvfb は主にテストに使用されます。

* 実際のコードが共有する以来 X サーバは、特定のハードウェアに関係のないコードの部分をテストするために使用することができます。
* それはそれ以外の場合、別のハードウェアの範囲を必要とする様々 な条件でクライアントをテストする使用ことができます。たとえば、
  することができます。クライアントの深さまたはほとんどのハードウェアでサポートされている画面サイズで正しく動作するかどうかをテストする使用します。
* バック グラウンド実行中のクライアントの。(xwd プログラムまたはスクリーン ショットをキャプチャするための同様のプログラム使用できます実際に結果   を見る)
* 実行中のプログラムを使用しない場合でも、アクティブにする X サーバを必要とします。（例： クローバー html レポート）
 

