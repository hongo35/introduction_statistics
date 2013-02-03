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


