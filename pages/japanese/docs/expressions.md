---
layout: page
title: Word to Motion
permalink: /docs/expressions
---

[English](../en/docs/expression)

# Word to Motion

`Word to Motion`はv0.9.0で追加された機能で、単語をタイピングするとキャラクターの表情が切り替えられたり、簡易的なモーションを再生できたりする機能です。

{% include docimg.html file="/images/about_settings/img01_100_word_to_motion_tab.png" %}

使い方によってはこの機能がかえって不自然になる事もあります。その場合、`Word to Motionを有効化`チェックをオフにします。

`Word to Motion`機能では、何の単語に、どのように反応するかをアイテムとして定義します。

各アイテムの左にある再生ボタンを押すか、または単語をタイピングすることで、それぞれのアイテムの動きを確認できます。上のスクリーンショットの例では"joy"とタイピングした直後の様子を示しています。

**NOTE:** `Word to Motion`機能でキャラを動かすとき、単語のタイピング中で制御キー(Shift, Ctrl, Altなど)を押さないように注意してください。また、タイピングが極端に遅い場合、単語として認識されない事があります。

VMagicMirror v0.9.1以降ではゲームコントローラを使ってモーションや表情を実行できます。`ゲームパッドのボタンで表情/モーションを実行`チェックをオンにして、左の列に書かれたボタンを押すと、モーションが実行できます。

{% include docimg.html file="/images/about_settings/img01_105_word_to_motion_by_gamepad.png" %}

この例ではコントローラの`Y`キーを押して、`fun`の表情を実行しています。

**NOTE:** `ゲームパッドのボタンで表情/モーションを実行`チェックをオンにすると、ゲームコントローラを握る動きは無効化されます。コントローラを使ったゲーム配信をする場合、この機能はオフにした方が良いかもしれません。


`上`ボタンや`下`ボタンでアイテムをソートできます。また、アイテムの右にある`削除`ボタンを押すと作成したアイテムを削除できます。

アイテムをカスタマイズするには以下の4ステップを行います。

1. `+`ボタンを押してアイテムを追加します。既に存在するアイテムを編集する場合、このステップは不要です。
2. 設定ボタンを押し、アイテムのカスタムウィンドウを開きます。
3. カスタムウィンドウ上でモーションや表情を設定します。
4. `OK`を押して変更を反映します。

{% include docimg.html file="/images/about_settings/img01_110_word_to_motion_custom_flow.png" %}

カスタムウィンドウで出来る主な操作は以下の4つです。

{% include docimg.html file="/images/about_settings/img01_120_word_to_motion_custom_window.png" %}

1. このアイテムを起動するワードを指定します。
2. モーションを選びます。
    * **NOTE:** v0.9.6時点では2種類のビルトインモーションのみをサポートしています。そのため、基本的には`なし`を選ぶ事になります。
3. 表情の基本設定です。
    * `表情の動作を有効化`をオンにすることで、このアイテムで表情を動かせるようになります。
    * `(全身モーションが「なし」の場合) 表情の変化時間 [sec]`では、表情をキープする時間を設定できます。
    * `アニメーション終了後も表情を維持`をオンにすると、表情を切り替えたままにできます。
4. ブレンドシェイプの設定です。基本的には1つのブレンドシェイプのみを大きな値にし、他はゼロにします。

v0.9.6以降ではMIDIコントローラでも表情が切り替えられます。

MIDIコントローラのキーと表情を関連づけるために3つのステップが必要です。

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr"><a href="https://twitter.com/hashtag/VMagicMirror?src=hash&amp;ref_src=twsrc%5Etfw">#VMagicMirror</a><br>MIDIコンを叩くと表情が変わるやつの進捗です。<br><br>・コントロールパネル側で、MIDIコンと実行するアイテムのマッピング設定を開く<br>・MIDIコンのキーを叩いてセットアップ<br>・セットアップ完了したら再びMIDIコンのキーを叩く<br><br>の3手順で動きます <a href="https://t.co/RDbsszWLpi">pic.twitter.com/RDbsszWLpi</a></p>&mdash; 獏星(ばくすたー) / Megumi Baxter (@baku_dreameater) <a href="https://twitter.com/baku_dreameater/status/1211990346525077504?ref_src=twsrc%5Etfw">December 31, 2019</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

1. `デバイスの割り当て`を`MIDIコントローラ`にした状態で`キー割り当て`右の編集ボタンをクリックします。
2. `MIDIのノート割り当て`ウィンドウが現れるので、この状態で使用したいMIDIキーを9個、順番に押します。押したキーの番号は`変更後のノート`に記録されます。
3. 設定が完了したら`OK`をクリックしてウィンドウを閉じます。

ウィンドウを閉じたのち、設定したMIDIキーを押してみて、表情が変わることを確認します。


**ヒント:**

`アニメーション終了後も表情を維持`をオンにしたアイテムで表情を切り替える場合、表情をリセットする機能が必要になるはずです。

以下のような設定のアイテムを作ることで、表情をリセットできます。このアイテムは既定の設定で、`reset`という名称で含まれています。

{% include docimg.html file="/images/about_settings/img01_130_word_to_motion_reset_tips.png" %}
