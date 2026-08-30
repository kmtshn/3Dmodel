# Realtime 3D Motion Capture

ブラウザのWebカメラまたは動画ファイルから人物の姿勢を推定し、Three.js上の3Dモデルへリアルタイム反映するデモです。

## Features

- Webカメラのリアルタイム姿勢推定
- カメラデバイス切替
- 動画ファイル入力
- MediaPipe Pose Landmarker（最大3人）
- Three.js / Xbot GLBへのボーン反映
- 入力映像の表示・非表示
- 骨格オーバーレイ
- 前後反転・基準リセット
- Render FPS / Pose FPS表示

## Run

カメラAPI (`getUserMedia`) のため、HTTPS または localhost で開いてください。GitHub Pagesでの公開に向いています。

`index.html` 単体の静的アプリなのでビルドは不要です。

## Notes

姿勢推定はブラウザ内で実行されます。このアプリ自身には録画・映像アップロード処理はありません。CDNからThree.js、MediaPipe、Xbotモデル、Pose Landmarkerモデルを読み込みます。
