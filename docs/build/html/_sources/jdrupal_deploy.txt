========
Drupal
========

概要
------------

Drupalのモジュールは、デフォルトモジュールの一部である。それはbuilderfyとdapperfyオートパイロットによって調整されているDrupalのためのオートパイロットを提供します。 builderfyとdapperfyに加えて、それは、DBの構成モジュールのdrupalのデータベース構成を提供します。

Drupalは、PHPで書かれており、GNU General Public Licenseの下で配布されるフリーでオープンソースのコンテンツ管理フレームワークです。それは、個人のブログからWhiteHouse.govとdata.gov.uk.含め、企業の政治的、および政府のサイトに至るまで、世界中のすべてのWebサイトの少なくとも2.1％のバックエンドフレームワークとして使用されているまた、ナレッジマネジメントと業務提携のために使用されている。

DrupalはMySQLのよう、MongoDBは、MariaDB、PostgreSQLは、SQLiteの、またはMicrosoftなどの（（アパッチ、LiteSpeedは、IIS、Lighttpdの、ハイアワサ、チェロキーまたはnginxのを含む）は、PHPを実行できるWebサーバーとデータベースの両方をサポートする任意のコンピューティングプラットフォーム上で動作しますSQL Server）はコンテンツと設定を保存します。

私たちはさまざまな側面で、このモジュールの下のDrupalをdapperfyする方法を見てみましょう。


helpコマンド
--------------------

helpコマンドは、ユーザーを簡単にし、同様に興味深い抽象的である。それは、その主要な役割に関する情報を提供する、宣言で使用することができる別のパラメータの詳細は、その三つの主要な機能（builderfy、dapperfy、実行）し、また、これら3つの興味深い機能を使用して宣言するためのシンタックス。ヘルプオプションの宣言に使用される構文は、以下のとおりである。

.. code-block:: bash

	ptdeploy Drupal help

上記のコマンドを入力した後、ユーザーは上記の詳細と共にヘルプオプションの表示結果を表示することができ、以下のスクリーンショットから示されているように、視覚的にhelpオプションのこれらの結果を得ることができます。

.. code-block:: bash

 kevell@corp:/# ptdeploy Drupal help
 ******************************


  This module is a Default Modules and provides autopilots for drupal tailored Builderfy and Dapperfy Autopilots.
  Also provides Drupal Database Configuration for the DBConfigure Module.

  Drupal, drupal

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Drupal.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy drupal --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

DrupalのをDapperfyする方法
--------------------------------------------
 
私たちはDrupalのをdapperfyingでこのモジュールの別の側面について見てみましょう。以下に示すように、この目的のために使用されるコマンドは、すべての面で同一である

.. code-block:: bash

	ptdeploy dapperfy drupal

テーブルから描かれているように、上記のコマンドを入力した後、以下の詳細が実行時に問い合わせをしている、


.. cssclass:: table-bordered

 +--------------------------+-------------------+---------------+----------------------------------------------------------------+
 | パラメーター             | 代替パラメータ    | オプション    | コメント                                                       |
 +==========================+===================+===============+================================================================+
 |Dapperfy This for         | Drupal, drupal    | Y(Yes)        | ユーザーは、Yと入力できるdrupalのをdapperfyする必要がある場合  |
 |Drupal? (Y/N)             |                   |               |                                                                |
 +--------------------------+-------------------+---------------+----------------------------------------------------------------+
 |Dapperfy This for         | Drupal, drupal    | N(No)         | ユーザーはN.として入力できるdrupalのをdapperfy                 |
 |Drupal? (Y/N)             |                   |               | が必要でない場合には|                                          |
 +--------------------------+-------------------+---------------+----------------------------------------------------------------+



ユーザー進み、Yと入力することにより、Drupalのをdapperfying場合は、以下のステップを実行中に関与している、

ステップ1：

Do you want to add another environment? (Y/N)

ユーザーが別の環境を追加するための彼らの必要性に応じて、入力YまたはNにあります。

次のスクリーンショットのDrupalをdapperfyingのこのプロセスについて視覚的に示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

Drupalののdapperfyingを宣言するの2番目の形式は、以下に説明され、そのために使用されるコマンドは、同じです

.. code-block:: bash

	ptdeploy dapperfy drupal

テーブルから描かれているように、上記のコマンドを入力した後、以下の詳細が実行時に問い合わせをしている、

.. cssclass:: table-bordered

 +---------------------------+--------------------+------------+---------------------------------------------------------------------+
 | パラメータ                | 別のパラメータ     | オプション | 注釈                                                                |
 +===========================+====================+============+=====================================================================+
 |Dapperfy This for Drupal?  | Drupal, drupal     | Y(Yes)     | ユーザーは、Yと入力できるdrupalのをdapperfyする必要がある場合       |
 |(Y/N)                      |                    |            |                                                                     |
 +---------------------------+--------------------+------------+---------------------------------------------------------------------+
 |Dapperfy This for Drupal?  | Drupal, drupal     | N(No)      | ユーザーはN.として入力できるdrupalのをdapperfyが必要でない場合には  |
 |(Y/N)                      |                    |            |                                                                     |
 +---------------------------+--------------------+------------+---------------------------------------------------------------------+
 |Use existing environment   |                    | Y(Yes)     | ユーザーは、Yと入力することができ、既存の環境設定を続行したい場合は |
 |settings? (Y/N)            |                    |            |                                                                     |
 +---------------------------+--------------------+------------+---------------------------------------------------------------------+
 |Use existing environment   |                    | N(No)      | ユーザー願いが新しい環境設定を続行する場合、                        |
 |settings? (Y/N)            |                    |            | それらはNとして入力をすることができます|                            |
 +---------------------------+--------------------+------------+---------------------------------------------------------------------+

上記の問い合わせが完了した後、説明したように、次の手順が実行されます、

ステップ1：Do you want to modify entries applicable to any app in environment default-local (Y/N)

ユーザは、入力YまたはNに持っている

ステップ2：Environment 1 default-local:

このステップでは、環境とする一時ディレクトリの値は、問い合わせをされ、ユーザーは、入力にそれらを持っている。

ステップ3：Enter Servers-this is an array of entries

Enter target?

Enter User?

Enter Password?

ユーザが入力したものは、データの問い合わせがある。

ステップ4：Add Another Server? (Y/N)

ユーザーは自分の願いに応じて、入力YまたはNに持っている。

ステップ5：Do you want to modify entries applicable to any app in environment default-local -0000 (Y/N)

ユーザは、入力YまたはNに持っている

ステップ6：入力デフォルト以外の値に必要に応じて環境の設定は手動で定義することができます。

データのは、以下のように定義されている設定を適用するの実行中に尋ね

Value for Git repo URL

Value for Optional Private SSH Key for Git Repo.

Value for Git Custom Branch

Value for Apache VHost URL

Value for Apache VHost Hostname/IP

Value for how many revisions to keep

Value for DB IP Address

Value for DB App User Name

Value for DB App User Pass

ステップ7：

Do you want to add another environment? (Y/N)

ユーザーは、自分のニーズに応じて、入力YまたはNに持っている。

次のスクリーンショットは、上記で説明のステップのための図的表現を与えるだろう。

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal

 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to modify entries applicable to any app in environment default-local (Y/N) 
 Y
 Environment 1 default-local : 
 Default Settings for Any App not setup for environment default-local enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /root/gg
 Enter user ?
 root
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 Do you want to modify entries applicable to any app in environment default-local-8080 (Y/N) 
 n
 Settings for dapper not setup for environment default-local-8080 enter them manually.
 Environment 2 default-local-8080 : 
 Value for: Project Container directory, (inc slash)
 /root/vv
 Value for: Git Repo URL
 
 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch
 
 Value for: Apache VHost URL (Don't Include http://)
 
 Value for: Apache VHost Hostname/IP
 
 Value for: How many revisions to keep
 
 Value for: DB IP Address
 
 Value for: DB App User Name (Will be created if not existing)
 
 Value for: DB App User Pass
 
 Value for: DB Name (Will be created if not existing)
 
 Value for: DB Admin User Name
 
 Value for: DB Admin User Pass
 
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************
 
 
 Success
 In Dapperfy
 ******************************
 
実行の第3の形態は、今後のステップから説明される。コマンドは同じです

.. code-block:: bash

	ptdeploy dapperfy drupal

テーブルから描かれているように、上記のコマンドを入力した後、以下の詳細が実行時に問い合わせをしている、

.. cssclass:: table-bordered

 +---------------------------+-------------------+--------------+---------------------------------------------------------------------+
 | パラメーター              | 代替パラメータ    | オプション   | コメント                                                            |
 +===========================+===================+==============+=====================================================================+
 |Dapperfy This for          | Drupal, drupal    | Y(Yes)       | ユーザーは、Yと入力できるdrupalのをdapperfyする必要がある場合       | 
 |Drupal? (Y/N)              |                   |              |                                                                     |
 +---------------------------+-------------------+--------------+---------------------------------------------------------------------+
 |Dapperfy This for          | Drupal, drupal    | N(No)        | ユーザーはN.として入力できるdrupalのをdapperfyが必要でない場合には  |
 |Drupal? (Y/N)              |                   |              |                                                                     |
 +---------------------------+-------------------+--------------+---------------------------------------------------------------------+
 |Use existing environment   |                   | Y(Yes)       | ユーザーは、Yと入力することができ、既存の環境設定を続行したい場合は | 
 |settings? (Y/N)            |                   |              |                                                                     |
 +---------------------------+-------------------+--------------+---------------------------------------------------------------------+
 |Use existing environment   |                   | N(No)        | ユーザー願いが新しい環境設定を続行する場合、                        |
 |settings? (Y/N)            |                   |              | それらはNとして入力をすることができます|                            |
 +---------------------------+-------------------+--------------+---------------------------------------------------------------------+

上記の問い合わせが完了した後、説明したように、次の手順が実行されます、

ステップ1：Do you want to add another environment settings? (Y/N)

ユーザは、入力YまたはNに持っている


ステップ2：Environment 3 default-local:

このステップでは、環境とする一時ディレクトリの値は、問い合わせをされ、ユーザーは、入力にそれらを持っている。

入力デフォルト以外の値に必要に応じて環境の設定は手動で定義することができます。

データのは、以下のように定義されている設定を適用するの実行中に尋ね

プロジェクトコンテナディレクトリーの値。

Value for Project Container Directory.

Value for Git repo URL

Value for Optional Private SSH Key for Git Repo.

Value for Git Custom Branch

Value for Apache VHost URL

Value for Apache VHost Hostname/IP

Value for how many revisions to keep

Value for DB IP Address

Value for DB App User Name

Value for DB App User Pass

次のスクリーンショットは、上記で説明のステップのための図的表現を与えるだろう。

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Value for: Project Container directory, (inc slash)

 Value for: Git Repo URL

 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch

 Value for: Apache VHost URL (Don't Include http://)

 Value for: Apache VHost Hostname/IP

 Value for: How many revisions to keep

 Value for: DB IP Address

 Value for: DB App User Name (Will be created if not existing)

 Value for: DB App User Pass

 Value for: DB Name (Will be created if not existing)

 Value for: DB Admin User Name

 Value for: DB Admin User Pass

 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

drupalのをdapperfying第4のタイプは、以下に説明し、使用されるコマンドは、同じである

.. code-block:: bash

	ptdeploy dapperfy drupal

テーブルから描かれているように、上記のコマンドを入力した後、以下の詳細が実行時に問い合わせをしている、

.. cssclass:: table-bordered

 +------------------------------+---------------------+--------------+---------------------------------------------------------------------+
 | パラメータ                   | 別のパラメータ      | オプション   | 注釈                                                                |
 +==============================+=====================+==============+=====================================================================+
 |Dapperfy This for             | Drupal, drupal      | Y(Yes)       | ユーザーは、Yと入力できるdrupalのをdapperfyする必要がある場合       |
 |Drupal? (Y/N)                 |                     |              |                                                                     |
 +------------------------------+---------------------+--------------+---------------------------------------------------------------------+
 |Dapperfy This for             | Drupal, drupal      | N(No)        | ユーザーはN.として入力できるdrupalのをdapperfyが必要でない場合には  |
 |Drupal? (Y/N)                 |                     |              |                                                                     |
 +------------------------------+---------------------+--------------+---------------------------------------------------------------------+
 |Use existing environment      |                     | Y(Yes)       | ユーザーは、Yと入力することができ、既存の環境設定を続行したい場合は |
 |settings? (Y/N)               |                     |              |                                                                     |
 +------------------------------+---------------------+--------------+---------------------------------------------------------------------+
 |Use existing environment      |                     | N(No)        | ユーザー願いが新しい環境設定を続行する場合、                        |
 |settings? (Y/N)               |                     |              | それらはNとして入力をすることができます|                            |
 +------------------------------+---------------------+--------------+---------------------------------------------------------------------+

ユーザー進み、Yと入力することにより、Drupalのをdapperfying場合は、以下のステップを実行中に関与している、

ステップ1：Do you want to add another environment? (Y/N)

ユーザーが別の環境を追加するための彼らの必要性に応じて、入力YまたはNにあります。

次のスクリーンショットのDrupalをdapperfyingのこのプロセスについて視覚的に示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

Builderfy
---------------

これは、ビルドをインストールするには、 Drupalのテンプレートを作成します。ユーザーは複数のテンプレートを追加することができます。我々は、ユーザーのターゲット生産に新しいバージョンを展開するユーザー·リポジトリに変更を加えるときは。次のようにbuilderfyのために使用されるコマンドは、ある

.. code-block:: bash


        ptdeploy builderfy continuous-drupal

.. code-block:: bash


 kevell@corp:/# ptdeploy builderfy continuous-drupal
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this? 

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ****************************** 


 Success
 In Builderfy
 ******************************


メリット
-----------

* これは、セントのOSのように裕福な両方のUbuntuで、同様である。
* 宣言で使用されるパラメータは、大文字と小文字を区別しません。
* dapperfying実行中*環境の設定を定義することができる。
