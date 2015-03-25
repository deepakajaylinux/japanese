==============
Project
==============

概要
-------------

現代ビジネスと科学の共同企業、関係の研究やデザインなど、プロジェクトが定義されている慎重に特定の目的を達成するために予定です。プロジェクトは、さらに永久的な社会システム、または内または時間の制約の下で特定のタスクを達成するために組織間のチームによって構成され作業システムではなく一時として定義することができます。進行中のプロジェクトは通常と呼ばれるに発展する) プログラム。

このコマンドの既定のモジュールの一部であるし、プロジェクトの初期化機能を処理する、プロジェクト、またはプロジェクト コンテナーを構成して、ジェンキンスさんもインストールのような組み込むファイル ジェンキンス インスタンスを実行します。


Helpコマンド
----------------------

このコマンドは、プロジェクト モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
	
		ptdeploy project help
       

 kevell@corp:/# ptdeploy Project help
 ******************************


  This command is part of Default Modules and handles Project initialisation functions, like configuring a project, or a project
  container and also installing Jenkins build files into a running Jenkins instance.

  Project, project, proj


          - container
          make a container folder for revisions (like /var/www/applications/*APP NAME*)
          example: ptdeploy proj container
          example: ptdeploy proj container --yes --proj-container="/var/www/applications/the-app"

          - init
          initialize Dapper project
          example: ptdeploy proj init
          example: ptdeploy proj init --yes

          - build-install
          copy jenkins project stored in repo to running jenkins so you can run builds
          example: ptdeploy proj build-install
          example: ptdeploy proj build-install
                        --jenkins-fs-dir=/var/lib/jenkins # --guess will set this to /var/lib/jenkins
                        --original-build-dir="/var/www/applications/the-app/build/config/ptconfigure/Project/jenkins-builds"
                        --target-job-name="Project_Build"
                        --new-job-dir="Project_Build_Alternate_Name"  # If target one is not available

 ------------------------------
 End Help
 ******************************


Container
----------------

このコマンドは、改定のコンテナー フォルダーを作ることができます （のように/var/www/アプリケーション/* アプリ名 * )。

インストールする必要があるとき、ユーザーは DBIstall のため、次のコマンドを発行できます。システムがインストールの手順を実行します。


.. code-block:: bash
	
		 ptdeploy proj container

 kevell@corp:/# ptdeploy proj container
 Do you want to Modify Project Container Settings? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project Container? (Y/N) 
 Y
 What is your Project Container directory?
 /root/gg
 Project Container directory created
 /root/gg space /root/ggMoving to Container
 /root/gg
 Showing Container Directory
 Project Container file created
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



init
----------------

Dapper のプロジェクトを初期化する必要があるとき、ユーザーは、次のコマンドを発行できます。システムは、プロセスを実行します。


.. code-block:: bash
	
		 ptdeploy proj init


.. code-block:: bash

 kevell@corp:/# ptdeploy proj init
 Do you want to Modify Project Settings To initialise Project? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project? (Y/N) 
 Y
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



Build-Install
----------------

ユーザーがジェンキンス プロジェクト実行ジェンキンスさんにレポに格納されたコピー、ユーザーは、次のコマンドを発行できます。システムは、プロセスを実行します。


.. code-block:: bash
	
		 ptdeploy proj build-install

代替パラメータ
--------------------------------        

コマンドで使用できる 2 つの代替パラメーターがあります。

Project, project and proj

eg: ptdeploy Project help/  ptdeploy proj help
                       
メリット
--------------

* やすく改訂コンテナー フォルダー 
* dapper プロジェクトを初期化するのに役立ちます


