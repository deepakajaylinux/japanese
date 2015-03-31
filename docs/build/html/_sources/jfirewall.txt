===========
Firewall
===========

あらすじ
---------

ファイアウォールは、ネットワークのセキュリティ システム、適用されているルールのセットに基づいて着信および発信のネットワーク トラフィックを制御します。ファイアウォールは、ソフトウェア ソリューションとハードウェア ・ アプライアンスの両方に存在します。

ヘルプ コマンド
----------------

このヘルプ コマンド アシスト ptconfigureについてユーザー。ユーザーのアクセス許可をについて説明します。
ユーザーの願いに従って変更を行うことができます。ヘルプ イメージを案内します。それを視覚化しよう。

.. code-block:: bash

  ptconfigure Firewall help

上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure Firewall help
 ******************************
 This command allows you to modify create or modify firewalls

  Firewall, firewall

        - enable
        Enable system firewall
        example: ptconfigure firewall enable

        - disable
        Disable system firewall
        example: ptconfigure firewall disable

        - allow
        Allow a Firewall rule
        example: ptconfigure firewall allow --firewall-rule="ssh/tcp"

        - deny
        Deny a Firewall rule. Allow connection attempts to be ignored and time out.
        example: ptconfigure firewall deny --firewall-rule="ssh/tcp"

        - reject
        Reject a Firewall rule. Terminate connections attempts with an error to the connector.
        example: ptconfigure firewall reject --firewall-rule="ssh/tcp"

        - limit
        Limit a Firewall rule. ufw will deny connections if an IP address has attempted
        to initiate 6 or more connections in the last 30 seconds.
        example: ptconfigure firewall limit --firewall-rule="ssh/tcp"

        - delete
        Delete a Firewall rule.
        example: ptconfigure firewall delete --firewall-rule="ssh/tcp"

        - insert
        Insert a Firewall rule.
        example: ptconfigure firewall insert --firewall-rule="ssh/tcp"

        - reset
        Reset a Firewall rule.
        example: ptconfigure firewall reset --firewall-rule="ssh/tcp"

        - default
        Set default policy, should be allow, deny, or reject
        example: ptconfigure firewall default --policy="deny"

 ------------------------------
 End Help
 ******************************



オプション
------------

ファイアウォール規則は、あなたのニーズ、要件とセキュリティ脅威のレベルに従ってカスタマイズできます。ユーザーを作成したり、ファイアウォール ルールとしてそのような条件に基づいて無効にします。


.. cssclass:: table-bordered


 +----------------+-------------------------------------------------------------+----------------------------------------+
 | パラメーター   | 関数                                                        | コマンド                               |
 +================+=============================================================+========================================+
 |IP address      | あなたが思う捕食され、特定のIPアドレスまたはIPアドレスの    |                                        |
 |                | 範囲を、遮断する                                            |                                        |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Enable          | システムのファイアウォールを有効にする                      | ptconfigure firewall enable            |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Disable         | 無効にするシステムのファイアウォール                        | ptconfigure firewall disable           |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Allow           | ファイアウォールルールを許可する                            | ptconfigure firewall allow –firewall-  |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Deny            | 許可接続の試行は無視されるとアウト時間                      | ptconfigure firewall deny –firewall-   |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Reject          | コネクタへのエラーで接続試行を終了                          | ptconfigure firewall reject –firewall- |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Limit           | IPアドレスが6を開始するか、最後の30秒以上の接続しようとし   | ptconfigure firewall limit –firewall-  |
 |                | た場合、UFWは接続を拒否します。                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Delete          | ファイアウォールルールを削除                                | ptconfigure firewall delete –firewall- |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Insert          | ファイアウォールルールを挿入します                          | ptconfigure firewall insert –firewall- |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Reset           | ファイアウォールルールをリセット                            | ptconfigure firewall reset –firewall-  |
 |                |                                                             | rule=”ssh/tcp”                         |
 +----------------+-------------------------------------------------------------+----------------------------------------+
 |Default         | デフォルトポリシーは、拒否または拒否、許可するべきである.   | ptconfigure firewall default – policy  |
 |                |                                                             | =”deny”|                               |
 +----------------+-------------------------------------------------------------+----------------------------------------+


コマンドの絵図には、許可、拒否、拒否してリセットを以下にリストされている



.. code-block:: bash

 kevell@corp:/# ptconfigure firewall enable 


 Firewall is active and enabled on system startup 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 

 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall disable 


 Firewall stopped and disabled on system startup 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 

 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptconfigure firewall allow --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall deny --firewall-rule="ssh/tcp"


 Skipping adding existing rule
 Skipping adding existing rule (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reject --firewall-rule="ssh/tcp"

 Rules updated
 Rules updated (v6)
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure firewall reset --firewall-rule="ssh/tcp"

 Resetting all rules to installed defaults. Proceed with operation (y|n)? Backing up 'user.rules' to '/lib/ufw/user.rules.20150324_190113'
 Backing up 'after.rules' to '/etc/ufw/after.rules.20150324_190113'
 Backing up 'after6.rules' to '/etc/ufw/after6.rules.20150324_190113'
 Backing up 'before6.rules' to '/etc/ufw/before6.rules.20150324_190113'
 Backing up 'user6.rules' to '/lib/ufw/user6.rules.20150324_190113'
 Backing up 'before.rules' to '/etc/ufw/before.rules.20150324_190113'
 
 ******************************


 Firewall Modifications:
 --------------------------------------------

 Firewall: Success

 ------------------------------
 Firewall Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure firewall limit --firewall-rule="1" 


 Rules updated 
 Rules updated (v6) 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 

 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptconfigure firewall delete --firewall-rule="1" 


 Rules updated 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 

 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptconfigure firewall insert --RowNum="1" --firewall-rule="ssh" 

 Rules updated 
 Rules updated (v6) 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 
 
 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptconfigure firewall default --policy="deny" 


 [Pharaoh Logging] Policy param for set default must be allow, deny or reject 
 Default incoming policy changed to 'deny' 
 (be sure to update your rules accordingly) 
 ****************************** 


 Firewall Modifications: 
 -------------------------------------------- 

 Firewall: Success 

 ------------------------------ 
 Firewall Mods Finished 
 ******************************



利点
------------

* ファイアウォール アクセスできなくなります不要なシステムにネットワーク接続を介して識別し、危険なポートを介した通信を防止します。
* システムが多くの異なる認識ポートを介した通信やファイアウォールはこれらを求めるか、ユーザーに警告せずに許可する傾向があります。
* ファイアウォールも、外からの「疑わしい」活動をを検出できます。 します
* ユーザーは彼らの願いによると自分のルールを設定できます。

