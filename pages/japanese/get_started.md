---
layout: page
title: Get Started
permalink: /get_started
---

[English](./en/get_started)

# Get Started
{: .no_toc }

このページでは、ダウンロードした`VMagicMirror`の基本的な使い方を紹介します。

セットアップの様子は以下の動画でも紹介していますが、やや古いバージョンを使用していることに注意してください。

<iframe class="youtube" width="560" height="315" data-src="https://www.youtube.com/embed/kYk-YHqPeMU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<div class="toc-area" markdown="1">

#### Content
{: .toc-header .no_toc }

* ToC
{:toc .table-of-contents }

</div>

### 1. 起動してキャラクターを表示する
{: .doc-sec1 }

`VMagicMirror.exe`を起動すると、GUIがある「コントロールパネル」と、キャラクターが映る「キャラクター表示ウィンドウ」が立ち上がります。

コントロールパネルかキャラクター表示ウィンドウの一方を閉じると、もう片方の画面も閉じて`VMagicMirror`が終了します。コントロールパネルが邪魔な場合は最小化しておきます。

<div class="note-area" markdown="1">

**NOTE**

`VMagicMirror.exe`が正常に起動しない場合、zipの解凍方法を確認して下さい。

zipファイルを右クリックして`プロパティ`を選び、`セキュリティ`の項目があるか確認します。

もし項目があれば`許可する`をチェックして`OK`で変更を適用します。その後、再びzipを解凍してください。

<div class="row">
{% include docimg.html file="./images/get_started/img00_005_before_unzip.jpg" customclass="col l6 m6 s12" imgclass="fit-doc-img" %}
</div>

</div>

キャラクターはPC上のVRMファイルからロードするか、またはVRoid Hubからロードできます。

PC上のVRMファイルをロードする場合、`ホーム`タブの`PC上のファイルをロード`ボタンをクリックします。

`.vrm`ファイルを選択し、キャラクター表示ウィンドウに表示される規約を確認します。

`OK`をクリックすると、キャラクターがロードされます。

<div class="row">
{% include docimg.html file="./images/get_started/img00_015_started.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_020_load_vrm.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

VRoid Hubのモデルをロードする場合、`VRoid Hubからロード`ボタンをクリックします。

Webブラウザが開くため、指示に従ってアプリ連携を完了し、認可コードを表示します。表示された認可コードをVMagicMirrorの入力欄にペーストし、ログインします。

その後、使いたいモデルを選び、規約を確認してロードします。利用できるのは自分のモデル、「いいね」したモデル、ピックアップされたモデルの3種類です。

<div class="row">
{% include docimg.html file="./images/get_started/img00_032_connect_vroid_hub.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_034_vroid_hub_characters.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_037_vroid_hub_confirmation.jpg" customclass="col s12 m6 l4" imgclass="fit-doc-img" %}
</div>

<div class="note-area" markdown="1">

**NOTE**

他者がアップロードしたモデルは「いいね」をしても使用できるとは限りません。

詳しくは[VRoid Hubのアバター利用について](./tips/use_vroid_hub)をご覧下さい。

</div>

ロードしたキャラクターを次回以降も使いたい場合、`ホーム`タブの`次回の起動時にも同じVRMを読み込む`のチェックをオンにします。

<div class="row">
{% include docimg.html file="./images/get_started/img00_030_load_vrm_confirmation.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_040_after_loaded.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

また、この時点でキーボードやタッチパッドの位置、視点がキャラクターに合わない場合、`キャラ体格で補正`ボタンをクリックします。

<div class="row">
{% include docimg.html file="./images/get_started/img00_160_not_good_layout_example.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_170_after_adjust.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

ここで補正した視点などは、後で紹介する手順でより細かく調整できます。


### 2. 配信タブ: メイン機能の使い方
{: .doc-sec1 }

コントロールパネルの`配信`タブでは`VMagicMirror`のすべての主要機能にアクセスできます。

キャラクターをロードしたら色々な基本機能を試してみましょう。

{% include docimg.html file="./images/get_started/img00_050_streaming_tab.jpg" %}

#### 2.1. ウィンドウ
{: .doc-sec2 }

`ウィンドウ`で`背景を透過`をチェックすると、背景を透明にできます。`VMagicMirror`は通常、この状態で使用します。

背景が透明であり、かつ`(透過中)キャラ付近を掴んでドラッグ`のチェックがオンであれば、キャラクターを`左クリック+ドラッグ`で移動できます。

移動後に`(透過中)キャラ付近を掴んでドラッグ`をオフにすると、キャラクターがクリックに反応しなくなり、背面のアプリケーションをクリックできます。

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

<div class="doc-ul" markdown="1">

- `リップシンク`: PCに接続されたマイクを選択して、音声にあった口の動きを反映します。
- `マイク感度[dB]`: マイク入力が小さい場合にプラスの値を指定することで、リップシンクが正しく動作するようになります。`音量をチェック`を使って適正な値を確認して下さい。
- `音量をチェック`: オンにするとマイク音量バーが表示されます。喋っている間はほぼ緑色で、ときどき赤色になるのが適正な音量です。
- `顔をトラッキング`: ウェブカメラを選択することで、首の動作を反映します。
- `高解像度モード`: CPU負荷が情報する代わり、ややトラッキングの反応速度が向上します。v1.5.0時点ではベータ版の機能です。
- `顔とセットで手もトラッキング`: ウェブカメラによる簡易的なハンドトラッキングを有効にします。

</div>

顔をトラッキングさせてもモデルの首が回らない場合、[FAQ](./questions)の「顔トラッキングで首が回らない」を参照下さい。

また、ハンドトラッキングには制限事項や注意点があります。詳細は[ハンドトラッキングの使用について](./tips/using_hand_tracking)を参照下さい。

ウェブカメラが正面にない場合やウェブカメラを移動させた場合は、普段の姿勢でディスプレイを見ながら`姿勢・表情を補正`ボタンをクリックしてキャラクターの位置を戻します。

<div class="note-area" markdown="1">

**HINT** 

キャラクターがうつむきがちな場合は、少し下を向いて`姿勢・表情を補正`をクリックすると、キャラが上を向きやすくなります。反対に、キャラクターが上を向きすぎる場合、上を向いて`姿勢・表情を補正`ボタンをクリックすることで、キャラが下を向きやすくなります。

</div>

`視線の動き`ではキャラクターの目の動かし方を選択します。通常は`マウス`選択にすることで、キャラクターがマウスポインターの方向を見つめます。

<div class="note-area" markdown="1">

**NOTE** 

本機能とは別に、iOSアプリによる表情トラッキングも可能です。

詳細は[外部トラッキング](./docs/external_tracker)を参照ください。

</div>


#### 2.3. Word To Motion
{: .doc-sec2 }

`Word To Motion`はキャラクターの表情をコントロールできる機能です。

<div class="row">
{% include docimg.html file="./images/get_started/img00_105_word_to_motion.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

デフォルト設定の場合、キーボードで"joy"とタイピングするとキャラクターの表情が変化します。

それ以外でも、`デバイスの割り当て`で`ゲームパッド`を選んでA,B,X,Yボタンを押したり、`キーボード (数字の0-8)`を選んで数字キーの1,2,3,4を押したりしても表情が変化します。

詳しくは[Docs](./docs)の[Word To Motion](./docs/expressions)を参照下さい。

とくに`デバイスの割り当て`で`ゲームパッド`や`MIDIコントローラ`を選ぶことで、キャラクターの動作に反映させずに表情を切り替えられます。


#### 2.4. 表示
{: .doc-sec2 }

`表示`ではキャラクター以外のデバイス表示やエフェクトのオン・オフを切り替えます。

とくにキーボードを表示して`タイピング時のエフェクト`で`None`以外を選択した場合、タイピング時にエフェクトが表示されます。

<div class="row">
{% include docimg.html file="./images/get_started/img00_125_view_typing_effect_example.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

<div class="note-area" markdown="1">

**Hint**

影の見栄えが悪い場合、[FAQ](./questions)の"影が綺麗に映らない"の項目を確認してください。

それでも見栄えが改善しない場合、影の表示をオフにします。

</div>


#### 2.5. カメラ
{: .doc-sec2 }

カメラ機能では、キャラクターをうつす視点を操作できます。

本機能を使うときは基本的に`ウィンドウ`メニューの`背景を透過`をオフにします。その後、`フリーカメラモード`チェックをオンにすると、キャラクター表示ウィンドウ上で直接視点を動かせます。

<div class="doc-ul" markdown="1">

- `右クリック + ドラッグ`: 視線を上下左右に回転します。
- `中クリック + ドラッグ`: カメラを上下左右に平行移動します。
- `中ホイール`: カメラを前後に移動します。

</div>

調整が終わったら`背景を透過`をオンに、`フリーカメラモード`をオフに戻します。

キャラクターを見失った場合や始めからやり直す場合、`位置をリセット`ボタンで初期状態に戻します。

<div class="row">
{% include docimg.html file="./images/get_started/img00_130_free_camera_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
{% include docimg.html file="./images/get_started/img00_140_after_free_camera_mode.jpg" customclass="col s12 m6" imgclass="fit-doc-img" %}
</div>

また、`クイックセーブ`の`[1], [2], [3]`いずれかのボタンで現在の視点を保存したり、`クイックロード`の対応するボタンでロードしたりできます。

<div class="note-area" markdown="1">

**Hint**

`背景を透過`をオンにしたままでも、`フリーカメラモード`チェックをオンにすると視点を調整できます。

<div class="doc-ul" markdown="1">

1. `(透過中)キャラ付近を掴んでドラッグ`をオンにする
2. キャラクターを左クリックし、各操作で視点を調整
3. 調整後、`(透過中)キャラ付近を掴んでドラッグ`と`フリーカメラモード`をオフにする

</div>

ただし、この方法ではキャラクターが表示ウィンドウの外に見切れてしまいやすいです。

キャラクターを見失った場合は`位置をリセット`ボタンでリセットして下さい。

あるいは、`背景を透過`をオフにしてウィンドウの表示を確認して下さい。

</div>



#### 2.6. デバイスのレイアウト
{: .doc-sec2 }

`フリーレイアウトモード`をオンにすると、キーボード、タッチパッド、ゲームコントローラなどの位置を調整できます。

{% include docimg.html file="./images/get_started/img00_200_free_layout.jpg" %}

チェックをオンにすると自動的に`背景を透過`チェックがオフになります。

このモードでキャラクター表示ウィンドウの左上に現れる設定は次のような意味です。

<div class="doc-ul" markdown="1">

- `Control Mode`: デバイスの位置、回転、スケールのどれを調整するかを選択します。
- `Coordinate`: デバイスに沿った座標で動かすか、ワールド座標を用いるかを選択します。通常は`Local`のまま操作します。
- `Gamepad Scale`: ゲームパッドのモデル部分の大きさを調整します。ゲームパッドが手から突き抜けてしまう場合、値を小さくします。

</div>

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

さらに詳細な機能は以下のページで紹介しているので、より細かく設定したい方はあわせて参照下さい。

<div class="doc-ul" markdown="1">

- [Docs](./docs): このページで紹介しなかった詳細設定を、UIの項目別に紹介します。全ての機能を確認したいときに参照して下さい。 
- [Tips](./tips): VMagicMirrorの用途に応じた使い方を紹介しています。

</div>
