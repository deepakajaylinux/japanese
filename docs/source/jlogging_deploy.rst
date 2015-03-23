========
Logging
========

概要
-----------

このロギングモジュールは、コンソールにメッセージを記録する目的で使用され、必要に応じてPHPのエラーログのために使用される。私たちはインストールすると、メッセージを宣言し、PHPのエラー·ログにログを使用する方法を見てみましょう。

helpコマンド
--------------------

helpコマンドは、その使用方法や方法論についてのユーザーを導く簡単なユーザーマニュアルとして機能します。これは、ログを定義するための宣言、および構文の例で使用することができる別のパラメータを指定する。ヘルプオプションを宣言するために使用するコマンドは以下のとおりである：

.. code-block:: bash

	ptdeploy Logging help

以下のスクリーンショットは、helpコマンドの操作方法の絵で示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy Logging help
 ******************************


  Use this to log a message to the Console, and optionally the php error log.

  Logging, logging

        - log
        Logs a message the console or
        example: ptdeploy logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************

インストール
---------------

ptdeployの下でログをインストールするために使用するコマンドは以下のとおりである：

.. code-block:: bash

	ptdeploy logging log

入力後、上記のコマンドは、インストールプロセスは、次の表の列に示されている。

.. cssclass:: table-bordered

 +------------------------+----------------------+-------------+--------------------------------------------------------------------+
 | パラメーター           | 代替パラメータ       | オプション  | コメント                                                           |
 +========================+======================+=============+====================================================================+
 |Install Logging? (Y/N)  | Logging, logging     | Y(Yes)      | ユーザーは、Yと入力することができ、インストールプロセスを          |
 |                        |                      |             | 続行したい場合                                                     |
 +------------------------+----------------------+-------------+--------------------------------------------------------------------+
 |Install Logging? (Y/N)  | Logging, logging     | N(No)       | ユーザーは、Nと入力することができ、インストールプロセスを終        |
 |                        |                      |             | 了したい場合は|                                                    |
 +------------------------+----------------------+-------------+--------------------------------------------------------------------+
 

ユーザは、インストール処理を進めた場合、処理は尋ねることによって、ログメッセージを指定するようユーザに要求する


.. code-block:: bash

	"Enter Log Message"
	
	"Good Morning"

示されるように、ユーザ入力メッセージと、所与のログメッセージが画面に表示される。

"Good Morning"

最後に、インストールが完了されます。次のスクリーンショットは、絵でインストールのプロセスを示している。

.. code-block:: bash

 kevell@corp:/#  ptdeploy logging log
 Install Logging? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 No Data.

 ------------------------------
 Installer Finished

PHPのエラーログを定義する方法
-------------------------------------

PHPのエラーログのログを宣言するための構文は次のようになります。

.. code-block:: bash

	ptconfigure logging log --php- log --log-message="Here is something logging to the console and error log"

の代わりに

.. code-block:: bash

 	log-message="Here is something logging to the console and error log"

ユーザーは彼らの要求に応じて、ログメッセージの一部に任意のテキストを追加することができます。

.. code-block:: bash

 kevell@corp:/# ptdeploy logging log --php-log --log-message="Here is something logging to the console and error log" 

 Install Logging? (Y/N) 
 y 
 ******************************* 
 *   Golden Contact Computing  * 
 *           Logging!          * 
 ******************************* 
 [Pharaoh Logging] Here is something logging to the console and error log 
 [Pharaoh Logging] Here is something logging to the console and error log 

 ... All done! 
 ******************************* 
 Thanks for installing , visit www.gcsoftshop.co.uk for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 

 No Data. 

 ------------------------------ 
 Installer Finished 
 *********************** 




メリット
-----------

* ユーザーは、PHPのエラーログのために彼らの頻繁に使用されるログメッセージを追加することができます。
* ユーザが入力することができ、ログメッセージの表示を保証するログのインストール中。
* これは、セントのOSのように裕福な両方のUbuntuで、同様である。
* 宣言で使用されるパラメータは、大文字と小文字を区別しません。
