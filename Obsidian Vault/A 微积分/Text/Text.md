````col
```col-md

$$
\begin{array}{l}
求\ y'' + p y' + q y = 0\ 的通解 \\[8pt]  % 逐行加固定间距，2.0等效12pt
只用找到\ y_1(x),y_2(x)，且\frac{y_1(x)}{y_2(x)}\ne c即可 \\[8pt]
什么样的函数满足这个方程呢？ \\[8pt]
设\ y(x)=e^{ax} \ (a\in 常数) \\[8pt]
将其代入方程 \\[8pt]
(e^{ax})'' =a^2 e^{ax}，(e^{ax})' =ae^{ax} \\[8pt]
\Rightarrow a^2 e^{ax}+p\cdot ae^{ax}+q\cdot e^{ax}=0 \\[8pt]
e^{ax}(a^2+pa+q)=0 \\[8pt]
\Rightarrow a^2+pa+q=0 \\[8pt]
我们称\ a^2+pa+q=0\ 为\\[8pt]
\ y'' + p y' + q y = 0\ 的特征方程 \\[8pt]
\because a^2+pa+q=0\ 为关于a的一元二次方程 \\[8pt]
\therefore 我们可以求出其两个实根a_1与a_2
\end{array}
$$
- [*] ==1.==若$p^{2}-4q>0$，则$a_{1} \ne a_{2}$
则，$\frac{e^{a_{1} x}}{e^{a_{2} x}} =e^{(a_{1}-a_{2})x}\ne c$
$\Rightarrow$通解为$y(x)=c_{1} e^{a_{1} x}+c_{2} e^{a_{2} x}$
- [*] ==2.==若$p^{2}-4q=0$，则$a_{1} = a_{2}=a$
则，$\frac{e^{a_{1} x}}{e^{a_{2} x}} =e^{(a_{1}-a_{2})x}= 1$
$\Rightarrow$$e^{a_{1} x}$与$e^{a_{2} x}$线性相关
不能构成此方程的通解
记住这个结论：
$xe^{ax}$也是满足此方程的，且$\frac{xe^{ax}}{e^{ax}} \ne c$
$\Rightarrow$通解为$y(x)=c_{1} e^{a x}+c_{2} xe^{a x}=(c_{1}+c_{2}x)e^{a x}$

```

```col-md

- [*] ==3.==若$p^{2}-4q<0$，则没有实根
用虚根($i^{2}=-1$)

$$
\begin{align*}  % *号表示不自动加公式编号，更简洁
a &=\frac{-p\pm \sqrt{p^{2}-4q} }{2} 
，
{\color[RGB]{90,109,128} \mathit{\left\{\begin{matrix} 
 \bigtriangleup = p^{2}-4q<0\\ 
-\bigtriangleup>0
\end{matrix}\right. } } \\[10pt]

&=\frac{-p\pm \sqrt{-\bigtriangleup \cdot i^{2} } }{2} \\[10pt]

&=\frac{-p\pm \sqrt{-\bigtriangleup}\cdot i }{2} \\[10pt]

&=\frac{-p}{2} \pm \frac{\sqrt{-\bigtriangleup } }{2} \cdot i\\[10pt]

&设\alpha = \frac{-p}{2} ，\beta=  \frac{\sqrt{-\bigtriangleup } }{2}\\[10pt]

&=\alpha +\beta i\\[10pt]

&\alpha +\beta i是特征方程的一对共轭复根\\[10pt]

&\Rightarrow通解为y(x)=e^{\alpha x} (c_{1}cos\beta x+c_{2}sin\beta x )\\[10pt]
\end{align*}
$$

```
````
111
*111*
[^1]111
${\color[RGB]{128,128,128} i^{2}=-1}$

$$
111
\left\{
\begin{array}{l}
\quad Q_{n}(x)\\[10pt]
\quad p_{n}(x) \text{ 是 } x \text{ 的 } n \text{ 次特殊多项式} \\[10pt]
\quad Q_{n}(x) \text{ 是 } x \text{ 的 } n \text{ 次一般多项式} \\[10pt]
\quad Q_{n}(x)=a_nx^n+a_{n-1}x^{n-1}+\dots+a_1x+a_0\\[10pt]
\quad x \text{ 的 } n \text{ 次一般多项式就是 } x \text{ 的 } n \text{ 次的所有多项式}\\[10pt]
\quad x \text{ 的 } n \text{ 次特殊多项式，}\\[10pt]
\quad \text{就是在 } x \text{ 的 } n \text{ 次一般多项式的基础上加一些限制的条件}\\[10pt]
\quad \text{例：} \text{若 } p_{n}(x)=1，\text{ 则 } Q_{n}(x)=a_0x^0=a_0\\[10pt]
\quad \quad \quad \text{若 } p_{n}(x)=x，\text{ 则 } Q_{n}(x)=ax+b\ (a\neq0)\\[10pt]
\quad \quad \quad \text{若 } p_{n}(x)=x^2，\text{ 则 } Q_{n}(x)=ax^2+bx+c\ (a\neq0)\\[10pt]
\quad \quad \quad \text{若 } p_{n}(x)=x^3，\text{ 则 } Q_{n}(x)=ax^3+bx^2+cx+d\ (a\neq0)
\end{array}
\right.
$$

$$
e^{\alpha x} Q_{n} (x)x^{k}
\begin{cases}
\begin{align*}  % *号表示不自动加公式编号，更简洁

&e^{\alpha x} :从自由项中照抄过来\\[10pt]

&Q_{n} (x):
\begin{cases}
p_{n}(x)是x的n次特殊多项式 \\[3pt] 
Q_{n}(x)是x的n次一般多项式 \\[3pt]
Q_{n}(x)=a_nx^n+a_{n-1}x^{n-1}+\dots+a_1x+a_0\\[3pt]
x的n次一般多项式就是x的n次的所有多项式\\[3pt]
x的n次特殊多项式，就是在x的n次一般多项式的基础上加一些限制的条件\\[3pt]
eg：
\begin{cases}
若p_{n}(x)=1，则Q_{n} (x)=a_0x^0=a_0\\[3pt]
若p_{n}(x)=x，则Q_{n} (x)=ax+b（a≠0）\\[3pt]
若p_{n}(x)=x^2，则Q_{n} (x)=ax²+bx+c（a≠0）\\[3pt]
若p_{n}(x)=x^3，则Q_{n} (x)=ax^3+bx^2+cx+d（a≠0）\\[3pt]
\end{cases}\\[10pt]
\end{cases}\\[10pt]

&k:
\begin{cases}
先算非齐次方程的导出方程的特征方程的根 r_1与r_2 \\[3pt]  
k就是\alpha 与r_1，r_2相等的个数\\[3pt]
找k的步骤：\\[3pt]
一看：看自由项中的\alpha 是什么\\[3pt]
二算：算非齐次方程的导出方程的特征方程的根 r_1与r_2\\[3pt]
三比较：
\begin{cases}
看自由项中的\alpha 与特征方程的根 r_1，r_2相等的个数\\[3pt]
若\alpha \ne r_1，\alpha \ne r_2，则k=0\\[3pt]
若\alpha = r_1或\alpha = r_2(r_1 \ne r_2)，则k=1\\[3pt]
若\alpha =r_1=r_2，则k=2\\[3pt]
\end{cases}\\[10pt]
\end{cases}\\[10pt]


\end{align*}
\end{cases}\\[10pt]
$$
````col
```col-md

- [<] ==情况1.用待定系数法求特解的总结==

$$
\begin{align*}  % *号表示不自动加公式编号，更简洁
&y''+py'+qy=p_n(x)e^{\alpha x}\\[10pt]
&设特解为y=e^{\alpha x}Q_n(x)x^k\\[10pt]
\bullet&\quad e^{\alpha x}照抄\\[10pt]
\bullet&\quad p_n(x)写成Q_n(x) \\[10pt]
\bullet&\quad 求k
\begin{cases}
一看\alpha \\[10pt]

二算
\begin{cases}
非齐次方程的导出方程\\[3pt]
导出方程的特征方程\\[3pt]
解出r_1与r_2 \\[3pt]
\end{cases}\\[10pt]

三比较:\\[10pt]
k=
\begin{cases}
0，\alpha \ne r_1，\alpha \ne r_2\\[3pt]
1，\alpha = r_1或\alpha = r_2(r_1 \ne r_2)\\[3pt]
2，\alpha =r_1=r_2\\[3pt]
\end{cases}\\[10pt]
\end{cases}\\[10pt]

\bullet&\quad 将特解代入原方程可解出Q_n(x)的系数\\[1pt]
&\quad  \Rightarrow 特解\\[10pt]
\bullet&\quad 求出导出方程的通解\\[10pt]
\bullet&\quad 非齐次方程的通解\\[1pt]
&\quad =其导出方程的通解+其特解
\end{align*}
$$

```

```col-md

- [<] ==例子==

$$
\begin{align*}  % *号表示不自动加公式编号，更简洁
&y''-2y'+5y=1\cdot e^x\\[10pt]

&{\color[RGB]{90,109,128} 
自由项为1\cdot e^x
\begin{cases}
\alpha =1\\[3pt]
p_n(x)=1\\[3pt]
\end{cases}}\\[10pt]

&设特解为y^*=e^{\alpha x}Q_n(x)x^k\\[10pt]
\bullet&\quad e^x照抄\\[10pt]
\bullet&\quad p_n(x)=1，Q_n(x)=a_0x^0=a \\[10pt]
\bullet&\quad k=0
\begin{cases}
一看:\alpha =1\\[10pt]

二算
\begin{cases}
导出方程y''-2y'+5y=0 \\[3pt]
特征方程r^2-2r+5=0\\[3pt]
r_{1,2}=\frac{2\pm 4i}{2}=1\pm 2i\\[3pt]
r_1=1+2i，r_2=1-2i \\[3pt]
\end{cases}\\[10pt]

三比较:\\[10pt]
k=
\begin{cases}
\because \alpha \ne r_1 \ne r_2\\[3pt]
\therefore k=0\\[3pt]
\end{cases}\\[10pt]
\end{cases}\\[10pt]

&\quad  \Rightarrow 设y^*=ae^x\cdot x^0=ae^x\\[10pt]
\bullet&\quad 代入原方程\\[1pt]
&\quad \Rightarrow ae^x-2ae^x+5ae^x=e^x \\[8pt]
&\quad \Rightarrow 4a=1\\[8pt]
&\quad \Rightarrow a=\frac{1}{4} \\[8pt]
&\quad \Rightarrow 特解y^*=\frac{1}{4}e^x\\[8pt]
\bullet&\quad 导出方程的通解:\\[1pt]
&\quad y(x)=e^x (c_{1}cos2x+c_{2}sin2x )\\[10pt]
\bullet&\quad 非齐次方程的通解:\\[1pt]
&\quad y(x)=e^x (c_{1}cos2x+c_{2}sin2x )+\frac{1}{4}e^x
\end{align*}
$$

```
````

````col
```col-md

## 性质1（分配律）
$$
\begin{align*}

&若级数\sum_{n=1}^{\infty} u_n,\sum_{n=1}^{\infty} v_n均收敛\\[8pt]
&则\sum_{n=1}^{\infty}(au_n\pm bv_n)也收敛（a,b\in 常数）  \\[8pt]
&且\sum_{n=1}^{\infty}(au_n\pm bv_n)=a\sum_{n=1}^{\infty}u_n\pm b\sum_{n=1}^{\infty}v_n \\[8pt]

&注：
\begin{cases}
收敛\pm 发散=发散\\[3pt]
发散\pm 发散=不一定   \\[3pt]
\end{cases}\\[8pt]

\end{align*}
$$
## 性质3

$$
\begin{align*}
\quad &\quad改变级数任意有限项\\[8pt]
\quad &\quad不会改变该级数的敛散性  \\[8pt]
\quad &\quad(级数的敛散性取决于n\to \infty 时的情况)\\[8pt]
\quad &\quad 即 \\[3pt]

\quad &\quad \qquad \begin{cases}
\displaystyle \sum_{n=N}^{\infty} u_n收敛\Leftrightarrow \sum_{n=1}^{\infty} u_n收敛    \\[3pt]
\displaystyle \sum_{n=N}^{\infty} u_n发散\Leftrightarrow \sum_{n=1}^{\infty} u_n发散  \\[3pt]
\end{cases}\\[8pt]

\quad &\quad \qquad \begin{cases}
\displaystyle \sum_{n=1}^{\infty} u_n收敛\Leftrightarrow \sum_{n=1}^{\infty} u_{n+N}收敛  \\[3pt]
\displaystyle \sum_{n=1}^{\infty} u_n发散\Leftrightarrow \sum_{n=1}^{\infty} u_{n+N}发散  \\[3pt]
\end{cases}\\[8pt]

\quad &\quad \qquad (N\in 任一正整数)   \\[3pt]
\end{align*}
$$

```

```col-md

## 性质2（结合律）
$$
\begin{align*}
&收敛级数的项任意加括号后\\[4pt]
&所得的新级数仍收敛，且其和不变\\[4pt]
结论&：\\[8pt]

\bullet&\quad若加括号后所得的新级数发散， \\[3pt]
\quad &\quad则，原级数必然发散   \\[3pt]

\bullet&\quad若加括号后所得的新级数收敛， \\[3pt]
\quad &\quad不能断言原级数一定收敛   \\[3pt]
\quad &\quad eg:  \\[3pt]
\quad &\quad级数\displaystyle \sum_{n=1}^{\infty}(-1)^{n-1}a（a\in 非零常数） \\[3pt]
\quad &\quad \qquad=a-a+a-a+\dots   \\[3pt]
\quad &\quad \qquad (将相邻两项加括号)   \\[3pt]
\quad &\quad \qquad=(a-a)+(a-a)+\dots   \\[3pt]
\quad &\quad \qquad=0，收敛   \\[3pt]
\quad &\quad但，原级数\displaystyle \sum_{n=1}^{\infty}(-1)^{n-1}a是发散的   \\[3pt]
\end{align*}
$$
## 性质4（例16.13）

$$
\begin{align*}
&若级数\sum_{n=1}^{\infty} u_n收敛，则\lim_{n \to \infty} u_n=0\\[8pt]

\bullet&\quad u_n=S_n-S_{n-1} \ (n\ge 2)\\[3pt]

\bullet&\quad 此性质是级数收敛的必要条件 \\[3pt]
\quad &\quad 即使\lim_{n \to \infty} u_n=0 \\[3pt]
\quad &\quad 也不能保证\sum_{n=1}^{\infty} u_n收敛   \\[3pt]
\quad &\quad 因为，若通项趋于0的速度不够快   \\[3pt]
\quad &\quad 会让累加刹不住车   \\[3pt]
\quad &\quad 从而达不到收敛的目的   \\[3pt]
\quad &\quad 反推：   \\[3pt]
\quad &\quad 若\lim_{n \to \infty} u_n\ne 0，则\sum_{n=1}^{\infty} u_n发散   \\[3pt]
\end{align*}
$$




```
````
[[高阶线性微分方程]]
