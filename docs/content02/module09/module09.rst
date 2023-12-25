1.9 Office365判別用iRuleの作成とVSへの割り当て
======================================

1. 本項ではMicrosoft社にて公開されている情報を元にOffice365の関連アドレスをExternal Data-GroupでマッチングさせるiRuleを作成し、Virtual Serverへと適用します。

   インターネット上で公開されているものを本書では手動で取り込み、BIG-IP向けに加工・成型して取り込みを行っているため、公開もとの情報に関してはMicrosoft社へお問合せ願います。

   参考：　Office 365 の URL と IP アドレスの範囲（MicroSoft社ページ） (2023/12時点)

     https://learn.microsoft.com/ja-jp/microsoft-365/enterprise/urls-and-ip-address-ranges

   ※ XMLは2018/10/2で終了

   なお、iCallにより手動取り込みではなく、スケジュールベースでの自動取り込みにもBIG-IPは対応可能です。

   iRuleやExternal Data-Groupの利用について詳細は「iRulesかんたんセットアップガイド」をご参照下さい。
