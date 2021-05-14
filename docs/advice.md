# MEP MY advice
設計用の資料まとめ。目次は以下の通り、Ctrl+Fでキーワー検索したほうが使いやすいかもしれない。

* [定数・計算表](#定数・計算表)
* [災害対策](#)
* [空調](#)
* [衛生](#)
* [電気](#)
* [消防](#)
* [ガス](#)
* [](#)
* [](#)
* [](#)
* [](#)
* [建築基礎](#)
* [読んだり見たりして役に立ったもの](#読んだり見たりして役に立ったもの)


## 定数・計算表
ここにリストアップしているものはよく使うもの。

* [単位変換](https://www.convertworld.com/ja/)：CONVERT WORLD
* [空気状態計算（湿度・エンタルピ）](https://www.shinyei.co.jp/stc/service/water_converter.html)：神栄テクノロジー
* [各種公式（マニング等）](http://ebw.eng-book.com/heishin/vfs/)
* 騒音レベル計算：[点音源値自明の時](https://keisan.casio.jp/exec/user/1615367319)｜[点音源値不明の時](https://keisan.casio.jp/exec/user/1615366324)


### 物性値
* 乾き空気：密度*1.2*kg/m3、比熱*1.006*kJ/kg・K
* 水の融解熱：*334*kJ/kg
* 水の蒸発熱：*2257*kJ/kg

### 熱量の換算
* 1J = *4.186* cal
* 1USRT = *3.516* kwh

### 面積の換算
* 1坪 = *0.3025* m2

---

## A_基礎知識
まず役に立ちそうな基礎知識全般。

* 建築設備関連法規
* 事前調査
* 事前協議
* 建築確認申請の流れ
* 防災性能評価

* その他官庁諸届けの流れ
* 建築設備に関わる資格
* シックハウス法規制
* 省エネルギー法
* ハートビル法
* CASBEE

### 確認申請・行政協議
法規

* 消防法：具体的な消防同意のための細かな基準は[堺市消防同意基準](https://www.city.sakai.lg.jp/smph/kurashi/bosai/shobo/shokai/reiki/kijyun/setubikijun.html)が参考になる。]
* 省エネ法：確認審査機関の[TDC](http://www.tdc-web.co.jp/navi/01.html)に適合判定が必要な規模や検証方法あり。

## 災害対策
### 火事などの閉じ込めに対する「避難」対策
避難対策の仕様規定・性能規定の違い（ルートによる違い）は[この通り](https://www.izumi-bousai.jp/about/)。
* 地上から遠い位置から逃げるための[特別避難階段](https://syoubou123.com/2019/01/tokubetu-hinankaidan-toha/)
* 建築基準法と消防法両睨みする必要がある[排煙設備](https://archilink.jp/fluegas-facility)の概要。[設置基準](http://www.teral.info/pdf/t_catalog/2876/file.pdf)もそうだが、設備の場合ダクトやファンなどが火事の最中に[所定性能](https://www.mitsuyaj.co.jp/dcms_media/other/mitsuyafan-technote.pdf)を担保できることが大切。
* この[排煙設備設置基準のまとめ](https://kakunin-shinsei.com/smoke-exhaust-equipment/)も参考になる。

### 地震の揺れによる「崩壊」対策
* [Wikipedia耐震基準](https://ja.wikipedia.org/wiki/%E8%80%90%E9%9C%87%E5%9F%BA%E6%BA%96)
* [設備機器の耐震基準](https://setubisekou.com/construction-plan-earthquake-resistance/)




### 環境工学
* [貫流熱や表面からの熱損失の計算](https://www.hakko.co.jp/qa/qakit/html/s01050.htm)


### 原動機
設備機器はほとんどエネルギーを原動機に投じて仕事をさせる。

* 空気を送る[ファンモータ](https://www.orientalmotor.co.jp/tech/reference/)の性質。
* ファンなどは騒音も大きく[東京都環境確保条例](https://www.dinsgr.co.jp/sales/resolution/column/attention/28th/)などに該当する恐れもある
* 水を送る場合はポンプとなるが、能力（揚程）は[実揚程と全揚程](https://engineer-education.com/pump-11_actual-head/)が存在する。

### 弁
* 弁も流体の制御やかかる圧力によってフィットする種類がことなるので[これ](https://www.kitz-valvesearch.com/kiso/type_gatevalve.html)でしくみと併せて理解。

### 配管
くだらない語呂合わせですが、よく間違えるVU管とVP管の名称、それぞれ「ビニル薄い」と「ビニルポピュラー」で覚えています。。笑

* [配管の材料による違い](https://www.monotaro.com/s/pages/readingseries/haikankoujikisokouza/)は使用できる圧力や中を通る液体や気体の特性を考慮して選ぶ必要がある。
* [管材の寸法など（JIS規格ポケットブック）](https://jis.jts-tokyo.com/)
* [SUS管](http://www.jssa.gr.jp/contents/about_stainless/key_properties/types/)はその配合によって腐食耐性や脆性などが異なる。

### ダクト

* [ダクト風量計測器の例](https://www.wetmaster.co.jp/product/flowcontrol/ae/)

* [空気線図](https://www.techno-ryowa.co.jp/rrlab/)
* 
#### 塗装
* [日塗工]（https://www.toryo.or.jp/index.html）

### 制御
* [自動制御の専門用語](https://www.azbil.com/jp/corporate/pr/atoz/index.html)

### 工事・監理
* [CONCOMの現場管理の達人](https://concom.jp/contents/expert_supervision/)：写真付きでわかりやすい。

## 空調
### 熱負荷計算
* [熱負荷計算書](https://yunotebook.com/kutyo-netsukeisan/)は内部発熱として、[人体発熱](https://www.jstage.jst.go.jp/article/aijax/451/0/451_KJ00004077375/_pdf)を考慮する。

* [蒸気方式の基礎知識](https://www.tlv.com/ja/steam-info/steam-theory/steam-basis/1009steam/)


## 換気
* [電気室など特別室の換気回数](http://tkkankyo.eng.niigata-u.ac.jp/HASS/6.html)


## 【E】資料・関連法規
・[民間七会による工事請負約款契約書](http://www.gcccc.jp/contract/download.html)


### パッケージエアコン
室内機の種類を調べるには[こちら](https://kucho-ex.com/)（テクノ菱和）。
* [三菱電機](https://www.mitsubishielectric.co.jp/ldg/ja/air/guide/catalog/index.html)
* [木村工機](https://www.kimukoh.co.jp/catalog/)

### ビルマル
* [三菱電機](https://www.mitsubishielectric.co.jp/ldg/ja/air/guide/catalog/index.html)
* [ダイキン](https://ec.daikinaircon.com/ecatalog/index.html)

### EHP・モジュールチラー
* [三菱電機](https://www.mitsubishielectric.co.jp/ldg/ja/air/guide/catalog/index.html)

### 冷温水機
* [荏原冷熱](http://www.ers.ebara.com/product/absorption-h/)
* [Panasonic](https://panasonic.biz/appliance/air/nc/)

### ターボ冷凍機
[荏原冷熱](http://www.ers.ebara.com/product/absorption-h/)｜[三菱重工サーマルシステムズ](https://www.mhi-mth.co.jp/catalogue/list.html)｜[東芝キャリア](https://www.toshiba-carrier.co.jp/products/industry/index_j.htm)｜[川重冷熱工業](https://www.khi.co.jp/corp/kte/product/catalogue/)｜[日立グローバルライフソリューションズ（スクリュー冷凍機）](http://www.hitachi-ap-catalog.com/fl3/screw/html5.html#page=37)｜[ダイキン](https://ec.daikinaircon.com/ecatalog/DKCC012/index.html)｜[トレイン・ジャパン](https://www.jp.trane.com/commercial/asia-pacific/jp/ja/products/centrifugal.html)

### 冷却塔
冷却塔の基礎知識に関しては[こちら](http://shinwa-coolingtower.com/material/m01.html)（荏原冷熱技術資料）。
* [空研工業](https://www.kuken.com/catalog/)
* [荏原冷熱](http://www.ers.ebara.com/product/absorption-h/)
* [神鋼環境ソリューション](https://www.kobelco-eco.co.jp/product/cooling_tower/)


### ボイラ
ボイラの方式の違いに関しては[こちら](https://www.maedatekkou.co.jp/boiler/kind/)（前田鉄工所）。
* [サーモエナー](https://www.n-thermo.co.jp/products/)｜ [ヒラカワ](https://www.hirakawag.co.jp/products/)｜[昭和鉄工](https://www.showa.co.jp/data_download/catalog/heat.html)

### 放射空調
* [PS](https://ps-group.co.jp/download)
* [インターセントラル](https://www.i-central.co.jp/)

### 産業用除湿機
* [日立グローバルライフソリューションズ](http://www.hitachi-ap-catalog.com/fl3/sr-513r_01/html5.html#page=1)
* [三菱電機](https://dl.mitsubishielectric.co.jp/dl/ldg/wink/wink_doc/contents/doc/WEB_CATA/RIP6963482A/data/target.pdf)

### コジェネレーションシステム
* [ヤンマーエネルギーシステム](https://www.yanmar.com/jp/support/catalogs/energy.html)

### 吹出口
* [空研工業](https://www.kuken.com/catalog/)

### 加湿器
* [wetmaster](https://www.wetmaster.co.jp/download/)

### フィルタ
* [日本無機](https://www.nipponmuki.co.jp/catalog.html)

### ミスト
* [Panasonic](https://panasonic.biz/appliance/green-ac/)



## 衛生
### 給水
* 建物で必要な水量は主に1日の使用量を原単位から求め、[所定の計算方法](http://www.teral.info/pdf/t_catalog/356/file.pdf)で求めます。

### 排水
易しい[用語集](http://www.shincoo.com/shincoo/content/m044haisui-jitenn.html)があるので一読してから進めたい。特にこの分野は水理学者の名前が式名についていることも多く、[これ](http://library.jsce.or.jp/jsce/open/00027/1983/19-A06.pdf)も呼んでおくとよい。以下は図も豊富で排水の設計にがより楽になる資料。

・[排水ます・排水まわり工事イメージ](http://nihonhome.co.jp/blog/)
・[驚くほどわかりやすいマエザワの排水設備の設計の概要](https://www.maezawa-k.co.jp/school/sekkei/)

#### 汚水
* 排水の*自然流下の場合*には[マニングの式](http://ebw.eng-book.com/heishin/MeanFlowVelocityFormula_manning_formula_book.do?category=manning_formula)を利用して流速・流量を計算する、ただし宅内の配管材と屋外の管渠では係数等が異なるので注意が必要。
* 
* 地下など自然流下不可で、排水槽を設ける際の[注意点](https://www.gesui.metro.tokyo.lg.jp/contractor/pdf/41ccb1e759ec246374824ae10331a7e92a70595a.pdf)

#### 雨水
* 雨水の排水竪管はワイリーイートンの式に基づいて[SHASE学会基準でほぼ決まっています](https://www.chubu-net.co.jp/kenzai/pdf/D01.pdf)。
* 


### 消防
なかなかモノと名前、なんのためにその設備がそこに必要なのか分かりづらい部分もあるので一度目を通しておくと良いです。→[青木防災ブログ](https://www.aokibosai.com/%E3%83%96%E3%83%AD%E3%82%B0%E3%83%9A%E3%83%BC%E3%82%B8/)

* 自火報（自動火災報知器）の[種類・設置基準](https://electric-facilities.jp/denki9/kanchiki.html)
* また自火報によって感知したことを知らせる[地区音響装置の設置基準](https://www.minakami.co.jp/sekoukijun/design13.htm)

### ガス

### 電気
* 接地工事には[AからD](https://www.youtube.com/watch?v=oYDy0diGfi4)の種類があります。
* [駐車場のゲート管理](https://public-s.com/blog/2014/02/%E9%A7%90%E8%BB%8A%E5%A0%B4%E3%81%AE%E3%80%8C%E3%83%AB%E3%83%BC%E3%83%97%E3%82%B3%E3%82%A4%E3%83%AB%E3%80%8D%E3%81%AE%E5%BD%B9%E5%89%B2%E3%81%A8%E6%96%BD%E5%B7%A5%E6%96%B9%E6%B3%95/)

## 環境
気温度・圧力


・[【参考】日本建設連合会）建築技術者向け設備工事ポイントシート](https://www.nikkenren.com/kenchiku/equipmentpoint/mokuji.html)
・[建築各工事の流れ（東建）](https://www.token.co.jp/tochi_katsuyo/kenchiku_manu/index1.shtml)


* [大阪市建築基準法取扱い要領](https://www.city.osaka.lg.jp/toshikeikaku/page/0000021604.htm
* [EchoLand-plus. 冷凍機械責任者試験対策](http://www.echoland-plus.com/index.html)
* [オフィスビルの省エネ化とビルメンテナンス](http://www.fukuoka-bma.jp/%e3%83%93%e3%83%ab%e3%81%ae%e7%9c%81%e3%82%a8%e3%83%8d%e6%8c%87%e5%8d%97%e6%9b%b8-%e3%80%80%e3%81%9d%e3%81%ae%ef%bc%91/)：福岡県ビルメンテナンス協会


## 読んだり見たりして役に立ったもの
* [ヒートポンプの物理的背景](http://fnorio.com/0106heat_engine(refrigeration_cycle)1/heat_engine(refrigeration_cycle)1.htm)
* [1kPaとは？圧力の大きさについて](https://lifeisfruits.com/2018/07/28/about-pressure/)
* [ビル管理士総合情報.com](http://takeharu.lolipop.jp/)：設備士対策の入り口にはちょうど良いと思います。
* [図とキーワードで学ぶ建築設備のオーディオブック](https://www.youtube.com/user/niitPBL2012/videos)
* [下水のしくみ（分流・合流式）](https://www.youtube.com/watch?v=A5MFcMlckas)
* [交流の発明](https://www.youtube.com/watch?v=7QBDSJk7piE&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=22&t=4s)
* [ヒートポンプのしくみ](https://www.youtube.com/watch?v=sby40QSgfx4&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=16)
* [止水の重要性](https://www.youtube.com/watch?v=vy19g8MGht0&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=186)
* [冷凍機のしくみ](https://www.youtube.com/watch?v=uXjVsIDKn4E&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=15)
* [アルミニウムとカーテンウォール](https://www.youtube.com/watch?v=OPjXjdL1_wU&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=31&t=9s)
* [建築構造と振動](https://www.youtube.com/watch?v=t1Qz_buAsuQ&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=3)
* [生活とモデュール](https://www.youtube.com/watch?v=bCom11D_0qs&list=PLG8XhSHgFrA-Rd3gxoEQP6Q23trQzkDDe&index=42&t=9s)


