==========
Service
==========


あらすじ
----------
          
このモジュールは、システム ファイルの現在の状態を促進します。それとしてかどうかを実行している状態を言及することができます。自動化が可能です。このモジュールでは、環境の構成を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
------------------

Help コマンドは、指定されたコマンドに関する情報を見つけるために使用します。サービスの機能の変更についてこのヘルプ コマンドを使用できます。次のスクリーン ショットは、あなたをご案内いたします。


.. code-block:: bash

    ptconfigure Service help


.. code-block:: bash

	Kevell@corp:/# ptconfigure Service help

	******************************


	  This command allows you to view or modify service

	  Service, service

        - start
        Start a system service
        example: ptconfigure service start --service-name="apache2"

        - stop
        Stop a system service
        example: ptconfigure service restart --service-name="apache2"

        - restart
        Restart a system service
        example: ptconfigure service restart --service-name="apache2"

        - ensure-running
        Ensure a system service is running. If it is already running, dont attempt to start it
        If it is not running, start it
        example: ptconfigure service ensure-running --service-name="apache2"

        - is-running
        Checks whether a system service is running.
        example: ptconfigure service is-running --service-name="apache2"

        - run-at-reboots
        Ensure a system service will auto start on reboots.
        example: ptconfigure service run-at-reboots --service-name="apache2"

	------------------------------
	End Help
	******************************


オプション
------------


.. cssclass:: table-bordered

 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 | パラメータ   | 代替パラメータ    | 関数                                             | コメント                                          |
 +==============+===================+==================================================+===================================================+
 |start         | Service, service  | システムサービスを開始します                     | ptconfigure service start –service-               |
 |              |                   |                                                  | name=”apache2”                                    |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 |stop          | Service, service  | システムサービスを停止します                     | ptconfigure service stop –service-name=”apache2”  |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 |Restart       | Service, service  | システムサービスを再起動します                   | ptconfigure service restart –service-             |
 |              |                   |                                                  | name=”apache2”                                    |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 |Ensure-       | Service, service  | サービスが実行されていない場合をrunning.Inされ   | ptconfigure service ensure-running –service-      |
 |running       |                   | ているシステムを確認しようとしない。             | name=”apache2”                                    |
 |              |                   | それ以外を開始                                   |                                                   |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 |Is-running    | Service, service  | システムサービスが実行中かしないでください。     | ptconfigure service is-running –service-name      |
 |              |                   | それ以外を開始実行されていないかどうかを確認     | =”apache2”                                        |
 |              |                   | してください                                     |                                                   |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+
 |Run-at-       | Service, service  | 再起動後にシステムサービスの自動起動を確認し     | ptconfigure service run-at-reboots –service-      |
 |reboots       |                   | てください                                       | name=”apache2|                                    |
 +--------------+-------------------+--------------------------------------------------+---------------------------------------------------+


コマンド開始の絵画represenation 、停止、再起動、確認ランニング、 -実行中で、ラン·アット·再起動後、以下に記載されています、コマンド開始の絵画represenation 、停止、再起動、確認ランニング、 -実行中で、ラン·アット·再起動後、以下に記載されています、

.. code-block:: bash

 kevell@corp:/# ptconfigure service start --service-name="apache2"

 [Pharaoh Logging] Starting apache2 service
 * Starting web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure service stop --service-name="apache2"

 [Pharaoh Logging] Stopping apache2 service
 * Stopping web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure service restart --service-name="apache2"

 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure service ensure-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service is-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service run-at-reboots --service-name="apache2"

 [Pharaoh Logging] Removing current apache2 service startup links
 Removing any system startup links for /etc/init.d/apache2 ...
   /etc/rc0.d/K09apache2
   /etc/rc1.d/K09apache2
   /etc/rc2.d/S91apache2
   /etc/rc3.d/S91apache2
   /etc/rc4.d/S91apache2
   /etc/rc5.d/S91apache2
   /etc/rc6.d/K09apache2
 [Pharaoh Logging] Adding apache2 service startup links
 Adding system startup for /etc/init.d/apache2 ...
   /etc/rc0.d/K20apache2 -> ../init.d/apache2
   /etc/rc1.d/K20apache2 -> ../init.d/apache2
   /etc/rc6.d/K20apache2 -> ../init.d/apache2
   /etc/rc2.d/S20apache2 -> ../init.d/apache2
   /etc/rc3.d/S20apache2 -> ../init.d/apache2
   /etc/rc4.d/S20apache2 -> ../init.d/apache2
   /etc/rc5.d/S20apache2 -> ../init.d/apache2
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************




代替パラメーター
-------------------

2代替パラメータがあります。 Service, service

利点
---------

* ユーザーは、いつでもシステムの動作状態を確認できます。
* サービスは、システム間でデータ交換を提供します。
* それは、マシンのリソースの共有を許可します。
* サービスは、バックアップの機能も提供します。
* サービスは、柔軟なネットワーク環境を提供します。
* これは分散データの調整を含みます。


