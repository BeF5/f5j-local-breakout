BIG-IP LTM セットアップガイド　Office365向けOutbound通信対策編
==================

本ドキュメントでは、BIG-IP LTMを使ったMicrosoft Office 365(以下、O365)利用環境下におけるProxy負荷軽減対策の設定方法について解説します。

はじめに
--------------------------------
このページでは、これらのオフィシャルなドキュメントの補足となる資料や、複数の機能を組合せてソリューションを実現する方法をご紹介いたします。
F5のオフィシャルなドキュメントはこちらにございます。

- AskF5: https://support.f5.com/csp/home
- F5 Cloud Docs: https://clouddocs.f5.com/
- F5 DevCentral（コミュニティ）: https://community.f5.com/


その他参考リンク
--------------------------------

- F5 テクニカルインフォTop : https://f5j-tech-info.readthedocs.io/
- F5 Japan YouTube : https://www.youtube.com/channel/UCqX6rJEY6Ya8YbC8iqP34zg
- F5 NGINX YouTube(英語) : https://www.youtube.com/@nginx_official


本書利用環境
--------------------------------
- 利用ライセンスはLTMを利用
- Inline型ではなくExplicit型のProxyとしての利用
- ラボ作成時の最新バージョンであるBIG-IP LTM v17.1.1をベースに本書を作成
- BIG-IPにDNSの設定含め基本設定が終わっている
- BIG-IP LTMの基礎知識を学習する場合は以下をご参照ください。
   - `BIG-IP Local Traffic Manager (LTM) v17.1 簡単セットアップガイド <https://f5j-easy-setup-ltm-17.readthedocs.io/ja/latest/>`__ 


.. note::
  - 本書で設定されているパラメータは実構築環境でも同様とは限りません。
  - MicrosoftのURL内容の確認含め、動作確認の実施を欠かさない様宜しくお願い致します。
  - また、動作確認の上、実構築環境に合わせたパラメータをご用意願います。



.. toctree::
   :caption: Contents:
   :glob:

   content*/content*
