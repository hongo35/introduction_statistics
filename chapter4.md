### 第4章 確率
---
####4.1 確率とは？

1. さいころを一回投げたとき、6の目の出る確率は1/6。
2. 本当に6通りの結果が同等に起こりやすいのかは誰も証明できない。
3. 同等に起こりやすいと仮定すると現実現象を説明でき、大きな食い違いが無い為、そう約束する。

→上記のようなものを我々の構築する”確率モデル”とする。

---
####4.2 標本空間と確率

**基本事象** ・・・ 偶然に左右される実験可能な個々の結果（さいころを投げ、1の目が出る、2の目が出る…）e1,e2,…enと表せる。

**標本空間** ・・・ 基本事象の全体。Ω（オメガ）と表す。全事象とも呼ぶ。

さいころの例でiの目が出るという事象をeiと表せば標本空間Ωは下記のようになる。

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=\\Omega=\\{e_1,e_2,...e_n\\}) 

**事象** ・・・ 基本事象の集合であり、標本空間の部分集合。A,B,C,...等を用いて表す。

**空事象** ・・・ 何も含まない事象。φと表す。

![alt text](https://cacoo.com/diagrams/zvtzZh154Wz5NXG1-1190F.png) 

**和事象** ・・・ 二つの事象のどちらか一方が起こる。A ∪ B。

**積事象** ・・・ 二つの事象の両方が同時に起こる。A ∩ B。

**余事象** ・・・ 事象Aに対し、Aが起こらない。A（上にバーを付けた文字）。

**互いに排反** ・・・ 二つの事象が同時には起こりえない。


**確率**
> 確率は多数回の実験の中で, その事象の起こる回数の比率である

1. 任意の事象Aに対し、0 ≦ P(A) ≦ 1     
2. P(φ) =0, P(Ω)=1
3. AとBが互いに排反ならば、P(A ∪ B) =P(A) + P(B) [加法定理（確率の加法性）]

上記を満足する数値P(A)がそれぞれの事象Aに対し与えられるとき、P(A)を事象Aの確率とよぶことにする。


---
####4.3 確率の解釈

確率をどのように解釈するかは大きく二つに分けられる。

**客観説（頻度説）**
> 確率は多数回の実験の中で, その事象の起こる回数の比率である

だが、解釈しにくいものがある。
> 彼女の血液型がAB型である確率は40%だ

> K社の株式が2ヶ月いないに300円以上値上がりする確率は10%未満である

**主観説**
> 確率は特定の論理的命題によって表される事象が起こる確からしさの程度についての判断を表すものである


> 8章以降の統計的推測の議論では、客観説の解釈をとる。統計的推測は、現実の現象に付いて一定の確率モデル（あるいは統計モデルともいう）を想定し、その下ででーたから得られる客観的な乗法を分析し要約する事を目的とするので、主観的な要素を入れてはならないと考えるからである。

---
####4.4 条件つき確率、乗法公式、事象の独立性

**条件つき確率**
事象Aの確率P(A) > 0 の時、事象Aが起こったという条件の下で事象Bの条件つき確率P(B|A)は

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\(B|A\)={\\frac{P\(A{\\cap}B\)}{P\(A\)}) 

**乗法公式（乗法定理）**
条件つき確率を変形して下記。

![alt text](http://chart.apis.google.com/chart?cht=tx&chl={P\(A{\\cap}B\)}={{P\(A\)}\\times{P\(B|A\)}) 

**事象の独立性**

二つの事象A、Bについて下記が成り立つ場合をAとBとは独立であると言う。

![alt text](http://chart.apis.google.com/chart?cht=tx&chl={P\(A{\\cap}B\)}={{P\(A\)}{P\(B\)}) 

---
####4.5 ベイズの定理

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=A_1,A_2,...,A_a)が互いに排反であり、かつ、
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=A_1{\\cap}A_2{\\cap}...{\\cap}A_a=\\Omega)

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=B_1,B_2,...,B_b)が互いに排反であり、かつ、
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=B_1{\\cap}B_2{\\cap}...{\\cap}B_b=\\Omega)

とする。

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\(A_i\),\({i=1,2,...a,}\))

および

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\(B_j|A_k\)\({i=1,2,...a,}{j=1,2,...,b}\))

が与えられたとき、P(Ai|Bj)は

![alt text](http://chart.apis.google.com/chart?cht=tx&chl={P\(A_i|B_j\)}={\\frac{{P\(A_i\)}{P\(B_j|A_i\)}}{\\sum_{k=1}^aP\(A_k\)P\(B_j|A_k\)}}\({i=1,2,...a,}{j=1,2,...,b}\))


（※編者注：事象Aが先に起こった条件として得た確率を用いて、事象Bが先に起こる場合にはどのような確率になるかを示している？ツッコミ歓迎）

---
####4.6 順列・組合せ

#####4.6.1 順列
一般にn個の異なるものから、r個を取り出して並べて作る順列の数をnPrと表すと

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=_nP_r=n\(n-1\)...\(n-r%2b{1}\))

**階乗**の記号を

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=n!=n\(n-1\)...1)

で定義し、0!=1と約束すれば

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=_nP_r=\\frac{n!}{\(n-r\)!})

#####4.6.2 組合せ

一般に、n個の異なるものからr個を取り出して並べて作る**組合せ**の数をnCrと表すと

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=_nC_r=\\frac{_nP_r}{r!})

階乗の記号を用いて

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=_nC_r=\\frac{n!}{r!\(n-r\)!})
