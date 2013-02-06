### 第6章 主な確率分布  
---
  
#### 6.1 2項分布  

(1)試行の結果がSかFのどちらかである.  
(2)すべての試行についてSの起こる確率は一定である.  
(3)試行の間では何の関係もない(独立である).  

この3つの条件を満たす試行の列を **ベルヌーイ試行列** とよぶ.  

一般に,各試行でSの起こる確率をpとした時,n回のベルヌーイ試行列でSの起こる回数xの確率分布は次の確率関数により与えられる.  

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=p(x\)=\\begin{eqnarray}{}_nC_x\\end{eqnarray}p^{x}q^{n-x})  

ここで,q=1-pである.この確率分布を **二項分布** とよぶ.  

pおよびnを指定して初めて1つの具体的な分布になるが,これをB(n,p)と表す.  

**2項分布の平均と標準偏差**  

一般の2項分布B(n,p)については  
平均  μ=np  
分散  ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=\\sigma^2=npq)  
標準偏差  ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=\\sigma=\\sqrt{npq})  

であることが示される.(証明はテキストを参照)  

---
#### 6.2 ポアソン分布  

確率変数xの確率関数が,  

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=p(x\)=\\frac{\\lambda^x}{x!}e^{-\\lambda})  

で与えられる時,これを(平均λ)の **ポアソン分布** という.  

ポアソン分布は,事故の件数,機械の故障回数や電話の呼び出し数などのように,起こることが頻繁ではない事象の一定時間内の生起回数の確率分布として用いられることが多い.  
ポアソン分布は2項分布の極限として与えられる.数式はテキストを参照.  

---
#### 6.3 正規分布  

正規分布は,統計学において最も重要な連続型の確率分布であり,さまざまな現実現象の確率モデルとして用いられる一方,2項分布その他の分布の近似としても有用であり,さらに,さまざまな統計料の近似的分布としても重要な役割を持っている.  

正規分布の確率密度関数は,  

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=f(x\)=\\frac{1}{\\sqrt{2\\pi}\\sigma}e^{-\\frac{(x-\\mu\)^2}{2\\sigma^2}})  

平均μ,標準偏差σの正規分布を ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=N(\\mu,\\sigma^2\)) と書く  

* σの値を一定にしてμを変えた場合  
分布の形状はそのままに,平行移動されるだけ.  

* μの値を一定にしたままσの値を変えた場合  
標準偏差を2倍にすると,μでの高さを半分に押しつぶし,μの両側へ2倍押し広げた形になる.  

標準化をした場合,xが正規分布 ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=N(\\mu,\\sigma^2\)) にしたがう時, ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=\\frac{x-\\mu}{\\sigma}) は正規分布N(0,1)にしたがう.正規分布N(0,1)を特に **標準正規分布** という.  
一般の正規分布 ![alt text](http://chart.apis.google.com/chart?cht=tx&chl=N(\\mu,\\sigma^2\)) についての確率やパーセント点を求める問題は標準正規分布N(0,1)についてのそれに帰着される  

**確率およびパーセント点の計算**  

付表1,2を使いましょう.  


