==========
Ping
==========

あらすじ
-----------

動詞として、PING「の注意を引く"または」の有無のチェック」を意味する別のパーティー オンライン。PING (パケット インターネット痴漢） モジュール システムへの接続をテストするために使用します。ネットワーク データを送受信するネットワーク データはネットワーク上の別のコンピューターから PING を使用します。PING は、頻繁に別のシステムは、ネットワーク経由で到達可能かどうかをテストするために使用し、もしそうなら、どのくらいかかる時間そのデータを交換するため。

ヘルプ コマンド
------------------

このコマンドは、PING モジュールの使用状況を判断するのに役立ちます。このヘルプ コマンド図 PING コマンドと共に使用するためのオプションを。このコマンドは、エンドユーザーのさまざまなオプションの使用方法とそれらのオプションの構文を知っているをご案内いたします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

	ptconfigure ping help

 kevell@corp:/# ptconfigure ping help

 ******************************


  This command allows you to test the status of ports

  Ping, ping

        - once
        ping a target once
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - ten
        ping a target ten times
        example: ptconfigure ping ten --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - until-responding
        ping a target for a set amount of time until it responds
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2
            --max-wait=100 # no seconds in total to keep trying, will guess 60

 ------------------------------
 End Help
 ******************************



オプション
-----------

モジュールの PING コマンドで使用されるオプションに従ってデータを取得する 3 つの異なるオプションがあります。テーブルの下に同じについて説明します

.. cssclass:: table-bordered

 +--------------+-------------------------------------------------------+----------------------------------------------------------------+
 | オプション   | コマンド                                              | 関数                                                           |
 +==============+=======================================================+================================================================+
 |Once          | ptconfigure ping once – yes –guess –target=           | 一度私たちにターゲットをping。オプションは、一度だけデータを   | 
 |              | google.com – interval=5                               | 取得したら、                                                   |
 +--------------+-------------------------------------------------------+----------------------------------------------------------------+
 |Ten           | ptconfigure ping ten – yes –guess –target=            | 10回のための10のオプションプルデータ、5秒と間隔時間を持つ      |
 |              | google.com – interval=5                               | [秒間待機し、次のパケットを送信する前に]                       |
 +--------------+-------------------------------------------------------+----------------------------------------------------------------+
 |Until-        | ptconfigure ping once – yes –guess until –target=     | 目標のために試して5と最大100秒としてインターバル時間を過       |
 |responding    | google.com – interval=5 seconds – max-wait=100        | ごして、それが応答時間の設定された量のために私たちにター       |
 |              |                                                       | ゲットをping|                                                  |
 +--------------+-------------------------------------------------------+----------------------------------------------------------------+


注:

* 間隔の各要求間で待機する秒数

* 最大待機 - の合計を維持しようとする秒数

* 間隔の時間と最大待機時間周波数を要件に従ってユーザーによって決定することができます。



一度オプション
---------------


.. code-block:: bash

 kevell@corp:/# ptconfigure ping once --yes --guess --target=www.google.com

 [Pharaoh Logging] Ping Latency is 34 ms
 ******************************


 Ping Modifications:
 --------------------------------------------
 
 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


10 のオプション
------------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping ten --yes --guess --target=www.google.com 

 [Pharaoh Logging] Ping Latency is 36 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 36 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************

応答まで
-----------------


.. code-block:: bash

 kevell@corp:/# ptconfigure ping once -- yes --guess --target=google.com -- interval=5 -- max-wait=100

 [Pharaoh Logging] Ping Latency is 37 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************


利点
------------


PING は、特定の IP アドレスの存在を確認するユーザーを支援するし、要求を受け入れることができます。PING コマンドは、2 つのノード間の接続をテストする最良の方法です。それがローカル エリア ネットワーク (LAN) またはワイド エリア ネットワーク (WAN) かどうか。

 

