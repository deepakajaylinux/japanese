===================
Amazon ElastiCache
===================

概要
-------------

ElastiCacheは、それが簡単に展開、運用、およびクラウドにおけるメモリ内キャッシュを拡張することができますWebサービスです。サービスは、高速で管理され、インメモリキャッシュから情報を取得できるようにするのではなく、低速のディスクベースのデータベースに完全に依存することにより、Webアプリケーションのパフォーマンスを向上させます。 ElastiCacheは、2つのオープンソースのインメモリ·キャッシングエンジンをサポートしています。
Memcachedの - 広く採用されているメモリオブジェクトキャッシュシステム。 ElastiCacheはmemcachedのに準拠したプロトコルで、既存のMemcached環境と今日を使用するので、人気のあるツールは、サービスとシームレスに動作します。

€âRedisの「そのようなソートされたセットやリストなどのデータ構造をサポートしています人気の高いオープンソースのインメモリキーと値のストア。 ElastiCacheは、クロスAZの冗長性を達成するために使用することができるマスタ/スレーブのレプリケーションとマルチAZをサポートしています。

アマゾンElastiCacheは、自動的に検出し、置き換え失敗したノードを、自己管理インフラストラクチャに関連するオーバーヘッドを削減し、オーバーロードされたデータベースのリスクを軽減弾性システム、遅いウェブサイトやアプリケーションのロード時間を提供します。アマゾンCloudWatchのとの統合を通じて、アマゾンElastiCacheは、あなたのMemcachedのか、Redisのノードに関連する主要なパフォーマンスメトリックに強化された可視性を提供します。

アマゾンElastiCacheはを使用して、AWS管理コンソールを使用して、数分であなたのインフラストラクチャにインメモリキャッシュ層を追加することができます。

helpコマンド
----------------------

このコマンドは、アマゾンElastiCacheはの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSElastiCache help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    AWSElastiCache, awselasticache, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache create-cache-cluster
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess

          - reboot-cache-cluster
        Lets you reboot cache Cluster to AWS ElastiCache
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess

         - delete-cache-cluster
        Lets you delete cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure AWSElastiCache list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

CREATE-キャッシュクラスタ
---------------------------

このコマンドは、AWS ElastiCacheは、キャッシュクラスタを追加することができます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash

	ptconfigure AWSElastiCache create-cache-cluster â€“yes --guess 

CREATE-ヘルスチェック
---------------------------

このコマンドは、AWS Route53にヘルスチェックを追加することができます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check â€“yes â€“guess

再起動キャッシュ·クラスタ
------------------------------------------

このコマンドは、AWS ElastiCacheは、キャッシュクラスタを再起動するのに役立ちます。

.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 

削除キャッシュ·クラスタ
--------------------------------------

このコマンドは、AWS ElastiCacheは、キャッシュクラスタを削除するのに役立ちます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash     
	
	ptconfigure AWSElastiCache delete-cache-cluster --yes --guess

削除·複製グループ
-----------------------------------

このコマンドは、AWS ElastiCacheは、レプリケーショングループを削除するのに役立ちます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash 
	
	ptconfigure AWSElastiCache delete-replication-group --yes --guess
            
リスト
---------------------

このコマンドは、あなたのAWS ElastiCacheは約表示データを表示することができます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash 

	ptconfigure AWSElastiCache list --yes --guess

代替パラメータ
------------------------------

コマンドラインで使用することができる3つの代替のパラメータがある。

AWSElastiCache, awselasticache, aws-elasticache

メリット
--------------

デプロイメントするためのシンプル：アマゾンElastiCacheは、それは非常に簡単にMemcachedのか、Redisの対応のキャッシュ環境を展開することができます。 AWS管理コンソールを使用するか、単純なAPIは、インフラストラクチャのプロビジョニングを心配する、またはインストールするとキャッシュソフトウェアを維持することなく、数分で量産対応のクラウドキャッシュ·クラスタの機能にアクセスするために呼び出します。


管理：アマゾンElastiCacheは、パッチ管理、障害検出し、より価値の高いアプリケーション開発を追求することができrecovery--として--such時間のかかる管理タスクを自動化します。


互換性：アマゾンElastiCacheは使用すると、Memcachedのか、Redisのインメモリ·キャッシング環境へのネイティブアクセスを得る。これは、あなたの既存のツールやアプリケーションとの互換性を容易にします。


弾性：シンプルなAPI呼び出しまたはAWS Management Consoleの数回クリックすると、あなたのアプリケーションの負荷を満たすためにあなたのクラウド·キャッシュ·クラスタにキャッシュノードを追加または削除することができます。 Memcachedのための自動検出は、ノードがアマゾンElastiCacheはクラスタに追加または削除されるElastiCacheはクライアントでキャッシュノードの自動検出を可能にします。


信頼性の高い：アマゾンElastiCacheは、自動障害検出とリカバリなどの重要な生産の展開のための信頼性を高める複数の機能を備えています。アマゾンElastiCacheは、他のAmazon Webサービスによって使用されるのと同じ信頼性の高いインフラストラクチャ上で実行されます。


統合：アマゾンElastiCacheはアマゾンのリレーショナル·データベース·サービス（Amazon RDSは）、アマゾンDynamoDBは、アマゾン弾性計算クラウド（Amazon EC2で）、アマゾンCloudWatchの、とAmazonシンプル通知サービス（アマゾンSNS）など、他のAmazon Webサービス、とのシームレスな使用のために設計されています。


セキュア：アマゾンElastiCacheは、あなたのキャッシュ·クラスタを確保するために多くのメカニズムを提供します。

アマゾンElastiCacheは、あなたのキャッシュへのネットワークアクセスを制御するファイアウォールの設定を構成できるようにWebサービス·インターフェースを提供しています クラスタ。

アマゾンElastiCacheはあなたがAmazonで仮想プライベートクラウド（アマゾンVPC）であなたのキャッシュ·クラスタを実行することができます。アマゾンVPCは、IPを指定することで、あなたのキャッシュ·クラスタを隔離することができます、あなたのキャッシュノードに使用する、とAmazon VPC内部の既存のアプリケーションに接続したいの範囲である。 VPCでアマゾンElastiCacheは詳細については、アマゾンElastiCacheはユーザガイドを参照してください。

費用対効果：アマゾンElastiCacheははあなたにセットアップし、マルチノードキャッシュ·クラスタを管理するための管理コストを節約できます。あなたは、あなたが実際に消費するリソースを払って、スケールアップし、アプリケーションの使用パターンの変化に応じて最適なパフォーマンスを実現するために、あなたのキャッシュ·クラスタ内のキャッシュノードの数を縮小することができます。オンデマンドの価格設定では、無長期的なコミットメントを時間単位でメモリ/計算処理能力のために支払うことができます。これはアマゾンElastiCacheはの使用は非常に効果的なコストと計画、購買のコストと複雑さからあなたを解放して、ハードウェアを維持することができます。


マルチAZ：アマゾンElastiCacheははRedisのエンジンとマルチAZ機能のレプリケーション機能を提供します。あなたは、単一のキャッシュノードの容量制限を超えて利用可能性、およびスケールを得るために、複数のAWS利用可能ゾーンを利用することができます。プライマリノード損失の場合には、ElastiCacheは、自動的に手動の介入を必要とせずに、より高い可用性を提供するために、読み取りレプリカに失敗し、フェールオーバーを検出します。


バックアップと復元：RedisのためのアマゾンElastiCacheは、あなたのクラスターのスナップショットを作成して、データを保護するのに役立ちます。コンソールまたはシンプルなAPI呼び出しに数回のクリックを経由して、自動スナップショットを設定するだけでなく、あなたが選択するたびにバックアップを開始することができます。スナップショットは、その後Redisのクラスタのための新しいElastiCacheはをシードするために使用することができます。


キーユースケース：アマゾンElastiCacheはが大幅に（そのようなソーシャルネットワーキング、ゲーム、メディア共有とQ＆Aポータルなど）は、多くの読み取り重いアプリケーションワークロードまたは（例えば、リコメンデーション·エンジンなど）を計算集約型のワークロードの待ち時間とスループットを改善するために使用することができます。キャッシングは、低遅延アクセスのためにメモリ内のデータの重要な部分を格納することで、アプリケーションのパフォーマンスが向上します。キャッシュされた情報は、I / O集中型データベースクエリの結果や計算集約計算の結果を含むことができる。データ構造·サーバを必要とするアプリケーションは、Redisのエンジンは最も有用でしょう。
