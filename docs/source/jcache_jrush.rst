=========
Cache
=========


概要
-----------------

Jrush 補助一時的なメモリ内のキャッシュをクリアします。キャッシュの 2 種類があります。しかし、自分の名前で指定されているさまざまな機能を持つ両方。彼らは明確なサイトと明確な管理者です。Ubuntu で、セント満足です OS。ファイル、フォルダーおよびアプリケーションを削除して一時メモリからデータを消去する--場合つもりはトリックをしないリサイクル コンテンツされませんお使いのコンピューターで利用できます。

Helpコマンド
--------------------------

ヘルプ コマンド処理と同様、決定に関するユーザーとしてキャッシュに含まれているオプションについて。出力キャッシュの代替パラメーターが表示されます。また、Jrush モジュールの機能の構文について説明します。キャッシュのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		jrush cache help

コマンドの入力後それとしてアクション オプションを示します。次の図は、際立ってそれを想定します。

.. code-block:: bash

 kevell@corp:/# jrush cache help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to clear Cache.

  Cache, cache

        - site-clear
        Deletes a user
        example: jrush cache site-clear

        - admin-clear
        Clear the administrator cache
        example: jrush cache admin-clear

 ------------------------------
 End Help
 ****************************************

 
代替パラメータ
--------------------------------

一方で、ユーザーのキャッシュを使用して、次のオプションを授けることができます。

Cache, cache.

オプション
-------------

2 つのオプションが利用できます。彼らの次のとおりです。

* Site-clear 
* Admin-clear

今、私たちは両方のオプションについて知ってみましょう。

Site-clear
--------------

サイト明確です costoff ユーザーを削除します。次のコマンドは、サイトをオフに使用されます。


.. code-block:: bash

		jrush cache site-clear 

コマンドは、上記と入力後に、コーディングのような出力来る。終わりキャッシュ クリア完了を表示できます。スクリーン ショットでは、同じ。

.. code-block:: bash

 kevell@corp:/# jrush cache site-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["site_cache_clear"]=>
  string(19) "Site Cache Clearing"
  ["site_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************

Admin-clear
-------------------

着用この管理者のキャッシュをクリアします。コマンドは、サービスを次のように、管理者を解除するユーザー。

.. code-block:: bash

		jrush cache admin-clear

次の画面ショットは admin クリア機能についてユーザーを指示します。

.. code-block:: bash

 kevell@corp:/# jrush cache admin-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["admin_cache_clear"]=>
  string(20) "Admin Cache Clearing"
  ["admin_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************


メリット
---------------

* Ubuntu で、セント運動に満足それ OS。
* 非大文字小文字を区別します。
* それは中古ユーザーを削除します。
* それは明確な管理者ことができます。



