==========
Memcached
==========

概要
---------------

このモジュールの主要な側面は、最新バージョンでmemcacheのをインストールし、更新することです。
Memcachedのは、汎用の分散メモリキャッシュシステムです。それは頻繁に読み取らなければならない（例えば、データベースまたはAPIなどの）外部データソースの回数を減らすためにRAM内のデータおよびオブジェクトをキャッシュすることにより、動的なデータベース駆動型のWebサイトを高速化するために使用される。

私たちは今後のトピックでは、このモジュールのインストールと使用のプロセスについて見てみましょう。



helpコマンド
---------------------

helpコマンドは、とだけでなく、Memcachedのモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それは、Memcachedのモジュールの別のパラメータを示しています。また、Memcachedのモジュールをインストールするための構文について説明します。 Memcachedのモジュールのhelpコマンドは以下の通りである。

.. code-block:: bash 

	ptconfigure Memcached help 

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、Memcachedの下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash 

 kevell@corp:/# ptconfigure Memcached help 

 ****************************** 


  This command allows you to update Memcached. 

  Memcached, memcached 

        - install 
        Installs the latest version of memcache 
        example: ptconfigure memcached install 

 ------------------------------ 
 End Help 
 ****************************** 

インストール
----------------

ユーザーがマシンにMemcachedのをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash 

	ptconfigure memcached install 


表形式で示すように、上記のコマンドを入力した後、次の処理が発生します。


.. cssclass:: table-bordered

 +--------------------------+-------------------------------+-------------+--------------------------------------------+
 | パラメーター             | 代替パラメータ                | オプション  | コメント                                   |
 +==========================+===============================+=============+============================================+
 |Install Memcached? (Y/N)  | memcached, Memcached          | Y(Yes)      | ユーザーは、Yと入力することができ、        |
 |                          |                               |             | インストールプロセスを続行したい場合       |
 +--------------------------+-------------------------------+-------------+--------------------------------------------+
 |Install Memcached? (Y/N)  | memcached, Memcached          | N(No)       | ユーザーは、Nと入力することができ、        |
 |                          |                               |             | インストールプロセスを終了したい場合は|    |
 +--------------------------+-------------------------------+-------------+--------------------------------------------+


次のスクリーンショットは、あなたのインストールのプロセスに関する絵画的表現を与えることができます。


.. code-block:: bash 

memcachedのの機能
-------------------------------

memcachedのを使用している間、プロセスは読み、memcachedのに含まれている以下の機能を実装することができ、

 
* Memcache::add --サーバーにアイテムを追加 
* Memcache::addServer --接続プールにmemcachedサーバを追加します。
* Memcache::close --memcachedサーバとの接続を閉じる
* Memcache::connect --memcachedサーバへの接続をオープンする
* Memcache::decrement --デクリメント項目の値
* Memcache::delete --サーバーから項目を削除する
* Memcache::flush --サーバーのすべての既存項目をフラッシュします
* Memcache::get --サーバーからアイテムを取得する
* Memcache::getExtendedStats --プール内のすべてのサーバの統計情報を取得する
* Memcache::getServerStatus --サーバーの状態を返します。
* Memcache::getStats --サーバーの統計情報を取得する
* Memcache::getVersion --サーバーのバージョンを返す
* Memcache::increment --インクリメント項目の値
* Memcache::pconnect --オープンmemcachedサーバの持続的な接続
* Memcache::replace --既存の項目の値を置き換え
* Memcache::set --データをサーバに格納する
* Memcache::setCompressThreshold --大きな値の自動圧縮を有効にする 
* Memcache::setServerParams --実行時にサーバのパラメータとステータスを変更します 

メリット
------------

* ヘルプとインストールで使用されるパラメータは、他の人に比べながら、追加的な利点である大文字と小文字を区別しません。
* これは、Ubuntuと同様にセントOSの両方に裕福なです。 
* この意志モジュールが更新されたバージョンでのmemcachedをインストールします。
* モジュールがすでにユーザマシン内に存在されている場合は、それがすでに存在しているようにメッセージが表示されます。

