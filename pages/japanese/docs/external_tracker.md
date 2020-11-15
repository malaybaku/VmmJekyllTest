---
layout: page
title: 外部トラッキングアプリとの連携
permalink: /docs/external_tracker
---

[English](../en/docs/external_tracker)

# 外部トラッキングアプリとの連携
{: .no_toc }

`VMagicMirror` v1.1.0以降ではWebカメラを用いる代わり、外部トラッキングアプリを用いてもアバターを操作できます。

v1.1.0の時点ではiOSアプリにのみ対応しています。

<div class="toc-area" markdown="1">

#### 目次
{: .toc-header .no_toc }

* ToC
{:toc .table-of-contents }

</div>


### 外部トラッキングアプリの長所と制限
{: .doc-sec1 }

外部トラッキング機能を使うにあたり、長所と制限事項を確認してください。

#### 外部トラッキングアプリの長所
{: .doc-sec2 .no_toc }

<div class="doc-ul" markdown="1">

- **トラッキング精度の向上**: VMagicMirror自身のWebカメラによるトラッキングより高精度にトラッキングします。
- **CPU負荷の削減**: PC上で行っていた顔トラッキング処理をPC以外のデバイスで行えるため、PCの負荷が削減できます。
- **PCからのカメラ取り外し**: この機能を用いる場合、PCにWebカメラを接続する必要はありません。顔の映り込みが心配な場合、あらかじめカメラを外しておけます。

</div>

#### 外部トラッキングアプリの制限
{: .doc-sec2 .no_toc }

比較的新しいiPhoneまたはiPadが必要です。Face ID対応か、またはA12 Bionic以降のチップが搭載されていれば利用できます。

<div class="doc-ul" markdown="1">

- [Face ID対応機種の一覧](https://support.apple.com/ja-jp/HT209183)
- [iPadモデル一覧(「すべてのモデルを見る」から各端末の搭載チップを確認できます)](https://www.apple.com/jp/ipad/compare/)
- [iPhoneモデル一覧(「すべてのモデルを見る」から各端末の搭載チップを確認できます)](https://www.apple.com/jp/iphone/compare/)

</div>

そのほか、以下の制限にもご留意ください。

<div class="doc-ul" markdown="1">

- 安定性: 従来のWebカメラによる方法よりは安定性が下がります。これは、デバイス間をネットワーク経由で通信するためです。
- アプリ更新による不具合リスク: アプリが更新されることで正常動作しなくなる可能性があります。
- セットアップの複雑性: アプリ間の通信を含むため、設定がやや複雑になっています。

</div>


### あらかじめ準備すること
{: .doc-sec2 }

VMagicMirrorをiOSアプリと連携するために、以下の準備を行います。

1. PCと端末を同一のLAN環境に接続します。
2. LANでの通信が安定していることを確認します。
3. iOS端末を安定して置ける環境(台など)を用意します。
4. 眼鏡をかけている場合は外すか、またはフレームが細いものに付け替えます。

とくに眼鏡をかけていると、まばたきや眼球運動のトラッキング精度が著しく下がる事があります。


### セットアップ方法
{: .doc-sec2 }

VMagicMirrorのコントロールパネルで`Ex Tracker`タブを選択し、`外部トラッキングを有効化`チェックをオンにします。

<div class="row">
{% include docimg.html file="./images/docs/ex_tracker_00_enable_feature.png" customclass="col l6 m6 s12" imgclass="fit-doc-img" %}
</div>

`外部トラッキングを有効化`チェックをオンにすることで、外部アプリと接続できる状態になります。

### 各アプリの連携方法
{: .doc-sec2 }

アプリごとの連携方法は、以下のリンクを参照ください。

**[iFacialMocapとの連携](./external_tracker_ifacialmocap)**


(※他のアプリケーションがサポートされた場合、ここに随時追記されます。)


### 外部トラッキングによるリップシンク
{: .doc-sec2 }

`リップシンクも外部トラッキングの値を使用`をオンにすることで、口の動きも外部トラッキングで取得した値が適用されます。

<div class="row">
{% include docimg.html file="./images/docs/ex_tracker_40_replace_lipsync.png" customclass="col l6 m6 s12" imgclass="fit-doc-img" %}
</div>

このとき、PC上でのマイクによるリップシンクはオフになり、PC上の負荷が削減できます。

また外部アプリはカメラ画像から口の形を取得するため、小声で喋っている場合も口の動きが反映されます。


いっぽう、マイクで口元が遮られている場合などは口元のトラッキング精度が下がります。

その場合は`リップシンクも外部トラッキングの値を使用`をオフにし、従来のマイクによるリップシンクを使うことを検討してください。

### パーフェクトシンク

パーフェクトシンクはv1.3.0からサポートされた機能で、特定のセットアップを行ったモデルで利用できる発展的な機能です。

詳しくは[パーフェクトシンクのTips](../tips/perfect_sync)ご覧ください。


### 表情スイッチ機能を使う
{: .doc-sec2 }

表情スイッチ機能は、ユーザーの表情を使ってアバターの表情を切り替える機能です。

<div class="row">
{% include docimg.html file="./images/docs/ex_tracker_50_face_switch.png" customclass="col l6 m6 s12" imgclass="fit-doc-img" %}
</div>

表情スイッチ機能のセットアップでは3つのパラメータを使用します。

<div class="doc-ul" markdown="1">

- `しきい値`: どの程度その表情を明確にすると表情が切り替わるかを指定します。
- `表情`: 適用するブレンドシェイプ名を指定します。何も適用したくなければ、`(何もしない)`を指定します。
- `リップシンクを続行`: 表情を切り替えたままリップシンクを動かし続けます。目だけが切り替わるブレンドシェイプに対して適用してください。

</div>

個人差や表情のタイプによっては反応しにくいものもあることに注意してください。

なお、この機能は顔トラッキングの延長であるほか、ユーザーの表情を一種のショートカットキーとして使える機能でもあります。

たとえば「舌を出したら悲しい表情になる」など、見た目上は対応関係がないような割り当ても活用できます。

<div class="note-area" markdown="1">

**NOTE**

`Word to Motion`機能による表情切り替えと表情スイッチを同時に使用すると、`Word to Motion`機能による表情が優先して適用されます。

</div>
