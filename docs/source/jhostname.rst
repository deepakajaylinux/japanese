===========
Hostname
===========

あらすじ
---------------

IP アドレスではなく覚えにくいと特にわかりやすいではない）、以来、インターネットはまた番号文字列ではなく、名前でコンピューターを指定するユーザーをできます。この全体の文字列はコンピュ小胞体のホストとして知られている名前。2 つのオプションが利用できます。表示し、変更します。このモジュールを使用して、ユーザーが表示または、Host nameを変更できます。

ヘルプ コマンド
-----------------------

このコマンドは目標とHost nameのモジュールの下に利用可能なコマンドについて機能することができます。また、ホストの名前のモジュールを変更するコマンドについて説明します。Host nameを変更する前にユーザーを読むこのヘルプ コマンドはその機能について説明します。

.. code-block:: bash
         
                ptconfigure hostname help


次のスクリーン ショットはそれを気にさせることができます。



.. code-block:: bash

 kevell@corp:/# ptconfigure hostname help

 ******************************


  This command allows you to view or modify hostname

  Hostname, hostname

        - change
        Change the system hostname
        example: ptconfigure hostname change --hostname="my-laptop"

        - show
        Show the system hostname
        example: ptconfigure hostname show

 ------------------------------
 End Help
 ******************************



変更
----------------

Host name、管理能力で普通使用される、コンピューター ブラウザー リスト、アクティブ ディレクトリのリスト、IP アドレスをHost nameの解決、メール ヘッダーなどがあります。ユーザーがHost nameを変更する場合は、次のコマンドを使用できます。

.. code-block:: bash
           
                ptconfigure hostname change –hostname=”kevellcorp”

上記のコマンドから、新しいHost nameを入力できます。

.. code-block:: bash

 kevell@corp:/# ptconfigure hostname change –hostname=”kevellcorp”
 Enter Hostname:
 kevellcorp
 ******************************


 Hostname Modifications:
 --------------------------------------------

 Hostname: Success

 ------------------------------
 Hostname Mods Finished
 ******************************



ショー
-------------------

このモジュールは、Host name ptconfigure の下でちょうど、下記のコマンドを使用して表示する知覚プロセスです。


.. code-block:: bash
         
                ptconfigure hostname show

コマンド キーの後にHost nameが表示されます。

.. code-block:: bash

 kevell@corp:/# ptconfigure hostname show

 ******************************


 Hostname Modifications:
 --------------------------------------------

 Hostname: Success
 my-laptop


 ------------------------------
 Hostname Mods Finished
 ******************************


オプション
------------

.. cssclass:: table-bordered


 +------------------------------+----------------------------------+-------------+-------------------------------------------------------+
 | パラメーター                 | 代替パラメーター                 | オプション  | コメント                                              |
 +==============================+==================================+=============+=======================================================+
 |ptconfigure hostname          | Hostnameではなく、               | Show        | システムはptconfigure下hostnameプロセスを示す始める   |
 |                              | 我々は使用することができます     |             |                                                       |
 |                              | hostname                         |             |                                                       |
 +------------------------------+----------------------------------+-------------+-------------------------------------------------------+
 |ptconfigure hostname change   | Hostnameではなく、               | Change      | システムはptconfigure下hostname 変更処理を開始する    |
 |–hostname=”Name”              | 我々は使用することができます     |             |                                                       |
 |                              | hostname|                        |             |                                                       |
 +------------------------------+----------------------------------+-------------+-------------------------------------------------------+


利点
-------------

* Host name 1 つの単語または語句から成る簡易名または構造化される可能性があります。
* Host nameを区別することができます。
* Host nameは簡単に修正および表示できます。
 

