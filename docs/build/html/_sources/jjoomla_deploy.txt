==========
Joomla
==========

概要
----------------

Joomlaのは、統合ウェブサイトを提供しています。多くのWebホスティングサービスが提供する、シングルクリックのユーザー新しいサイトアップを取得し、わずか数分で実行して、インストールします。

その使いやすさと拡張性を含め、Joomlaの最も人気のあるWebサイトのソフトウェア作った。すべてのベストは、オートパイロット、builderfyとdapperfyはptdeployで利用可能であり、最善の解決策になります。これはUbuntuとセントOSと快適です。


Helpコマンド
------------------------

このhelpコマンドは、Joomlaのための統合を提供するために、ユーザーをガイドします。これは、DBの構成モジュールのデータベース構成を提供してオートパイロット、builderfyとdapperfyがptdeploy .Alsoでご利用いただけますパーソナライズされています。

Joomlaのためのhelpコマンドを以下に示します。

.. code-block:: bash

	ptdeploy joomla help

後、上記のコマンドを入力し、それはJoomlaのウェブサイトを統合するために機能して開始します。これは、スクリーンショットでjoomlaのの機能を教理。

.. code-block:: bash

 kevell@corp:/# ptdeploy Joomla help
 ******************************


  This module is a Default one, and provides integration for Joomla websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Joomla Database Configuration for the DBConfigure Module.

  Joomla, joomla

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Joomla.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy joomla --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

インストール
-------------------


このモジュールは、builderfyとdapperfyの両方に複数のアクションを追加します。これはインストールが簡単であり、Webデザイナーや開発者として、ユーザーはすぐに彼らのクライアントのためのサイトを構築することができ、ユーザは、Joomlaのは、非常に使いやすいです高度なuser.Sinceない場合でも、設定します。次のようにjoomlaのをインストールするために使用されるコマンドは、ある

.. code-block:: bash

	ptdeploy joomla install

コマンドを活性化した後、入力をcatechizeます。

はい自動的にシステムからのJoomlaをインストールするようにすると、ユーザー入力。インストールを終了しない場合。以下のスクリーンショットは、joomlaのと、その機能を実証する。


Dapperfy
---------------

このdapperfyは、ユーザーオートデプロイファイルを作成するために使用される。 Dapperfyはセットアップの価値は数分で複雑な設定なしで多くのプロジェクトのために働くことができます。使い方Dapperfyは非常に迅速であり、さらには常にちょうどその後、独自のカスタマイズを使用してファイルを変更することができ、ユーザのような複雑な構成のために、おそらく最高の出発点です。 dapperfyのために使用される次のコマンド。


.. code-block:: bash

	ptdeploy dapperfy joomla

上で述べコマンドとして入力した後、それはスクリーンショットによって示しdapperfy実行を要求します。

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy joomla
 Dapperfy This for Joomla? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************

Builderfy
--------------

これは、ビルドをインストールするためのテンプレートを作成します。ユーザーは複数のテンプレートを追加することができます。我々は、ユーザーのターゲット生産に新しいバージョンを展開する、ユーザー·リポジトリに変更を加えると。次のようにbuilderfyのために使用されるコマンドは、ある

.. code-block:: bash

	ptdeploy builderfy joomla

次のスクリーンショットは、その機能を説明しています。

.. code-block:: bash

実行する
------------

このプロセスは、自動操縦ビルドクリエーターを実行します。クイックアクセスが可能です。実行のためのコマンドは、次のように

.. code-block:: bash

	ptdeploy autopilot execute

以下のスクリーンショットは、その機能を説明します。

.. code-block:: bash

オプション
------------

.. cssclass:: table-bordered

 +----------------------+-------------------+--------------+---------------------------------------------------------+
 | パラメーター         | 代替パラメータ    | オプション   | コメント                                                |
 +======================+===================+==============+=========================================================+
 |Dapperfy this for     | Joomla, joomla    | Y(Yes)       | ユーザーの願いはdapperfying続行する場合、それらは、     | 
 |joomla? (Y/N)         |                   |              | Yなどの入力をすることができます                         |
 +----------------------+-------------------+--------------+---------------------------------------------------------+
 |Dapperfy this for     | Joomla, joomla    | N(No)        | ユーザーの願いはdapperfying終了した場合、彼らは、       |
 |joomla? (Y/N)         |                   |              | Nとして入力をすることができます                         |
 +----------------------+-------------------+--------------+---------------------------------------------------------+
 |Do you want to add    |                   | Y(Yes)       | ユーザーの願いは新しい環境を追加するには場合、それらは、|        
 |another               |                   |              | Yなどの入力をすることができます                         |
 |environment?(Y/N)     |                   |              |                                                         |
 +----------------------+-------------------+--------------+---------------------------------------------------------+
 |Do you want to add    |                   | N(No)        | ユーザーは、Nとして彼らができる新しい環境入力を         |
 |another               |                   |              | 追加する必要にない場合                                  |
 |environment?(Y/N)|    |                   |              |                                                         |
 +----------------------+-------------------+--------------+---------------------------------------------------------+
 

メリット
------------

ITプロフェッショナルのための*さてサポート

* 多言語プロセス
* 簡単なアップグレード
* スピーディシステム機能
* 大文字小文字を区別
* UbuntuとセントOSに適しています。

それはあなたのユーザーデザインの夢が叶うことを確認に使用する自由を可能にするためのJoomla自体は、式の全く新しい世界を開く！
