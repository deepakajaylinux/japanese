=================
Amazon S3 
=================

概要
-------------

アマゾンの単純なストレージ サービス (アマゾン S3) 開発者に提供し、安全、耐久性、拡張性の高いオブジェクトの記憶域を持つチームします。Amazon S3 は使いやすく、格納およびどこからでもデータの任意の金額を取得する単純な web サービス インターフェイスを持つ web 上。アマゾン S3 で実際に使用する記憶域のためにのみ支払います。いいえセットアップ費用があり、最低手数料はかかりません。

Amazon S3 は単独で、またはアマゾン弾性計算雲 (アマゾン EC2)、Amazon の Elastic ブロック ストア （アマゾン EBS） とアマゾン氷河と同様にサード パーティ製ストレージ ・ リポジトリおよびゲートウェイなどの他の AWS サービスと共に使用できます。Amazon S3 はさまざまなクラウド アプリケーション、コンテンツ配信、バックアップ、アーカイブ、災害復旧およびビッグデータ解析を含むユース ケースのコスト効果の高いオブジェクトのストレージを提供します。

Helpコマンド	
----------------------

このコマンドは、AWS S3 の使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSS3 help

 ******************************


    This is an extension provided for Handling AWSS3.

    AWSS3, awss3 aws-s3

        - ensure-bucket-exists
        Lets you add bucket to AWSS3 if doesnt exists
        example: ptconfigure AWSS3 ensure-bucket-exists
                    --yes
                    --guess
        - add-object
        Lets you upload object to bucket
        example: ptconfigure AWSS3 add-object
                    --yes
                    --guess


        - remove-bucket
          Lets you remove bucket
          example: ptconfigure AWSS3 remove-bucket
                    --yes
                    --guess

        - remove-object-all
       Lets you remove all object from a bucket
          example: ptconfigure AWSS3 remove-object-all
                    --yes
                    --guess


            - remove-object
       Lets you remove a object from a bucket
          example: ptconfigure AWSS3 remove-object
                    --yes
                    --guess

        - list
        Will display data about your AWS S3
        example: ptconfigure AWSS3 list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************


Ensure-bucket-exists
---------------------------

このコマンドは存在していない場合 AWSS3 にバケットを追加することができます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess


Add-object 
---------------------------

このコマンドは、バケツにオブジェクトをアップロードするのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash

	ptconfigure AWSS3 add-object --yes –guess

Remove-bucket 
---------------------------

このコマンドは、バケットを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。
 
.. code-block:: bash     

	ptconfigure AWSS3 remove-bucket --yes --guess

Remove-object-all
--------------------------

このコマンドはバケツからすべてのオブジェクトを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object-all --yes --guess

Remove-object	
--------------------------

このコマンドはバケツからオブジェクトを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object --yes --guess 


List
---------

このコマンドは、AWS S3 についてのデータを表示するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSS3 list --yes --guess

代替パラメータ
------------------------------       

コマンドラインで使用できる 3 つの代替パラメーターがあります。

AWSS3, awss3 aws-s3 

メリット
--------------

耐久性： Amazon の S3 の重要なデータを格納する耐久性のあるインフラストラクチャを提供し、オブジェクトの 99.999999999% の耐久性のために設計されます。あなたのデータは複数の施設および各施設の複数のデバイス間で重複して格納されます。

低コスト： Amazon の S3 を使用すると大量の非常に低コストでデータを格納できます。あなたは、何が必要最小コミットメントやアップ フロント手数料を支払います。

利用できる: Amazon S3 はオブジェクトの可用性を 99.99% 上設計与えられた年。Amazon S3 はまたあなたがそれを必要とするときはそれに依存することができますを確保する、Amazon S3 サービス レベル契約によってバックアップされます。遅延の最適化、コストを最小限に抑えるまたは規制要件に対応する、AWS の領域を選択できます。

Amazon S3 の保護： がアップロードされる over SSL とデータの自動暗号化にデータ転送をサポートします。オブジェクト権限の管理し、AWS のアイデンティティ管理とアクセス管理 (IAM) を使用してデータへのアクセスを制御するバケットのポリシーを構成することもできます。

拡張性： アマゾン S3、あなたがそれを必要とするとき、それをアクセスする量のデータを格納できます。停止できます将来のストレージのニーズと、必要に応じて上下のスケールを推測して大幅にビジネスの俊敏性を高めること。

イベント通知を送信する: Amazon S3 は、オブジェクトは Amazon S3 にアップロードするときのイベント通知を送信できます。Amazon S3 のイベント通知をアマゾン SQS またはアマゾン SNS を使用して配信または AWS ラムダ、ワークフローをトリガー、警告、またはその他の処理を有効にするのに直接送信することができます。たとえばは、彼らがアップロードされると、他のデータ ストアとデータ ファイル、利用可能になったときや Amazon の S3 のオブジェクトの同期処理でのメディア ファイルの変換をトリガーするのに Amazon の S3 イベント通知を使用可能性があります。
高パフォーマンス: マルチパートをアップロード ネットワーク スループットと回復力を最大化をすることができます Amazon S3 サポート終わりユーザーの近くにデータを格納し、ネットワーク ・ レーテンシーを最小限に抑えるに AWS 地域を選択します。Amazon の S3 をアマゾン CloudFront、低レイテンシ、高データ転送速度、いいえ最小使用率のコミットメントはエンドユーザーにコンテンツを配布するコンテンツ配信 web サービス統合されています。

統合: Amazon の S3 サービスが統合他 AWS をアップロードし、Amazon の S3 からデータをダウンロードを簡素化し、範囲の AWS のサービスを使用するソリューションの構築が容易になります。Amazon S3 の統合などのアマゾン CloudFront アマゾン キネシス、Amazon RDS、アマゾンの氷河、アマゾン EBS、アマゾン DynamoDB、アマゾン赤方偏移、アマゾン ルート 53、アマゾンの電子カルテ、AWS ラムダ。

使いやすい： Amazon S3 は使いやすい web ベースの管理コンソールとモバイル アプリと完全 REST Api と Sdk サード パーティーのテクノロジの統合が容易です。

