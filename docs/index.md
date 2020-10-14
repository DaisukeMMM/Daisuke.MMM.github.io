# Ladybug+Hanybee Q&A
Ladybug+Hanybee勉強会の質問事項の回答です。この資料はかなり勉強になるのでつまづいたときにあたるとよいかもしれません。[→ladybug-primer](https://mostapharoudsari.gitbooks.io/ladybug-primer/content/)LBはPythonで書かれていますが、*コンポーネント名は大文字始まり、パラメータ名は小文字始まり*の点に注意してください。
# 見出し1
## 見出し2
### 見出し3
#### 見出し4
##### 見出し5
###### 見出し6
## 2020年1月20日 16:00-
* [リストの操作等参考リンク](https://note.com/kazuma7/n/nf0045d44c007)


---

## 2020年1月7日 16:00-
### Ladybugで出力される図のサイズ調整はどのように行えばよいか_秋山
* RhinoのCAD機能をつかって凡例を描いているので、なかなか難しいらしいです。
* 2014年の質問なので今後も対応なし？
* 細かい微調整はAiデータで出力して、Ai上で処理するという手もあります。
* Ladybugで描画した図形に対してスケールを定数倍指定してサイズを決めているので難しいのだと思われます。
* 凡例を細かく作りたい場合には[Create Legend](>https://rhino.github.io/components/ladybug/createLegend.html)コンポーネントを使うという手もあります。
その場合には各コンポーネントに備え付けの凡例は使わないでください。
* [→開発元回答](https://www.grasshopper3d.com/group/ladybug/forum/topics/view-dependant-legend)

> 参考ファイル（J:\◆【BIM】\【シミュレーション】\NS_ladybug_training\1_gh\11_日影図を作ろう.gh）

### 凡例の代表値が小数点第2位まで出力されるのはどのように調整するか_秋山
* 回答中（わかる方いらっしゃったら追記してください。）

> 参考ファイル（J:\◆【BIM】\【シミュレーション】\NS_ladybug_training\1_gh\11_日影図を作ろう.gh）

### "Sunlight Hours Analysis"の"disFromBase"の値はなぜ解析面から0だとまずいのか_秋山
* 0を指定してしまうジオメトリと解析面が交差してしまうのがよくないらしいです。
* 実際は解析面を対象面からほんの数ミリ浮いたところで計算して実用上は問題ないと思います。
* [→開発元回答](https://discourse.ladybug.tools/t/ladybug-sunlight-hours-analysis/4256)
* [→元のPythonコード](https://github.com/ladybug-tools/ladybug-legacy/blob/master/src/Ladybug_Sunlight%20Hours%20Analysis.py)

> 参考ファイル（J:\◆【BIM】\【シミュレーション】\NS_ladybug_training\1_gh\11_日影図を作ろう.gh）

### 『Suface』コンポーネントにオブジェクトを格納するのはなぜか_川津
* Grasshopperにおいてどのパラメータコンポーネントに入れるかは、普通のプログラミング言語における**変数型をなにを選ぶか**と同じです。
* つまりRhino側のモデルをどんなジオメトリ記述で出力するかを示しています。
* もちろん上の方法ができない場合もあるので、その時にはエラーが吐かれます。
* またパラメータコンポーネントを使うシーンとしては、そのコンポーネントに入っているものを明示する役割もあります。
* 大規模なファイルや他人と共同でファイルを作っていると、このコンポーネントにどんな値が入っているかわからなくなることも多いので、それを防ぐ意味です。
* ジオメトリの種類については詳しくは次の項目を読んでください。
> 参考ファイル（J:\◆【BIM】\【シミュレーション】\NS_ladybug_training\1_gh\13_太陽光発電量を計算しよう.gh）

### 主要なジオメトリの格納コンポーネント	
* BOX：長方形の面を押し出した立体として記述される。
* BREP：立体物を面と境界線の集合体として記述する。
* **Mesh**：FDに入力できる。小さな三角形を組合わせて面を作る
* FD Extrusion：FlowDesigner独自の立体オブジェクト形式。GHの基本コンポーネントの`Extrude`と似ているが、よりピュアなデータ形式。特に領域指定のハコは`FD Extrude`でなければなりません。

### データツリーの概念図
* 質問ではありませんがデータツリーの概念が難しいとのことだったので解説画像貼っておきます。
![](img/img1.jpg)
