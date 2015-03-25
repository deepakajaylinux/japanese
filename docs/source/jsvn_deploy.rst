=======
SVN
=======


概要
------------

このモジュールはチェック アウト関数の処理で、ユーザーを支援します。Apache Subversion (頻繁に短縮された SVN、コマンド svn の名の後) は、Apache ライセンスの下でフリー ソフトウェアとして配布ソフトウェア バージョンとリビジョン コントロール システムです。[1] 開発者はソース コード、web ページ、およびドキュメントなどのファイルの現在と過去のバージョンを維持するために Subversion を使用します。その目標は、広く使われている並行版システム (CVS) に大抵互換性がある後継者であります。私たちを見てみましょうどのようにこのモジュール処理チェック アウト関数で容易にします。

Helpコマンド
---------------------

Help コマンドと同様、目的に関するユーザー ガイドとして SVN で含まれているオプションについて。それは SVN の代替パラメーターが一覧表示されます。また、チェック アウト機能を使用する構文について説明します。SVN モジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash

		ptdeploy svn help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、SVN の下で help コマンドについて視覚化します。

.. code-block:: bash

 kevell@corp:/# ptdeploy svn help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  Checkout, checkout, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************

チェックアウト機能を使用する方法
-------------------------------------------

Svn の下で機能をチェックを使用する構文は以下の通りです。


.. code-block:: bash

		ptdeploy svn co https: // svnhub.com/ phpengine/yourmum



上記のコマンドを入力し、チェック アウト機能の実行が開始で説明するようにテーブルの下で


.. cssclass:: table-bordered

 +----------------------------+--------------------------------------------+------------+-------------------------------------------+
 | パラメータ                 | 代替パラメータ                             | オプション | 注釈                                      |
 +============================+============================================+============+===========================================+
 |Perform a clone/download    | 代わりにCOが、我々は使用することができます | Y(Yes)     | ユーザは、 Yと彼らができるファイルの      |
 |of files? (Y/N)             | checkout, Checkout また                    |            | 複製/ダウンロード入力を行う必要がある場合 |
 +----------------------------+--------------------------------------------+------------+-------------------------------------------+
 |Perform a clone/download    | 代わりにCOが、我々は使用することができます | N(No)      | ユーザーがファイルのクローン/ダウンロ     |
 |of files? (Y/N)             | checkout, Checkout また                    |            | ードを実行する必要性でない場合には、      |
 |			      |					           |            | それらはN.として入力することができ|       |	
 +----------------------------+--------------------------------------------+------------+-------------------------------------------+

ユーザー Y と入力してチェック アウト機能が進むとすると、以下のとおり、次の手順に関与しています。

Step 1:

Also change permissions/owner? (Y/N)

ユーザー Y または N とアクセス許可の所有者を変更する彼らの自発性によってとして入力する必要があります。

Step 2:

What user is Apache Web Server running as?

ユーザーは、apache web サーバーを実行しているユーザーの名前を入力する必要があります。

Step 3:

それはフォルダーのアクセス許可、フォルダーの所有者を変更するプロセスを含みます。

次のスクリーン ショットは、プロセスとチェック アウト機能の働きについて絵を示しています。

.. code-block:: bash




メリット
-----------

* それは裕福な両方の ubuntu と同様セント OS のように。
* 宣言で使用されるパラメーターの大文字と小文字は区別されません。
* ユーザーは、実行し、この SVN を使用してチェック アウト機能を監視できます。

