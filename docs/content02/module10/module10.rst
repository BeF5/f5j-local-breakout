1.10 疎通確認(windows PC)
======================================

クライアントPCからBIG-IPが正常に振り分けができているかを確認します。

1. クライアントPCでMicrosoft Edgeを起動し、\ ``・・・``\から、\ ``設定``\をクリックします。 

.. figure:: images/Picture1.png
   :scale: 50%
   :align: center


2. システムとパフォーマンスから\ ``コンピュータのプロキシ設定を開く``\をクリックします。

.. figure:: images/Picture2.png
   :scale: 50%
   :align: center


3. 手動プロキシセットアップで\ ``プロキシサーバを使う``\を\ ``オン``\にし、アドレス、ポートを入力し、保存をクリックします。

.. figure:: images/Picture3.png
   :scale: 50%
   :align: center


以上で疎通確認の準備は終了です。

ブラウザでアクセスした後、BIG-IP上のログより動作を確認し、対象アドレス等を調整します。

