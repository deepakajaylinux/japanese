===================
PharaohTools
===================

あらすじ
------------


ファラオ ツール モジュールは ptdeploy、pttest、Jrush、ptconfigure レポートを生成するをインストールするのに役立ちます。インストールの前に可用性を確保するためにユーザーを容易にします。モジュールが不足して具体的にインストールことができます。

ヘルプ コマンド
---------------

Help コマンドを作成する方法についてユーザーを導くこの特定のモジュールの ptconfigure の下で使用します。

それもこの特定のモジュールで実行することができますオプションを認識します。

スクリーン ショット以下のようには、help コマンドの使用法についての絵の表現を与えます。


.. code-block:: bash

 kevell@corp:/# ptconfigure PharaohTools help
 ******************************


  This command allows you to install the Pharaoh Tools which are ready. These include
  ptconfigure - this Configuration Management tool, ptdeploy - the Automated Deployment tool,
  and pttest, the test configuration and automation tool.

  PharaohTools, pharaohtools, pharaoh-tools

        - install
        Installs the latest version of all of the Pharaoh Tools
        example: ptconfigure pharaoh-tools install

 ------------------------------
 End Help
 ******************************

インストール
-------------

ファラオ ツール モジュールは、ptdeploy、pttest、Jrush のインストールを包んで、短いルートとして機能します。任意の 1 つの特定のモジュールは、3 つの中で不足している、追加の利点があるだけで特定のモジュールがインストールされます。確認プロセスはモジュールの可用性に関するデータを掴んで重要な役割を果たしています。

ファラオのツールの下のインストール プロセスに使用されるコマンドは下記します。


.. code-block:: bash

		ptconfigure pharaoh-tools install


.. cssclass:: table-bordered

 +-------------------------+---------------------------+--------------------------------------------------------------------------+
 | パラメーター            | 使用できる入力オプション  | コメント                                                                 |
 +=========================+===========================+==========================================================================+
 |Install Pharaoh Tools?   | Y(Yes)                    | ユーザーの願いは、インストールプロセスを続行する場合は、                 |
 |(Y/N)                    |                           | Yなどの入力をすることができます                                          |
 +-------------------------+---------------------------+--------------------------------------------------------------------------+
 |Install Pharaoh Tools?   | N(No)                     | ユーザーがインストールプロセスを終了したい場合は、Nを使用して簡単に終    |
 |(Y/N)                    |                           | 了することができます|                                                    |
 +-------------------------+---------------------------+--------------------------------------------------------------------------+
                                 

ファラオのインストール中に工具の行われる次の手順を実行します。


確保するため
-------------

* ファラオ ツールは利用可能なモジュールを確認します。
* うえで、それはバージョンについてチェックされません。

ptdeploy
-------------

* インストールすると、存在の場合、モジュール ptdeploy 自体報告します。
* それはまた ptdeploy モジュールのバージョンを確認します。
* ptdeploy モジュールがない場合、コンピューターで利用可能なその後自動的に ptdeploy は進歩をインストールします。


pttest
---------------

* 完了後 ptdeploy をインストールする、それは pttest モジュールを確認します。
* モジュール pttest 存在の場合、インストール自体を報告します。
* pttest モジュールがない場合、コンピューターで利用可能なその後自動的に pttest は進歩をインストールします。


Jrush
---------

* 完了後 pttest をインストールする、それは Jrush モジュールを確認します。
* モジュール Jrush 存在の場合、インストール自体を報告します。
* Jrush モジュールがない場合、コンピューターで利用可能なその後自動的に Jrush は進歩をインストールします。


3 つすべてのモジュールが既に存在する場合は、下のスクリーン ショットで与えられる例外的なメッセージ表示使用されます。



.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************


その他のオプション
-------------------

pttest、ptdeploy のインストール中に、次のオプションとして必要な Jrush ユーザーの入力を。私たちを見てみましょうは、以下のように彼らがしたい場合に、ユーザーが指定できる追加オプションは表形式で表されます。



.. cssclass:: table-bordered


 +-----------------------+--------------------------+----------------+--------------------------------------------------------------------+
 | パラメーター          | パス                     | オプション     | コメント                                                           |
 +=======================+==========================+================+====================================================================+
 |Program data           | “/opt/pttest             | Yes            | ユーザーがデフォルトのプログラムのデータディレクトリを使用し       |
 |directory (デフォルト) | (corresponding module)”  |                | てインストールを続行する場合、それらはYESと入力をすること          |
 |                       |                          |                | ができます                                                         |
 +-----------------------+--------------------------+----------------+--------------------------------------------------------------------+
 |Program data directory | User specific            | No(エンドス    | ユーザーが自分自身のプログラムデータディレクトリを続行し           |
 |                       |                          | ラッシュ)      | たい場合は、入力Nとして、そして手に、彼らは場所を所有指定す        |
 |                       |                          |                | ることができます                                                   |
 +-----------------------+--------------------------+----------------+--------------------------------------------------------------------+
 |Program executor       | “/usr/bin”               | Yes            | ユーザーがデフォルトのプログラム実行ディレクトリを使用し           |
 |directory (デフォルト) |                          |                | てインストールを続行する場合、それらはYESと入力をすることが        |
 |                       |                          |                | できます                                                           |
 +-----------------------+--------------------------+----------------+--------------------------------------------------------------------+
 |Program executor       | User specific            | No(エンドス    | ユーザーが独自のプログラム実行ディレクトリを続行したい場合は、     |  
 |directory              |                          | ラッシュ)      | 入力Nとして、そして手に、彼らは場所を所有指定することができます。| |
 +-----------------------+--------------------------+----------------+--------------------------------------------------------------------+


それをインストールするは、git のクローンの場所を指定する、受信デルタ、接続を解決するオブジェクトのオブジェクトの数を表示します。

次のスクリーン ショットについて説明しますをグラフィカルにファラオ ツールのインストールに関与するプロセス。

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************

利点
------------

* それはインストールの前に確保するためにユーザーを容易にします。
* ユーザーの任意の特定のモジュールが不足している場合にその特定のモジュールだけをインストールする進むことができます。
* ユーザーは、自分のパスまたは場所のプログラムのデータ ディレクトリと遺言執行者を指定できます。
* インストール ツールが既に例外メッセージがスローされますその後に、マシンで任意の特定のモジュールが既に存在する場合
  インストールされています。
* を回避するモジュールの不要な上書き、それ故にそれは時間を節約します。

 

