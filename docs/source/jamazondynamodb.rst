================
Amazon DynamoDB
================

概要
-------------

アマゾンDynamoDBのは、任意の規模で一貫性のある、一桁のミリ秒の遅延を必要とするすべてのアプリケーションのための高速で柔軟なのNoSQLデータベースサービスです。それは完全に管理されているデータベースであり、ドキュメント、キーと値のデータモデルの両方をサポートしています。その柔軟なデータモデルと信頼性の高い性能は、それモバイル、ウェブ、ゲーム、広告、ハイテク、IoTの、および他の多くのアプリケーションのための偉大なフィット感を確認します。

helpコマンド
----------------------

このコマンドは、AWS DynamoDBのの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash


 kevell@corp:/# ptconfigure AWSDynamoDb help

 ******************************


    This is an extension provided for Handling AWSDynamoDb.

    AWSDynamoDb, awsdynamodb,aws-dynamodb

        - describe-table
        Describe a table
        example: ptconfigure AWSDynamoDb describe-table
                    --yes
                    --guess
        - delete-table
        Lets you delete a table
        example: ptconfigure AWSDynamoDb delete-table
                    --yes
                    --guess


        - create-table
          Lets you create a table
          example: ptconfigure AWSDynamoDb create-table
                    --yes
                    --guess




        - list
        Will display data about your AWS AWSDynamoDb
        example: ptconfigure AWSDynamoDb list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************

説明してテーブル
-------------------

このコマンドは、テーブルを記述するのに役立ちます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash

	 ptconfigure AWSDynamoDb describe-table --yes --guess

削除テーブル
-------------------

このコマンドは、テーブルを削除するのに役立ちます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash

	ptconfigure AWSDynamoDb delete-table --yes --guess

作成テーブル
---------------------

このコマンドは、テーブルを作成するのに役立ちます。最も重要な部分は、それは不可逆的である。

.. code-block:: bash     

	ptconfigure AWSDynamoDb create-table --yes --guess 

リスト
---------------------

このコマンドは、あなたのAWS AWSDynamoDbに関するデータを表示するのに役立ちます。以下のコマンドは、プロセスを実行します。

.. code-block:: bash 
	
	ptconfigure AWSDynamoDb list --yes --guess

代替パラメータ
------------------------------

コマンドラインで使用することができる2つの別のパラメータがある。

AWSDynamoDb, awsdynamodb,aws-dynamodb

メリット
--------------

€âセカンダリインデックススキャン」DynamoDBのテーブルをスキャンする簡単な方法：アマゾンDynamoDBはあなたがスキャン操作を使用して、テーブルからすべてのアイテムを取得することができます。セカンダリインデックス·スキャンを使用すると、今セカンダリインデックスでスキャン操作を使用することができ、セカンダリインデックス上に投影されている属性を選択し、項目からすべてのデータを取得する。二次索引スキャンは、グローバルとローカルセカンダリインデックスで動作します。セカンダリインデックスは、DynamoDBのコンソールから、またはインデックスを指定するために追加のパラメータを指定してスキャンAPIを呼び出すことでスキャンすることができます。

€Aオンライン索引作成の「グローバル2次索引を管理するための柔軟な方法：アマゾンDynamoDBはあなたが時間を作成し、テーブルのグローバル2次索引（GSI）を作成することができます。 GSISはフィルタを使用して豊かなクエリを作成することができます。オンラインインデックス作成を使用すると、DynamoDBのコンソールまたはシンプルなAPIの呼び出しを介してを使用して、いつでもDynamoDBのテーブルにGSISを追加または削除することができます。 GSIが追加または削除されている間、DynamoDBのテーブルがまだ生きてトラフィックを処理し、プロビジョニングされたスループットレベルでの継続的なサービスを提供することができます。

DynamoDBはストリームのプレビューにサインアップ：DynamoDBのストリームは、あらゆるDynamoDBのテーブル内のアイテム·レベルの変化の時間順序付けられたシーケンスを提供しています。変更が複製されたDEおよび24時間保存されます。この機能は、クロス領域レプリケーションで赤方偏移の統合、変更通知、および他の多くとの継続的な分析をDynamoDBの拡張を開発者に提供します。
