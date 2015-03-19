===================
Amazon CloudWatch
===================

概要
-------------

アマゾンCloudWatchのは、AWSクラウドリソースとあなたはAWS上で実行されるアプリケーションの監視サービスです。あなたが収集し、メトリックを追跡し、収集し、ログファイルを監視し、アラームを設定するためにアマゾンCloudWatchのを使用することができます。アマゾンCloudWatchのは、Amazon EC2インスタンス、アマゾンDynamoDBのテーブル、とAmazon RDS DBインスタンス、だけでなく、あなたのアプリケーションやサービスによって生成されたカスタムメトリック、およびアプリケーションが生成するログ·ファイルなどのAWSリソースを監視することができます。あなたは、リソース使用率、アプリケーションのパフォーマンス、および運用健康にシステム全体の可視性を得るためにはAmazon CloudWatchのを使用することができます。あなたが反応し、スムーズに実行しているアプリケーションを維持するためにこれらの洞察を使用することができます。

helpコマンド
----------------------

このコマンドは、アマゾンCloudWatchのの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudWatch help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  AWSCloudWatch, aws-cloud-watch, aws-cloudwatch

        - install
        Installs AWSCloudWatch. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudWatch
        example: ptconfigure aws-cloudwatch install

 ------------------------------
 End Help
 ******************************

インストール
----------------

ユーザーがマシンにアマゾンCloudWatchのモジュールをインストールする必要がある場合は、以下のコマンドは、インストールのプロセスを実行します。

.. code-block:: bash
        
        ptconfigure aws-cloudwatch install

.. code-block:: bash 

メリット
--------------

追加料金なしのためのAmazon EC2インスタンスからCPU使用率、データ転送、およびディスクの使用状況活性（基本的な監視）用の表示メトリック：Amazon EC2のを監視します。追加料金で、CloudWatchのは、高解像度化、メトリックの集計でEC2インスタンスの詳細な監視を提供します。追加のソフトウェアをインストールする必要はありません。

アマゾンDynamoDBのテーブル、アマゾンEBSボリューム、Amazon RDSは、DBインスタンス、Amazon Elastic MapReduceはジョブフロー、弾性ロードバランサ、アマゾンSQSキュー、アマゾンのSNSのトピックに関するメトリックを監視し、追加料金なしのためのより：他のAWSリソースを監視。追加のソフトウェアをインストールする必要はありません。

カスタムメトリックを監視：シンプルなAPIリクエストを経由して、独自のアプリケーションによって生成されたカスタムメトリックを提出し、それらをアマゾンCloudWatchので監視がある。あなたがトラブルとスポットを助けるためにあなたの€アプリケーションの€の™sの操作性能にとって重要なメトリックを送信して保存することができます
傾向。

監視し、ストアログ：あなたはあなたの既存のシステム、アプリケーション、およびカスタムログファイルを使用して、システムとアプリケーションを監視し、トラブルシューティングするためにCloudWatchのログを使用することができます。あなたはCloudWatchのログへの既存のシステム、アプリケーション、およびカスタムログファイルを送信し、ほぼリアルタイムで、これらのログを監視することができます。これは、あなたがより良いあなたのシステムとアプリケーションを理解し、操作することができ、あなたは、後でアクセスするための高耐久性、低コストのストレージを使用して、ログを保存することができます。

アラームを設定：あなたの測定基準のいずれかに設定したアラームはあなたに通知を送信したり、他の自動アクションを実行する。たとえば、特定のAmazon EC2のメトリックは、あなたのアラームしきい値を超えたとき、あなたは動的に追加または削除EC2インスタンスを、またはあなたに通知を送信するオートスケーリングを使用することができます。

ビューグラフと統計：ビューのグラフとAmazon CloudWatchのダッシュボード上のあなたの測定基準のいずれかの統計情報、および、すべてのアラームの概要を取得し、一箇所にAWSリソースを監視した。
