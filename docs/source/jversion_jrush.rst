==============
Version
==============


概要
-------------

この記事は様々 な文脈で使われることが「バージョン」という用語についてです。ソフトウェアのバージョンは、コンピューター ソフトウェアの独特な状態に一意のバージョン名または一意のバージョン番号を割り当てるプロセスです。カテゴリ内で、特定のバージョン番号 （主要なマイナー）、これらの数字は一般的に昇順に割り当てられているし、ソフトウェアの新たな展開に対応しています。細かいレベルではこの情報は、コンピューターのソフトウェアかどうかリビジョン管理はしばしば電子情報の少しずつ異なるバージョンを追跡するため使用されます。
 
Helpコマンド
----------------------

このコマンドはバージョン モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        jrush  version help

Help コマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# jrush  version help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command Joomls Version information.

  Version, version

        - available
        Returns available Joomla Versions
        example: jrush version available

        - current
        Returns the current Joomla Version
        example: jrush version current

 ------------------------------
 End Help
 ****************************************


Available
----------------

ユーザーは、ご利用いただけます joomla のバージョンについて知る必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush version available ..config file=”bootstrap file path”


スクリーンショットの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# jrush version available --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(1) {
  ["availableVersions"]=>
  array(2) {
    [0]=>
    string(5) "1.5.0"
    [1]=>
    string(6) "1.5.26"
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************

Current
----------------

ユーザーは現在の joomla のバージョンについて知っている必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。

.. code-block:: bash
        
	        jrush version current ..config file=”bootstrap file path”

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# jrush version current --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(3) {
  ["shortVersion"]=>
  string(5) "3.3.3"
  ["longVersion"]=>
  string(53) "Joomla! 3.3.3 Stable [ Ember ] 25-July-2014 13:00 GMT"
  ["detailed"]=>
  object(ArrayObject)#47 (1) {
    ["storage":"ArrayObject":private]=>
    object(JVersion)#7 (11) {
      ["PRODUCT"]=>
      string(7) "Joomla!"
      ["RELEASE"]=>
      string(3) "3.3"
      ["DEV_LEVEL"]=>
      string(1) "3"
      ["DEV_STATUS"]=>
      string(6) "Stable"
      ["BUILD"]=>
      string(0) ""
      ["CODENAME"]=>
      string(5) "Ember"
      ["RELDATE"]=>
      string(12) "25-July-2014"
      ["RELTIME"]=>
      string(5) "13:00"
      ["RELTZ"]=>
      string(3) "GMT"
      ["COPYRIGHT"]=>
      string(72) "Copyright (C) 2005 - 2014 Open Source Matters, Inc. All rights reserved."
      ["URL"]=>
      string(107) "<a href="http://www.joomla.org">Joomla!</a> is Free Software released under the GNU General Public License."
    }
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************


代替パラメータ
----------------------------

2 つの代替のパラメーターのいずれかのコマンドで使用することができます。-  

jarticle, JArticle

eg:  jrush version current ..config file=”bootstrap file path”/ jrush Version current ..config file=”bootstrap file path”

メリット
--------------

* 簡単な方法で、バージョン情報を取得することができます 
* joomla のバージョンの可用性について知ってもらうことができます 
* 現在の joomla のバージョンについて知ってもらうことができます


