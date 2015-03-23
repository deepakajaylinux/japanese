=================
AWS RDS 
=================

概要
-------------

アマゾンのリレーショナル データベース サービス (Amazon RDS) は簡単に設定すると、web サービスの操作、およびリレーショナル データベース、クラウドのスケールします。アプリケーションやビジネスに焦点を当てるまであなたを解放する、時間のかかるデータベース管理タスクを管理しながらのコスト効率の高いサイズ変更可能な容量を提供します。

Amazon RDS MySQL、Oracle、Microsoft SQL Server、PostgreSQL は、またはアマゾンのオーロラのリレーショナル データベース管理システムの機能へのオンライン アクセスを与えます。つまり、Amazon rds. とコード、アプリケーション、およびツールを既に使用している今日、既存のデータベースを使用することができます。Amazon RDS は自動的にパッチ データベース ソフトウェアとデータベースをバックアップする、バックアップを格納するユーザー定義の期間のため、ポイント ・ イン ・ タイム ・ リカバリを有効にします。コンピューティング リソースまたは 1 回の API 呼び出しを介してデータベース インスタンス （DB インスタンス) に関連付けられているストレージ容量を拡張することができるという柔軟性を恩恵を受ける。

Amazon RDS MySQL、Oracle、SQL Server、PostgreSQL のエンジンを使用してデータベース インスタンスは一般目的 （SSD） ストレージ、プロビジョニング IOPS （SSD） ストレージ、または磁気記憶装置でプロビジョニングすることができます。アマゾン オーロラ エンジンを使用してデータベース インスタンスはセルフヒー リング データベース ワークロードに関して特化した SSD バックアップ仮想化ストレージ レイヤー、フォルト ・ トレラントな採用しています。

さらに、Amazon RDS の可用性と運用環境のワークロードの信頼性を強化するために使用するレプリケーションなります。実行することができますマルチ AZ 展開オプションを使用するミッション ・ クリティカルなワークロードが故障した場合の同期的にレプリケートされたセカンダリ データベースをプライマリ データベースから内蔵自動フェールオーバーと高可用性を実現します。読み取りのレプリカを使用して、MySQL、PostgreSQL は、およびアマゾン オーロラ Amazon RDS もできます読み取り重いデータベース ワークロードの配置を 1 つのデータベースの容量を超えてスケール アウト。すべての Amazon Web サービスと同様、必要な先行投資がないと使用するリソースに対してのみ支払います。

Helpコマンド
----------------------

このコマンドは Amazon rds. の使用状況を判断するのに役立ちますユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

 kevel@corp:/# ptconfigure Amazon RDS help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    Amazon RDS, Amazon RDS, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure Amazon RDS create-cache-cluster
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
        example: ptconfigure Amazon RDS delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure Amazon RDS delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure Amazon RDS list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Describe-instance 
---------------------------

このコマンドは AWS rds. のインスタンスを記述するのに役立ちます特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
	ptconfigure AWSRDS describe-instance --yes --guess 


Delete-instance 
---------------------------

このコマンドは、インスタンスを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash
	
	ptconfigure AWSRDS delete-instance --yes --guess

Create-db-snapshot 
---------------------------

このコマンドにより再起動する db スナップショットを作成します。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     

	ptconfigure AWSRDS create-db-snapshot --yes --guess 


Delete-db-snapshot 
-------------------------

このコマンドは、データベース スナップショットを削除するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash     
	
	ptconfigure AWSRDS delete-db-snapshot –yes –guess

Copy-db-snapshot 
-----------------------------------

このコマンドは、db のスナップショットをコピーするのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 
	
	ptconfigure AWSRDS copy-db-snapshot --yes --guess
        
Create-instance
------------------------

このコマンドは、インスタンスを作成するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSRDS create-instance --yes –guess

Reboot-instance
------------------------

このコマンドは、インスタンスを再起動するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSRDS reboot-instance --yes --guess

Create-instance-read replica
--------------------------------------

このコマンドは、db インスタンスのレプリカを読み取りを作成するのに役立ちます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSRDS create-instance-readreplica --yes --guess

List
---------

このコマンドにより、AWS rds. に関するデータを表示できます。特定のコマンドの下、プロセスが実行されます。

.. code-block:: bash 

	ptconfigure AWSRDS list --yes --guess

代替パラメータ
------------------------------       

コマンドラインで使用できる 3 つの代替パラメーターがあります。

AWSRDS, awsrds, aws-rds 

メリット
--------------

データベース、Web サービスを配置する単純な: Amazon RDS を簡単に展開するプロジェクトの概念から行きます。AWS 管理コンソールまたは単純な API 呼び出しを使用して、インフラストラクチャのプロビジョニングやデータベース ソフトウェアのインストールと保守について心配することがなく分生産準備のリレーショナル データベースの機能にアクセスします。

管理: Amazon RDS 時間のかかるデータベース管理タスクを処理、バックアップ、パッチ管理、レプリケーションなど高い値アプリケーション開発またはデータベースの改良を追求することができます。

互換性: Amazon RDS のネイティブ アクセスを取得するリレーショナル データベース管理システム。これは、既存のツールやアプリケーションとの互換性を促進します。さらに、Amazon RDS 制御できますオプション DB エンジン バージョン管理による DB インスタンスのエンジン バージョン力を支えた。
高速で予測可能なパフォーマンス： データベース インスタンス Amazon RDS の MySQL を使用して Oracle、SQL Server、および Oracle エンジン プロビジョニングできる一般目的 （SSD） ストレージ、プロビジョニング IOPS （SSD） ストレージ、または磁気記憶装置と。
Amazon RDS 一般目的 （SSD） ストレージ ・ プロビジョニングされた GB あたり 3 IOPS の一貫性のあるベースラインを提供最大 3,000 IOPS をバーストする能力を提供しています。

Amazon RDS プロビジョニング IOPS （SSD） ストレージ I/O の集中的なトランザクション データベースのワークロードの高速で予測可能な一貫したパフォーマンスを提供するために設計された高パフォーマンスのストレージ オプションです。30,000 IOPS DB インスタンスごとに 1,000 IOPS からプロビジョニングできます。（最大） が実現 IOPS はエンジンの種類によって異なります。
磁気記憶装置 (以前 Amazon RDS 標準ストレージとして知られている) データがそれほど頻繁にアクセスされる小さなデータベース ワークロードに適しています。

アマゾン オーロラ エンジンを使用してデータベース インスタンスはセルフヒー リング データベース ワークロードに関して特化した SSD バックアップ仮想化ストレージ レイヤー、フォルト ・ トレラントな採用しています。

クラウドのスケーラブルなデータベース: 計算をスケールすることができ、ストレージ ・ リソースをあなたのアプリケーションを満たすためにデータベースに使用できる Amazon RDS API または AWS 管理コンソールを使用して必要があります。プロビジョニングし、最大ストレージをスケールすることができます Amazon RDS と共に MySQL、Oracle、または PostgreSQL Amazon RDS プロビジョニング IOPS ストレージを使用する場合に最大 30,000 IOPS と 3 TB です。その最大実現 IOPS はエンジンの種類によって異なります注意してください。さらに、MySQL、PostgreSQL とアマゾン オーロラ データベース エンジンを関連付けることもできます 1 つ以上の読み取りレプリカ、データベース インスタンスの展開を読み取り重いワークロードを 1 つのデータベース インスタンスの容量を超えて拡張することができます。

アマゾン オーロラ データベース エンジンは、ストレージを拡張することができます最大 64 TB です。データベース インスタンスの配置を最大 15 アマゾン オーロラ レプリカを関連付けることができます。アマゾン オーロラ レプリカ共有ソース インスタンスとして同じ基になるストレージのコスト削減とレプリカ ノードにデータをコピーする必要を回避します。

信頼性： Amazon RDS は自動バックアップ、DB スナップショット、自動ホスト交換マルチ AZ 展開など重要な本番データベースの信頼性を向上させる複数の機能。Amazon RDS 他 Amazon の Web サービスで使用される同じ信頼性の高いインフラストラクチャで実行されます。

アマゾン オーロラ エンジン Amazon RDS は 3 つの利用可能ゾーンのいずれかで作成した最大 15 のオーロラ レプリカの 1 つへのフェイル オーバーを自動化する RDS マルチ-アリゾナ州技術を使用します。

その他 Amazon Web サービスで使用するために設計された： Amazon RDS は他の Amazon の Web サービスと緊密に統合されます。たとえば、Amazon EC2 で実行されるアプリケーションは Amazon RDS DB インスタンスに同じ地域で低レイテンシのデータベースへのアクセスを発生します。
セキュアな： Amazon RDS あなた DB Instances.Amazon RDS をセキュリティ保護するメカニズムの数は、AWS キー管理サービス (KMS) を通しての管理キーを使用して MySQL 又は PostgreSQL データベースを暗号化することができます提供します。Amazon RDS 暗号化を実行して、データベース インスタンスは、レプリカ、およびスナップショットの読み取りその自動バックアップとして基になるストレージの残りの部分に格納されているデータは暗号化されます。

Amazon RDS には SQL Server と Oracle の透過的なデータ暗号化をサポートします。Oracle での透過的なデータ暗号化を安全に生成、保存、および AWS クラウド内のシングル テナントのハードウェア セキュリティ モジュール (HSM) アプライアンスで暗号化キーを管理することができます AWS CloudHSM と統合されます。

Amazon RDS には、データベースへのネットワーク アクセスを制御するファイアウォール設定を構成する web サービス インターフェイスが含まれています。
Amazon RDS では、DB インスタンス アマゾン仮想プライベート クラウド (Amazon VPC) で実行することができます。Amazon VPC 業界標準暗号化 IPsec VPN を通じてインフラストラクチャ DB インスタンスに既存の接続を使用して、希望する ip アドレスの範囲を指定することによって分離することができます。VPC で Amazon RDS に関する詳細については、Amazon RDS のユーザーズ ガイドを参照してください。

安価な: 非常に低料金を支払うし、あなたが実際に消費するリソースに対してのみです。また、オン ・ デマンドいいえ前払いまたは長期的なコミットメントと価格設定のオプションの恩恵やさらに低い時間別料金私たちの予約価格のオプションを介して。
オンデマンド DB インスタンス – オン ・ デマンド DB インスタンス計算容量ない長期的なコミットメントと時間で支払うことができます。これは、コストと計画、購買、および維持するハードウェアの複雑さから解放し、はるかに小さい変動費によく大規模な固定費とは何です変換します。

予約済み DB インスタンス-予約済み DB インスタンス オプションを選択できる各 DB インスタンスを留保し、その DB インスタンスの 1 時間ごとの使用料に大幅な割引を受け取るのため低い、1 回の支払いを行います。あなたの用途に応じての 3 つの予約済み DB インスタンス タイプ (ライト、媒体と重い利用) を選択し、オン ・ デマンド価格より 30% ～ 55% 割引のどこでも受信できます。

