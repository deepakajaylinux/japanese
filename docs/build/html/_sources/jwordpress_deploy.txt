============
Wordpress
============

概要
-----------

このモジュールは、既定ワード プレスの web サイトを統合することでユーザーを容易に 1 つの罰金の一部です。その機能 dapperfy、builderfy が含まれていますまた、DBConfigure モジュールのワード プレス データベースの構成を提供しています。

ワード プレスは無料とオープン ソースのブログツールで PHP と MySQL に基づくコンテンツ管理システム （CMS） です。プラグイン アーキテクチャとテンプレート システムが備わっています。ワード プレスは、2015 年 1 月時点のトップ 1000 万のウェブサイトの 23.3% によって使用されました。ワード プレスは以上 6000 万のウェブサイトで、Web 上で最も人気の高いブログ システムです。


Helpコマンド
-------------------

ヘルプ コマンド説明その代替パラメーター宣言、3 つの主要な機能で使用することができますが、このモジュールの主な機能についてのユーザー (ex: dapperfy、builderfy、実行)、および 3 つの主要な機能を宣言する構文についても。ヘルプ オプションを宣言するために使用されるコマンドは下図します。


.. code-block:: bash

		ptdeploy Wordpress help


次のスクリーン ショットをこのモジュールの下に、help コマンドについて視覚的に表しています。宣言で使用する構文は、非大文字小文字を区別です。


.. code-block:: bash

 kevell@corp:/# ptdeploy Wordpress help
 ******************************


  This module is a Default one, and provides integration for Wordpress websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Wordpress Database Configuration for the DBConfigure Module.

  Wordpress, wordpress

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Wordpress.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy wordpress --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************




どのようにdapperfyワードプレスを使用する方法
-------------------------------------------------

ワードプレスは以下のとおりであるdapperfyのために使用されるコマンド、

.. code-block:: bash

		ptdeploy dapperfy wordpress


Dapperfying のプロセスが開始されますに描かれているように上記のコマンドを入力した後、テーブルの下で

.. cssclass:: table-bordered

 +-----------------------------------+-------------------------------------------+----------------+--------------------------------------+
 | パラメータ                        | 代替パラメータ                            | オプション     | 注釈                                 |
 +===================================+===========================================+================+======================================+
 |Dapperfy This for Wordpress? (Y/N) | の代わりに wordpress, 我々は使用すること  | Y(Yes)         | ユーザーは、 Yとして入力することが   |
 |                                   | ができます Wordpress また                 |                | できるワードプレスをdapperfy         |
 |                                   |                                           |                | する必要がある場合                   |
 +-----------------------------------+-------------------------------------------+----------------+--------------------------------------+
 |Dapperfy This for Wordpress? (Y/N) | の代わりに wordpress, 我々は使用すること  | N(No)          | ユーザは、 Nとして入力することがで   |
 |                                   | ができます Wordpress また                 |                | きるワードプレスをdapperfy           |
 |                                   |                                           |                | が必要でない場合には|                |
 +-----------------------------------+-------------------------------------------+----------------+--------------------------------------+
 	

ユーザー dapperfying の実行中に dapperfying、ワードプレスのプロセスが進むと、次の手順が発生します、

Step 1:

Use existing environment settings? (Y/N)

ユーザー Y または N、によって既存の環境設定を使用するために願いを指定しなければなりません。


Step 2:

Do you want to add another environment? (Y/N)

ユーザー Y または N、によって別の環境を追加するために願いを指定しなければなりません。


これらの手順の完了後 dapperfying、ワードプレスの完了を取得します。以下に、スクリーン ショットから視覚的に描かれています。


.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress
 Dapperfy This for Wordpress? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 

WordPressの自動の作業は、ファイルを展開
------------------------------------------------

自動展開ファイルを生成するためにワードプレスでは、ユーザーは、下記のコマンドを入力する必要があります。

.. code-block:: bash

		ptdeploy dapperfy wordpress --yes --guess


上記のコマンドを入力した後、自動展開ファイルが生成されますから絵として描かれている、以下のスクリーン ショット、

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy wordpress --yes --guess
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Wordpress Dapperfies:
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************


メリット
----------

* それは裕福な両方の ubuntu と同様セント OS のように。
* 宣言で使用されるパラメーターの大文字と小文字は区別されません。
* ワードプレスの機能の統合もリンク管理;検索エンジン-フレンドリー、きれいなパーマリンク構造
* それは記事; を複数のカテゴリを割り当てる機能記事と記事のタグ付けをサポートします。
* ワードプレスの自動フィルターも含まれています、書式とスタイルの記事内のテキストの標準
  化を提供します。


