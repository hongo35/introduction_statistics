### 第5章 確立分布とその特性値
---

#### 5.1 確率変数と確率分布  
* 確率変数  
どのような値をどのような確率でとるか、一定の法則により定まっている変数

* 確率分布  
確率変数を定める法則


例）
サイコロを１回投げる　⇒　出る目の数が確率変数

<table>
<tr>
  <td>出る目の数</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td>
</tr>
<tr>
  <td>確率（分布）</td><td>1/6</td><td>1/6</td><td>1/6</td><td>1/6</td><td>1/6</td><td>1/6</td>
</tr>
</table>


例）
サイコロを２回投げる　⇒　出る目の数が確率変数

<table>
<tr>
  <td>出る目の数</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>7</td><td>8</td><td>9</td><td>10</td><td>11</td><td>12</td>
</tr>
<tr>
  <td>確率（分布）</td><td>1/36</td><td>2/36</td><td>3/36</td><td>4/36</td><td>5/36</td><td>6/36</td><td>5/36</td><td>4/36</td><td>3/36</td><td>2/36</td><td>1/36</td>
</tr>
</table>

標本空間を斜めに数えると上の分布がわかる。

<table>
<tr><td>1+1 </td><td>2+1 </td><td>3+1 </td><td>4+1 </td><td>5+1 </td><td>6+1</td></tr>
<tr><td>1+2 </td><td>2+2 </td><td>3+2 </td><td>4+2 </td><td>5+2 </td><td>6+2</td></tr>
<tr><td>1+3 </td><td>2+3 </td><td>3+3 </td><td>4+3 </td><td>5+3 </td><td>6+3</td></tr>
<tr><td>1+4 </td><td>2+4 </td><td>3+4 </td><td>4+4 </td><td>5+4 </td><td>6+4</td></tr>
<tr><td>1+5 </td><td>2+5 </td><td>3+5 </td><td>4+5 </td><td>5+5 </td><td>6+5</td></tr>
<tr><td>1+6 </td><td>2+6 </td><td>3+6 </td><td>4+6 </td><td>5+6 </td><td>6+6</td></tr>
</table>


**標本空間の関心事**  
標本空間には、組としての情報があるが（1+4, 2+3など）、確率変数としてはその和にのみ関心を注いでいる。（よって1+4=2+3=5となり組の情報は失われる。）
実験結果のある一つの変数に着目し、元の標本空間について議論する必要は無い。(組の情報が必要な場合は「組」を含んで確率変数とすることもできる。)




* 質的確率変数  
例）内閣の政策に賛成か？{YES, NO}  
例）好きな国は？ {アメリカ, フランス, 中国, ブラジル}  

のように、取り得る値が実数値での表現ではなく、カテゴリーとして表現される。






* 離散型確率変数  
上記サイコロの例のように確率変数が離散値。

事象A       = {2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12}  


事象A全体の確率  
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\(A\)={\\displaystyle%20\\sum_{x\\in%20A}%20p(x\)=1}) 

事象Aの部分が起きる確率  
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\\{a\\le x\\le b\\}={\\displaystyle%20\\sum_{x=a}^{b}%20p(x\)\\le 1}) 


例）  {5, 6, 7} ⊂ A  
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\\{5\\le x\\le 7\\}={\\displaystyle%20\\sum_{x=5}^{7}%20p(x\)= \\frac{15}{36}}) 





* 連続型確率変数  
100人のヒストグラム  
500人のヒストグラム  
無限人のヒストグラム  

![alt text](https://lh6.googleusercontent.com/-7mpGuiE0fJw/URkBNduz5XI/AAAAAAAAArc/FlnjgESUUlA/s402/%25E3%2583%2592%25E3%2582%25B9%25E3%2583%2588%25E3%2582%25AF%25E3%2582%2599%25E3%2583%25A9%25E3%2583%25A0.png) 


ある程度、データ数を大きくすればグラフが「なめらか」になり連続としての性質を持つようになる。

連続の曲線は関数 f(x) で表され、全域では

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\\{-\\infty\\le x\\le \\infty\\}={\\displaystyle \\int_{-\\infty}^{\\infty} f(x\) dx = 1})  


区間[a, b]に属する確率は区間の部分積分で求めることが出来る。

![alt text](http://chart.apis.google.com/chart?cht=tx&chl=P\\{a\\le x\\le b\\}={\\displaystyle \\int_{a}^{b} f(x\) dx\\le 1})  



さて、離散と連続を統一的に扱うことはできるでしょうか？




* 累積分布関数  
![alt text](http://chart.apis.google.com/chart?cht=tx&chl=F\\( b \)=P\\{-\\infty \\le  x\\le b \\})  

で記述的な統一が出来る。  
※便宜上、有限離散定義域の最小値も無限を用いて表している。



#### 5.2 確率変数の平均値と標準偏差  
* 平均値  
大学生20人が１週間に大学に出ている回数  

5, 4, 3, 6, 5, 4, 4, 3, 2, 3, 5, 4, 5, 4, 2, 5, 3, 4, 3, 1


<table>
<tr>
  <td>日数</td><td>1</td><td>2</td><td>3</td><td>4</td><td>5</td><td>6</td><td>計</td>
</tr>
<tr>
  <td>度数</td><td>1</td><td>2</td><td>5</td><td>6</td><td>5</td><td>1</td><td>20</td>
</tr>
<tr>
  <td>相対度数</td><td>1/20</td><td>1/10</td><td>1/4</td><td>3/10</td><td>1/4</td><td>1/20</td><td>1</td>
</tr>
</table>


* 期待値  
* 分散  
* 標準偏差



