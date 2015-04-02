===============
GitCommand
===============

概要
-------------

Gitはスピードと効率を持つに小さな非常に大規模なプロジェクトからすべてを処理するように設計され、フリーでオープンソースの分散バージョン管理システムです。


Helpコマンド
---------------

helpコマンドは、とだけでなく、 gitのモジュールに含まれているオプションについての目的について、ユーザーをガイドします。これは、 Gitのモジュールの別のパラメータを示しています。 Gitのモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash

	ptconfigure gitcommand help

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure gitcommand help

 ******************************



  This command handles Git Functionality

  Git, GitCommand, git-command, gitcommand

  - checkout-branch
    checkout a branch
    example: ptconfigure git checkout-branch --branch=*branchname*

  - create-checkout-branch
    checkout a branch, creating a new branch if needed
    example: ptconfigure git create-checkout-branch --branch=*branchname*

  - delete-branch
    delete a branch
    example: ptconfigure git delete-branch --branch=*branchname*
    
  - ensure-branch
    ensure a branch
    example: ptconfigure git ensure-branch --branch=*branchname*
    
  - add
    add new files to a git repository
    example: ptconfigure git add 
	
  - commit
    commit new messages to a git repository
    example: ptconfigure git  commit --message=*some commit message*

  - push
    push to a git repo
    example: ptconfigure git push --branch=*origin yourbranch*
  
  - pull
    pull a git repo
    example: ptconfigure git pull --branch=*origin yourbranch*

 ------------------------------
 End Help
 ******************************


Checkout-branch
-------------------

のgit checkoutコマンドを使用すると、 gitのブランチが作成した枝間を移動することができます。このコマンドは、ブランチをチェックアウトし、実行プロセスは以下の通りです

.. code-block:: bash

	ptconfigure git checkout-branch --branch=*branchname*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************



Create-checkout-branch
---------------------------

Gitの作成チェックアウトの分岐が必要な場合は、新しいブランチを作成し、ブランチをチェックアウトすることができます。このコマンドの実行プロセスは、示されている
以下に、


.. code-block:: bash

	ptconfigure git create-checkout-branch --branch=*branchname*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure git create-checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Attempting to create branch karthi
 Switched to a new branch 'karthi'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************


delete-branch
-----------------

このコマンドは、存在する場合は、ブランチを削除するために使用されます。このコマンドの実行プロセスは、以下に示す

.. code-block:: bash

	ptconfigure git delete-branch --branch=*branchname*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git delete-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell exists, deleting...
 git branch -d mmmm
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


ensure-branch
----------------

このコマンドは、新しいブランチを作成していない場合、分岐が存在することを保証するために用いられる。このコマンドの実行プロセスは、以下に記載されている

.. code-block:: bash

	ptconfigure git ensure-branch --branch=*branchname*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell does not exist, creating...
 Switched to a new branch 'kevell'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Branch karthi already exists, continuing...
 Now in: /opt/ptconfigure-enterprise

 ******************************


 1 : In GitCommand View
 ******************************

Add
------

のgit addコマンドは、 gitリポジトリに新しいファイルを追加するために使用されている。このコマンドの実行プロセスは、以下に記載されている

.. code-block:: bash

	ptconfigure git add 

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git add
 
 Enter the file path to add ? (Enter nothing to add all new & modified files in the git repo).
 test1
 [Pharaoh Logging] All new files in the git repository were added
 ******************************


 0 : In GitCommand View
 ******************************

Commit
---------

このコマンドはgitリポジトリに新しいメッセージをコミットするために使用されます。このコマンドの実行プロセスは、以下に示す

.. code-block:: bash

	ptconfigure git  commit --message=*some commit message*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git commit

 Enter message to commit:
 testing
 [Pharaoh Logging] Git commit successfully
 ******************************


 0 : In GitCommand View
 ******************************


Push
----------

このコマンドはgitリポジトリにファイルをプッシュするために使用されます。このコマンドの実行プロセスは、以下の通りである

.. code-block:: bash

	ptconfigure git push --branch=*origin yourbranch*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure git push

 What branch?
 origin master
 Username for 'https://github.com': muralivel
 Password for 'https://muralivel@github.com': 
 Counting objects: 5, done.
 Delta compression using up to 2 threads.
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (5/5), 394 bytes | 0 bytes/s, done.
 Total 5 (delta 0), reused 0 (delta 0)
 To https://github.com/muralivel/kumar.git
  * [new branch]      master -> master
 [Pharaoh Logging] Git push to branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************


Pull
----------

このコマンドは、 gitリポジトリを引くために使用されます。このコマンドの実行プロセスは、以下に示す

.. code-block:: bash

	ptconfigure git pull --branch=*origin yourbranch*

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash


 kevell@corp:/# ptconfigure git pull

 What branch?
 origin master
 remote: Counting objects: 3, done.
 remote: Compressing objects: 100% (2/2), done.
 Unpacking objects: 100% (3/3), done.
 remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 From https://github.com/muralivel/kumar
 * branch            master     -> FETCH_HEAD
   4f390f3..c3e9feb  master     -> origin/master
 [Pharaoh Logging] Git pull from branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************



別のパラメータ
--------------------------

コマンドラインで使用することができる4つの別のパラメータがある。

Git, GitCommand, git-command, gitcommand


メリット
--------------

* フリー·オープンソース
* 高速と小
* 暗黙のバックアップ
* セキュリティ
* 強力なハードウェアの必要はありません
* 簡単分岐


