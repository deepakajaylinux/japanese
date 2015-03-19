==================
AWSCloudFormation
==================

概要
-------------

AWS CloudFormationは、開発者やシステムが作成および管理に関連するAWSリソース、プロビジョニングのコレクションをし、秩序ある予測可能な方法でそれらを更新する簡単な方法を管理者に提供。

あなたは、あなたのアプリケーションを実行するために必要な、AWSCloudFormationâ€™sのサンプル·テンプレートを使用するか、AWSリソース、および関連する依存関係や実行時パラメータを記述するために独自のテンプレートを作成することができます。あなたDONA€™tはAWSサービスまたはそれらの依存関係の仕事をするの機微をプロビジョニングするための順序を把握する必要があります。 CloudFormationには、あなたのためにこれを処理します。 AWSリソースが展開された後は、実際にはあなたのAWSインフラストラクチャにお手元のソフトウェアで行うのと同じ方法でバージョン管理を適用し、制御され、予測可能な方法でそれらを変更し、更新することができます。

あなたは、AWS Management Consoleの、AWSコマンドラインインターフェイス、またはAPIを使用して、テンプレートと（スタックと呼ばれる）資源の関連付けられたコレクションを展開し、更新することができます。 CloudFormationは追加料金なしで利用可能であり、あなたは、あなたのアプリケーションを実行するために必要なAWSリソースのために支払う。


helpコマンド
----------------------

このコマンドは、AWS CloudFormationはの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudFormation help

 ******************************


  This command allows you to install a The AWS Cloud Formation Command
  Line Tools. This tool is provided by

  AWSCloudFormation, aws-cloud-formation, aws-cloudformation

        - install
        Installs AWSCloudFormation. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudFormation.
        example: ptconfigure aws-cloud-formation install

 ------------------------------
 End Help
 ******************************

インストール
-------------------

ユーザーがマシンにAWSCloudFormationモジュールをインストールする必要がある場合は、以下のコマンドは、インストールのプロセスを実行します。

.. code-block:: bash
        
       ptconfigure aws-cloud-formation install

.. code-block:: bash 

 kevell@corp:/# ptconfigure aws-cloud-formation install

 Install AWSCloudFormation? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         AWS CloudFn!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-17956189939.sh
 chmod 755 /tmp/ptconfigure-temp-script-17956189939.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-17956189939.sh Permissions
 Executing /tmp/ptconfigure-temp-script-17956189939.sh
 Cloning into 'aws-cloudformation'...
 remote: Counting objects: 64, done.
 remote: Total 64 (delta 0), reused 0 (delta 0), pack-reused 64
 Unpacking objects: 100% (64/64), done.
 Checking connectivity... done.
 mv: cannot move â€˜/tmp/aws-cloudformation/binâ€™ to â€˜/opt/aws-cloudformation/binâ€™: Directory not empty
 mv: cannot move â€˜/tmp/aws-cloudformation/libâ€™ to â€˜/opt/aws-cloudformation/libâ€™: Directory not empty
 Temp File /tmp/ptconfigure-temp-script-17956189939.sh Removed
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 AWSCloudFormation: Success
 ------------------------------
 Installer Finished
 ******************************

代替パラメータ
------------------------------

コマンドラインで使用することができる3つの代替のパラメータがある。

AWSCloudFormation, aws-cloud-formation, aws-cloudformation 

メリット
--------------

AWSリソースの広い範囲をサポート：AWS CloudFormationは、あなたのアプリケーションのニーズのために、可用性、信頼性、および拡張性のAWSインフラストラクチャを構築することができ、AWSリソースの広い範囲をサポートしています。 AWS CloudFormationは、現在、以下のAWSのリソースをサポートしています

サービス：

自動スケーリング

アマゾンCloudFrontは

AWS CloudWatchの

アマゾンDynamoDBは

Amazon EC2の

アマゾンElastiCacheは

AWS弾性豆の木

AWS弾性ロードバランシング

AWSアイデンティティおよびアクセス管理

Amazon RDSは

アマゾン赤方偏移

アマゾンルート53

Amazon S3の

Amazon SimpleDBは

アマゾンSNS

アマゾンSQS

アマゾンVPC

使いやすい：CloudFormationははAWSリソースのコレクションを整理し、展開することが容易になり、実行時に渡すように依存関係や特殊なパラメータを記述することができます。あなたは多くのCloudFormationはサンプルテンプレートのいずれかを使用することができます - いずれか逐語的または出発点として。
車輪の再発明する必要はありません：テンプレートが同じスタックの同一のコピーを作成する（または新しいスタックを開始するための基盤として使用すること）を繰り返し使用することができます。あなたは、キャプチャし、そのようなアマゾンEC2のAMIのほか、アマゾン弾性ブロックストア（EBS）とAmazon RDSのスナップショット名などの地域固有のインフラの変動を制御することができます。

透明でオープン：テンプレートは、Amazon S3のようなプライベートまたはパブリックの場所に保存され、通常のソース制御メカニズムの下に置かれ、電子メールを介して交換することができるシンプルなJSON形式のテキストファイルです。 AWS CloudFormationは使用すると、AWSリソースがスタックを構成しているかを正確に表示するには」、ボンネットを開く」ことができます。あなたは完全な制御を保持し、スタックの一部として作成されたAWSリソースのいずれかを変更する機能を持っている。

宣言型と柔軟性：あなたが欲しいインフラを作成するには、どのようなAWSリソース、構成値、およびテンプレートに必要な相互接続を列挙して、AWS CloudFormationははAWS Management Consoleの、使用して、一つのコマンドでいくつかの簡単なクリックで残りをやらせるAWSコマンドラインインターフェース、またはAPIを呼び出すことによって、単一の要求。あなたは™tの作成とそれらのサービスAPIを介して各AWSリソースを相互接続する方法の詳細をリコールする必要が€wonâ。 AWS CloudFormationにはあなたのためにこれを行います。あなたがAWS CloudFormationに付属している多くのサンプルテンプレートの1で始まる場合にも、ドナ€™tは最初からテンプレートを記述する必要があります。

パラメータでカスタマイズ：あなたは、スタックが構築されたとき、実行時にテンプレートの側面をカスタマイズするためのパラメータを使用することができます。あなたはスタックを作成するときにたとえば、AWS CloudFormationはへRDSデータベースのサイズ、EC2のインスタンスタイプ、データベース、およびWebサーバのポート番号を渡すことができます。また、制御された方法で異なる場合があります複数のスタックを作成するためにパラメータ化されたテンプレートを使用することができます。たとえば、Amazon EC2インスタンスの種類、アマゾンCloudWatchのアラームしきい値、とAmazonはRDS読み取り専用レプリカあなたはヨーロッパよりも米国で多くの顧客のトラフィックを受信した場合の設定は、AWSの地域間で異なる場合があります。あなたは個別に調整するために、各地域での設定としきい値をテンプレートパラメータを使用し、まだアプリケーションが地域全体に一貫して展開されていることを確認することができます。
統合準備：あなたはあなたの選択の開発および管理ツールで、AWS CloudFormationは統合することができます。

AWS CloudFormationはアマゾンシンプル通知サービス（SNS）を通じてprogressイベントを発行しています。 SNSを使用すると、電子メールを介してスタックの作成と削除の進行状況を追跡することができますし、プログラム的に他のプロセスと統合する。

追加料金なし：AWS CloudFormationは追加料金なしで利用できません。あなたは、AWS CloudFormationは、作成し、アプリケーションが使用するAWSリソースに対してのみ、通常の料金を請求されます。
