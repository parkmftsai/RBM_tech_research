# RBM_tech_research
```
20180528~20180601
RBM(Restricted Boltzmann Machine)，一種簡易神經網路，為目前所有神經網路鼻祖，大抵知識如下
1.RBM架構是complete bipartite graph，相關定義可以參考[2]
2.RBM是非監督是學習，主要用來降維、分類，但是我們需要的只有降維功能
3.RBM取出降維後之樣本特徵，比PCA(Principal components analysis)相比，可以保留更多樣本的特性，其原因在於
RBM在訓練時採用forward propagation ＆ backward propagation，這些方法可以讓NN(Neural Network)，更快收斂
，不陷入local optimum，是一種最佳化演算法，詳情請看[3]

個人想法如下
1.RBM是基礎NN，如果在使用單一層RBM來看，運算時間應該很低
2.與將來的工作有關，如果一開始在取資料時，如果所取的特徵對樣本本身有很強的關聯性，那特徵就很有用
3.如果特徵很有用，在使用RBM進行降維，降維後的特徵能保留更多未降維前的特徵的特性且大幅降低特徵資料量
4.如果第3點成立，再使用降維後的特徵進行classify，或許classify之後的結果會很準


REFERENCES
1.受限玻尔兹曼机基础教程,https://deeplearning4j.org/cn/restrictedboltzmannmachine
2.Bipartite_graph,https://en.wikipedia.org/wiki/Bipartite_graph
3.MNIST with Autoencoder,https://allenlu2007.wordpress.com/2017/07/08/mnist-with-autoencoder/

ysd:針對rbm進行實做
```
