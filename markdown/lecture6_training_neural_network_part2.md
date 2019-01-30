![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Training Neural Networks,

Part 2

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 1 25 Jan 2016

> ![](media/image3.jpeg){width="9.7625in" height="4.215277777777778in"}
>
> A2 is out. It's meaty. It's due Feb 5 (next Friday)
>
> You'll implement:
>
> Neural Nets (with Layer Forward/Backward API)
>
> Batch Norm
>
> Dropout
>
> ConvNets

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 2 25 Jan 2016

> ![](media/image5.jpeg){width="9.772222222222222in"
> height="4.769444444444445in"}
>
> Loop:

1.  **Sample** a batch of data

2.  **Forward** prop it through the graph, get loss

3.  **Backprop** to calculate the gradients

4.  **Update** the parameters using the gradient

![](media/image6.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 3 25 Jan 2016

+----------------------+------------------+--+
| Activation Functions | > **Leaky ReLU** |  |
+----------------------+------------------+--+
|                      | > max(0.1x, x)   |  |
+----------------------+------------------+--+
| > **Sigmoid**        |                  |  |
+----------------------+------------------+--+

![](media/image7.jpeg){width="9.449305555555556in"
height="0.9131944444444444in"}

> **Maxout**
>
> **tanh** tanh(x)

![](media/image9.jpeg){width="3.827777777777778in"
height="1.7861111111111112in"}

> **ELU**

![](media/image11.jpeg){width="4.85625in" height="1.1784722222222221in"}

> **ReLU** max(0,x)

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 4 25 Jan 2016

> ![](media/image13.jpeg){width="9.6375in"
> height="2.1868055555555554in"}
>
> Preprocessing

![](media/image14.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 5 25 Jan 2016

> ![](media/image16.jpeg){width="9.960416666666667in"
> height="4.909027777777778in"}
>
> **Reasonable initialization.** (Mathematical derivation assumes linear
> activations)
>
> Weight Initialization

![](media/image17.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 6 25 Jan 2016

> Batch Normalization
>
> Normalize:
>
> And then allow the network to squash the range if it wants to:
>
> \[Ioffe and Szegedy, 2015\]

![](media/image18.jpeg){width="9.815972222222221in"
height="4.726388888888889in"}

-   Improves gradient flow through the network

-   Allows higher learning rates

-   Reduces the strong dependence on initialization

-   Acts as a form of regularization in a funny way, and slightly
    reduces the need for dropout, maybe

![](media/image19.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 7 25 Jan 2016

+------------------+--------------------+--+--+--+--+--+--+
| Babysitting the  | > Cross-validation |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+
| learning process |                    |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+
|                  |                    |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+
|                  |                    |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+
|                  |                    |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+
|                  |                    |  |  |  |  |  |  |
+------------------+--------------------+--+--+--+--+--+--+

![](media/image20.jpeg){width="5.208880139982502e-3in"
height="5.0465277777777775in"}

> Loss barely changing:
>
> Learning rate is probably
>
> too low

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 8 25 Jan 2016

> ![](media/image22.jpeg){width="8.535416666666666in"
> height="4.720138888888889in"}

-   Parameter update schemes

-   Learning rate schedules

-   Dropout

-   Gradient checking

-   Model ensembles

![](media/image23.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 9 25 Jan 2016

![](media/image24.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Parameter Updates

![](media/image25.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 10 25 Jan 2016

> ![](media/image26.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image27.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 11 25 Jan 2016

> ![](media/image29.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image30.jpeg){width="5.781944444444444in"
height="3.5145833333333334in"}

> simple gradient descent update
>
> now: complicate.

![](media/image31.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 12 25 Jan 2016

![](media/image32.jpeg){width="7.002777777777778in"
height="4.273611111111111in"}

> Image credits: Alec Radford

![](media/image33.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 13 25 Jan 2016

> ![](media/image34.jpeg){width="9.694444444444445in"
> height="0.5847222222222223in"}

![](media/image35.jpeg){width="9.0in" height="1.8416666666666666in"}

Q.  What is the trajectory along which we converge towards the minimum
    > with SGD?

![](media/image37.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 14 25 Jan 2016

> ![](media/image38.jpeg){width="9.694444444444445in"
> height="0.5847222222222223in"}

![](media/image39.jpeg){width="8.254861111111111in"
height="0.6305555555555555in"}

Q.  What is the trajectory along which we converge towards the minimum
    > with SGD?

![](media/image43.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 15 25 Jan 2016

> ![](media/image44.jpeg){width="9.694444444444445in"
> height="0.5847222222222223in"}

![](media/image45.jpeg){width="8.254861111111111in"
height="0.6305555555555555in"}

Q.  What is the trajectory along which we converge towards the minimum
    > with SGD? very slow progress along flat direction, jitter along
    > steep one

![](media/image47.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 16 25 Jan 2016

> ![](media/image48.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image49.jpeg){width="4.559027777777778in"
height="0.5902777777777778in"}

-   Physical interpretation as ball rolling down the loss function +
    > friction (mu coefficient).

-   mu = usually \~0.5, 0.9, or 0.99 (Sometimes annealed over time, e.g.
    > from 0.5 -\> 0.99)

![](media/image54.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 17 25 Jan 2016

> ![](media/image55.jpeg){width="9.86111111111111in"
> height="2.6666666666666665in"}

![](media/image56.jpeg){width="5.208880139982502e-3in"
height="0.6902777777777778in"}

-   Allows a velocity to "build up" along shallow directions

-   Velocity becomes damped in steep direction due to quickly changing
    > sign

![](media/image58.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 18 25 Jan 2016

> ![](media/image59.jpeg){width="6.7965277777777775in"
> height="3.9972222222222222in"}
>
> vs
>
> Momentum

![](media/image60.jpeg){width="2.8881944444444443in"
height="2.2118055555555554in"}

> notice momentum overshooting the target, but overall getting to the
> minimum much faster.

![](media/image61.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 19 25 Jan 2016

> ![](media/image62.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image63.jpeg){width="7.038194444444445in"
height="1.1652777777777779in"}

Ordinary momentum update:

![](media/image64.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> momentum
>
> step
>
> actual step

![](media/image66.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> gradient
>
> step

![](media/image67.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 20 25 Jan 2016

> ![](media/image68.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image69.jpeg){width="7.903472222222222in"
height="3.529166666666667in"}

> Momentum update

![](media/image70.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> momentum
>
> step

actual step

![](media/image71.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> gradient
>
> step

Nesterov momentum update

![](media/image72.jpeg){width="5.077083333333333in"
height="1.8416666666666666in"}

+----------+----------------------------+--+
|          | > "lookahead" gradient     |  |
+----------+----------------------------+--+
| momentum | > step (bit different than |  |
+----------+----------------------------+--+
|          | > original)                |  |
+----------+----------------------------+--+
| step     |                            |  |
+----------+----------------------------+--+
|          | > actual step              |  |
+----------+----------------------------+--+

![](media/image73.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 21 25 Jan 2016

> ![](media/image74.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image75.jpeg){width="5.208880139982502e-3in"
height="2.5180555555555557in"}

> Momentum update

![](media/image77.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> momentum
>
> step

actual step

![](media/image78.jpeg){width="1.4472222222222222in"
height="5.208880139982502e-3in"}

> gradient
>
> step

Nesterov momentum update

+----------+----------------------------+--+
|          | > "lookahead" gradient     |  |
+----------+----------------------------+--+
| momentum | > step (bit different than |  |
+----------+----------------------------+--+
|          | > original)                |  |
+----------+----------------------------+--+
| step     |                            |  |
+----------+----------------------------+--+
|          | > actual step              |  |
+----------+----------------------------+--+

Nesterov: the only difference\...

![](media/image79.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 22 25 Jan 2016

> ![](media/image80.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image81.jpeg){width="9.690972222222221in"
height="1.2486111111111111in"}

> Slightly inconvenient... usually we have :

![](media/image82.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 23 25 Jan 2016

> ![](media/image83.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image84.jpeg){width="9.690972222222221in"
height="1.2486111111111111in"}

> Slightly inconvenient... usually we have :

![](media/image85.jpeg){width="9.566666666666666in"
height="1.0416666666666666e-2in"}

> Variable transform and rearranging saves the day:

![](media/image87.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 24 25 Jan 2016

> ![](media/image88.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image89.jpeg){width="9.690972222222221in"
height="1.2486111111111111in"}

> Slightly inconvenient... usually we have :

![](media/image90.jpeg){width="9.566666666666666in"
height="1.0416666666666666e-2in"}

> Variable transform and rearranging saves the day:
>
> Replace all thetas with phis, rearrange and obtain:

![](media/image92.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 25 25 Jan 2016

![](media/image94.jpeg){width="7.182638888888889in"
height="3.9972222222222222in"}

> nag =
>
> Nesterov
>
> Accelerated
>
> Gradient

![](media/image95.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 26 25 Jan 2016

![](media/image96.jpeg){width="6.176388888888889in"
height="0.4361111111111111in"}

> AdaGrad update

![](media/image97.jpeg){width="6.600694444444445in"
height="0.8701388888888889in"}

\[Duchi et al., 2011\]

![](media/image98.jpeg){width="6.600694444444445in"
height="0.5513888888888889in"}

> Added element-wise scaling of the gradient based on the historical sum
> of squares in each dimension

![](media/image100.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 27 25 Jan 2016

> ![](media/image101.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image102.jpeg){width="9.0in" height="3.5930555555555554in"}

> Q: What happens with AdaGrad?

![](media/image103.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 28 25 Jan 2016

> ![](media/image104.jpeg){width="6.176388888888889in"
> height="0.4361111111111111in"}

![](media/image105.jpeg){width="9.0in" height="3.5930555555555554in"}

> Q2: What happens to the step size over long time?

![](media/image106.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 29 25 Jan 2016

> RMSProp update

![](media/image107.jpeg){width="10.0in" height="0.5888888888888889in"}

\[Tieleman and Hinton, 2012\]

![](media/image110.jpeg){width="9.620833333333334in"
height="0.4840277777777778in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 30 25 Jan 2016

> ![](media/image111.jpeg){width="9.705555555555556in"
> height="3.6625in"}

![](media/image112.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 31 25 Jan 2016

> ![](media/image113.jpeg){width="9.705555555555556in"
> height="3.6625in"}

![](media/image114.jpeg){width="8.99236111111111in"
height="0.8611111111111112in"}

> Cited by several papers as:

![](media/image115.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 32 25 Jan 2016

![](media/image116.jpeg){width="6.276388888888889in"
height="3.9972222222222222in"}

> adagrad

![](media/image117.jpeg){width="0.46944444444444444in"
height="0.22708333333333333in"}

> rmsprop

![](media/image118.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 33 25 Jan 2016

> Adam update

![](media/image119.jpeg){width="4.540972222222222in"
height="0.5006944444444444in"}

\[Kingma and Ba, 2014\]

![](media/image120.jpeg){width="9.620833333333334in"
height="0.4840277777777778in"}

> (incomplete, but close)

![](media/image121.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 34 25 Jan 2016

+-------------------------+---------------------------+--+
| Adam update             | > \[Kingma and Ba, 2014\] |  |
+-------------------------+---------------------------+--+
|                         |                           |  |
+-------------------------+---------------------------+--+
| (incomplete, but close) |                           |  |
+-------------------------+---------------------------+--+

![](media/image123.jpeg){width="6.176388888888889in"
height="0.4361111111111111in"}

> momentum
>
> RMSProp-like
>
> Looks a bit like RMSProp with momentum

![](media/image126.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 35 25 Jan 2016

+-------------------------+---------------------------+--+
| Adam update             | > \[Kingma and Ba, 2014\] |  |
+-------------------------+---------------------------+--+
|                         |                           |  |
+-------------------------+---------------------------+--+
| (incomplete, but close) |                           |  |
+-------------------------+---------------------------+--+

![](media/image127.jpeg){width="6.176388888888889in"
height="0.4361111111111111in"}

> momentum
>
> RMSProp-like
>
> Looks a bit like RMSProp with momentum

![](media/image130.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 36 25 Jan 2016

> Adam update

![](media/image131.jpeg){width="7.3375in" height="2.329861111111111in"}

\[Kingma and Ba, 2014\]

![](media/image133.jpeg){width="9.620833333333334in"
height="0.4840277777777778in"}

> momentum
>
> bias correction
>
> (only relevant in first few iterations when t is small)

![](media/image135.jpeg){width="2.265972222222222in"
height="0.6777777777777778in"}

> RMSProp-like
>
> The bias correction compensates for the fact that m,v are initialized
> at zero and need some time to "warm up".

![](media/image136.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 37 25 Jan 2016

> ![](media/image137.jpeg){width="9.440972222222221in"
> height="0.5333333333333333in"}**learning rate** as a hyperparameter.

![](media/image138.jpeg){width="9.13263888888889in"
height="3.397222222222222in"}

> Q: Which one of these learning rates is best to use?

![](media/image139.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 38 25 Jan 2016

> ![](media/image140.jpeg){width="9.440972222222221in"
> height="0.5333333333333333in"}**learning rate** as a hyperparameter.

![](media/image141.jpeg){width="9.373611111111112in"
height="3.4868055555555557in"}

> **=\> Learning rate decay over time!**
>
> **step decay:**
>
> e.g. decay learning rate by half every few epochs.
>
> **exponential decay:**
>
> **1/t decay:**

![](media/image142.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 39 25 Jan 2016

> ![](media/image143.jpeg){width="9.286111111111111in"
> height="0.6152777777777778in"}

![](media/image144.jpeg){width="8.722222222222221in" height="1.31875in"}

> second-order Taylor expansion:

![](media/image145.jpeg){width="8.36111111111111in"
height="0.4583333333333333in"}

> Solving for the critical point we obtain the Newton parameter update:

![](media/image146.jpeg){width="3.6631944444444446in"
height="0.6319444444444444in"}

> Q: what is nice about this update?

![](media/image148.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 40 25 Jan 2016

> ![](media/image149.jpeg){width="9.286111111111111in"
> height="0.6152777777777778in"}

![](media/image150.jpeg){width="8.722222222222221in" height="1.31875in"}

> second-order Taylor expansion:

![](media/image151.jpeg){width="8.36111111111111in"
height="0.4583333333333333in"}

> Solving for the critical point we obtain the Newton parameter update:

![](media/image152.jpeg){width="8.847222222222221in"
height="0.6402777777777777in"}

> notice:

no hyperparameters! (e.g. learning rate)

![](media/image153.jpeg){width="8.92986111111111in"
height="0.6319444444444444in"}

Q2: why is this impractical for training Deep Neural Nets?

![](media/image154.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 41 25 Jan 2016

> ![](media/image155.jpeg){width="9.286111111111111in"
> height="0.6152777777777778in"}

![](media/image156.jpeg){width="9.170833333333333in"
height="0.5270833333333333in"}

-   Quasi-Newton methods (**BGFS** most popular): *instead of inverting
    > the Hessian (O(n\^3)), approximate inverse Hessian with rank 1
    > updates over time (O(n\^2) each).*

-   **L-BFGS** (Limited memory BFGS):

> *Does not form/store the full inverse Hessian.*

![](media/image158.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 42 25 Jan 2016

> ![](media/image159.jpeg){width="9.83611111111111in"
> height="4.229166666666667in"}

-   **Usually works very well in full batch, deterministic mode** i.e.
    > if you have a single, deterministic f(x) then L-BFGS will probably
    > work very nicely

-   **Does not transfer very well to mini-batch setting**. Gives bad
    > results. Adapting L-BFGS to large-scale, stochastic setting is an
    > active area of research.

![](media/image160.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 43 25 Jan 2016

> ![](media/image161.jpeg){width="5.586805555555555in"
> height="0.5284722222222222in"}

![](media/image162.jpeg){width="8.409027777777778in"
height="2.8159722222222223in"}

-   **Adam** is a good default choice in most cases

-   If you can afford to do full batch updates then try out

> **L-BFGS** (and don't forget to disable all sources of noise)

![](media/image163.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 44 25 Jan 2016

![](media/image164.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Evaluation:

Model Ensembles

![](media/image165.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 45 25 Jan 2016

![](media/image166.jpeg){width="8.08125in" height="2.45in"}

1.  Train multiple independent models

2.  At test time average their results

> Enjoy 2% extra performance

![](media/image167.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 46 25 Jan 2016

> ![](media/image168.jpeg){width="8.659722222222221in"
> height="3.7270833333333333in"}

-   can also get a small boost from averaging multiple model checkpoints
    > of a single model.

![](media/image169.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 47 25 Jan 2016

> ![](media/image170.jpeg){width="8.659722222222221in"
> height="4.448611111111111in"}

-   can also get a small boost from averaging multiple model checkpoints
    > of a single model.

-   keep track of (and use at test time) a running average parameter
    > vector:

![](media/image171.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 48 25 Jan 2016

![](media/image172.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Regularization **(dropout)**

![](media/image173.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 49 25 Jan 2016

> ![](media/image174.jpeg){width="9.722916666666666in"
> height="1.2951388888888888in"}**Dropout**
>
> "randomly set some neurons to zero in the forward pass"

![](media/image175.jpeg){width="9.264583333333333in"
height="3.5458333333333334in"}

*\[Srivastava et al., 2014\]*

![](media/image176.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 50 25 Jan 2016

> ![](media/image177.jpeg){width="9.75763888888889in"
> height="4.311111111111111in"}

![](media/image178.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 51 25 Jan 2016

> ![](media/image179.jpeg){width="9.497916666666667in"
> height="0.85625in"}
>
> How could this possibly be a good idea?

![](media/image180.jpeg){width="10.0in" height="3.9659722222222222in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 52 25 Jan 2016

> ![](media/image181.jpeg){width="9.497916666666667in"
> height="0.85625in"}
>
> How could this possibly be a good idea?

![](media/image182.jpeg){width="9.345138888888888in" height="3.0625in"}

Forces the network to have a redundant representation.

![](media/image183.jpeg){width="5.878472222222222in"
height="1.4541666666666666in"}

> has an ear

![](media/image184.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> has a tail

![](media/image185.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> is furry

![](media/image186.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> has claws

![](media/image188.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> mischievous

![](media/image189.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> look

![](media/image190.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6

> **X**

![](media/image191.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

-   ![](media/image193.jpeg){width="0.9097222222222222in"
    > height="0.12430555555555556in"} cat

> ![](media/image194.jpeg){width="0.9298611111111111in"
> height="0.23125in"} score

![](media/image195.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> **X**

![](media/image198.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

53 25 Jan 2016

> ![](media/image199.jpeg){width="9.497916666666667in"
> height="0.85625in"}
>
> How could this possibly be a good idea?

![](media/image200.jpeg){width="9.2875in" height="3.05625in"}

> Another interpretation:
>
> Dropout is training a large ensemble of models (that share
> parameters).
>
> Each binary mask is one model, gets trained on only \~one datapoint.

![](media/image201.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 54 25 Jan 2016

> ![](media/image202.jpeg){width="7.95625in"
> height="0.7020833333333333in"}

![](media/image203.jpeg){width="5.702083333333333in"
height="3.3847222222222224in"}

> **Ideally**:

![](media/image204.jpeg){width="2.6756944444444444in"
height="3.05625in"}

> want to integrate out all the noise
>
> **Monte Carlo approximation:** do many forward passes with different
> dropout masks, average all predictions

![](media/image205.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 55 25 Jan 2016

> ![](media/image206.jpeg){width="9.527083333333334in"
> height="4.382638888888889in"}
>
> Can in fact do this with a single forward pass! (approximately) Leave
> all input neurons turned on (no dropout).

![](media/image207.jpeg){width="5.208880139982502e-3in"
height="0.7416666666666667in"}

> (this can be shown to be an
>
> approximation to evaluating the
>
> whole ensemble)

![](media/image208.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 56 25 Jan 2016

> ![](media/image209.jpeg){width="9.527083333333334in"
> height="4.382638888888889in"}
>
> Can in fact do this with a single forward pass! (approximately) Leave
> all input neurons turned on (no dropout).

![](media/image210.jpeg){width="5.208880139982502e-3in"
height="0.7416666666666667in"}

> Q: Suppose that with all inputs present at test time the output of
> this neuron is x.
>
> What would its output be during training time, in expectation? (e.g.
> if p = 0.5)

![](media/image211.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 57 25 Jan 2016

> ![](media/image212.jpeg){width="9.527083333333334in"
> height="4.690277777777778in"}
>
> Can in fact do this with a single forward pass! (approximately)
>
> a

![](media/image213.jpeg){width="5.208880139982502e-3in"
height="0.7416666666666667in"}

> w0 w1
>
> x y

Leave all input neurons turned on (no dropout).

> during test: **a = w0\*x + w1\*y** during train:

E\[a\] = ¼ \* (w0\*0 + w1\*0

w0\*0 + w1\*y

-   ¼ \* (2 w0\*x + 2 w1\*y)

    -   **½ \* (w0\*x + w1\*y)**
        > ![](media/image214.jpeg){width="8.958333333333333e-2in"
        > height="8.402777777777778e-2in"}

![](media/image215.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 58 25 Jan 2016

> ![](media/image216.jpeg){width="9.570833333333333in"
> height="4.657638888888889in"}
>
> Can in fact do this with a single forward pass! (approximately) Leave
> all input neurons turned on (no dropout).
>
> a

![](media/image217.jpeg){width="5.208880139982502e-3in"
height="0.7416666666666667in"}

> w0 w1
>
> x y

during test: **a = w0\*x + w1\*y** during train:

E\[a\] = ¼ \* (w0\*0 + w1\*0 w0\*0 + w1\*y

-   ¼ \* (2 w0\*x + 2 w1\*y)

    -   **½ \* (w0\*x + w1\*y)**
        > ![](media/image218.jpeg){width="8.75e-2in"
        > height="8.680555555555555e-2in"}

![](media/image219.jpeg){width="10.0in" height="0.5888888888888889in"}

With p=0.5, using all inputs in the forward pass would inflate the
activations by 2x from what the network was "used to" during training!
=\> Have to compensate by scaling the activations back down by ½

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 59 25 Jan 2016

> ![](media/image220.jpeg){width="9.755555555555556in"
> height="0.8652777777777778in"}

![](media/image221.jpeg){width="9.018055555555556in"
height="3.4930555555555554in"}

> At test time all neurons are active always
>
> =\> We must scale the activations so that for each neuron:
>
> [output at test time]{.underline} = [expected output at training
> time]{.underline}

![](media/image222.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 60 25 Jan 2016

![](media/image223.jpeg){width="9.84375in" height="4.756944444444445in"}

> drop in forward pass
>
> scale at test time

![](media/image224.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 61 25 Jan 2016

> ![](media/image225.jpeg){width="9.4625in"
> height="0.6347222222222222in"}

![](media/image226.jpeg){width="9.38888888888889in"
height="4.060416666666667in"}

test time is unchanged!

![](media/image227.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 62 25 Jan 2016

![](media/image228.jpeg){width="7.397916666666666in"
height="1.5597222222222222in"}

> \<fun story time\>
>
> *(Deep Learning Summer School 2012)*

![](media/image229.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 63 25 Jan 2016

![](media/image230.jpeg){width="9.902777777777779in"
height="4.895833333333333in"}

(see class notes\...)

fun guaranteed.

![](media/image231.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 64 25 Jan 2016
>
> ![](media/image232.jpeg){width="9.73125in"
> height="1.4534722222222223in"}

![](media/image233.jpeg){width="7.934027777777778in"
height="2.204861111111111in"}

> *\[LeNet-5, LeCun 1980\]*

![](media/image235.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 65 25 Jan 2016

> ![](media/image236.jpeg){width="5.208880139982502e-3in"
> height="5.05in"}
>
> **Hubel & Wiesel**, 1959
>
> RECEPTIVE FIELDS OF SINGLE NEURONES IN
>
> THE CAT\'S STRIATE CORTEX
>
> 1962
>
> RECEPTIVE FIELDS, BINOCULAR INTERACTION
>
> AND FUNCTIONAL ARCHITECTURE IN THE CAT\'S VISUAL CORTEX
>
> 1968\...

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 66 25 Jan 2016

![](media/image238.jpeg){width="9.238888888888889in"
height="0.5298611111111111in"}

> Video time
> [[https://youtu.be/8VdFf3egwfg?]{.underline}](https://youtu.be/8VdFf3egwfg?t=1m10s)
>
> [[t=1m10s]{.underline}](https://youtu.be/8VdFf3egwfg?t=1m10s)

![](media/image239.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 67 25 Jan 2016

> ![](media/image240.jpeg){width="10.0in" height="4.677777777777778in"}

**Topographical mapping in the cortex:** nearby cells in cortex
represented nearby regions in the visual field

![](media/image241.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 68 25 Jan 2016
>
> ![](media/image242.jpeg){width="8.70486111111111in"
> height="0.6736111111111112in"}

![](media/image243.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 69 25 Jan 2016

> A bit of history:
>
> **Neurocognitron** *\[Fukushima 1980\]*

"sandwich" architecture (SCSCSC...) simple cells: modifiable parameters
complex cells: perform pooling

![](media/image245.jpeg){width="10.0in" height="5.625in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 70 25 Jan 2016

> ![](media/image246.jpeg){width="5.160416666666666in"
> height="0.6736111111111112in"}

![](media/image247.jpeg){width="2.86875in" height="4.509722222222222in"}

> **Gradient-based learning applied to document recognition**
>
> *\[LeCun, Bottou, Bengio, Haffner 1998\]*

![](media/image248.jpeg){width="4.697916666666667in"
height="2.0006944444444446in"}

> LeNet-5

![](media/image249.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 71 25 Jan 2016

> ![](media/image250.jpeg){width="9.70625in" height="2.08125in"}
>
> **ImageNet Classification with Deep Convolutional Neural Networks**
> *\[Krizhevsky, Sutskever, Hinton, 2012\]*

![](media/image251.jpeg){width="5.756944444444445in"
height="2.2159722222222222in"}

> "AlexNet"

![](media/image252.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 72 25 Jan 2016

> ![](media/image253.jpeg){width="9.589583333333334in"
> height="1.0881944444444445in"}
>
> Classification Retrieval

![](media/image254.jpeg){width="8.850694444444445in"
height="3.7381944444444444in"}

*\[Krizhevsky 2012\]*

![](media/image255.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 73 25 Jan 2016

> ![](media/image256.jpeg){width="9.953472222222222in"
> height="4.973611111111111in"}
>
> Detection Segmentation
>
> *\[Faster R-CNN: Ren, He, Girshick, Sun 2015\]* *\[Farabet et al.,
> 2012\]*

![](media/image257.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 74 25 Jan 2016

> ![](media/image258.jpeg){width="9.589583333333334in"
> height="4.36875in"}

NVIDIA Tegra X1

![](media/image259.jpeg){width="5.097222222222222in"
height="0.4583333333333333in"}

> self-driving cars

![](media/image260.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 75 25 Jan 2016

> ![](media/image261.jpeg){width="9.82638888888889in"
> height="4.95625in"}

*\[Taigman et al. 2014\]*

> *\[Simonyan et al. 2014\]*

![](media/image262.jpeg){width="10.0in" height="0.5888888888888889in"}

*\[Goodfellow 2014\]*

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 76 25 Jan 2016

> ![](media/image263.jpeg){width="9.589583333333334in"
> height="2.81875in"}
>
> *\[Toshev, Szegedy 2014\]*

![](media/image264.jpeg){width="9.290277777777778in"
height="1.7020833333333334in"}

> *\[Mnih 2013\]*

![](media/image265.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 77 25 Jan 2016

> ![](media/image266.jpeg){width="9.589583333333334in"
> height="0.9104166666666667in"}

![](media/image267.jpeg){width="9.493055555555555in"
height="3.6368055555555556in"}

> *\[Ciresan et al. 2013\]* *\[Sermanet et al. 2011\]*
>
> *\[Ciresan et al.\]*

![](media/image268.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 78 25 Jan 2016

> ![](media/image269.jpeg){width="9.916666666666666in"
> height="4.983333333333333in"}

*\[Denil et al. 2014\]*

> *\[Turaga et al., 2010\]*

![](media/image270.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 79 25 Jan 2016

![](media/image271.jpeg){width="9.084027777777777in"
height="4.090277777777778in"}

+-----------------+-----------------+-----------------+-----------------+
| > *Whale        | > *Mnih and     |                 |                 |
| > recognition,  | > Hinton, 2010* |                 |                 |
| > Kaggle        |                 |                 |                 |
| > Challenge*    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 6 80  | > 25 Jan 2016   |                 |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image272.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image273.jpeg){width="9.708333333333334in"
> height="4.897916666666666in"}
>
> *\[Vinyals et al., 2015\]*

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 81 25 Jan 2016

![](media/image275.jpeg){width="9.917361111111111in"
height="4.886805555555555in"}

*reddit.com/r/deepdream*

![](media/image276.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 82 25 Jan 2016

![](media/image277.jpeg){width="10.0in" height="5.625in"}

+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 6 83        | > 25 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image278.jpeg){width="9.501388888888888in"
height="4.777777777777778in"}

> *Deep Neural Networks Rival the Representation of Primate IT Cortex
> for Core Visual Object Recognition \[Cadieu et al., 2014\]*

![](media/image279.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 84 25 Jan 2016

![](media/image280.jpeg){width="9.79375in" height="4.904861111111111in"}

> *Deep Neural Networks Rival the Representation of Primate IT Cortex
> for Core Visual Object Recognition \[Cadieu et al., 2014\]*

![](media/image281.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 6 85 25 Jan 2016

![](media/image282.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 6 86        | > 25 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
