# Left Slinger

# 組み立てに必要なもの

## キットに同梱されているもの

|部品|個数|備考|
|:--|:--|:--|
|基板|1||
|キースイッチプレート|1||
|ボトムプレート|1||
|MCUカバープレート|1||
|底上げプレート|2 or 3|2mm厚を3枚 or 3mm厚を2枚のいずれか。|
|[ダイオード(リードタイプ)](https://shop.yushakobo.jp/products/a0800di-01-100)|18||
|[ウレタンクッション](https://shop.yushakobo.jp/products/a0800ur-01-6)|3|滑り止めとして底面に貼ります。|
|[ウレタンクッション(5mm厚)](https://www.yodobashi.com/product-detail/100000001003359892/)|3|滑り止めとして底面に貼ります。|
|[ネジ(M2 5mm)](https://shop.yushakobo.jp/products/a0800n2?variant=37665432993953)|12||
|ネジ(M2 12mm)|6||
|[スペーサー(M2 6mm以上)](https://shop.yushakobo.jp/products/a0800c2?variant=37665435189409)|9||

## ご自身で用意いただくもの
|部品|個数|備考|
|:--|:--|:--|
|[RP2040-Zero](https://talpkeyboard.net/items/640ea9f3072c3c538731c515)|1||
|[ロータリーエンコーダ](https://shop.yushakobo.jp/products/3762)|1||
|[小型アナログジョイスティック](https://www.switch-science.com/products/2892?srsltid=AfmBOorPHoOU9B2cyXs_Br7kAcbDDWK3j9G4ZUs7ezuBqDBhf63sDdMf)|1||
|[Cherry MX互換キースイッチ](https://shop.yushakobo.jp/collections/all-switches)|18||

## お好みで

|部品|個数|備考|
|:--|:--|:--|
|[キースイッチソケット(MX)](https://shop.yushakobo.jp/products/a01ps)|18|キースイッチの取り替えが容易になります。|

## ファームウェア

ファームウェアは[こちら](https://github.com/takashicompany/left_slinger/raw/refs/heads/master/firmwares/takashicompany_left_slinger_via.uf2)からダウンロードできます。
ソースコードは[こちら](https://github.com/takashicompany/qmk_firmware/tree/master/keyboards/takashicompany/left_slinger)です。

ファームウェアは[Remap](https://remap-keys.app/)に対応しておりますので、ブラウザからキーマップを変更可能です。

レイヤー6はマウスレイヤーとなっており、ジョイスティックを操作してポインターが移動した際に自動で切り替わるレイヤーです。

レイヤー7は設定変更のために用意したレイヤーです。赤丸の箇所を同時押しすると有効になります。  

<img src = "https://github.com/user-attachments/assets/3fe65462-c83e-4e15-8d9c-a42ca1d6b176" width = "600px" />

不要の場合は使用しなくてもOKです。  

以下は Left Slinger専用のキーです。
Remapなどで指定すると使用可能となります。

|Remapでの表記|キー名|説明|
|:---|:---|:---|
|USER 0|左クリック|マウスの1ボタン目です。主に左クリックとなります。|
|USER 1|右クリック|マウスの2ボタン目です。主に左クリックとなります。|
|USER 2|第3クリック|マウスの3ボタン目です。|
|USER 3|スクロール入力|ジョイスティックがポインター操作になっている場合、このキーを押下した状態でジョイスティックを操作するとスクロール入力になります。|
|USER 4|マウスレイヤー移行移動量増加|マウスレイヤーを有効にするための判定の閾値を増加させます。値が大きくなるほどポインター操作を長くしないとマウスレイヤーが有効になりません。|
|USER 5|マウスレイヤー移行移動量減少|マウスレイヤーを有効にするための判定の閾値を減少させます。値が少なくなるほどポインター操作が小さくてもマウスレイヤーが有効になります。|
|USER 6|縦スクロール方向|スクロール入力キーを用いてスクロールする際の垂直方向の向きを変えます。|
|USER 7|横スクロース方向|スクロール入力キーを用いてスクロールする際の水平方向の向きを変えます。|
|USER 8|ジョイスティック除数増加|ジョイスティックの入力の除数を増加させます。除数が増えるほどポインターの移動量が少なくなります。|
|USER 9|ジョイスティック除数減少|ジョイスティックの入力の除数を減少させます。除数が減るほどポインター移動量が多くなります。|
|USER 10|設定変更完了|設定変更レイヤーを終了してキーボードに保存します。|
|USER 11|ジョイスティック操作切り替え|ジョイスティックの操作を切り替えます。(ポインター操作 / 3方向キー入力)|
|USER 12|ジョイスティック3方向キー入力有効|このキーを押下している間は、ジョイスティック操作による3方向キー入力が可能です。|





