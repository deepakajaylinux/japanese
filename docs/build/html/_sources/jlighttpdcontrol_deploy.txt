=====================
LighttpdControl
=====================

概要
---------------

Lighttpdのは、高性能環境に最適化された、高速で、セキュリティで保護さに準拠した、と非常に柔軟なWebサーバである。急速にptdeployの効率を再定義されているLighttpdの。それは、高性能環境用に設計され、最適化される。小さなメモリフットプリントを持つ他のWebサーバ、CPU負荷の効果的な管理、および高度な機能セットのlighttpdのに比べて、負荷の問題に悩まされているすべてのサーバーのための完璧なソリューションです。これはUbuntuとセントのOSで動作するのに適している。

Helpコマンド
----------------------

ヘルプには、lighttpdのについての情報にアクセスするために使用されている。あなたはまた、helpコマンドを使用することができますptdeployのバージョンのいずれかのヘルプコマンドとクイックリファレンスのために。 helpコマンドは、内部コマンドであるとptdeployモジュールで利用可能です。

.. code-block:: bash
   
	ptdeploy lighttpdcontrol help

次のスクリーンショットは、ptdeployに隷属するユーザーを支援します。

.. code-block:: bash

 kevell@corp:/# ptdeploy LighttpdControl help
 ******************************


  This command is part of Default Modules and handles Lighttpd Server Control Functions.

  LighttpdControl, lighttpdcontrol, lighttpdctl

          - start
          Start the Lighttpd server
          example: ptdeploy lighttpdcontrol start
          example: ptdeploy lighttpdcontrol start --yes

          - stop
          Stop the Lighttpd server
          example: ptdeploy lighttpdcontrol stop
          example: ptdeploy lighttpdcontrol stop --yes

          - restart
          Restart the Lighttpd server
          example: ptdeploy lighttpdcontrol restart
          example: ptdeploy lighttpdcontrol restart --yes

          - reload
          Reloads the Lighttpd server configuration without restarting
          example: ptdeploy lighttpdcontrol reload
          example: ptdeploy lighttpdcontrol reload --yes

 ------------------------------
 End Help
 ******************************

代替パラメータ
--------------------------------

好ましくは、Lighttpdのは、ユーザーが次のオプションを行使することができます使用。

LighttpdControl, lighttpdcontrol, lighttpdctl

スタート
--------------

lighttpdのサーバーを起動するために使用するオプションを起動します。 Lighttpdcontrolはptdeployモジュールオプションで実行されているインタラクティブなセッションです。サーバーが実行される方法に応じて、startコマンドは、Linuxのレジストリに、スクリプトに格納されることがあります。
サーバーは、追加のオプションを取得するためにサーバーを制御するために戻って接続するためのオプションを指定して簡単なコマンドを使用して起動することができます。

.. code-block:: bash
   
        ptdeploy lighttpdcontrol start

コマンドを入力した後、ユーザーがlighttpdのサーバーの機能を開始することができます。

停止
-------

lighttpdのサービスを停止するために使用されるこの停止オプション。具体的にUbuntu Linuxのは、stopコマンドは、システム上で実行されているジョブを停止するlighttpdのを呼び出します。それは、コマンドサービス停止に相当します。以下停止コマンドの完全な記述である。

.. code-block:: bash
   
        ptdeploy lighttpdcontrol stop

上記のコマンドとして入力した後、サービスが機能を停止。

再起動
------------

長期的な再起動がウォームリスタートlighttpdのサーバーの前に、すべてのプログラムを終了し、オペレーティング·システムを指します。再起動が時々エラーから回復するために必要であるか、または再初期ドライバやハードウェアデバイスへ。コンピュータ記憶プログラムは、通常、次の簡単なコマンドで再起動を実行します。

.. code-block:: bash
   
        ptdeploy lighttpdcontrol restart

上記のコマンドとして入力した後、サービスはlighttpdのサービスを再起動します。

リロード
------------

リロードは、物事が変化していることを意味します。 lighttpdのはオーバーホールとクリーンアップを受けている。それは、lighttpdのとサービスの再利用を容易にします。プロセスを強制終了することなく、それがlighttpdのをリロードすることができます。次のコマンドは、リロードするユーザーをアシス。コマンドとともに、ユーザが...はい、自動的にそれが機能することができ、任意の質問をせずにオプションを使用する場合。

.. code-block:: bash
   
        ptdeploy lighttpdcontrol reload

メリット
--------------

* 柔軟な仮想ホスティング。
* すべてのモジュールタイプをサポートしています。
* 軽量（1 MB未満）。
* 大文字小文字を区別し。
* ユーザーは自分の願い通りに機能することができます。
* 終了は可能です。
* 自動化が可能です。
