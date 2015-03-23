=================
AMAZON ROUTE 53 
=================

概要
-------------

アマゾン ルート 53 は、高い可用性とスケーラビリティの雲ドメイン ネーム システム (DNS) web サービスです。それは、開発者や企業、非常に信頼性の高い、コスト効果的な方法を提供するルート エンドユーザー インターネット アプリケーションに www.example.com のような名前、数値の IP アドレス 192.0.2.1 互いに接続するコンピューターを使用するように変換することによって設計されています。

アマゾン ルート 53 効果的にインフラストラクチャに接続ユーザーの要求する-Amazon EC2 インスタンス、弾性負荷分散ロード バランサー、Amazon S3 のバケットなど – AWS で実行されていると、AWS の外のインフラストラクチャにルート ユーザーを使用することもできます。健康的なエンドポイントへのトラフィックのルーティングに DNS チェックを構成するか、アプリケーションとそのエンドポイントの正常性を監視するアマゾン ルート 53 を使用できます。アマゾン ルート 53 グローバル ルーティング タイプ、遅延ベース ルーティング、Geo DNS、およびラウンド ロビンの重み付けなどの様々 な通過するトラフィックを管理するため可能-すべての様々 な低レイテンシ、フォルト ・ トレラントなアーキテクチャを実現するために DNS フェールオーバーと組み合わせること。アマゾン ルート 53 はまたドメイン ・ ネーム登録を提供しています-購入および example.com などのドメイン名を管理することができ、アマゾン ルート 53 は自動的にあなたのドメインの DNS 設定を構成します。

Helpコマンド
----------------------

このコマンドは、アマゾンのルート 53 の使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSRoute53 help

 ******************************


    This is an extension provided for Handling AWS ROUTE53.

    AWSRoute53, awsroute53, aws-route53

        - create-hosted-zone
        Lets you add Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 create-hosted-zone
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess
          - delete-hosted-zone
        Lets you delete Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess
         - delete-health-check
        Lets you delete Health Check to AWS Route53
        example: ptconfigure AWSRoute53 delete-health-check
                    --yes
                    --guess

        - list
        Will display data about your AWS Route53
        example: ptconfigure AWSRoute53 list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-hosted-zone 
---------------------------

このコマンドは、AWS Route53 にホストされているゾーンを追加するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess

Create-health-check 
---------------------------

このコマンドは、AWS Route53 にヘルス チェックを追加するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check --yes --guess

Delete-hosted-zone 
---------------------------

このコマンドは、AWS Route53 にホストされるゾーンを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 

Delete-health-check 
-------------------------

このコマンドは、AWS Route53 へのヘルス チェックを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     
	
	ptconfigure AWSRoute53 delete-health-check --yes --guess

List
---------

このコマンドは、AWS Route53 についてのデータを表示するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSRoute53 list --yes --guess


代替パラメータ
----------------
  
コマンドラインで使用できる 3 つの代替パラメーターがあります。

AWSRoute53, awsroute53, aws-route53 

メリット
--------------

高い信頼性と可用性： アマゾン ルート 53 AWS の可用性と信頼性の高いインフラストラクチャを使用しています。我々 の DNS サーバーの分散性質、エンドユーザー アプリケーションにルーティングする一貫した能力を確保するために役立ちます。国道 53 号線は重要なアプリケーションに必要な信頼性のレベルを提供するために設計されています。アマゾン ルート 53 アマゾン ルート 53 サービス レベル契約によってバックアップされます。

拡張性： 国道 53 号線を自動的にスケーリングするからの介入なしの非常に大きなクエリ ボリュームを処理するために設計されています。

その他 Amazon Web サービスで使用するために設計された： アマゾン ルート 53 は他 AWS 機能と製品とよく動作するように設計されています。アマゾン ルート 53 を使用して、Amazon EC2 インスタンス、Amazon S3 のバケット、アマゾン CloudFront ディストリビューションおよび他 AWS リソースへのドメイン名をマップできます。アマゾン ルート 53 AWS のアイデンティティ管理とアクセス管理 (IAM) サービスを使用して、DNS データを更新できるユーザーを細かく粒状制御を得る。アマゾン ルート 53 を使用するには、ゾーンの頂上 (www.example.com 対 example.com) 弾性負荷分散インスタンス、アマゾン CloudFront ディストリビューションまたはエイリアス レコードと呼ばれる機能を使用して Amazon S3 web サイトのバケットにマップします。

シンプル： セルフ サービス サインアップ、ルート 53 分以内、DNS クエリに応答を開始できます。AWS 管理コンソールまたは私たちの使いやすい API で DNS 設定を構成できます。また、プログラムで、web アプリケーション全体にルート 53 API を統合できます。たとえば、ルート 53 API を使用して、EC2 インスタンスを新しく作成するたびに、新しい DNS レコードを作成することができます。

高速： 世界中の DNS サーバーのグローバルなエニー キャスト ネットワークを使用して、アマゾン ルート 53 はネットワークの状態に応じて最適な場所にユーザーを自動的に回覧する設計されています。この結果、エンド ・ ユーザーのための低いクエリの待機時間として DNS レコード管理のニーズのための安値更新遅延、サービス提供しています。

費用対効果： アマゾン ルート 53 AWS のスケール メリットでを渡します。ドメイン サービスと、サービスは各ドメイン、低コストで、最低利用約束または任意のアップ フロント料なしの応答クエリ数を管理するためにのみ支払います。

保護： 統合によりアマゾン ルート 53 AWS アイデンティティとアクセス管理 (IAM)、一意の資格情報を付与し AWS アカウント内のすべてのユーザーのアクセス許可を管理し、できますアマゾン ルート 53 サービスの部分へのアクセスを持つユーザーを指定します。

柔軟性： アマゾン ルート 53 加重ラウンドロビン （WRR）、DNS 負荷分散とも呼ばれますを提供しています。これはあなたのトラフィックのどの部分がさまざまなエンドポイントにルーティングを指定する DNS レコードに重みを割り当てることができます。

