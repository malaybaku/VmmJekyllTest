
# Frequently Asked Questions

[English](./en_frequently_asked_questions.html)

## Q1. 動作環境は？

Windows 10で動作します。

リップシンクでは通常のマイクのほか、仮想マイク入力も選択できます。このため、ボイスチェンジャー出力をもとにリップシンクすることも可能です。

ウェブカメラは視野角が狭めで、顔全体が映るものを使用してください。VMagicMirrorではおよそ320x240の解像度に圧縮してウェブカメラの映像を用いるため、解像度が低いカメラを使っても問題ありません。

CPUやグラフィックボードは最低要件としてはほぼ何でも動作しますが、リップシンク、影の表示、顔トラッキングではCPU負荷が高くなります。

開発者は以下の環境で動作チェックしています。

* 環境1: デスクトップPC 
    + CPU: Intel Core i7-6700K
    + GPU: GeForce GTX 1080
    + チェックしたマイク入力
        + VoiceMeeter Bananaの出力
        + VT-4 WET (変声済みのVT-4の出力)
        + C922 Pro Stream Webcam
    + チェックしたウェブカメラ
        + C922 Pro Stream Webcam
* 環境2: ノートPC(Surface Book 2)
    + チェックしたマイク入力
        + PC本体マイク
    + チェックしたウェブカメラ
        + PC本体フロントカメラ

開発者はVMagicMirrorの課題として、特定環境で動作が重くなることを認識しています。

もしお手元のPCでVMagicMirrorの動作が重すぎる場合、分かる範囲でPC環境を記載のうえ開発者までご連絡下さい。


{% include_relative sitemap.md %}
