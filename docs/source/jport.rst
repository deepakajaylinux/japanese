========
Port
========

あらすじ
-------------

ポートをポートおよびサービスの状態を確認する証明します。このモジュールは ptconfigure の下でポート サービスをチェックするのに役立ちます。このモジュールは、最も快適な Ubuntu で、セント OS。

ヘルプ
-------

このコマンドのヘルプガイド ポート モジュールに関するユーザー。これは、人々 のすべてのタイプに適しています。


.. code-block:: bash

          ptconfigure port help


ヘルプ コマンド ポート モジュールに組み込まれたコマンドの短いリストが表示されます。



.. code-block:: bash

	kevell@corp:/# ptconfigure Port  help
	******************************


	  This command allows you to test the status of ports and services running on them

	  Port, port

        - is-responding
        Test if a port is responding
        example: ptconfigure port is-responding --port-number="25"

        - process
        See which process is using a port
        example: ptconfigure port process --port-number="25"

	------------------------------
	End Help
	******************************


プロセス
---------

ユーザは、特定のポート、同じ下コマンド処理を使用しているプロセスを参照する必要がある場合。

.. code-block:: bash

	ptconfigure port process --port-number="25"

次のスクリーンショットは、上記のproceesを示している

.. code-block:: bash

 kevell@corp:/# ptconfigure port process --port-number="22"
 [Pharaoh Logging] Port 22 is being used by the process sshd
 *****************************
 Port Modifications:
 --------------------------------------------
 Port: Success
 ------------------------------
 Port Mods Finished
 ******************************



IS-応答
---------------

ユーザは、特定のポートは、以下のコマンド処理を、同じ応答されているかどうかをテストする必要がある場合。

.. code-block:: bash

	ptconfigure port process --port-number="25"


利点
-------------

* ユーザーは、ポートの現在の動作状態を確認できます。
* ユーザーフレンドリー モジュールです。
* より時間がかかる。

 

