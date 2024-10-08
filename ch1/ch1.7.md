## 課税と死荷重損失

市場取引を通じた均衡では余剰が最大化されることがわかった．一方で我々が普段財を購入する市場では税が課されている．この節では課税がどのような影響をもたらすのかを簡単に見てみよう．

課税には消費税、所得税、法人税などいろいろあるが、ここでは財の購入に税が課されるものとしよう．一単位購入するごとに$t$円を税として支払わなければならないとする．こういったタイプの課税を**従量税**と呼ぶ[^note9]．
つまり消費者は$q$だけ財を購入すると$(p+t)\times q$だけ支払わなくてはならない．これは価格が実質$p+t$になったようなものである．


[^note9]:日本の消費税は価格に比例するタイプの税である．つまり消費者の支払額は$(1+\tau)\times p\times q$となる．（$\tau$は税率）こういうタイプの税を**従価税**と呼ぶ．

一方で生産者の方は$p\times q$だけ受け取る．$t\times q$の部分は税収となり政府の懐に入る．この事実からわかることは消費に課税すると消費者と生産者が直面する価格が変わるということである[^note10]．

[^note10]:生産に課税しても同じ．

社会的総余剰の最大化条件は$v'(q)=C'(q)$であった．
いま、課税がなされている状況で消費者の効用最大化条件から導かれるのは$v'(q)=p+t$という条件である．消費者にとっての価格は$p+t$に変わってしまっているからだ．一方で生産者にとっての条件は$p=C'(q)$のままである．したがって
```{math}
v'(q)=p+t>p=C'(q)
```
となり、社会的総余剰最大化条件と一致しない．したがって課税があれば市場での余剰最大化はうまく行かない[^note11]．

[^note11]: この場合、生産量が過少になる．これはなぜか確かめてみよ．(少し難)

このことを図を用いて確かめてみる．
課税のある場合の均衡を図示すると{numref}`tax`のようになる．

```{figure} ./ch1_img/tax_ch1.svg
:name: tax

従量税の影響
```

消費者の直面する価格は$p^*+t$であるが、生産者の直面する価格は$p^*$である．それらの価格のもとでの需要量と供給量が一致する場合が均衡である．需要関数と供給関数を使って書くと$D(p^*+t)=S(p^*)$となる価格が均衡価格になる．{numref}`tax`における四角形の部分は税収を表している．税収も余剰に含めるとしても余剰の合計は減少している．その減少した余剰のことを課税による**死荷重損失**と呼ぶ．

### どのような財に課税すべきか

従量税を課すと死荷重損失が出ることは見てきた．これは課税が社会にどれだけ悪さをしているかを表す一つの指標となる．では課税（一定額の税収）がどうしても必要なとき、そしてそれが従量税でなくてはならないとき、どのような財に課税するのが良いのだろうか．この問題は**最適課税理論**という財政学の一分野で研究されている問題である[^note12]．
ここでは極めて簡単な場合を考えよう．

[^note12]: 詳しくは財政学や公共経済学の教科書を参照せよ．最適課税論の教科書としては洋書であるが、Salanié (2011) _the Economics of Taxation_, 2nd ed., MIT press がある．

まず、供給曲線を水平にする．そして均衡点を基準に需要曲線を回転させて、傾きの異なる需要曲線を比較する．これを見たのが{numref}`optax1`である．一段目左図を基準に需要曲線を水平にしたものが右の図であり、より傾きを急にしたのが二段目の図である．これを見ると、傾きを水平にしたものは死荷重損失が税収に比べてはるかに多い．一方、傾きを急にした図では死荷重損失は税収と比べてみても少ない．したがって同じだけ従量税を課すならば税収に比べて死荷重が少ない、傾きが急な財に課税すべきであるということだ．

では需要曲線の傾きが急な財とはどのような財であろうか．これは価格が変化しても需要量の減りが少ない財である．{numref}`optax1`をみてもわかるように傾きが急な需要曲線をみた図では課税前の均衡取引量$q^{\text{前}}$と課税後の取引量$q^{*}$の差は比較的小さいが、傾きが水平に近い需要曲線の場合にはその差ははるかに大きい．このように価格の変化に対して需要量が変化しにくい財、つまり傾きが急な需要曲線を持つは**必需財**と呼ばれている．一方で、価格の変化に対して需要量が大きく変化しやすい、水平に近い需要曲線を持つ財は**奢侈財**と呼ばれる．
この分析が示すことは、奢侈財よりも必需財に課税すべきであるということだ[^note4].

[^note4]:これを考案者の名前をとってラムジールールと呼ぶ．

もちろんこの分析は考慮すべき要素をいくつも省いている．ここで考慮しなかったことを含めればどのような財に課税すべきという結論になるかは最適課税論の重大な論題のひとつである．

```{figure} ./ch1_img/optax1_ch1.svg
:name: optax1

死荷重損失の比較
```

以下の動画で確認するとよりわかりやすい．死荷重損失の大きさを表す三角形の面積のうち，需要曲線の傾きが水平に近くなるにつれ，高さは変わらず，底辺だけが増えていく．すると面積（死荷重損失）は増大する．

```{figure} ./ch1_img/tax.gif
:name: taxgif

動画で見る死荷重損失の比較
```