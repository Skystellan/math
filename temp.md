10．4（4）试问：对初始状态如下（长度为 $n$ ）的各序列进行直接插人排序时，至多需进行多少次关键字间的比较（要求排序后的序列按关键字自小至大顺序有序）？
（1）关键字（自小至大）顺序有序；$\left(k e y_1<k e y_2<\cdots<k e y_n\right)$
（2）关键字（自大至小）逆序有序；$\left(k e y_1>k e y_2>\cdots>k e y_n\right)$
（3）序号为奇数的关键字顺序有序，序号为偶数的关键字顺序有序；
$$
\left(k e y_1<k e y_3<\cdots, \quad k e y_2<k e y_4 \cdots\right)
$$
（4）前半个序列中的关键字顺序有序，后半个序列中的关键字逆序有序：
$$
\left(\text { key }_1<\text { key }_2<\cdots<\text { key }_{\mathbf{n} / 2}, \quad \text { key }_{\mathbf{n} / 2} \mathbf{n}+1>\cdots \text { key }_n\right)
$$
（1）$n-1$
（2）$\sum_{i=1}^{n-1} i+\underbrace{n-1}_{\text {找哨兵 }}=\frac{n^2+n-2}{2}$
（3）$\underbrace{\left\lfloor\frac{n-1}{2}\right\rfloor}_{\text {找哨兵 }}+\sum_{i=1}^{\left\lfloor\frac{n-1}{2}\right\rfloor} i=\frac{\left(\left\lfloor\frac{n-1}{2}\right\rfloor\right)^2+3\left\lfloor\frac{n-1}{2}\right\rfloor}{2}$
（4）假设后半序列非常小
$$
\underbrace{\frac{n}{2}}_{\text {找哨兵 }}+\sum_{\frac{n}{2}}^{n-1} i=\frac{\frac{3}{2} n^2+n}{4}
$$