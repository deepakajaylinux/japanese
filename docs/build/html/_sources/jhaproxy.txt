===========
HAProxy
===========


あらすじ
-------------

HAProxy はフリー、オープン ソースの高可用性ソリューションでは、TCP および HTTP ベースのアプリケーションの複数のサーバー要求を広めることで負荷分散とプロキシを提供することです。高速かつ (プロセッサとメモリの使用量） の面で効率的であるという評判をしています。

ヘルプ コマンド
----------------------

このコマンドは HAProxy モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドは、エンド ユーザー ガイドをいつ、どのように知っているに使用されるコマンドです。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure HAproxy help



上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure HAProxy help

 ******************************


  This module provides installs HA Proxy Server

  HAProxy, ha-proxy, haproxy

        - install
        Installs HA Proxy Server
        example: ptconfigure haproxy install

        - configure
        Configure Load Balancing with HA Proxy Server
        example: ptconfigure haproxy configure

 ------------------------------
 End Help
 ******************************




インストール
----------------

私たちのディストリビューションのパッケージ マネージャーを使用して HAProxy をインストールできます。とき、ユーザーはマシンで HAproxy モジュールをインストールする必要があります。特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
        
	        ptconfigure HAproxy install

上記のコマンドの絵の表現は以下します。



.. code-block:: bash

 
 kevell@corp:/# ptconfigure haproxy install
 Install HA Proxy Server? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!        *
 *******************************
 [Pharaoh Logging] Package haproxy from the Packager Apt is already installed, so not installing
 HA Proxy Init script config file /etc/default/haproxy added
 [Pharaoh Logging] Restarting haproxy service
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:25] : unknown keyword '1' in 'defaults' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:32] : unknown option 'tcp-check'.
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:34] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:35] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:36] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:37] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:38] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:39] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : Error(s) found in configuration file : /etc/haproxy/haproxy.cfg
 [ALERT] 041/154050 (17460) : Fatal errors found in configuration.
 * Restarting haproxy haproxy
   ...fail!
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HAProxy: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
-----------                               


.. cssclass:: table-bordered


 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
 | パラメーター                | 代替パラメーター                | オプション    | コメント                                         |
 +=============================+=================================+===============+==================================================+
 |ptconfigure HAProxy Install  | HAProxy , ha-proxy, haproxy     | Y(Yes)        | システムは、インストールプロセスを開始します     |
 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
 |ptconfigure HAProxy Install  | HAProxy , ha-proxy, haproxy     | N(No)         | システムは、インストール·プロセスを停止し、|     |
 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
      



構成
--------------------

このコマンドは HAproxy サーバーと分散負荷を構成するに役立ちます。一度、下特定のコマンドが実行されるシステムが提供する各セクションの既定値を任意に変更が行われる場合、ユーザー データを提供できます。


.. code-block:: bash

                ptconfigure HAproxy configure


上記のコマンドのスクリーン ショットは以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure haproxy configure

 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!        *
 *******************************
 
 What is the environment name you want to balance load to? 
 
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Warning:  Invalid argument supplied for foreach() in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 75
 Set non-default value for global_log? Default is 127.0.0.1 local0 notice (Y/N) 

 Set non-default value for global_maxconn? Default is 20000 (Y/N) 

 Set non-default value for global_user? Default is haproxy (Y/N) 

 Set non-default value for global_group? Default is haproxy (Y/N) 

 Set non-default value for defaults_log? Default is global (Y/N) 

 Set non-default value for defaults_mode? Default is http (Y/N) 

 Set non-default value for defaults_option_string? Default is option dontlognull
    option redispatch (Y/N) 

 Set non-default value for defaults_retries? Default is 3 (Y/N) 

 Set non-default value for defaults_timeout_connect? Default is 5000 (Y/N) 

 Set non-default value for defaults_timeout_client? Default is 10000 (Y/N) 

 Set non-default value for defaults_timeout_server? Default is 10000 (Y/N) 

 Set non-default value for listen_appname? Default is appname (Y/N) 

 Set non-default value for listen_ip_port? Default is 0.0.0.0:80 (Y/N) 

 Set non-default value for listen_mode? Default is http (Y/N) 

 Set non-default value for listen_balance? Default is roundrobin (Y/N) 

 Set non-default value for listen_option_string? Default is option httpclose
    option forwardfor (Y/N) 

 Set non-default value for listen_server_string? Default is  (Y/N) 

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HA Proxy Server: Success
 ------------------------------
 Installer Finished
 ******************************

利点
--------------

* すべてのアプリケーション 1 つの単一の ip アドレス経由でクラスターにアクセスします。HAProxy の背後に隠されたデータベース クラスターのトポロジ。
* それは、アプリケーションを変更せずにデータベース ノードを追加することが可能です。
* (MySQL にて) データベース接続の最大数に達すると、HAProxy キュー新しい接続を追加します。これは制限のきちんとした方法です。
  データベース接続を要求し、過負荷保護を実現します。
 
