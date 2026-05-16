# Driving in the USA
<img width="300" height="210" alt="image" src="https://github.com/user-attachments/assets/74440051-63fe-4233-81cd-393cf6f773d9" />

### アメリカの砂漠道路を走りながら音楽を楽しむ雰囲気系ゲーム。
* スタン・ハンセン味、テリーマン感、イージーライダー味、西部劇味、アメリカ西部の砂漠を走るイメージ。
* 映画『バグダッドカフェ』（見てない）、『シェルタリングスカイ』など夕日の砂漠イメージから着想。

イメージ↓
* https://www.youtube.com/watch?v=XTYLsULsefs&list=RDXTYLsULsefs&start_radio=1 （※シェルタリングスカイの砂漠は北アフリカ）
* https://www.youtube.com/watch?v=oCLpLWcX2cg&list=RDoCLpLWcX2cg&start_radio=1

### PC専用、スマホ非対応
* PC専用。ゲームコントローラー使用可能。
* スマホ適応するとボタン配置が必要で没入が妨げられるし、何分もスマホ構えてプレイするようなゲームではないのでスマホは切り捨てる。

## 内容・制作情報

### ラジオ
* NHKと米国等のネットラジオをリアルタイムに聴ける。
* 日本のRdaiko系はめんどいので回避。

### 音楽
* 音楽は裏でyoutube接続して音を引っ張ってくる仕組みなので著作権問題をたぶんクリア。
* 自前リソースに依存せずyoutubeを使用するので、ほぼ無限にラインナップを増やすことが可能。
* 公式動画、公式音声をなるべく使用している。
* ラインナップは好みとか知ってるやる等を入れてるが、大原則として雰囲気に合致するか否かの基準でピックアップしている。
* 70~80~年代を多くしている。平成感、2000年以降感が強いものはあまり入れていない。
* 特定アーティストからのピックアップは多くて3～4曲までに限定した。

### 演出
音楽に合わせて空の色、星の有無、雨の有無などが変化する。
空は上空と地平線近くの2種類を設定可能。
個別設定なので、とくに設定していない曲が多い。
雰囲気系だと紫系の色を選びがちで、それじゃ芸がないというのもある。
一部、youtubeの音が大きすぎるものは個別で音量自動設定しているものがある。
設定はmusiclistに記述する仕組み。

### 砂漠空間
* 8つの砂漠空間をつなげて延々と走り続けることができる仕組み。
* たまに道路看板、ガソリンスタンド、ケンタッキーフライドチキン、バグダッドカフェが登場する。
* エドワード・ホッパー『ナイトホーク』みたいな店が出てきたらそろそろループの終末が近い。
* 3D空間はスケッチアップWEBで制作、謎の独自型式SKPから一般的なGLBに変換する際の色情報喪失などに苦戦した。
* 無料著名ソフト・ブレンダーなど使ってみたが煩雑すぎて難易度が高そうだったので早々に見切りをつけた。
* 最終的には、スケッチアップの7日間フリートライアルに加入してGLB出力した。
* 衝突設定は無し。ゴーストライダー的な。死んで浮遊しているのかもしれない。

* <img width="300" height="303" alt="image" src="https://github.com/user-attachments/assets/9170510b-f5f2-4e37-b8d1-92dd9f11373d" />  　
* <img width="300" height="140" alt="image" src="https://github.com/user-attachments/assets/935ae174-6fad-47cd-94f5-6ad42bae2e22" />  
* <img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/3922ddbd-f3e2-4e99-9780-c017fb9b27e3" />  
* <img width="300" height="320" alt="image" src="https://github.com/user-attachments/assets/4fbee28e-7c48-4b03-8076-ec77f5b4bdf4" />  
* <img width="300" height="270" alt="image" src="https://github.com/user-attachments/assets/4183cdd6-c4e2-40fc-b026-1e6075e4ed3f" />  

## インストール
* ウェブのブラウザでプレイできる。
* インストールしてmusiclistをいじれば誰でも好きな音楽ラインナップでゲームできる。
* デスクトップでプレイする場合はサーバー云々の手間が発生するが、AIを使えば問題ないレベル。

## ゲーム概要
* タイトル: Driving in the USA
* ファイル: index.html（シングルファイル構成）
* エンジン: Three.js r0.163.0（importmap CDN経由）
* 音楽: YouTube IFrame API + hls.js（ネットラジオ）

## 捜査

### キーボード:
* Space       アクセル（押しっぱなし）
* B           ブレーキ（押しっぱなし）
* ↑↓         曲選択（musiclistを上下に移動）
* ←→         YouTubeの巻き戻し／早送り（±10秒）
* Y           曲を決定・再生 / 再生中は再生停止トグル
* A           速度計・曲名表示 の 表示/非表示トグル
* ESC         タイトル画面（ポインターロック解除）

### ゲームパッド（Standard Mapping 準拠）:
* RT(buttons[7])      アクセル
* LT(buttons[6])      ブレーキ
* Bボタン(buttons[1]) ブレーキ（LTと同じ）
* Yボタン(buttons[3]) 決定・再生停止
* Aボタン(buttons[0]) 表示/非表示トグル
* 十字上(buttons[12]) 曲を上に選択
* 十字下(buttons[13]) 曲を下に選択
* 十字左(buttons[14]) 巻き戻し -10秒
* 十字右(buttons[15]) 早送り +10秒
* Selectボタン(buttons[8]) タイトル画面

