### transformer中没有seq2seq中的时间序列的概念，添加了位置编码进行定位，位置编码能够捕捉到位置之间的相对关系，并且能够在不同的维度上区分不同的位置；实际使用的话就是创建一个比较大的矩阵然后维度需要和词嵌入的维度相等，然后每个列维度分偶数和奇数进行sin、cos变换，同时乘上一个指数的变化率。
### transformer直接用nn中的库，定义好embedding维度、N个头(多头注意力)，encoder、decoder层数、前馈网络非线性的变换。
  
