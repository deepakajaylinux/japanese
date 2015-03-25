=============
Extension
=============

概要
--------------

拡張機能は、オペレーティング システムがそれらに対処することができますようにされる必要があります。これらのファイル名は、特定の規則があります。ピリオドの左側に名前の最初の部分はルート名と呼ばれます。ルート名はデバイス名と同じにすることはできません。期間の右側に 2 番目の部分は、拡張子です。省略可能なありは頻繁、しかし必ずしも、3 文字長です。拡張機能はコーディングを追加できます。それは、Ubuntu や centOS 詐鞠を増強しました。

Helpコマンド
-----------------

Help コマンドと同様、目的に関するユーザー ガイドとして拡張機能に含まれているオプションについて。拡張機能の代替パラメーターを示します。また、Jrush モジュールの機能の構文について説明します。ヘルプ コマンド拡張機能が表示されます以下の通りです。

.. code-block:: bash

		jrush extension help

コマンドの入力後それとしてアクション オプションを示します。次のイメージは、明らかにそれを視覚化します。

.. code-block:: bash

 kevell@corp:/# jrush Extension help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla Extensions (Component, Module or Plugin).

  Extension, extension

        - disable
        Deletes a extension
        example: jrush extension disable

        - enable
        Enables a extension
        example: jrush extension enable

        - info
        Display the details of a extension
        example: jrush extension info


 ------------------------------
 End Help
 ****************************************


代替パラメータ
----------------------------

選択の問題として、次のオプションの使用、ユーザーが行うことができます拡張機能を使用します。

Extension, extension

オプション
------------

3 つのオプションが利用できます。拡張オプションについて見てみましょう。

* Enable
* Disable
* Info

Disable
-----------

ときユーザーとして有効にすると自動的にそれを入力、拡張子を削除します。次のコマンドを有効にするために使用します。

.. code-block:: bash

		jrush extension Disable

以下のマントルショットはその機能を視覚化することができます。


.. code-block:: bash

 kevell@corp:/# jrush Extension disable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************


Enable
-----------

拡張機能を有効にするを有効にするを使用します。次のコマンドを有効にするユーザーを助けます。

.. code-block:: bash

 		jrush extension enable

次のスクリーン ショットはその機能を有効にするユーザーをガイドします。

.. code-block:: bash

 kevell@corp:/# jrush Extension enable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:
 
 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 1
 ------------------------------
 Extension Manage Finished
 ****************************************



Info
--------

情報は、拡張の詳細を表示するユーザーを支援する援助です。拡張 id を頼みます。値を入力した後、拡張機能の詳細を表示。次のコマンド情報を表示するために使用します。

.. code-block:: bash

		jrush extension info

これは、スクリーンショットによる可視化することができます。


.. code-block:: bash

 kevell@corp:/# jrush Extension info --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************

メリット
----------------

* 拡張機能は、メタデータの種類と見なすことができます。
* 複数のアプリケーションに、特定の拡張子に関連付けられます。
* 非大文字小文字を区別 
* 快適に Ubuntu とセント OS。
* 使用して、拡張子を削除する 
* 拡張機能に関する情報を表示する情報を使用します。


