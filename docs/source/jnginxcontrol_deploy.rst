===============
Nginx Control
===============

概要
-------------

nginxの（発音は「エンジン-X」）は、HTTP、HTTPS、SMTP、POP3、IMAPプロトコルのほか、ロードバランサ、HTTPキャッシュ、およびWebサーバ（オリジンサーバ）のためのオープンソースのリバースプロキシサーバーです。 nginxのプロジェクトは、高同時実行、高性能と低メモリ使用量に重点を始めています。それは、2節のBSDライクなライセンスの下でライセンスされて、それは、Linux、BSDの変種やMac OS X、Solaris版、AIX、HP-UX上だけでなく、他のnixのフレーバーで実行されます。

nginxのではなく、そのイベントMPMは、非同期処理のために必要とされるスレッド化またはプロセス指向のアプローチ、デフォルトのApache HTTPサーバモデルの、要求を処理する非同期イベント駆動型のアプローチを使用しています。 nginxののモジュラーイベント駆動型アーキテクチャは、高負荷の下で、より予測可能な性能を提供することができる。

helpコマンド
----------------------

このコマンドは、nginxのモジュールの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行するためのさまざまな方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash
	
	ptdeploy nginxcontrol help
       
 kevell@corp:/# ptdeploy NginxControl help
 ******************************


  This command is part of Default Modules and handles Nginx Server Control Functions.

  NginxControl, nginxcontrol, nginxctl

          - start
          Start the Nginx server
          example: ptdeploy nginxcontrol start

          - stop
          Stop the Nginx server
          example: ptdeploy nginxcontrol stop

          - restart
          Restart the Nginx server
          example: ptdeploy nginxcontrol restart

          - reload
          Reloads the Nginx server configuration without restarting
          example: ptdeploy nginxcontrol reload

 ------------------------------
 End Help
 ******************************

スタート
----------------

ユーザーはnginxのサーバーを起動する必要がある場合、下記のコマンドは、プロセスを実行します。

.. code-block:: bash
	
	ptdeploy nginxcontrol start                           

あなたは 'Y'を入力続行したい場合は何が 'N'を入力した場合、実行する前に、システムは、続行するに確認をお願いします。

停止
----------------

ユーザーはnginxのサーバーを停止する必要がある場合、下記のコマンドは、プロセスを実行します。

.. code-block:: bash
	
	ptdeploy nginxcontrol stop	

あなたは 'Y'を入力続行したい場合は何が 'N'を入力した場合、実行する前に、システムは、続行するに確認をお願いします。

再起動
----------------

ユーザーは（すべての変更は、設定ファイルにそこに起こっているとき、このオプションが使用されます）nginxのサーバーを再起動する必要がある場合、下記のコマンドは、プロセスを実行します。

.. code-block:: bash
 	
	ptdeploy nginxcontrol restart                          

あなたは 'Y'を入力続行したい場合は何が 'N'を入力した場合、実行する前に、システムは、続行するに確認をお願いします。

リロード
----------------

ユーザーは再起動せずにnginxのサーバをリロードする必要がある場合、下記のコマンドは、プロセスを実行します。

.. code-block:: bash
	
	ptdeploy nginxcontrol reload

あなたは 'Y'を入力続行したい場合は何が 'N'を入力した場合、実行する前に、システムは、続行するに確認をお願いします。

代替パラメータ
------------------------

3つの代替のパラメータのいずれかは、コマンドで使用することができる- ngnixcontrol , NgnixControl and nginxcil 

例えば: ptdeploy ngnixcontrol help/ ptdeploy ngnixControl help


メリット
--------------

* 低メモリフットプリントと10,000人以上の同時接続を処理する能力を
* 静的ファイル、インデックスファイル、および自動インデックス作成の取扱い
* キャッシング*リバースプロキシ
* インバンドヘルスチェックと*ロードバランシング
* フォールトトレランス
* OpenSSLの経由SNIとOCSPステープリングをサポートして* TLS / SSL、。
* FastCGIは、SCGI、キャッシングとuWSGIサポート
* 品名 - とIPアドレスベースの仮想サーバー
* IPv6の互換性
* SPDYプロトコルのサポート
* WebSocketをとHTTP / 1.1のアップグレード（101スイッチングプロトコル）
* FLVとMP4ストリーミング
* ウェブページのアクセス認証
* gzip圧縮と解凍
* URLの書き換え
* オンザフライgzip圧縮と*カスタムログ
* 回答率との同時リクエスト制限
* 帯域幅調整
* サーバサイドインクルード
* IPアドレスベースの地理位置情報
* ユーザー追跡
* WebDAVの
* XSLTデータ処理
* 組み込みのPerlスクリプト
