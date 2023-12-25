1.9.1 External Data-Group用ファイルの作成
======================================

1. BIG-IPのHost側(Linux側)に、Data-Group用の外部ファイルを保存
~~~~~~~~

    事前にエディタ等を用いて公開されているアドレスをBIG-IPで利用可能な形に整形しておきます。


.. NOTE::
   公開情報はいくつか注意点に伴い登録情報の作成と運用方針の決定が必要となります。

   ・大文字だがアクセスは小文字などの差分修正

   ・「equivioprod*.cloudapp.net」などの文字列内に「*」がある場合の登録方針

   ・公開情報への反映前に発生する実アクセス先に対する方針

   例) 2016/7/4時点はSkypeに関する公開情報では以下のアクセス先が登録されていないが実アクセスあり

    a.config.skype.com

    swx.cdn.skype.com

   2016/7/23時点はSkypeに関する公開情報へ登録されている
----

   この様な例があるためマッチング対象の選定は事前確認をお願い致します。

<アドレスサンプル>

   - .. image:: ./images/Picture1.jpg
       :width: 400


   ファイルを保存するディレクトリはどこでも問題ありませんが、本書では、/var/tmp ディレクトリに保存します。

また、本書ではファイル名「o365_url_v2」として保存しています。


   - .. image:: ./images/Picture2.jpg
       :width: 400


2. 作成した外部ファイルの読み込み
~~~~~~~~

tmshで 以下のコマンドで、外部ファイルをオブジェクトとして読み込みます。

.. code-block:: cmdin

   (tmos)# create sys file data-group ext_o365_url_object type string source-path file:/var/tmp/o365_url_v2

   Copying file "file:/var/tmp/o365_url_v2" ...

     % Total    % Received % Xferd  Average Speed  Time　Time 　Time	Current

                                    Dload  Upload  Total　Spent   Left	Speed

   100  8701  100  8701   0    0  12.0M      0　　--:--:--　--:--:--　--:--:--     0
















