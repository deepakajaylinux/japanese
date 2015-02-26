================
JenkinsPlugins
================

あらすじ
-------------

ジェンキンスさんはビルド サーバーに人気です。Jenins は、Java で記述されたソースの継続的な統合ツールです。ジェンキンスさんはソフトウェア開発のための継続的な統合サービスを提供します。

ジェンキンス Java 以外の言語で記述したプロジェクトにその使用を拡張するためのプラグインをリリースされています。プラグインは、ジェンキンスさんほとんどのバージョン管理システムと大規模なデータベースを統合するために利用可能です。多くのビルド ツールは、それぞれのプラグイン経由でサポートされます。プラグインは、ジェンキンス見えるか新しい機能を追加する方法を変更することもできます。ビルド プラグイン (JUnit サポートは現在バンドルされています) でサポートされているさまざまな形式でテスト レポートを生成することができ、ジェンキンスは、レポートを表示することができますとトレンドを生み出すし、GUI でそれらをレンダリングします。

ヘルプ コマンド
-----------------

このコマンドは、JenkinsPlugins モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
             
   		ptconfigure JenkinsPlugins help


 kevell@corp:/# ptconfigure JenkinsPlugins help
 ******************************


  This command allows you to install a bunch of plugins that we recommend for
  PHP builds in Jenkins.

  JenkinsPlugins, jenkinsplugins, jenkins-plugins, jenkins-plugs

        - install
        Installs the latest version of Jenkins Plugins for PHP recommended by Golden Contact
        example: ptconfigure jenkins-plugins install

 ------------------------------
 End Help
 ******************************




インストール
----------------

このコマンドでは、PHP ビルド ジェンキンスさんにお勧めするプラグインの束をインストールすることができます。ユーザーのマシンでジェンキンス モジュールをインストールする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
        
		ptconfigure JenkinsPlugins install


上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash

 

 kevell@corp:/# ptconfigure JenkinsPlugins install
 Install Jenkins Plugins? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Jenkns Plgs!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80223312434.sh
 chmod 755 /tmp/ptconfigure-temp-script-80223312434.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80223312434.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80223312434.sh
 Cloning into 'jplugins'...
 remote: Counting objects: 39, done.
 remote: Total 39 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (39/39), done.
 Checking connectivity... done.
 chown: invalid user: ‘jenkins’
 jenkins: unrecognized service
 Temp File /tmp/ptconfigure-temp-script-80223312434.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsPlugins: Success
 ------------------------------
 Installer Finished
 ******************************





オプション
-----------     

.. cssclass:: table-bordered


 +------------------------+-------------------------------------------------------+-------------+--------------------------------------------+
 | パラメータ             | 代替パラメータ                                        | オプション  | 注釈                                       |
 +========================+=======================================================+=============+============================================+
 |ptconfigure             | 4代替パラメータのいずれかのコマンドで使用する         | Y(Yes)      | ユーザがオプションを提供すると、           | 
 |JenkinsPlugins Install  | ことができる JenkinsPlugins, jenkinsplugins,          |             | システムはインストールプロセスを開始します |
 |                        | jenkins-plugins, jenkins-plugs例:                     |             |                                            |
 |                        | ptconfigure jenkins-plugins Install                   |             |                                            |
 +------------------------+-------------------------------------------------------+-------------+--------------------------------------------+
 |ptconfigure             | 4代替パラメータのいずれかのコマンドで使用する         | N(No)       | ユーザがオプションを提供すると、           |
 |JenkinsPlugins Install  | ことができる JenkinsPlugins, jenkinsplugins,          |             | システムはインストールプロセスを停止します |
 |                        | jenkins-plugins, jenkins-plugs例:                     |             |                                            |
 |                        | ptconfigure jenkins-plugins Install|                  |             |                                            |
 +------------------------+-------------------------------------------------------+-------------+--------------------------------------------+


利点
--------------

* プラグインはすべてのジョブで使用されるどのくらいのすべてのプラグインに関する報告書を与えます。従ってそれは使用される拡張を分析します。
  各ジョブのポイント。
* このプラグインは、インストールされたプラグインの使用状況を分析する可能性を与えます。
* 非大文字小文字の区別
* Ubuntu や CentOS で裕福な。
