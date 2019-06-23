- 自作キーボードは 2019/03 から
- ソフトウェア系から来た新参


Notes:
軽ーく自己紹介。  
どうでもいいけど新参ってしんざんって読むらしいね。  
SKKで普通にしんさんで変換できたからそう読んじゃったよ〜〜〜 はい

---

<!-- .slide: data-background="img/normal-keyboard-background.jpg" -->

- Majestouch Minila Air 赤軸
- RealForce All 30g テンキーレス
- ちょうどいいキーボードがない

Notes:
MinilaAirはいいんだけどFnレイヤーの配置を変えたくなった  
RealForceを会社に買わせたけど、このときはALL30gのUS配列がなくてブチ切れながら妥協した

---

<!-- .slide: data-background="img/tweet-which-i-found-x-switch.png" data-background-size="70%" -->

Notes:
ぺかそさんのツイートを見かけてX Switchに出会った  
でもググっても情報がほとんどないんだな〜これが

---

<!-- .slide: data-background="img/kailh-compare.jpg" data-background-size="70%" -->

Notes:
比較記事を見つけた、ノートブック用と書いてある  
めっちゃ薄い やばい

---

## これや！！！(大阪弁)

Notes:
神やんけ。
(大阪出身なんで。)

---


<!-- .slide: data-background="img/aliexpress-x-switch.png" data-background-size="70%"  -->

Notes:
発表は2017年にされてたっぽいけど、調べても買ってる人はいないっぽい……  
AliExpressに見つけたけど、3月時点で購入数は0 (笑うところです)

---

<!-- .slide: data-background="img/x-switch-keycap-negotiation.png" data-background-size="auto 90%"  -->

Notes:
説明にはChocスイッチとキーキャップが同じと書いてあるけど、そんなわけはない(笑うところだよ)のでショップに問い合わせたら、白い無刻印キーキャップを売ってくれた！やったね！

---

- Let's splitを参考にキーボード用基板を作成
- [X switch用フットプリント](https://github.com/shikamiya/kicad-footprint-kailh-pg1425-x-switch)作成

Notes:
そこから沼に転落

---

<!-- .slide: data-background="img/x-switch-footprint-crane.png" data-background-size="50%"  -->

Notes:
今使ってるフットプリントの紹介  
ALPS/MX/Choc/X switch対応・WS2812-2020のボトムマウント対応・全部リバーシブル  
Chocスイッチは半田面の真ん中のジャンパを半田で繋いでね

---

<!-- .slide: data-background="img/x-switch-ready.jpg" data-background-size="30%"  -->

Notes:
私のフットプリントを使っておいていただければ、いつでもX Switchに対応できるので検討してみてください〜

---

<!-- .slide: data-background="img/pro-micro-roof.png" data-background-size="auto 90%"  -->

Notes:
Pro Microの屋根っていうのも作ってます。Pro Microを表面に配置するキーボードは、  
Pro Microの上にカバーを付けたり、持て余しているスペースだと思うので、その上にキーを配置できるようなものを考えてみました。  
他のキーがMXスイッチで、この上にX switchを配置すると、同じくらいの高さにできます。

---


<!-- .slide: data-background="img/infinity-possibility.png" data-background-size="auto 90%"  -->

Notes:
しろとりさんの無限の可能性を参考に、プレートが不要になるようにソルダジャンパでPCBマウントオンリーでキーボードを組めるようにしてみました。  
今のrev2では1/4Uずらしにも対応したので、任意のキーボードを作ることができます。  
LEDはSK6812miniではなく、WS2812-2020を採用しているのは、LEDが落ちてしまったりうまくいかないという声を聞いたからです。  
WS2812-2020は凸型になっているので、裏から穴にはまって比較的簡単に半田付けできると思います。  
ダイオードは表面実装とスルーホール部品に対応してます。  
スルーホールの方は、表面実装パッド近くの丸いスルーホールと、「K」シルク横の四角いスルーホールに接続することを想定してます。