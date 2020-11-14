---
layout: page
title: Get Started
permalink: /get_started
---

[English](./en/get_started)

# Get Started
{: .no-toc }

このドキュメントでは、ダウンロードした`VMagicMirror`の基本的な使い方を紹介します。

セットアップの様子はこちらの動画でも紹介していますが、やや古いバージョンを使用していることに注意してください。

<iframe class="youtube" width="560" height="315" data-src="https://www.youtube.com/embed/kYk-YHqPeMU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<div class="toc-area">

<h4 class="toc-header">Content</h4>

*ToC
{:toc .table-of-contents }

</div>

### 1. 起動してキャラクターを表示する
{: .doc-sec1 }

`VMagicMirror.exe`を起動すると、GUIがある「コントロールパネル」と、キャラクターが映る「キャラクター表示ウィンドウ」が立ち上がります。

**注意:** `VMagicMirror.exe`が正常に起動しない場合、Windows OSのセキュリティ処理でzipの解凍に失敗した可能性があります。zipファイルを右クリックして`プロパティ`を選び、`セキュリティ`の項目があるかどうか確認します。もし項目があれば`許可する`をチェックを入れて`OK`で変更を適用し、その後あらためてzipを解凍してください。

<div class="row">
{% include docimg.html file="./images/get_started/img00_005_before_unzip.jpg" customclass="col l6 m6 s12" imgclass="fit-doc-img" %}
</div>

コントロールパネルかキャラクター表示ウィンドウの一方を閉じると、もう片方の画面も閉じて`VMagicMirror`が終了します。コントロールパネルが邪魔な場合は最小化しておきます。

キャラクターはPC上のVRMファイル、またはVRoid Hubからロードできます。

※VRoid Hubはv1.0.0以降で利用可能です。

PC上のVRMファイルをロードする場合、`ホーム`タブの`PC上のファイルをロード`ボタンをクリックし、PC上の`.vrm`ファイルを選択します。キャラクター表示ウィンドウに表示される規約を確認して`OK`をクリックすると、キャラクターをロードします。

<div class="row">
{% include docimg.html file="./images/get_started/img00_015_started.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_020_load_vrm.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

VRoid Hubのキャラクターをロードする場合、`VRoid Hubからロード`ボタンをクリックするとブラウザ上でアプリ連携を行ったのち、認可コードが表示されます。認可コードをコピーし、VMagicMirrorの入力欄にペーストしてログインします。

ログイン後、キャラクター表示ウィンドウ側にキャラクター選択画面が表示されます。自分でアップロードしたキャラクター、「いいね」したキャラクター、ピックアップされたキャラクターのいずれかを選択し、規約を確認してロードします。

<div class="row">
{% include docimg.html file="./images/get_started/img00_032_connect_vroid_hub.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_034_vroid_hub_characters.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_037_vroid_hub_confirmation.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
</div>

※他者によるキャラクターの一部は「いいね」をしていても非表示になることがあります。詳細は[VRoid Hubのアバター利用について](./tips/use_vroid_hub)を参照して下さい。

ロード後、同じキャラクターを次回以降も使いたい場合、`次回の起動時にも同じVRMを読み込む`のチェックをオンにします。

<div class="row">
{% include docimg.html file="./images/get_started/img00_030_load_vrm_confirmation.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_040_after_loaded.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

**Hint:** この時点でキーボードやタッチパッドの位置、視点がキャラクターに合わない場合、ひとまず`キャラ体格で補正`ボタンをクリックしておきます。

<div class="row">
{% include docimg.html file="./images/get_started/img00_160_not_good_layout_example.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_170_after_adjust.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>


### 2. 配信タブ: メイン機能の使い方
{: .doc-sec1 }

コントロールパネルの`配信`タブでは`VMagicMirror`のすべての主要機能にアクセスできます。

キャラクターをロードしたら色々な基本機能を試してみましょう。

{% include docimg.html file="./images/get_started/img00_050_streaming_tab.jpg" %}

#### 2.1. ウィンドウ
{: .doc-sec2 }

`ウィンドウ`で`背景を透過`のチェックをオンにすると、背景を透明にできます。`VMagicMirror`は通常、この状態で使用します。

背景が透明なとき、`(透過中)キャラ付近を掴んでドラッグ`のチェックがオンであればキャラクターを左クリック+ドラッグして移動できます。

移動後は`(透過中)キャラ付近を掴んでドラッグ`をオフにすることでキャラクターがクリックに反応しなくなり、背面のアプリケーションをクリックできるようになります。

<div class="row">
{% include docimg.html file="./images/get_started/img00_060_transparent_bg.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_070_transparent_bg_drag.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_090_transparent_bg_can_click.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
</div>


#### 2.2. 顔・表情
{: .doc-sec2 }

`顔・表情`メニューは、顔の動きに関連する主要な機能です。

<div class="row">
{% include docimg.html file="./images/get_started/img00_100_streaming_face.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

`リップシンク`: PCに接続されたマイクを選択して、音声にあった口の動きを反映します。

`マイク感度[dB]`: マイク入力が小さすぎる場合はプラスの値を指定することで、リップシンクが正しく動作するようになります。`音量をチェック`を使って適正な感度か確認して下さい。

`音量をチェック`: オンにするとマイク音量バーが表示されます。喋っているあいだ、ほぼ緑色で、ときどき赤色になるのが適正な音量です。

`顔をトラッキング`: ウェブカメラを選択することで、首の動作を反映します。

`高解像度モード`: CPU負荷が情報する代わり、ややトラッキングの反応速度が向上します。v1.5.0時点ではベータ版の機能です。

`顔とセットで手もトラッキング`: ウェブカメラによる簡易的なハンドトラッキングを有効にします。

顔をトラッキングさせてもモデルの首が回らない場合、[FAQ](./questions)の「顔トラッキングで首が回らない」を参照下さい。

ハンドトラッキングには制限事項や注意点があります。詳細は[ハンドトラッキングの使用について](./tips/using_hand_tracking)を参照下さい。

ウェブカメラが正面にない場合やウェブカメラを移動させた場合は、普段の姿勢でディスプレイを見ながら`姿勢・表情を補正`ボタンをクリックしてキャラクターの位置を戻します。

**NOTE:** キャラクターがうつむきがちになる場合は、少し下を向いて`姿勢・表情を補正`ボタンをクリックすると、キャラが上を向きやすくなります。反対に、キャラクターが上を向きすぎる場合は、上を剥いて`姿勢・表情を補正`ボタンをクリックすることで、キャラが下を向きやすくなります。

`視線の動き`はキャラクターの目の動かし方を選択します。通常は`マウス`選択にすることで、キャラクターがマウスポインターの方向を見つめます。

**NOTE:** 本機能とは別に、v1.1.0以降ではiOSアプリによる表情トラッキングも可能です。詳細は[外部トラッキング](./docs/external_tracker)を参照ください。


#### 2.3. Word To Motion
{: .doc-sec2 }

`Word To Motion`はいくつかの方法でキャラクターの表情をコントロールできる機能です。

<div class="row">
{% include docimg.html file="./images/get_started/img00_105_word_to_motion.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

デフォルト設定の場合、キーボードで"joy"とタイピングするとキャラクターの表情が変化します。それ以外でも、`デバイスの割り当て`で`ゲームパッド`を選んでA,B,X,Yボタンを押したり、`キーボード (数字の0-8)`を選んで数字キーの1,2,3,4を押したりしても表情が変化します。

詳しくは[Docs]](./docs)の[Word To Motion](./docs/expressions)を参照下さい。

とくに`デバイスの割り当て`で`ゲームパッド`や`MIDIコントローラ`を選ぶことにより、こっそりと表情を切り替えられます。


#### 2.4. 表示
{: .doc-sec2 }

`表示`では`VMagicMirror`の対応デバイスやエフェクトのオン・オフを切り替えます。

とくにキーボードを表示して`タイピング時のエフェクト`で`None`以外を選択した場合、タイピング時にエフェクトが表示されます。

<div class="row">
{% include docimg.html file="./images/get_started/img00_125_view_typing_effect_example.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

**Hint:** 影の見栄えが悪い場合、[FAQ](./questions)の"影が綺麗に映らない"の項目を確認してください。それでも見栄えが改善しない場合、影の表示をオフにします。


#### 2.5. カメラ
{: .doc-sec2 }

カメラ機能では、キャラクターをうつす視点を操作できます。

本機能を使うときは基本的に`ウィンドウ`メニューの`背景を透過`をオフにします。その後、`フリーカメラモード`チェックをオンにすると、キャラクター表示ウィンドウ上で直接視点を動かせます。

`右クリック + ドラッグ`: 視線を上下左右に回転します。

`中クリック + ドラッグ`: カメラを上下左右に平行移動します。

`中ホイール`: カメラを前後に移動します。

調整が終わったら`背景を透過`をオンに、`フリーカメラモード`をオフに戻します。

キャラクターを見失った場合や始めからやり直したい場合、`位置をリセット`ボタンで初期状態に戻せます。

<div class="row">
{% include docimg.html file="./images/get_started/img00_130_free_camera_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_140_after_free_camera_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

また、動かした視点は`クイックセーブ`の`[1], [2], [3]`いずれかのボタンを押して保存したり、`クイックロード`の対応するボタンを押してロードしたりできます。


**Hint:** 操作に慣れてきたら、`背景を透過`をオンにしたまま`フリーカメラモード`チェックをオンにしても視点を調整できます。

1. `(透過中)キャラ付近を掴んでドラッグ`をオンにする
2. キャラクターを左クリックし、各操作で視点を調整
3. 調整が終わったら`(透過中)キャラ付近を掴んでドラッグ`と`フリーカメラモード`をオフにする

ただし、この操作方法では気づかないうちにキャラクターがキャラクター表示ウィンドウから見切れることがあります。キャラクターを見失ってしまい、直し方がわからなくなった場合は`位置をリセット`ボタンを押してやり直すか、`背景を透過`をオフにしてウィンドウの表示を確認します。


#### 2.6. デバイスのレイアウト
{: .doc-sec2 }

`フリーレイアウトモード`のチェックをオンにするとキーボード、タッチパッド、ゲームコントローラなどの位置を調整できます。

{% include docimg.html file="./images/get_started/img00_200_free_layout.jpg" %}

チェックをオンにした時点で自動的に`背景を透過`チェックがオフになります。`フリーレイアウト`は背景が透明なままだと使用できないことに注意して下さい。

フリーレイアウトモード中の、キャラクター表示ウィンドウ左上の設定は次のような意味です。

`Control Mode`: デバイスの位置、回転、スケールのどれを調整するかを選択します。

`Coordinate`: デバイスに沿った座標で動かすか、ワールド座標を用いるかを選択します。通常は`Local`のまま操作します。

`Gamepad Scale`: ゲームパッドのモデル部分の大きさを調整します。ゲームパッドが手から突き抜けてしまう場合、値を小さくします。

レイアウトが極端に崩れてしまった場合、`リセット`で標準的なレイアウトに戻します。

#### 2.7. モーション
{: .doc-sec2 }

`プレゼン風に右手を動かす`のチェックをオンにしてマウスを動かすと、キャラクターが右手でマウスポインタの方向を指し示します。

<div class="row">
{% include docimg.html file="./images/get_started/img00_150_presentation_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

このスタイルは解説動画やプレゼンテーションで`VMagicMirror`を使う際に便利です。詳しくは[Tips: プレゼンテーションでVMagicMirrorを使う](./tips/presentation)もあわせてご覧下さい。

`つねに手下げモード`チェックをオンにすると、手が常に下がった姿勢で使用できます。この状態ではビルトインモーション(手を振る動作など)を除き、プレゼンテーションの手の動作なども無効になります。また、このモードではキャラクターの体の移動幅が大きくなります。

<div class="row">
{% include docimg.html file="./images/get_started/img00_155_hand_down_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

### 3. もっと細かく調整したい場合は
{: .doc-sec1 }

[Docs](./docs)や[Tips](./tips)にて、さらに詳細な機能をいくつか紹介しています。

より細かく調整したい方はあわせてご覧下さい。
