==========
Examples
==========


このページは、 ``sphinx_cch_theme`` テーマに含まれるスタイルのデモページです。このページに記載のある主要なコンポーネントについてはスタイルを定義しています。

:auther: @hanyacch
:create: 2016-04-09
:version: 0.1

.. contents::



Heading
==========

これは ``<h2>`` 相当の見出しです。


Sub-heading
------------

これは ``<h3>`` 相当の見出しです。


Sub-sub-heading
''''''''''''''''''

これは ``<h4>`` 相当の見出しです。



Inline markup
===============

- *強調* の例
- **強い強調** の例
- ``inline code text`` の例



List
==========

番号なしリスト:

- りんご
- みかん
- ぶどう
    - 巨峰
    - デラウェア

番号つきリスト:

#. ひとつめ
#. ふたつめ
#. みっつめ
    #. みっつめ　その１
    #. みっつめ　その２

定義リスト:

ある用語
   この言葉の定義をここで説明します。


フィールドリスト:

:date: 2016-04-09
:tags: Sphinx


Block Quote
==============

引用パラグラフの例

    The world is full of fascinating problems waiting to be solved.

    -- Eric Steven Raymond



Table
=======

``csv-table`` ディレクティブの例。 

.. csv-table::
   :header: "項目", "値"

   好きな食べ物, ラーメン
   好きな飲み物, ビール
   好きな言語, Python



Foot notes
============

Lorem ipsum [#f1]_ dolor sit amet ... [#f2]_

.. rubric:: Footnotes

.. [#f1] Text of the first footnote.
.. [#f2] Text of the second footnote.



Admonitions
===============

.. hint::
   
   Hint direcitve

.. tip::

   Tip direcitve

.. note::

   Note directive

.. warning::

   Warning directive

.. danger::

   Danger directive

.. error::

   Error directive



Code
=====

まずは通常のコードブロックの例。

.. code-block:: python

   import awesomemodule

   def hello(name="World"):
       """sample code"""
       print("Hello, {}!".format(name))

行番号付きのコードブロックの例。

.. code-block:: python
   :linenos:

   #!/usr/bin/env python
   # -*- coding: utf-8 -*-
   """Sample script"""

   def main():
       """This is main part"""
       a = 1
       b = 2
       c = a + b
       print(c)

    if __name__ == '__main__':
        main()



Code document
==============

PythonコードのDocstringを ``autodoc`` で取り込んだ例。

*元のコード* ::

    #!/usr/bin/env python
    """Docstring example module

    This code will be used for docstring example in ``sphinx_cch_theme`` . 
    If you want to create document from docstring in python code, please use 
    ``.. automodule::`` directive. 

    Usage::

        python docstring_example.py
    """

    def introduce_myself(name, age):
        """Function for introducing myself with given arguments.

        Args:    
            - name: your name
            - age: your age
        """
        pass

*自動生成したドキュメント* :

.. automodule:: docstring_example
   :members:










