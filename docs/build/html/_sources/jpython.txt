==============
Python
==============


あらすじ
-----------

Python は広く使われている一般的な目的は、高水準プログラミング言語。このモジュールは、最新バージョンの python パッケージとその依存関係のインストールを目指しています。

ヘルプ コマンド
-----------------

ヘルプ コマンドはタスクを達成するために必要を提供するためにユーザーをガイドします。確認するコマンド、ターミナルの下でのヘルプの使用を次のように与えられる

.. code-block:: bash

	ptconfigure python help


下のスナップショットは、help コマンドの絵の表現を与えるし、Python と python として 2 つのパラメーターを一覧表示します。(パラメーターは大文字と小文字)

.. code-block:: bash

	  kevell@corp:/# ptconfigure Python help
	  ******************************


	  This command allows you to install the latest available Python in the Ubuntu
	  repositories.

	  Python, python

          - install
           Installs the latest version of Python
           example: ptconfigure python install

	  ------------------------------
	  End Help
	  ******************************


インストール
-------------

Python モジュールをインストールするために使用されるコマンドは下記します。


.. code-block:: bash

	ptconfigure python install

上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure python install

 Install Python? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Python!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
  python is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package python from the Packager Apt is already installed, so not installing.
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47618 package 'ptconfigure':
  missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47618 package 'ptconfigure':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  docutils-common docutils-doc python-pygments python-roman
 Suggested packages:
  texlive-latex-recommended texlive-latex-base texlive-lang-french
  ttf-linux-libertine ttf-bitstream-vera
 The following NEW packages will be installed:
  docutils-common docutils-doc python-docutils python-pygments python-roman
 0 upgraded, 5 newly installed, 0 to remove and 13 not upgraded.
 Need to get 2,190 kB of archives.
 After this operation, 8,623 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main docutils-common all 0.8.1-4ubuntu1 [153 kB]
 Get:2 http://us.archive.ubuntu.com/ubuntu/ precise/main docutils-doc all 0.8.1-4ubuntu1 [1,289 kB]
 Get:3 http://us.archive.ubuntu.com/ubuntu/ precise/main python-roman all 0.8.1-4ubuntu1 [12.6 kB]
 Get:4 http://us.archive.ubuntu.com/ubuntu/ precise/main python-docutils all 0.8.1-4ubuntu1 [382 kB]
 Get:5 http://us.archive.ubuntu.com/ubuntu/ precise/main python-pygments all 1.4+dfsg-2 [353 kB]
 Fetched 2,190 kB in 7s (277 kB/s)
 Selecting previously unselected package docutils-common.
 (Reading database ... 254879 files and directories currently installed.)
 Preparing to unpack .../docutils-common_0.8.1-4ubuntu1_all.deb ...
 Unpacking docutils-common (0.8.1-4ubuntu1) ...
 Selecting previously unselected package docutils-doc.
 Preparing to unpack .../docutils-doc_0.8.1-4ubuntu1_all.deb ...
 Unpacking docutils-doc (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-roman.
 Preparing to unpack .../python-roman_0.8.1-4ubuntu1_all.deb ...
 Unpacking python-roman (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-docutils.
 Preparing to unpack .../python-docutils_0.8.1-4ubuntu1_all.deb ...
 Unpacking python-docutils (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-pygments.
 Preparing to unpack .../python-pygments_1.4+dfsg-2_all.deb ...
 Unpacking python-pygments (1.4+dfsg-2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for sgml-base (1.26+nmu4ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Setting up docutils-common (0.8.1-4ubuntu1) ...
 update-catalog: Suppressing action on super catalog. Invoking trigger instead.
 Setting up docutils-doc (0.8.1-4ubuntu1) ...
 Setting up python-roman (0.8.1-4ubuntu1) ...
 Setting up python-pygments (1.4+dfsg-2) ...
 Processing triggers for sgml-base (1.26+nmu4ubuntu1) ...
 Setting up python-docutils (0.8.1-4ubuntu1) ...
 update-alternatives: using /usr/share/docutils/scripts/python2/rst-buildhtml to provide /usr/bin/rst-buildhtml (rst-buildhtml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2html to provide /usr/bin/rst2html (rst2html) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2latex to provide /usr/bin/rst2latex (rst2latex) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2man to provide /usr/bin/rst2man (rst2man) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2odt to provide /usr/bin/rst2odt (rst2odt) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2odt_prepstyles to provide /usr/bin/rst2odt_prepstyles (rst2odt_prepstyles) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2pseudoxml to provide /usr/bin/rst2pseudoxml (rst2pseudoxml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2s5 to provide /usr/bin/rst2s5 (rst2s5) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2xetex to provide /usr/bin/rst2xetex (rst2xetex) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2xml to provide /usr/bin/rst2xml (rst2xml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rstpep2html to provide /usr/bin/rstpep2html (rstpep2html) in auto mode
 [Pharaoh Logging] Adding Package python-docutils from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Python: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
-----------

.. cssclass:: table-bordered

 +-----------------------+-------+-------------------------------------------------------------------------------------+
 | パラメータ            | 必須  | 注釈                                                                                |
 +-----------------------+-------+-------------------------------------------------------------------------------------+
 |ptconfigure python     | Yes   | このコマンドは、Pythonモジュールをインストールします                                |
 |install                |       |                                                                                     |
 +-----------------------+-------+-------------------------------------------------------------------------------------+
 |Install python (Y/N)   | Y     | ユーザーは、Yを入力すると、以前にインストールしたパッケージのために、               |
 |                       |       | このmodueチェックは、終了した場合、新しいバージョンに更新されたか、そうでなければ、 |
 |                       |       | 新鮮なパッケージをインストールします。                                              |
 +-----------------------+-------+-------------------------------------------------------------------------------------+
 |Install python (Y/N)   | N     | ユーザーは、Nを入力すると、インストールが中止された。|                              |
 +-----------------------+-------+-------------------------------------------------------------------------------------+


ユーザーのメリット
----------------------

* 時間がかかる
* アクセス、インストールの使いやす
* コーディングは大文字小文字の区別
* 完全なソースコードが利用できるとライセンス コストはありません。

 
