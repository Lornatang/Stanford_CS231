![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Training Neural Networks,

Part I

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 1 20 Jan 2016

> ![](media/image3.jpeg){width="9.7625in" height="4.215277777777778in"}
>
> A1 is due **[today]{.underline}** (midnight)
>
> I'm holding make up office hours on today: 5pm @ Gates 259
>
> A2 will be released \~tomorrow. It's meaty, but educational!
>
> Also:

-   We are shuffling the course schedule around a bit

-   the grading scheme is subject to few % changes

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 2 20 Jan 2016

> ![](media/image5.jpeg){width="9.481944444444444in"
> height="0.8576388888888888in"}

![](media/image6.jpeg){width="5.35625in" height="1.3027777777777778in"}

> "ConvNets need a lot
>
> of data to train"

![](media/image7.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 3 20 Jan 2016

> ![](media/image8.jpeg){width="9.481944444444444in"
> height="0.8576388888888888in"}

![](media/image9.jpeg){width="7.960416666666666in"
height="1.7881944444444444in"}

> "ConvNets need a lot of data to train"

![](media/image10.jpeg){width="6.172916666666667in"
height="0.7451388888888889in"}

> **finetuning!** we rarely ever train ConvNets from scratch.

![](media/image11.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 4 20 Jan 2016

+-----------------------+---------------------------+
| 1\. Train on ImageNet | > 2\. Finetune network on |
+-----------------------+---------------------------+
|                       | > your own data           |
+-----------------------+---------------------------+

![](media/image12.jpeg){width="9.122222222222222in"
height="0.38055555555555554in"}

> ImageNet data

![](media/image14.jpeg){width="10.0in" height="0.5888888888888889in"}

your

![](media/image15.jpeg){width="1.1625in" height="0.5423611111111111in"}

data

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 5 20 Jan 2016

> ![](media/image16.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image17.jpeg){width="5.648611111111111in"
height="3.9541666666666666in"}

> 1\. Train on 2. If small dataset: fix
>
> ImageNet all weights (treat CNN
>
> as fixed feature extractor), retrain only the classifier
>
> i.e. swap the Softmax layer at the end

![](media/image18.jpeg){width="10.0in" height="0.5888888888888889in"}

3.  If you have medium sized dataset, **"finetune"** instead: use the
    old weights as initialization, train the full network or only some
    of the higher layers

![](media/image19.jpeg){width="3.615972222222222in"
height="3.990972222222222in"}

retrain bigger portion of the network, or even all of it.

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 6 20 Jan 2016

> ![](media/image20.jpeg){width="8.27361111111111in"
> height="0.8951388888888889in"}
>
> https://github.com/BVLC/caffe/wiki/Model-Zoo

![](media/image21.jpeg){width="9.222916666666666in"
height="3.8881944444444443in"}

\...

![](media/image22.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 7 20 Jan 2016

> ![](media/image23.jpeg){width="9.481944444444444in"
> height="0.8576388888888888in"}

![](media/image24.jpeg){width="5.35625in" height="1.3027777777777778in"}

> "We have infinite
>
> compute available
>
> because Terminal."

![](media/image25.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 8 20 Jan 2016

> ![](media/image26.jpeg){width="9.481944444444444in"
> height="0.8576388888888888in"}

![](media/image27.jpeg){width="7.084027777777778in"
height="1.7881944444444444in"}

> "We have infinite compute available because Terminal."

![](media/image28.jpeg){width="5.209027777777778in"
height="0.7173611111111111in"}

> You have finite compute.
>
> Don't be overly ambitious.

![](media/image29.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 9 20 Jan 2016

> ![](media/image30.jpeg){width="8.278472222222222in"
> height="0.6909722222222222in"}

![](media/image31.jpeg){width="7.4743055555555555in" height="0.8in"}

> **Mini-batch SGD**

![](media/image32.jpeg){width="10.0in" height="3.751388888888889in"}

> Loop:

1.  **Sample** a batch of data

2.  **Forward** prop it through the graph, get loss

3.  **Backprop** to calculate the gradients

4.  **Update** the parameters using the gradient

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 10 20 Jan 2016

> ![](media/image33.jpeg){width="8.278472222222222in"
> height="0.9659722222222222in"}

![](media/image34.jpeg){width="9.646527777777777in"
height="3.3916666666666666in"}

> (image credits
>
> to Alec Radford)

![](media/image35.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 11 20 Jan 2016

> ![](media/image36.jpeg){width="9.051388888888889in"
> height="4.905555555555556in"}
>
> input tape

loss

![](media/image37.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 12 20 Jan 2016

> ![](media/image38.jpeg){width="10.0in" height="5.625in"}
>
> "local gradient"
>
> f

![](media/image39.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 13 20 Jan 2016

> ![](media/image41.jpeg){width="9.177777777777777in"
> height="0.6729166666666667in"}: forward/backward API

![](media/image42.jpeg){width="6.163194444444445in"
height="3.826388888888889in"}

Graph (or Net) object. *(Rough psuedo code)*

![](media/image43.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 14 20 Jan 2016

> ![](media/image45.jpeg){width="9.611805555555556in"
> height="4.861111111111111in"}: forward/backward API
>
> x

\*

> y

z

![](media/image46.jpeg){width="0.6673611111111111in"
height="5.208880139982502e-3in"}

> (x,y,z are scalars)

![](media/image47.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 15 20 Jan 2016

> ![](media/image48.jpeg){width="9.261111111111111in"
> height="4.990277777777778in"}
>
> =

![](media/image49.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 16 20 Jan 2016

> ![](media/image50.jpeg){width="7.299305555555556in"
> height="0.8597222222222223in"}without the brain stuff

![](media/image51.jpeg){width="7.283333333333333in"
height="0.6111111111111112in"}

> (**Before**) Linear score function:

![](media/image52.jpeg){width="9.239583333333334in" height="0.56875in"}

> (**Now**) 2-layer Neural Network or 3-layer Neural Network

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 17 20 Jan 2016

![](media/image55.jpeg){width="9.938888888888888in"
height="5.565972222222222in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 18        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image56.jpeg){width="7.084027777777778in"
> height="0.5201388888888889in"}

![](media/image57.jpeg){width="5.208880139982502e-3in"
height="2.4520833333333334in"}

+-----------------------------+--------------------------------+--+
| "2-layer Neural Net", or    | > "3-layer Neural Net", or     |  |
+-----------------------------+--------------------------------+--+
|                             | > "2-hidden-layer Neural Net"  |  |
+-----------------------------+--------------------------------+--+
| "1-hidden-layer Neural Net" | > **"Fully-connected" layers** |  |
+-----------------------------+--------------------------------+--+
|                             |                                |  |
+-----------------------------+--------------------------------+--+

![](media/image59.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 19 20 Jan 2016

![](media/image60.jpeg){width="8.804166666666667in"
height="3.832638888888889in"}

> Training Neural Networks
>
> A bit of history\...

![](media/image61.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 20 20 Jan 2016

> ![](media/image62.jpeg){width="9.771527777777777in"
> height="4.638888888888889in"}
>
> The **Mark I Perceptron** machine was the first implementation of the
> perceptron algorithm.
>
> The machine was connected to a camera that used 20×20 cadmium sulfide
> photocells to produce a 400-pixel image.
>
> recognized
>
> letters of the alphabet
>
> update rule:
>
> *Frank Rosenblatt, \~1957: Perceptron*

![](media/image63.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 21 20 Jan 2016

> ![](media/image64.jpeg){width="9.765277777777778in"
> height="4.638888888888889in"}
>
> *Widrow and Hoff, \~1960: Adaline/Madaline*

![](media/image65.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 22 20 Jan 2016

![](media/image66.jpeg){width="7.1875in" height="4.415277777777778in"}

> **A bit of history**

![](media/image67.jpeg){width="3.092361111111111in" height="3.1875in"}

> recognizable maths

![](media/image70.jpeg){width="8.360416666666667in"
height="0.4583333333333333in"}

> *Rumelhart et al. 1986: First time back-propagation became popular*

![](media/image71.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 23        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image72.jpeg){width="9.960416666666667in" height="4.875in"}

*\[Hinton and Salakhutdinov 2006\]*

Reinvigorated research in Deep Learning

![](media/image73.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 24 20 Jan 2016
>
> ![](media/image74.jpeg){width="9.486805555555556in"
> height="2.884027777777778in"}
>
> ***Context-Dependent Pre-trained Deep Neural Networks for Large
> Vocabulary Speech Recognition***
>
> George Dahl, Dong Yu, Li Deng, Alex Acero, 2010
>
> ***Imagenet classification with deep convolutional neural networks***
>
> Alex Krizhevsky, Ilya Sutskever, Geoffrey E Hinton, 2012

![](media/image75.jpeg){width="10.0in" height="2.3513888888888888in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 25 20 Jan 2016

> ![](media/image76.jpeg){width="8.364583333333334in" height="4.5in"}

1.  **One time setup**

> *activation functions, preprocessing, weight initialization,
> regularization, gradient checking*

2.  **Training dynamics**

> *babysitting the learning process,*
>
> *parameter updates, hyperparameter optimization*

3.  **Evaluation** *model ensembles*

![](media/image77.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 26 20 Jan 2016

![](media/image78.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Activation Functions

![](media/image79.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 27 20 Jan 2016

> ![](media/image80.jpeg){width="5.63125in"
> height="0.8298611111111112in"}

![](media/image81.jpeg){width="10.0in" height="4.589583333333334in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 28 20 Jan 2016

+----------------------+------------------+--+
| Activation Functions | > **Leaky ReLU** |  |
+----------------------+------------------+--+
|                      | > max(0.1x, x)   |  |
+----------------------+------------------+--+
| > **Sigmoid**        |                  |  |
+----------------------+------------------+--+

![](media/image82.jpeg){width="9.449305555555556in"
height="0.9131944444444444in"}

> **Maxout**
>
> **tanh** tanh(x)

![](media/image84.jpeg){width="3.827777777777778in"
height="1.7861111111111112in"}

> **ELU**

![](media/image86.jpeg){width="4.85625in" height="1.1784722222222221in"}

> **ReLU** max(0,x)

![](media/image87.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 29 20 Jan 2016

![](media/image88.jpeg){width="9.581944444444444in"
height="3.8555555555555556in"}

> Activation Functions

-   Squashes numbers to range \[0,1\]

-   Historically popular since they have nice interpretation as a
    > saturating "firing rate" of a neuron

> **Sigmoid**

![](media/image89.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 30        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Activation Functions
>
> **Sigmoid**

-   Squashes numbers to range \[0,1\]

-   Historically popular since they have nice interpretation as a
    > saturating "firing rate" of a neuron

![](media/image90.jpeg){width="9.690972222222221in"
height="4.720833333333333in"}

-   problems:

    1.  Saturated neurons "kill" the gradients

![](media/image91.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 31        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> x

![](media/image92.jpeg){width="1.7027777777777777in"
height="5.208880139982502e-3in"}

sigmoid

![](media/image94.jpeg){width="1.9118055555555555in"
height="5.208880139982502e-3in"}

gate

![](media/image96.jpeg){width="1.8027777777777778in"
height="5.208880139982502e-3in"}

> What happens when x = -10?
>
> What happens when x = 0?
>
> What happens when x = 10?

![](media/image98.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 32        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Activation Functions
>
> **Sigmoid**

-   Squashes numbers to range \[0,1\]

-   Historically popular since they have nice interpretation as a
    > saturating "firing rate" of a neuron

![](media/image99.jpeg){width="9.690972222222221in"
height="4.720833333333333in"}

-   problems:

    1.  Saturated neurons "kill" the gradients

    2.  Sigmoid outputs are not zero-centered

![](media/image100.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 33        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image101.jpeg){width="9.127083333333333in"
> height="1.1368055555555556in"}
>
> is always positive:

![](media/image102.jpeg){width="8.32013888888889in"
height="3.0548611111111112in"}

> What can we say about the gradients on **w**?

![](media/image103.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 34 20 Jan 2016

allowed gradient update directions

> ![](media/image104.jpeg){width="9.505555555555556in"
> height="4.222222222222222in"}

![](media/image105.jpeg){width="5.208880139982502e-3in"
height="3.027083333333333in"}

+---------+---------+---------+---------+---------+---------+---------+
|         | > allow |         | > zig   |         |         |         |
|         | ed      |         | > zag   |         |         |         |
|         |         |         | > path  |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > gradi |         |         |         |         |         |
|         | ent     |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > updat |         |         |         |         |         |
|         | e       |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > direc |         |         |         |         |         |
|         | tions   |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | > hypot |         |         |         |         |
|         |         | hetical |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| What    |         |         |         |         |         |         |
| can we  |         |         |         |         |         |         |
| say     |         |         |         |         |         |         |
| about   |         |         |         |         |         |         |
| the     |         |         |         |         |         |         |
| gradien |         |         |         |         |         |         |
| ts      |         |         |         |         |         |         |
| on      |         |         |         |         |         |         |
| **w**?  |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > optim |         |         |         |         |         |
|         | al      |         |         |         |         |         |
|         | > w     |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Always  | > vecto |         |         |         |         |         |
| all     | r       |         |         |         |         |         |
| positiv |         |         |         |         |         |         |
| e       |         |         |         |         |         |         |
| or all  |         |         |         |         |         |         |
| negativ |         |         |         |         |         |         |
| e       |         |         |         |         |         |         |
| :(      |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+

![](media/image108.jpeg){width="0.7048611111111112in"
height="5.208880139982502e-3in"}

> (this is also why you want zero-mean data!)

![](media/image110.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 35 20 Jan 2016

![](media/image111.jpeg){width="9.690972222222221in"
height="4.720833333333333in"}

> Activation Functions
>
> **Sigmoid**

-   Squashes numbers to range \[0,1\]

-   Historically popular since they have nice interpretation as a
    > saturating "firing rate" of a neuron

<!-- -->

-   problems:

    1.  Saturated neurons "kill" the gradients

    2.  Sigmoid outputs are not zero-centered

    3.  exp() is a bit compute expensive

![](media/image112.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 36        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image113.jpeg){width="5.63125in"
height="0.8298611111111112in"}

> Activation Functions

![](media/image114.jpeg){width="9.934722222222222in"
height="4.404861111111111in"}

-   Squashes numbers to range \[-1,1\]

-   zero centered (nice)

-   still kills gradients when saturated :(

> **tanh(x)**

\[LeCun et al., 1991\]

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 37        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Activation Functions

![](media/image115.jpeg){width="3.816666666666667in"
height="0.5229166666666667in"}

> **ReLU**
>
> (Rectified Linear Unit)

-   Computes **f(x) = max(0,x)**

-   Does not saturate (in +region)

-   Very computationally efficient

-   Converges much faster than sigmoid/tanh in practice (e.g. 6x)

![](media/image116.jpeg){width="9.914583333333333in" height="3.2in"}

\[Krizhevsky et al., 2012\]

![](media/image118.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 38        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Activation Functions

![](media/image119.jpeg){width="3.816666666666667in"
height="0.5229166666666667in"}

> **ReLU**
>
> (Rectified Linear Unit)

-   Computes **f(x) = max(0,x)**

-   Does not saturate (in +region)

-   Very computationally efficient

-   Converges much faster than sigmoid/tanh in practice (e.g. 6x)

-   Not zero-centered output

-   An annoyance:

![](media/image120.jpeg){width="9.914583333333333in" height="3.2in"}

hint: what is the gradient when x \< 0?

![](media/image121.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 39 20 Jan 2016

> x

![](media/image122.jpeg){width="1.7027777777777777in"
height="5.208880139982502e-3in"}

ReLU

![](media/image124.jpeg){width="1.9118055555555555in"
height="5.208880139982502e-3in"}

> gate

![](media/image126.jpeg){width="1.8027777777777778in"
height="5.208880139982502e-3in"}

> What happens when x = -10?
>
> What happens when x = 0?
>
> What happens when x = 10?

![](media/image128.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 40        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image129.jpeg){width="5.208880139982502e-3in"
height="4.742361111111111in"}

> active ReLU
>
> **DATA CLOUD**

![](media/image131.jpeg){width="8.25763888888889in"
height="5.208880139982502e-3in"}

> dead ReLU
>
> will never activate
>
> =\> never update

![](media/image132.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 41 20 Jan 2016

![](media/image133.jpeg){width="5.208880139982502e-3in"
height="4.742361111111111in"}

> active ReLU
>
> **DATA CLOUD**

![](media/image135.jpeg){width="8.25763888888889in"
height="5.208880139982502e-3in"}

+---------------------------------+-----------------------+--+
| > =\> people like to initialize | > dead ReLU           |  |
+---------------------------------+-----------------------+--+
| > ReLU neurons with slightly    |                       |  |
+---------------------------------+-----------------------+--+
| > positive biases (e.g. 0.01)   | > will never activate |  |
+---------------------------------+-----------------------+--+
|                                 | > =\> never update    |  |
+---------------------------------+-----------------------+--+
|                                 |                       |  |
+---------------------------------+-----------------------+--+

![](media/image136.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 42 20 Jan 2016

+-------------+-------------+-------------+-------------+-------------+
| Activation  |             |             | > \[Mass et |             |
| Functions   |             |             | > al.,      |             |
|             |             |             | > 2013\]    |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             | > \[He et   |             |
|             |             |             | > al.,      |             |
|             |             |             | > 2015\]    |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > \-        | > Does not  |             |             |
|             |             | > saturate  |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > \-        | > Computati |             |             |
|             |             | onally      |             |             |
|             |             | > efficient |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > \-        |             |             |             |
|             | > Converges |             |             |             |
|             | > much      |             |             |             |
|             | > faster    |             |             |             |
|             | > than      |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             | > sigmoid/t |             |             |
|             |             | anh         |             |             |
|             |             | > in        |             |             |
|             |             | > practice! |             |             |
|             |             | > (e.g. 6x) |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **-**     | > **will    |             |             |
|             |             | > not       |             |             |
|             |             | > "die".**  |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image137.jpeg){width="5.63125in" height="4.430555555555555in"}

> **Leaky ReLU**

![](media/image138.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 43 20 Jan 2016

> Activation Functions
>
> **Leaky ReLU**
>
> \[Mass et al., 2013\]

![](media/image139.jpeg){width="9.914583333333333in"
height="4.979861111111111in"}

> \[He et al., 2015\]

-   Does not saturate

-   Computationally efficient

-   Converges much faster than sigmoid/tanh in practice! (e.g. 6x)

-   **will not "die".**

![](media/image140.jpeg){width="5.208880139982502e-3in"
height="2.171527777777778in"}

> **Parametric Rectifier (PReLU)**
>
> backprop into \\alpha
>
> (parameter)

![](media/image141.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 44        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image142.jpeg){width="9.799305555555556in"
> height="1.4395833333333334in"}

\[Clevert et al., 2015\]

> **Exponential Linear Units (ELU)**

![](media/image143.jpeg){width="9.775694444444444in"
height="3.0166666666666666in"}

> **-** All benefits of ReLU - Does not die

\- Closer to zero mean outputs

> \- Computation requires exp()

![](media/image144.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 45 20 Jan 2016

> ![](media/image145.jpeg){width="9.849305555555556in"
> height="0.8298611111111112in"}

\[Goodfellow et al., 2013\]

-   Does not have the basic form of dot product -\> nonlinearity

-   Generalizes ReLU and Leaky ReLU

-   Linear Regime! Does not saturate! Does not die!

![](media/image146.jpeg){width="9.0875in" height="1.7826388888888889in"}

> Problem: doubles the number of parameters/neuron :(

![](media/image147.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 46 20 Jan 2016

> ![](media/image148.jpeg){width="9.849305555555556in"
> height="0.8298611111111112in"}

![](media/image149.jpeg){width="9.64375in" height="3.702777777777778in"}

-   Use ReLU. Be careful with your learning rates

-   Try out Leaky ReLU / Maxout / ELU

-   Try out tanh but don't expect much

-   Don't use sigmoid

![](media/image150.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 47 20 Jan 2016

![](media/image151.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Data Preprocessing

![](media/image152.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 48 20 Jan 2016

![](media/image153.jpeg){width="8.730555555555556in"
height="3.595833333333333in"}

> [Step 1: Preprocess the data]{.underline}

![](media/image154.jpeg){width="6.059027777777778in"
height="0.36319444444444443in"}

> (Assume X \[NxD\] is data matrix,
>
> each example in a row)

![](media/image156.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 49        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image157.jpeg){width="9.672222222222222in"
> height="1.3875in"}
>
> In practice, you may also see **PCA** and **Whitening** of the data

![](media/image158.jpeg){width="8.253472222222221in"
height="3.111111111111111in"}

> (data has diagonal (covariance matrix is the
>
> covariance matrix) identity matrix)

![](media/image159.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 50 20 Jan 2016

![](media/image160.jpeg){width="9.849305555555556in"
height="0.8298611111111112in"}

> **TLDR: In practice for Images:** center only

![](media/image161.jpeg){width="9.671527777777778in"
height="2.4118055555555555in"}

> e.g. consider CIFAR-10 example with \[32,32,3\] images
>
> \- Subtract the mean image (e.g. AlexNet)
>
> (mean image = \[32,32,3\] array)
>
> \- Subtract per-channel mean (e.g. VGGNet)
>
> (mean along each channel = 3 numbers)

![](media/image162.jpeg){width="3.3944444444444444in"
height="1.0993055555555555in"}

> Not common to normalize
>
> variance, to do PCA or
>
> whitening

![](media/image163.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 51        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image164.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Weight Initialization

![](media/image165.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 52 20 Jan 2016

> ![](media/image166.jpeg){width="8.952083333333333in"
> height="4.479861111111111in"}

![](media/image167.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 53 20 Jan 2016

-   ![](media/image168.jpeg){width="8.384722222222223in"
    > height="4.360416666666667in"}**Small random numbers**

> (gaussian with zero mean and 1e-2 standard deviation)

![](media/image169.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 54 20 Jan 2016

-   ![](media/image170.jpeg){width="8.384722222222223in"
    > height="4.360416666666667in"}**Small random numbers**

> (gaussian with zero mean and 1e-2 standard deviation)
>
> Works \~okay for small networks, but can lead to non-homogeneous
> distributions of activations across the layers of a network.

![](media/image171.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 55 20 Jan 2016

![](media/image172.jpeg){width="9.509027777777778in"
height="4.805555555555555in"}

> Lets look at
>
> some
>
> activation
>
> statistics

![](media/image173.jpeg){width="2.7472222222222222in"
height="1.9166666666666667in"}

> E.g. 10-layer net with 500 neurons on each layer, using tanh
> non-linearities, and initializing as described in last slide.

![](media/image174.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 56        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image175.jpeg){width="9.614583333333334in" height="5.625in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 57        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image176.jpeg){width="9.946527777777778in"
> height="4.979166666666667in"}

Q.  think about the backward pass. What do the gradients look like?

![](media/image177.jpeg){width="3.1791666666666667in"
height="0.8666666666666667in"}

> Hint: think about backward pass for a W\*X gate.

![](media/image178.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 58 20 Jan 2016

![](media/image179.jpeg){width="9.6625in" height="4.920138888888889in"}

> \*1.0 instead of \*0.01

![](media/image180.jpeg){width="10.0in" height="0.5888888888888889in"}

Almost all neurons completely saturated, either -1 and 1. Gradients will
be all zero.

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 59 20 Jan 2016

> ![](media/image181.jpeg){width="9.960416666666667in"
> height="4.909027777777778in"}
>
> **Reasonable initialization.** (Mathematical derivation assumes linear
> activations)

![](media/image182.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 60 20 Jan 2016

> ![](media/image183.jpeg){width="9.878472222222221in"
> height="4.958333333333333in"}
>
> nonlinearity it breaks.

![](media/image184.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 61 20 Jan 2016

> ![](media/image185.jpeg){width="9.865972222222222in"
> height="4.845833333333333in"}

![](media/image186.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 62 20 Jan 2016

> ![](media/image187.jpeg){width="9.865972222222222in"
> height="4.845833333333333in"}

![](media/image188.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 63 20 Jan 2016

> ![](media/image189.jpeg){width="9.854861111111111in"
> height="0.43125in"}
>
> ***Understanding the difficulty of training deep feedforward neural
> networks*** by Glorot and Bengio, 2010
>
> ***Exact solutions to the nonlinear dynamics of learning in deep
> linear neural networks*** by Saxe et al, 2013
>
> ***Random walk initialization for training very deep feedforward
> networks*** by Sussillo and Abbott, 2014
>
> ***Delving deep into rectifiers: Surpassing human-level performance on
> ImageNet classification*** by He et al., 2015
>
> ***Data-dependent Initializations of Convolutional Neural Networks***
> by Krähenbühl et al., 2015 ***All you need is a good init***, Mishkin
> and Matas, 2015
>
> ...

![](media/image190.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 64 20 Jan 2016

> ![](media/image191.jpeg){width="9.729861111111111in"
> height="0.7548611111111111in"}

![](media/image192.jpeg){width="9.280555555555555in"
height="0.5756944444444444in"}

\[Ioffe and Szegedy, 2015\]

> "you want unit gaussian activations? just make them so."

![](media/image193.jpeg){width="7.278472222222222in"
height="0.8847222222222222in"}

> consider a batch of activations at some layer.
>
> To make each dimension unit gaussian, apply:

![](media/image194.jpeg){width="8.144444444444444in"
height="1.3263888888888888in"}

> this is a vanilla differentiable function\...

![](media/image195.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 65 20 Jan 2016

> ![](media/image196.jpeg){width="9.729861111111111in"
> height="0.7548611111111111in"}

![](media/image197.jpeg){width="9.280555555555555in"
height="0.5756944444444444in"}

\[Ioffe and Szegedy, 2015\]

> "you want unit gaussian activations?
>
> just make them so."

![](media/image198.jpeg){width="5.808333333333334in"
height="0.8645833333333334in"}

1.  compute the empirical mean and variance independently for each
    > dimension.

![](media/image199.jpeg){width="2.8965277777777776in"
height="2.2888888888888888in"}

> ^N^ X

![](media/image200.jpeg){width="3.745138888888889in"
height="5.208880139982502e-3in"}

> 2\. Normalize

![](media/image202.jpeg){width="3.173611111111111in"
height="1.0590277777777777in"}

> D

![](media/image204.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 66 20 Jan 2016

> ![](media/image205.jpeg){width="9.729861111111111in"
> height="0.7548611111111111in"}

![](media/image206.jpeg){width="5.208880139982502e-3in"
height="0.40555555555555556in"}

\[Ioffe and Szegedy, 2015\]

> FC

![](media/image208.jpeg){width="5.208880139982502e-3in"
height="0.19930555555555557in"}

> BN

![](media/image209.jpeg){width="5.208880139982502e-3in"
height="0.19930555555555557in"}

> tanh

![](media/image210.jpeg){width="5.208880139982502e-3in"
height="0.2520833333333333in"}

> FC

![](media/image211.jpeg){width="5.208880139982502e-3in"
height="0.19930555555555557in"}

> BN

![](media/image212.jpeg){width="5.208880139982502e-3in"
height="0.19930555555555557in"}

> tanh

![](media/image213.jpeg){width="5.208880139982502e-3in"
height="0.2604166666666667in"}

> \...
>
> Usually inserted after Fully Connected / (or Convolutional, as we'll
> see soon) layers, and before nonlinearity.

![](media/image214.jpeg){width="0.4777777777777778in"
height="5.208880139982502e-3in"}

Problem: do we necessarily want a unit gaussian input to a tanh layer?

![](media/image215.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 67 20 Jan 2016

> ![](media/image216.jpeg){width="9.729861111111111in"
> height="0.7548611111111111in"}

![](media/image217.jpeg){width="9.311805555555555in"
height="3.595138888888889in"}

\[Ioffe and Szegedy, 2015\]

> Normalize:
>
> And then allow the network to squash the range if it wants to:

![](media/image218.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 68 20 Jan 2016

> Batch Normalization
>
> \[Ioffe and Szegedy, 2015\]

![](media/image219.jpeg){width="9.815972222222221in" height="4.81875in"}

-   Improves gradient flow through the network

-   Allows higher learning rates

-   Reduces the strong dependence on initialization

-   Acts as a form of regularization in a funny way, and slightly
    reduces the need for dropout, maybe

![](media/image220.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 69 20 Jan 2016

> Batch Normalization
>
> \[Ioffe and Szegedy, 2015\]

![](media/image221.jpeg){width="9.815972222222221in" height="4.81875in"}

**Note: at test time BatchNorm layer functions differently:**

The mean/std are not computed based on the batch. Instead, a single
fixed empirical mean of activations during training is used.

(e.g. can be estimated during training with running averages)

![](media/image222.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 70 20 Jan 2016

![](media/image223.jpeg){width="8.804166666666667in" height="3.95625in"}

Babysitting the Learning Process

![](media/image224.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 71 20 Jan 2016

![](media/image225.jpeg){width="8.730555555555556in"
height="3.595833333333333in"}

> [Step 1: Preprocess the data]{.underline}

![](media/image226.jpeg){width="6.059027777777778in"
height="0.36319444444444443in"}

> (Assume X \[NxD\] is data matrix,
>
> each example in a row)

![](media/image228.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 72        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image229.jpeg){width="9.661805555555556in"
height="0.5090277777777777in"}

> **Step 2: Choose the architecture:**
>
> say we start with one hidden layer of 50 neurons:

![](media/image230.jpeg){width="3.2569444444444446in"
height="0.5861111111111111in"}

50. hidden

> neurons

![](media/image231.jpeg){width="0.9298611111111111in"
height="5.208880139982502e-3in"}

+---------+---------+---------+---------+---------+---------+---------+
|         |         |         | > outpu | > **10* |         |         |
|         |         |         | t       | *       |         |         |
|         |         |         | > layer | > outpu |         |         |
|         |         |         |         | t       |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > CIFAR | > input |         |         | > neuro |         |         |
| -10     |         |         |         | ns,     |         |         |
|         |         |         |         | > one   |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | > hidde |         | > per   |         |         |
|         |         | n       |         | > class |         |         |
|         |         | > layer |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > image | > layer |         |         |         |         |         |
| s,      |         |         |         |         |         |         |
| > **307 |         |         |         |         |         |         |
| 2**     |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > numbe |         |         |         |         |         |         |
| rs      |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Fei-F | > Lectu | > 20    |         |         |         |         |
| ei      | re      | > Jan   |         |         |         |         |
| > Li &  | > 5 73  | > 2016  |         |         |         |         |
| > Andre |         |         |         |         |         |         |
| j       |         |         |         |         |         |         |
| > Karpa |         |         |         |         |         |         |
| thy     |         |         |         |         |         |         |
| > &     |         |         |         |         |         |         |
| > Justi |         |         |         |         |         |         |
| n       |         |         |         |         |         |         |
| > Johns |         |         |         |         |         |         |
| on      |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+

![](media/image234.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image235.jpeg){width="9.661805555555556in"
height="0.5090277777777777in"}

> Double check that the loss is reasonable:

![](media/image236.jpeg){width="6.9430555555555555in"
height="1.8972222222222221in"}

> loss \~2.3.
>
> "correct " for
>
> 10 classes

disable regularization

returns the loss and the gradient for all parameters

![](media/image238.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 74        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image239.jpeg){width="9.661805555555556in"
> height="0.5090277777777777in"}

![](media/image240.jpeg){width="6.9430555555555555in"
height="1.8972222222222221in"}

> crank up regularization
>
> ![](media/image242.jpeg){width="1.5923611111111111in"
> height="0.26666666666666666in"} loss went up, good. (sanity check)

![](media/image243.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 75 20 Jan 2016

Lets try to train now...

**Tip**: Make sure that you can overfit very small portion of the
training data

The above code:

![](media/image244.jpeg){width="10.0in" height="4.513888888888889in"}

-   take the first 20 examples from CIFAR-10

-   turn off regularization (reg = 0.0)

-   use simple vanilla 'sgd'

![](media/image245.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 76 20 Jan 2016

![](media/image246.jpeg){width="9.949305555555556in" height="4.94375in"}

**Tip**: Make sure that you can overfit very small portion of the
training data

> Very small loss,
>
> train accuracy 1.00,
>
> nice!

![](media/image247.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 77 20 Jan 2016

![](media/image248.jpeg){width="10.0in" height="3.165277777777778in"}

I like to start with small regularization and find learning rate that
makes the loss go down.

![](media/image249.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 78 20 Jan 2016

![](media/image250.jpeg){width="10.0in" height="4.3375in"}

I like to start with small regularization and find learning rate that
makes the loss go down.

Loss barely changing

![](media/image251.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 79 20 Jan 2016

Lets try to train now...

I like to start with small regularization and find learning rate that
makes the loss go down.

**loss not going down:**

learning rate too low

Loss barely changing: Learning rate is probably too low

![](media/image252.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 80 20 Jan 2016
>
> Lets try to train now...
>
> I like to start with small regularization and find learning rate that
> makes the loss go down.
>
> **loss not going down:**
>
> learning rate too low

Loss barely changing: Learning rate is probably too low

![](media/image254.jpeg){width="10.0in" height="4.3375in"}

Notice train/val accuracy goes to 20% though, what's up with that?
(remember this is softmax)

![](media/image255.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 5 81        | > 20 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

Lets try to train now...

I like to start with small regularization and find learning rate that
makes the loss go down.

Okay now lets try learning rate 1e6. What could possibly go wrong?

![](media/image256.jpeg){width="9.879166666666666in" height="3.05in"}

**loss not going down:**

learning rate too low

![](media/image257.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 82 20 Jan 2016

Lets try to train now...

I like to start with small regularization and find learning rate that
makes the loss go down.

**loss not going down:** learning rate too low **loss exploding:**
learning rate too high

cost: NaN almost

![](media/image258.jpeg){width="3.592361111111111in"
height="0.9902777777777778in"}

always means high

learning rate\...

![](media/image260.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 83 20 Jan 2016

Lets try to train now...

I like to start with small regularization and find learning rate that
makes the loss go down.

**loss not going down:**

learning rate too low **loss exploding:**

learning rate too high

3e-3 is still too high. Cost explodes....

![](media/image261.jpeg){width="9.945833333333333in"
height="4.595833333333333in"}

=\> Rough range for learning rate we should be cross-validating is
somewhere \[1e-3 ... 1e-5\]

![](media/image262.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 84 20 Jan 2016

![](media/image263.jpeg){width="8.804166666666667in"
height="3.6993055555555556in"}

> Hyperparameter Optimization

![](media/image264.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 85 20 Jan 2016

> ![](media/image265.jpeg){width="9.7875in" height="4.66875in"}
>
> I like to do **coarse -\> fine** cross-validation in stages
>
> **First stage**: only a few epochs to get rough idea of what params
> work
>
> **Second stage**: longer running time, finer search ... (repeat as
> necessary)
>
> Tip for detecting explosions in the solver:
>
> If the cost is ever \> 3 \* original cost, break out early

![](media/image266.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 86 20 Jan 2016

> ![](media/image267.jpeg){width="9.89861111111111in"
> height="2.660416666666667in"}
>
> note it's best to optimize
>
> in log space!

![](media/image268.jpeg){width="7.090972222222222in"
height="2.0694444444444446in"}

> nice

![](media/image270.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 87 20 Jan 2016

> ![](media/image272.jpeg){width="9.777083333333334in"
> height="4.858333333333333in"}
>
> adjust range

![](media/image273.jpeg){width="2.0833333333333335in"
height="5.208880139982502e-3in"}

> **53%** - relatively good for a 2-layer neural net with 50 hidden
> neurons.

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 88 20 Jan 2016

> ![](media/image275.jpeg){width="9.777083333333334in"
> height="4.858333333333333in"}
>
> adjust range

![](media/image276.jpeg){width="2.0833333333333335in"
height="5.208880139982502e-3in"}

> **53%** - relatively good for a 2-layer neural net with 50 hidden
> neurons.
>
> But this best cross-validation result is
> ![](media/image277.jpeg){width="1.0416666666666666e-2in"
> height="0.15486111111111112in"} worrying. Why?

![](media/image279.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 89 20 Jan 2016

> ![](media/image281.jpeg){width="9.360416666666667in"
> height="3.933333333333333in"}

![](media/image282.jpeg){width="4.930555555555555in"
height="0.2951388888888889in"}

> *Random Search for Hyper-Parameter Optimization*
>
> Bergstra and Bengio, 2012

![](media/image283.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 90 20 Jan 2016

> ![](media/image284.jpeg){width="9.567361111111111in"
> height="4.850694444444445in"}

-   network architecture

-   learning rate, its decay schedule, update type

-   regularization (L2/Dropout strength)

> neural networks practitioner music = loss function

![](media/image285.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 91 20 Jan 2016

> ![](media/image286.jpeg){width="9.439583333333333in"
> height="4.904861111111111in"}

![](media/image287.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 92 20 Jan 2016

> ![](media/image288.jpeg){width="9.033333333333333in"
> height="0.5826388888888889in"}

![](media/image289.jpeg){width="10.0in" height="4.8902777777777775in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 93 20 Jan 2016

> ![](media/image290.jpeg){width="5.208880139982502e-3in"
> height="3.488888888888889in"}

![](media/image292.jpeg){width="5.1097222222222225in"
height="5.208880139982502e-3in"}

time

![](media/image294.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 94 20 Jan 2016

> ![](media/image295.jpeg){width="5.208880139982502e-3in"
> height="3.488888888888889in"}
>
> Bad initialization
>
> a prime suspect

![](media/image297.jpeg){width="5.1097222222222225in"
height="5.208880139982502e-3in"}

> time

![](media/image299.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 95 20 Jan 2016

> ![](media/image300.jpeg){width="8.254861111111111in"
> height="0.7805555555555556in"} Loss function specimen

![](media/image301.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 96 20 Jan 2016

> ![](media/image303.jpeg){width="6.138194444444444in"
> height="0.7805555555555556in"}

![](media/image304.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 97 20 Jan 2016

![](media/image306.jpeg){width="9.491666666666667in"
height="4.847916666666666in"}

> [lossfunctions.tumblr.com]{.underline}

![](media/image307.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 98 20 Jan 2016

> ![](media/image308.jpeg){width="9.033333333333333in"
> height="0.5826388888888889in"}

![](media/image309.jpeg){width="5.208880139982502e-3in"
height="1.9055555555555554in"}

> big gap = overfitting

=\> increase regularization strength?

> no gap
>
> =\> increase model capacity?

![](media/image311.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 5 99 20 Jan 2016

![](media/image312.jpeg){width="9.033333333333333in"
height="0.5826388888888889in"}

> Track the ratio of weight updates / weight magnitudes:

![](media/image313.jpeg){width="8.813194444444445in"
height="0.4583333333333333in"}

> ratio between the values and updates: \~ 0.0002 / 0.02 = 0.01 (about
> okay) **want this to be somewhere around 0.001 or so**

![](media/image315.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 5     | 10              | > 20 Jan 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 0               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image316.jpeg){width="8.722916666666666in"
height="4.410416666666666in"}

> Summary ^TLDRs^
>
> We looked in detail at:

-   Activation Functions (use ReLU)

-   Data Preprocessing (images: subtract mean)

-   Weight Initialization (use Xavier init)

-   Batch Normalization (use)

-   Babysitting the Learning process

-   Hyperparameter Optimization

> (random sample hyperparams, in log space when appropriate)

![](media/image317.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 5     | 10              | > 20 Jan 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 1               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image318.jpeg){width="8.722916666666666in"
height="4.410416666666666in"}

> TODO
>
> Look at:

-   Parameter update schemes

-   Learning rate schedules

-   Gradient Checking

-   Regularization (Dropout etc)

-   Evaluation (Ensembles etc)

![](media/image319.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 5     | 10              | > 20 Jan 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 2               |                 |
+-----------------+-----------------+-----------------+-----------------+
