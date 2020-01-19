---
layout: page
title: Effects
permalink: /docs/effects
---

[English](../en/docs/effects)

# エフェクト

`エフェクト`タブでは光、影、Bloom、風の設定を調節できます。

キャラクターに照明を当てるライトと影の向きは別々になっています。これは、キャラクターには上から光を当て、影は正面から当てるための仕組みです。

影の向きと奥行きを調節すると、キャラクターとデスクトップ画面の距離感を変更することもできます。以下の例ではデフォルト設定に加えて、キャラと画面が離れているような見え方に調整した例を並べています。

<div class="row">
{% include docimg.html file="/images/about_settings/img01_070_shadow_depth_default.png" customclass="col s12 m6 l6" imgclass="fit-doc-img" %}
{% include docimg.html file="/images/about_settings/img01_080_shadow_depth_look_far.png" customclass="col s12 m6 l6" imgclass="fit-doc-img" %}
</div>

ライトおよび影については、VRMで`Unlit`系統のシェーダーを使っていると機能しないことに注意してください。

また、`風`は`VRMSpringBone`をセットアップしてある場合にのみ動作します。また`風`はキャラクターに設定された全ての`VRMSpringBone`が影響を受けます。髪だけを揺らしてスカートは揺らさない、といった設定はサポートしていません。
