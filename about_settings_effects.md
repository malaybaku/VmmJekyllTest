
# 3.4. エフェクト

`エフェクト`タブでは光、影、Bloom、風の設定を調節できます。

キャラクターに照明を当てるライトと影の向きは別々の設定になっています。

これは、キャラクターには上から光を当て、影は正面から当てるための仕組みです。

影の向きと奥行を調節すると、キャラクターとデスクトップ画面の距離感を変更することもできます。

デフォルト設定の影:

[![Default Depth Shadow](./images/about_settings/img01_070_shadow_depth_default.png)](./images/about_settings/img01_070_shadow_depth_default.png){: data-lightbox="img01_070"}

キャラと画面が離れているように見せるための調整例: 

[![Default Depth Shadow](./images/about_settings/img01_080_shadow_depth_look_far.png)](./images/about_settings/img01_080_shadow_depth_look_far.png){: data-lightbox="img01_080"}

ライトおよび影については、VRMで`Unlit`系統のシェーダーを使っていると機能しないことに注意してください。

また、`風`の設定については以下にも注意して下さい。

* `VRMSpringBone`をセットアップしてある場合にのみ動作します。
* 風機能ではキャラクターに設定された全ての`VRMSpringBone`が影響を受けます。髪だけを揺らしてスカートは揺らさない、といった設定はサポートしていません。

{% include_relative sitemap.md %}

