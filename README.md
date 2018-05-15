五月祭プログラミング教室
====
## 概要
* ArduBlock(ScratchのArduino版みたいなやつ)を用いて車を動かしてもらう
* 立体迷路を用意して, 車が迷路をクリアできるようなプログラムを作ってもらう    
![車](https://user-images.githubusercontent.com/25577208/40037747-d11ff9e8-5849-11e8-8799-b406a3193a66.png)![ArduBlock](https://user-images.githubusercontent.com/25577208/40037817-2dd02168-584a-11e8-8b94-d6802e7f7ccc.png)  
* 車には前と右に超音波距離センサがついている  


## 当日の流れ
* mae-stop.abp→mae-kabe-stop.abp→right-hand-method.abpの順にやってもらう  
* ArduBlockはArduinoの「ツール」→「ArduBlock」で開く
* ArduBlockの「開く」→「〇〇.abp」を選択するとスケッチが開く

### mae-stop.abp
* 「1秒前進し, 1秒停止する」プログラムの作成

### mae-kabe-stop.abp
* 「前との距離が10cm以内になると前進していた車が停止する」プログラムの作成

### right-hand-method.abp
* 「右手法」プログラムの作成  
![迷路](https://user-images.githubusercontent.com/25577208/40037298-9ce214b0-5847-11e8-9323-f2db94f5e7b9.png)  

![右手法](https://user-images.githubusercontent.com/25577208/40037323-c1f00834-5847-11e8-8c52-8ad546b0adec.png)

* 右手法とは「迷路の右側をひたすらカベ沿いに歩くとゴールにたどりつく」という手法  
* ただし, スタートやゴールが迷路の内部にあると右手法が使えない場合がある  

## プログラムの実行の仕方
* ArduinoとArduBlockを開いた状態  
* 車とパソコンをUSBケーブルで接続し, Arduinoの「ツール」→「シリアルポート」→「COM〇(車によって数字が異なる)」を選択  
* ArduBlockで「Arduinoにアップロード」を選ぶとArduinoにコードが反映される  
* Arduinoで「検証(チェックマーク)」→「マイコンボードに書き込む(矢印マーク)」  
* USBケーブルを外し, 車の電源をonにすると動く
* 電源をoffにして終了

## 注意点
* PCは借り物なので, 近くに飲食物を置かせない
* はんだ付けが取れやすいので, できるだけ車の配線部分に触らないよう注意喚起
* ケーブルをつけたり外したりするのを力任せで行わせない
* 車がカベにぶちあたることがよくあるので, 当たった時に放置せずすぐに車を持ち上げることで故障を防ぐ
* ギヤボックス部分の六角シャフトが抜けやすいので, イモネジがきっちり締まっているか確認

