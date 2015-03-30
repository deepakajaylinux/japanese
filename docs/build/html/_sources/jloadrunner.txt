==============
Loadrunner
==============

概要
----------

実際の負荷を発生させながら、システムの動作とパフォーマンスを調べる：HP LoadRunnerは、アプリケーションの負荷テスト用のヒューレット·パッカード社からの自動性能とテスト自動化製品です。 LoadRunnerは、さまざまな開発ツール、技術や通信プロトコルをサポートしています。

Helpコマンド
--------------

 helpコマンドは、とだけでなく、 LoadRunnerのモジュールに含まれているオプションについての目的について、ユーザーをガイドします。また、 LoadRunnerのモジュールをインストールするための構文について説明します。 LoadRunnerのためのhelpコマンドは以下の通りである。


.. code-block:: bash

	ptconfigure Loadrunner help

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure Loadrunner help 
 ****************************** 


  This command allows you to install HardyCssRegression from a GC Repo. 

  Loadrunner 

        - install 
        Installs the latest GC Repo version of Loadrunner 
        example: ptconfigure Loadrunner install 

 ------------------------------ 
 End Help 
 ******************************   



インストール
--------------

端末上のLoadRunnerのモジュールをインストールするために使用するコマンドは、以下に記載されている

.. code-block:: bash

	ptconfigure loadrunner install 

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure loadrunner install 
 Install Loadrunner? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Loadrunner !         * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-32374780925.sh 
 chmod 755 /tmp/ptconfigure-temp-script-32374780925.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-32374780925.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-32374780925.sh 
 mkdir: cannot create directory â€˜loadrunnerâ€™: File exists 
 Cloning into 'loadrunner'... 
 remote: Counting objects: 1284, done. 
 remote: Total 1284 (delta 0), reused 0 (delta 0), pack-reused 1284 
 Receiving objects: 100% (1284/1284), 5.63 MiB | 21.00 KiB/s, done. 
 Resolving deltas: 100% (592/592), done. 
 Checking connectivity... done. 
 Temp File /tmp/ptconfigure-temp-script-32374780925.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Loadrunner: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


メリット
----------

* テスト対象のサーバにインストールする必要はありません。それは、ネイティブのモニターを使用しています。例の場合： 
  UNIX用のWindowsまたはrstatdは デーモンのPERFMON
* デフォルトのプログラミングlanguage1とJavaやVBのような他の言語としてANSI Cを使用します。
* 優秀な監視とあなたは色付きのチャートやグラフィックスを理解しやすいのレポートを見ることができ、分析インターフェース。
  protocols2のほとんどをサポートしています。
* がはるかに簡単correlation3にします。私たちは、後にポスト一連の相関関係を掘り下げます。
  1クリックの記録を通して*ニースのGUIが生成されたスクリプトは、もちろん、あなたのニーズに応じてスクリプトを変更する必要があります。

