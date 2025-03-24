# Left Slinger

*※ 2025/03/25 キーケット2025で頒布したLeft SlingerのキットにてMCUカバープレート取り付け用のネジが不足している可能性があります。ご自身で[8mmのネジを購入して頂く](https://shop.yushakobo.jp/products/a0800n2?variant=37665433026721)か、[@takashicompany](https://x.com/takashicompany)までご連絡いただけましたら発送致します。お手数をおかけしますが、どうぞよろしくお願いいたします。*

<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/01.jpg?raw=true" width = "600px" />

Left Slinger(レフトスリンガー)はジョイスティックとロータリーエンコーダーを搭載した18キーの左手用のマクロパッドです。  
奥側の放射状のキーレイアウトと手前側の矢印キーのユニークな配列を採用しました。  
キースイッチソケットを搭載可能なため、キースイッチの交換が容易に行えます。  
ジョイスティックはポインター操作の他に、奥、左奥、左の3方向にキー入力をアサインするモードを搭載しております。  

<img src = "https://github.com/user-attachments/assets/e409d76a-e8d3-4c19-93c4-f15289b5f3ee?raw=true" height = "300px" /><img src = "https://github.com/user-attachments/assets/0e51f79d-1dd9-4cca-963b-64446c8a8563" height = "300px" />

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
|[短いネジ(M2 5mm)](https://shop.yushakobo.jp/products/a0800n2?variant=37665432993953)|9||
|[中ぐらいのネジ(M2 8mm)](https://shop.yushakobo.jp/products/a0800n2?variant=37665433026721)|3||
|長いネジ(M2 12mm)|6||
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
|[キースイッチソケット(MX)](https://shop.yushakobo.jp/products/a01ps)|18|キースイッチの取り替えが容易になります。基本的には使用することをオススメします。当ビルドガイドはキースイッチソケットを用いた例のみを紹介しております。|

# 組み立て方

## 1. 基板の表裏を確認する

### 表
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/010-01.jpg?raw=true" width = "600px" />

### 裏
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/010-02.jpg?raw=true" width = "600px" />

## 2. ダイオードのハンダ付け

基板にダイオードをハンダ付けします。ダイオードはキースイッチを押下した際に電流をMCUに伝達する役目を持ちます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-01.jpg?raw=true" width = "600px" />

ダイオードは基板の裏側から取付けます。ダイオードの配置箇所の「`▷|`」の縦線とダイオードの黒い線の方向が同じになるように置きます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-02.jpg?raw=true" width = "600px" />

ダイオードが基板の穴を通るように足を折り曲げます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-03.jpg?raw=true" width = "600px" />

ダイオードの足を基板に通します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-04.jpg?raw=true" width = "600px" />

反対側からダイオードの足が出ていることを確認します。
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-05.jpg?raw=true" width = "600px" />

基板とダイオードの足をハンダ付けします。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-06.jpg?raw=true" width = "600px" />

ハンダ付けした後にダイオードの足をニッパーなどで切ります。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/020-diode-a-07.jpg?raw=true" width = "600px" />

## 3. MCUの取付け

MCU(Micro Controller Unit)は簡単に説明するとキーボードの頭脳部分です。キースイッチ等の入力を処理してPC等に伝達します。  

当キーボードでは、Waveshare RP2040-Zeroを使用します。  
<img src = "https://github.com/user-attachments/assets/f00b9381-6d04-48e2-aeb9-90fa7b754eb1" width = "600px" />

下図の位置にMCUを置きます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/040-rp2040-zero-02.jpg?raw=true" width = "600px" />

基板のハンダ付けの銀箔とMCUのハンダ付け箇所が合致するように位置合わせを行います。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/040-rp2040-zero-03.jpg?raw=true" width = "600px" />

基板とMCUをハンダ付けします。置き場所がズレていないかを随時確認しながらハンダ付けを行います。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/040-rp2040-zero-04.jpg?raw=true" width = "600px" />

全部で23箇所をハンダ付けしたら完了です。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/040-rp2040-zero-05.jpg?raw=true" width = "600px" />

## 4. ファームウェアの書き込み

ファームウェアは[こちら](https://github.com/takashicompany/left_slinger/raw/refs/heads/master/firmwares/takashicompany_left_slinger_via.uf2)からダウンロードできます。
ソースコードは[こちら](https://github.com/takashicompany/qmk_firmware/tree/master/keyboards/takashicompany/left_slinger)です。

ファームウェアの書き込み方は[こちら](https://github.com/takashicompany/build-guide/blob/master/firmware/qmk-rp2040-zero.md)を御覧ください。

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

3方向入力は下図になります。  
<img src = "https://github.com/user-attachments/assets/e409d76a-e8d3-4c19-93c4-f15289b5f3ee?raw=true" height = "300px" /><img src = "https://github.com/user-attachments/assets/0e51f79d-1dd9-4cca-963b-64446c8a8563" height = "300px" />


## 5. キースイッチソケットの取付け

キースイッチソケットは基板とキースイッチを接続するものです。この部品を用いることでキースイッチ自体を基板にハンダ付けする必要がなくなるのでキースイッチの交換が容易になります。  

<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/060-switch-socket-01.jpg?raw=true" width = "600px" />

キースイッチソケットは基板の裏側に取付けます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/060-switch-socket-02.jpg?raw=true" width = "600px" />

基板にあるキースイッチハンダ付け箇所の片側にハンダを載せておきます。([予備ハンダ](https://www.p-ban.com/htmlmail_qanda/2019/12/))  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/060-switch-socket-03.jpg?raw=true" width = "600px" />

キースイッチソケットをピンセットで持ちながら予備ハンダを溶かしながらソケットの片側と基板をハンダ付けします。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/060-switch-socket-04.jpg?raw=true" width = "600px" />

もう片方もハンダ付けをします。  
<!--
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/060-switch-socket-05.jpg?raw=true" width = "600px" />
-->

## 6. ジョイスティックの取り付け

ジョイスティックを基板にハンダ付けします。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-04-js-01.jpg?raw=true" width = "600px" />

ジョイスティックはキーボードの右手前側に取り付けます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-04-js-02.jpg?raw=true" width = "600px" />

穴に挿し込んだ後、基板を裏返してジョイスティックの足が出ていることを確認してハンダ付けを行います。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-04-js-03.jpg?raw=true" width = "600px" />

## 6. キースイッチとプレートの取付け

スイッチプレートに保護シートがある場合は剥がしてください。アクリル板の場合は水を少量つけてピンセットで端を持つと剥がれやすいことがあります。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-01.jpg?raw=true" width = "600px" />

基板の上にスイッチプレートを載せます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-02.jpg?raw=true" width = "600px" />


キースイッチを用意します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-03.jpg?raw=true" width = "600px" />

数個のキースイッチをスイッチプレートに挿し込んで、基板とスイッチプレートをキースイッチで仮止めします。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-04.jpg?raw=true" width = "600px" />

全てのキースイッチを取付けます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/070-switch-07.jpg?raw=true" width = "600px" />

## 7. ロータリーエンコーダの取付け

ロータリエンコーダは回転操作による入力が可能です。スクロール操作によく使われます。ロータリーエンコーダによっては押し込みによりキー入力が可能なものもあります。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/071-rotary-01.jpg?raw=true" width = "600px" />

基板の表面にロータリーエンコーダーを差し込みます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/071-rotary-02.jpg?raw=true" width = "600px" />

基板の裏側からロータリーエンコーダの足が出ていることを確認します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/071-rotary-03.jpg?raw=true" width = "600px" />

ロータリーエンコーダの足と基板をハンダ付けしたら完了です。
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/071-rotary-04.jpg?raw=true" width = "600px" />

## 8. ボトムプレートの取付け

ボトムプレートに保護シートがある場合は剥がしてください。アクリル板の場合は水を少量つけてピンセットで端を持つと剥がれやすいことがあります。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/080-bottom-01.jpg?raw=true" width = "600px" />

底上げプレートが2-3枚同梱されている場合はそちらも保護シートを剥がしてください。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8988.jpg?raw=true" width = "600px" />

スペーサーとネジを使用してボトムプレートとスイッチプレートを固定します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/080-bottom-02.jpg?raw=true" width = "600px" />

底面側からネジ穴にネジを挿します。  
底上げプレートは重ねて長いネジで、それ以外の箇所は短いネジを挿してください。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8990.jpg?raw=true" width = "600px" />

ボトムプレートの上面側から挿したネジをスペーサーで固定します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/080-bottom-04.jpg?raw=true" width = "600px" />

ボトムプレートの上に基板とスイッチプレートを重ねます。  
(写真では底上げプレートを付け忘れています。ご了承ください。)  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/080-bottom-05.jpg?raw=true" width = "600px" />

スペーサーとスイッチプレートをネジで固定します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8979.jpg?raw=true" width = "600px" />

## 9. MCUカバープレートの取り付け

*※ 2025/03/25 キーケット2025で頒布したLeft SlingerのキットにてMCUカバープレート取り付け用のネジが不足している可能性があります。ご自身で8mmのネジを購入して頂くか、[@takashicompany](https://x.com/takashicompany)までご連絡いただけましたら発送致します。お手数をおかけしますが、どうぞよろしくお願いいたします。*

MCUカバープレートに保護シートがある場合は剥がしてください。アクリル板の場合は水を少量つけてピンセットで端を持つと剥がれやすいことがあります。  

<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8981.jpg?raw=true" width = "600px" />

取り付けには8mm程度のネジを使います。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8984.jpg?raw=true" width = "600px" />

MCUカバープレートをスイッチプレートに重ねます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8982.jpg?raw=true" width = "600px" />

ネジでMCUカバープレートとスイッチプレートをスペーサで固定します。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8985.jpg?raw=true" width = "600px" />

## 9. ゴム足シールの取り付け

当キーボードはゴム足シールを2種類用意しています。

手前側 : 薄め(3個入りです。画像は6個になっていますが。)  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8986.jpg?raw=true" width = "600px" />

底上げプレート用 : 厚め(3個入りです)  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8991.jpg?raw=true" width = "600px" />

ご自身の打鍵スタイルにあわせてゴム足シールを貼り付けてください。以下は例です。
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8992.jpg?raw=true" width = "600px" />

## 10. キーキャップを取り付ける

キーキャップを取り付けます。  
<img src = "https://github.com/takashicompany/left_slinger/blob/master/images/build/IMG_8994.jpg?raw=true" width = "600px" />

### 11. 完成した後の楽しみ方

完成しましたら、ぜひSNSなどに写真を投稿頂ければと思います。
Twitterのハッシュタグは [`#LeftSlinger #自作キーボード`](https://twitter.com/search?q=%23%E8%87%AA%E4%BD%9C%E3%82%AD%E3%83%BC%E3%83%9C%E3%83%BC%E3%83%89%20%23LeftSlinger&src=typed_query) を付けていただけると幸いです。
キットを組み立てた感想や、キーボードを使った所感などをお待ちしております！

また、毎週日曜日の１9時より実施されている[#KEEP_PD](https://twitter.com/hashtag/KEEB_PD?f=live)に投稿頂くこともオススメです。  
開催の告知は[@KEEB_PD](https://twitter.com/KEEB_PD)にて行われております。

ご不明な点などございましたら、[@takashicompany](https://twitter.com/takashicompany)にメンションやDM頂ければ回答できるかと思います。







