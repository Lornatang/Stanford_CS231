![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

> Convolutional Neural Networks

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 1 27 Jan 2016

> ![](media/image3.jpeg){width="9.7625in" height="4.215277777777778in"}
>
> [A2]{.underline} is due Feb 5 (next Friday)
>
> [Project proposal]{.underline} due Jan 30 (Saturday)

-   ungraded, one paragraph

-   feel free to give 2 options, we can try help you narrow it

<!-- -->

-   What is the problem that you will be investigating? Why is it
    > interesting?

-   What data will you use? If you are collecting new datasets, how do
    > you plan to collect them?

-   What method or algorithm are you proposing? If there are existing
    > implementations, will you use them and how? How do you plan to
    > improve or modify such implementations?

-   What reading will you examine to provide context and background?

-   How will you evaluate your results? Qualitatively, what kind of
    > results do you expect (e.g. plots or figures)? Quantitatively,
    > what kind of analysis will you use to evaluate and/or compare your
    > results (e.g. what performance metrics or statistical tests)?

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 2 27 Jan 2016

> ![](media/image5.jpeg){width="9.772222222222222in"
> height="4.769444444444445in"}
>
> Loop:

1.  **Sample** a batch of data

2.  **Forward** prop it through the graph, get loss

3.  **Backprop** to calculate the gradients

4.  **Update** the parameters using the gradient

![](media/image6.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 3 27 Jan 2016

> ![](media/image7.jpeg){width="2.7152777777777777in"
> height="1.6416666666666666in"}

**We covered:**

![](media/image8.jpeg){width="6.8069444444444445in"
height="3.9972222222222222in"}

sgd,

momentum,

nag,

adagrad,

rmsprop,

adam (not in this vis),

we did not cover adadelta

![](media/image9.jpeg){width="2.7118055555555554in" height="0.2in"}

> Image credits: Alec Radford

![](media/image10.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 4 27 Jan 2016

> ![](media/image11.jpeg){width="9.497916666666667in"
> height="0.85625in"}

![](media/image12.jpeg){width="9.345138888888888in" height="3.0625in"}

Forces the network to have a redundant representation.

![](media/image13.jpeg){width="5.878472222222222in"
height="1.4541666666666666in"}

> has an ear

![](media/image14.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> has a tail

![](media/image15.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> is furry

![](media/image16.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> has claws

![](media/image18.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> mischievous

![](media/image19.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> look

![](media/image20.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7

> **X**

![](media/image21.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

-   ![](media/image23.jpeg){width="0.9097222222222222in"
    > height="0.12430555555555556in"} cat

> ![](media/image24.jpeg){width="0.9298611111111111in"
> height="0.23125in"} score

![](media/image25.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

> **X**

![](media/image27.jpeg){width="0.7736111111111111in"
height="5.208880139982502e-3in"}

-   27 Jan 2016

> ![](media/image28.jpeg){width="9.73125in"
> height="1.4534722222222223in"}

![](media/image29.jpeg){width="7.934027777777778in"
height="2.204861111111111in"}

> *\[LeNet-5, LeCun 1980\]*

![](media/image31.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 6 27 Jan 2016

> ![](media/image32.jpeg){width="5.208880139982502e-3in"
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

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 7 27 Jan 2016

> ![](media/image34.jpeg){width="8.70486111111111in"
> height="0.6736111111111112in"}

![](media/image35.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 8 27 Jan 2016

![](media/image37.jpeg){width="9.686111111111112in"
height="1.7236111111111112in"}

> Convolutional Neural Networks
>
> (First without the brain stuff)

![](media/image38.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 9 27 Jan 2016

![](media/image39.jpeg){width="8.436805555555555in"
height="0.7326388888888888in"}

> Convolution Layer

![](media/image40.jpeg){width="3.691666666666667in"
height="0.5465277777777777in"}

> 32x32x3 image

![](media/image41.jpeg){width="5.1722222222222225in"
height="3.198611111111111in"}

32. height

<!-- -->

32. width

> ~3~ depth

![](media/image42.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 10        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image43.jpeg){width="8.436805555555555in"
height="0.7326388888888888in"}

> Convolution Layer

![](media/image44.jpeg){width="3.691666666666667in"
height="0.5465277777777777in"}

> 32x32x3 image

![](media/image45.jpeg){width="1.675in" height="3.198611111111111in"}

> 5x5x3 filter
>
> 32

![](media/image47.jpeg){width="5.507638888888889in"
height="1.2604166666666667in"}

> **Convolve** the filter with the image
>
> i.e. "slide over the image spatially,
>
> computing dot products"
>
> 32
>
> 3

![](media/image48.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 11        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Convolution Layer

Filters always extend the full depth of the input volume

![](media/image49.jpeg){width="10.0in" height="4.715972222222222in"}

> 32x32x3 image
>
> 5x5x3 filter
>
> 32
>
> **Convolve** the filter with the image
>
> i.e. "slide over the image spatially,
>
> computing dot products"
>
> 32
>
> 3

![](media/image50.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 12        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image51.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image52.jpeg){width="8.692361111111111in" height="4.03125in"}

32

> 32
>
> 3

32x32x3 image

5x5x3 filter

> **1 number:**
>
> the result of taking a dot product between the filter and a small
> 5x5x3 chunk of the image (i.e. 5\*5\*3 = 75-dimensional dot product +
> bias)

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 13 27 Jan 2016

> ![](media/image54.jpeg){width="9.6125in" height="4.559722222222222in"}

**activation map**

> 32x32x3 image
>
> 5x5x3 filter
>
> 32
>
> 28

![](media/image55.jpeg){width="2.5875in"
height="5.208880139982502e-3in"}

> convolve (slide) over all
>
> spatial locations

  ---- ----
  32   28
  3    1
  ---- ----

![](media/image56.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 14 27 Jan 2016

> Convolution Layer

consider a second, green filter

![](media/image57.jpeg){width="9.881944444444445in"
height="4.622222222222222in"}

+---------------+-----------------------+
| 32x32x3 image | > **activation maps** |
+---------------+-----------------------+
| 5x5x3 filter  |                       |
+---------------+-----------------------+

> 32
>
> 28

![](media/image58.jpeg){width="2.5875in"
height="5.208880139982502e-3in"}

> convolve (slide) over all
>
> spatial locations

  ---- ----
  32   28
  3    1
  ---- ----

![](media/image59.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 15 27 Jan 2016

![](media/image60.jpeg){width="9.565277777777778in"
height="0.45069444444444445in"}

> For example, if we had 6 5x5 filters, we'll get 6 separate activation
> maps:

![](media/image61.jpeg){width="5.674305555555556in"
height="3.8131944444444446in"}

> **activation maps**

![](media/image62.jpeg){width="1.6972222222222222in"
height="3.198611111111111in"}

> 32

28

![](media/image63.jpeg){width="2.5875in"
height="5.208880139982502e-3in"}

> Convolution Layer

  ---- ----
  32   28
  3    6
  ---- ----

![](media/image64.jpeg){width="9.103472222222223in"
height="0.3090277777777778in"}

> We stack these up to get a "new image" of size 28x28x6!

![](media/image65.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 16        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image66.jpeg){width="9.57986111111111in"
> height="4.232638888888889in"}ConvNet is a sequence of Convolution
> Layers, interspersed with activation functions
>
> 32 28

![](media/image67.jpeg){width="1.0798611111111112in"
height="5.208880139982502e-3in"}

+----+-----------+----+--+
|    | > CONV,   |    |  |
+----+-----------+----+--+
|    | > ReLU    |    |  |
+----+-----------+----+--+
|    | > e.g. 6  |    |  |
+----+-----------+----+--+
| 32 | > 5x5x3   | 28 |  |
+----+-----------+----+--+
|    | > filters |    |  |
+----+-----------+----+--+
|    |           |    |  |
+----+-----------+----+--+

> 3 6

![](media/image68.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 17 27 Jan 2016

> ![](media/image69.jpeg){width="9.770833333333334in"
> height="4.232638888888889in"}ConvNet is a sequence of Convolutional
> Layers, interspersed with activation functions
>
> 32 28 24
>
> ....

![](media/image70.jpeg){width="1.0798611111111112in"
height="5.208880139982502e-3in"}

+----+-----------+----+-------------+---------+--+
|    | > CONV,   |    | > CONV,     | > CONV, |  |
+----+-----------+----+-------------+---------+--+
|    | > ReLU    |    | > ReLU      | > ReLU  |  |
+----+-----------+----+-------------+---------+--+
|    | > e.g. 6  |    | > e.g. 10   |         |  |
+----+-----------+----+-------------+---------+--+
| 32 | > 5x5x3   | 28 | > 5x5x**6** | 24      |  |
+----+-----------+----+-------------+---------+--+
|    | > filters |    | > filters   |         |  |
+----+-----------+----+-------------+---------+--+
| 3  |           | 6  |             | 10      |  |
+----+-----------+----+-------------+---------+--+
|    |           |    |             |         |  |
+----+-----------+----+-------------+---------+--+

![](media/image73.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 18 27 Jan 2016

> **Preview**

*\[From recent Yann*

![](media/image74.jpeg){width="9.800694444444444in"
height="4.978472222222222in"}

*LeCun slides\]*

![](media/image75.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 19 27 Jan 2016

> **Preview**

*\[From recent Yann LeCun slides\]*

![](media/image76.jpeg){width="10.0in" height="5.588888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 20 27 Jan 2016

> one filter =\>
>
> one activation map

![](media/image77.jpeg){width="10.0in" height="0.5888888888888889in"}

> example 5x5 filters

![](media/image78.jpeg){width="9.55in" height="4.970833333333333in"}

> (32 total)

We call the layer convolutional because it is related to convolution of
two signals:

![](media/image79.jpeg){width="5.208880139982502e-3in"
height="0.4951388888888889in"}

> elementwise multiplication and sum of a filter and the signal (image)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 21 27 Jan 2016

![](media/image80.jpeg){width="2.765972222222222in"
height="0.14097222222222222in"}

![](media/image81.jpeg){width="10.0in" height="5.372222222222222in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 22 27 Jan 2016
>
> ![](media/image82.jpeg){width="9.1875in"
> height="4.7243055555555555in"}
>
> 32x32x3 image
>
> 5x5x3 filter
>
> 32

![](media/image83.jpeg){width="2.5875in"
height="5.208880139982502e-3in"}

> convolve (slide) over all
>
> spatial locations
>
> 32
>
> 3

![](media/image84.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7

> **activation map**
>
> **28**
>
> **28**

1

23 27 Jan 2016

> ![](media/image85.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image86.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image87.jpeg){width="9.378472222222221in" height="3.0625in"}

> 7x7 input (spatially)
>
> assume 3x3 filter

![](media/image88.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image89.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 24 27 Jan 2016

> ![](media/image90.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image91.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image92.jpeg){width="9.378472222222221in" height="3.0625in"}

> 7x7 input (spatially)
>
> assume 3x3 filter

![](media/image93.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 25 27 Jan 2016

> ![](media/image95.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image96.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image97.jpeg){width="9.378472222222221in" height="3.0625in"}

> 7x7 input (spatially)
>
> assume 3x3 filter

![](media/image98.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image99.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 26 27 Jan 2016

> ![](media/image100.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image101.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image102.jpeg){width="9.369444444444444in" height="3.0625in"}

> 7x7 input (spatially)
>
> assume 3x3 filter

![](media/image103.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image104.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 27 27 Jan 2016

> ![](media/image105.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image106.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image107.jpeg){width="9.369444444444444in" height="3.0625in"}

> 7x7 input (spatially)
>
> assume 3x3 filter
>
> **=\> 5x5 output**

![](media/image108.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image109.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 28 27 Jan 2016

> ![](media/image110.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image111.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image112.jpeg){width="5.0in" height="2.0118055555555556in"}

> 7x7 input (spatially)

![](media/image113.jpeg){width="2.9583333333333335in"
height="3.0229166666666667in"}

> assume 3x3 filter
>
> applied **with stride 2**

![](media/image114.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image115.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 29 27 Jan 2016

> ![](media/image116.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image117.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image118.jpeg){width="5.0in" height="2.0118055555555556in"}

> 7x7 input (spatially)

![](media/image119.jpeg){width="2.9583333333333335in"
height="3.0229166666666667in"}

> assume 3x3 filter
>
> applied **with stride 2**

![](media/image120.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image121.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 30 27 Jan 2016

> ![](media/image122.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image123.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image124.jpeg){width="5.0in" height="2.0118055555555556in"}

> 7x7 input (spatially)

![](media/image125.jpeg){width="2.95in" height="3.0229166666666667in"}

> assume 3x3 filter
>
> applied **with stride 2**
>
> **=\> 3x3 output!**

![](media/image126.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image127.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 31 27 Jan 2016

> ![](media/image128.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image129.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image130.jpeg){width="5.0in" height="2.0118055555555556in"}

> 7x7 input (spatially)

![](media/image131.jpeg){width="2.9583333333333335in"
height="3.0229166666666667in"}

> assume 3x3 filter
>
> applied **with stride 3?**

![](media/image132.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

> 7

![](media/image133.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 32 27 Jan 2016

> ![](media/image134.jpeg){width="9.1875in"
> height="0.6888888888888889in"}

![](media/image135.jpeg){width="0.6277777777777778in"
height="0.5277777777777778in"}

> 7

![](media/image136.jpeg){width="5.0in" height="3.1118055555555557in"}

> 7x7 input (spatially)

![](media/image137.jpeg){width="2.9583333333333335in"
height="3.0229166666666667in"}

> assume 3x3 filter
>
> applied **with stride 3?**

![](media/image138.jpeg){width="0.6701388888888888in"
height="0.3402777777777778in"}

+---+------------------------------+
| 7 | > **doesn't fit!**           |
+---+------------------------------+
|   | > cannot apply 3x3 filter on |
+---+------------------------------+
|   | > 7x7 input with stride 3.   |
+---+------------------------------+

![](media/image139.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 33 27 Jan 2016

> ![](media/image140.jpeg){width="0.8743055555555556in"
> height="0.4583333333333333in"}

![](media/image141.jpeg){width="2.9479166666666665in"
height="5.208880139982502e-3in"}

> Output size:

![](media/image143.jpeg){width="5.208880139982502e-3in"
height="2.8381944444444445in"}

> **(N - F) / stride + 1**
>
> F
>
> e.g. N = 7, F = 3:

![](media/image145.jpeg){width="0.8743055555555556in"
height="0.4583333333333333in"}

> ^F^ ^N^ stride 1 =\> (7 - 3)/1 + 1 = 5
>
> stride 2 =\> (7 - 3)/2 + 1 = 3
>
> stride 3 =\> (7 - 3)/3 + 1 = 2.33 :\\

![](media/image146.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 34 27 Jan 2016

> ![](media/image147.jpeg){width="9.725in" height="4.696527777777778in"}
>
> 0 0 0 0 0 0
>
> 0
>
> 0
>
> 0
>
> 0

e.g. input 7x7

**3x3** filter, applied with **stride 1**

**pad with 1 pixel** border =\> what is the output?

> (recall:)
>
> (N - F) / stride + 1

![](media/image148.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 35 27 Jan 2016

> ![](media/image149.jpeg){width="9.725in" height="4.696527777777778in"}
>
> 0 0 0 0 0 0
>
> 0
>
> 0
>
> 0
>
> 0

e.g. input 7x7

**3x3** filter, applied with **stride 1**

**pad with 1 pixel** border =\> what is the output?

**7x7 output!**

![](media/image150.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 36 27 Jan 2016

![](media/image151.jpeg){width="9.725in" height="4.696527777777778in"}

> In practice: Common to zero pad the border
>
> 0 0 0 0 0 0
>
> 0
>
> 0
>
> 0
>
> 0

e.g. input 7x7

**3x3** filter, applied with **stride 1**

**pad with 1 pixel** border =\> what is the output?

**7x7 output!**

in general, common to see CONV layers with stride 1, filters of size
FxF, and zero-padding with (F-1)/2. (will preserve size spatially)

e.g. F = 3 =\> zero pad with 1

> F = 5 =\> zero pad with 2
>
> F = 7 =\> zero pad with 3

![](media/image152.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 37        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image153.jpeg){width="9.376388888888888in"
height="0.6854166666666667in"}

> **Remember back to...**
>
> E.g. 32x32 input convolved repeatedly with 5x5 filters shrinks volumes
> spatially! (32 -\> 28 -\> 24 \...). Shrinking too fast is not good,
> doesn't work well.

![](media/image154.jpeg){width="8.474305555555556in"
height="3.198611111111111in"}

> 32 28 24

![](media/image155.jpeg){width="1.073611111111111in"
height="0.41458333333333336in"}

> ....

![](media/image156.jpeg){width="1.0798611111111112in"
height="5.208880139982502e-3in"}

+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > CONV |        | > CONV |        | CONV,  |        |        |
|        | ,      |        | ,      |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > ReLU |        | > ReLU |        | ReLU   |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > e.g. |        | > e.g. |        |        |        |        |
|        | > 6    |        | > 10   |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 32     | > 5x5x | 28     | > 5x5x | 24     |        |        |        |
|        | 3      |        | **6**  |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > filt |        | > filt |        |        |        |        |
|        | ers    |        | ers    |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      |        | 6      |        | > 10   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| > Fei- | > Lect |        | > 27   |        |        |        |        |
| Fei    | ure    |        | > Jan  |        |        |        |        |
| > Li & | > 7 38 |        | > 2016 |        |        |        |        |
| > Andr |        |        |        |        |        |        |        |
| ej     |        |        |        |        |        |        |        |
| > Karp |        |        |        |        |        |        |        |
| athy   |        |        |        |        |        |        |        |
| > &    |        |        |        |        |        |        |        |
| > Just |        |        |        |        |        |        |        |
| in     |        |        |        |        |        |        |        |
| > John |        |        |        |        |        |        |        |
| son    |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

![](media/image159.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image160.jpeg){width="3.325in" height="0.8347222222222223in"}

> Examples time:

![](media/image163.jpeg){width="6.284722222222222in"
height="1.2131944444444445in"}

> Input volume: **32x32x3**
>
> 10 5x5 filters with stride 1, pad 2
>
> Output volume size: ?

![](media/image166.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 39        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image167.jpeg){width="9.677777777777777in"
height="2.5027777777777778in"}

> Examples time:

![](media/image168.jpeg){width="0.8055555555555556in"
height="5.208880139982502e-3in"}

> Input volume: **32x32x3**
>
> 10 5x5 filters with stride 1, pad 2
>
> Output volume size:
>
> (32+2\*2-5)/1+1 = 32 spatially, so **32x32x10**

![](media/image170.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 40        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image171.jpeg){width="9.677777777777777in"
height="2.5027777777777778in"}

> Examples time:

![](media/image172.jpeg){width="0.8055555555555556in"
height="5.208880139982502e-3in"}

> Input volume: **32x32x3**
>
> 10 5x5 filters with stride 1, pad 2
>
> Number of parameters in this layer?

![](media/image174.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 41        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image175.jpeg){width="9.677777777777777in"
height="2.5027777777777778in"}

> Examples time:

![](media/image176.jpeg){width="0.8055555555555556in"
height="5.208880139982502e-3in"}

> Input volume: **32x32x3**
>
> 10 5x5 filters with stride 1, pad 2
>
> Number of parameters in this layer?
>
> each filter has 5\*5\*3 + 1 = 76 params (+1 for bias) =\> 76\*10 =
> **760**

![](media/image177.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 42        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image178.jpeg){width="9.602777777777778in"
height="5.083333333333333in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 43        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image179.jpeg){width="9.006944444444445in"
> height="4.533333333333333in"}
>
> K = (powers of 2, e.g. 32, 64, 128, 512)

-   F = 3, S = 1, P = 1

-   F = 5, S = 1, P = 2

-   F = 5, S = 2, P = ? (whatever fits)

-   F = 1, S = 1, P = 0

![](media/image180.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 44 27 Jan 2016

> ![](media/image181.jpeg){width="9.323611111111111in"
> height="4.322916666666667in"}

+----+--------------------------+-------------------+--+--+
| 56 |                          | > 1x1 CONV        |  |  |
+----+--------------------------+-------------------+--+--+
|    |                          | > with 32 filters |  |  |
+----+--------------------------+-------------------+--+--+
|    |                          |                   |  |  |
+----+--------------------------+-------------------+--+--+
|    | > (each filter has size  |                   |  |  |
+----+--------------------------+-------------------+--+--+
|    | > 1x1x64, and performs a |                   |  |  |
+----+--------------------------+-------------------+--+--+
|    | > 64-dimensional dot     |                   |  |  |
+----+--------------------------+-------------------+--+--+
| 56 | > product)               |                   |  |  |
+----+--------------------------+-------------------+--+--+
| 64 | > 32                     |                   |  |  |
+----+--------------------------+-------------------+--+--+

![](media/image182.jpeg){width="10.0in" height="0.5888888888888889in"}

56

56

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 45 27 Jan 2016

> ![](media/image184.jpeg){width="2.9763888888888888in"
> height="1.051388888888889in"}

![](media/image185.jpeg){width="10.0in" height="5.456944444444445in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 46 27 Jan 2016

> ![](media/image187.jpeg){width="2.9763888888888888in"
> height="1.051388888888889in"}

![](media/image188.jpeg){width="10.0in" height="4.854166666666667in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 47 27 Jan 2016

> ![](media/image190.jpeg){width="10.0in" height="5.604166666666667in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 48 27 Jan 2016

![](media/image191.jpeg){width="9.293055555555556in"
height="4.669444444444444in"}

> The brain/neuron view of CONV Layer
>
> 32x32x3 image
>
> 5x5x3 filter
>
> 32

+-------------+-------------+-------------+-------------+-------------+
|             | > **1       |             |             |             |
|             | > number:** |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 32          | > the       |             |             |             |
|             | > result of |             |             |             |
|             | > taking a  |             |             |             |
|             | > dot       |             |             |             |
|             | > product   |             |             |             |
|             | > between   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 3           | > the       |             |             |             |
|             | > filter    |             |             |             |
|             | > and this  |             |             |             |
|             | > part of   |             |             |             |
|             | > the image |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > (i.e.     |             |             |             |
|             | > 5\*5\*3 = |             |             |             |
|             | > 75-dimens |             |             |             |
|             | ional       |             |             |             |
|             | > dot       |             |             |             |
|             | > product)  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > Fei-Fei   | > Lecture 7 | > 27 Jan    |             |             |
| > Li &      | > 49        | > 2016      |             |             |
| > Andrej    |             |             |             |             |
| > Karpathy  |             |             |             |             |
| > & Justin  |             |             |             |             |
| > Johnson   |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image192.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image193.jpeg){width="9.390972222222222in"
height="4.669444444444444in"}

> The brain/neuron view of CONV Layer
>
> 32x32x3 image
>
> 5x5x3 filter
>
> 32

+-------------+-------------+-------------+-------------+-------------+
|             |             | > It's just |             |             |
|             |             | > a neuron  |             |             |
|             |             | > with      |             |             |
|             |             | > local     |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **1       | > connectiv |             |             |
|             | > number:** | ity\...     |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 32          | > the       |             |             |             |
|             | > result of |             |             |             |
|             | > taking a  |             |             |             |
|             | > dot       |             |             |             |
|             | > product   |             |             |             |
|             | > between   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 3           | > the       |             |             |             |
|             | > filter    |             |             |             |
|             | > and this  |             |             |             |
|             | > part of   |             |             |             |
|             | > the image |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > (i.e.     |             |             |             |
|             | > 5\*5\*3 = |             |             |             |
|             | > 75-dimens |             |             |             |
|             | ional       |             |             |             |
|             | > dot       |             |             |             |
|             | > product)  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > Fei-Fei   | > Lecture 7 | > 27 Jan    |             |             |
| > Li &      | > 50        | > 2016      |             |             |
| > Andrej    |             |             |             |             |
| > Karpathy  |             |             |             |             |
| > & Justin  |             |             |             |             |
| > Johnson   |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image194.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image195.jpeg){width="9.807638888888889in"
height="4.446527777777778in"}

> The brain/neuron view of CONV Layer

32

> 32
>
> 3

+----+------------------------------------------------+
| 28 | > An activation map is a 28x28 sheet of neuron |
+----+------------------------------------------------+
|    | > outputs:                                     |
+----+------------------------------------------------+

1.  Each is connected to a small region in the input

2.  All of them share parameters

+----+----------------------------------------------------------+
| 28 | > "5x5 filter" -\> "5x5 receptive field for each neuron" |
+----+----------------------------------------------------------+

![](media/image196.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 51        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image197.jpeg){width="9.807638888888889in"
height="4.572222222222222in"}

> The brain/neuron view of CONV Layer
>
> 32
>
> E.g. with 5 filters,
>
> ^28^ CONV layer consists of
>
> neurons arranged in a 3D grid
>
> (28x28x5)

+-------------+-------------+-------------+-------------+-------------+
| 32          | 28          | > There     |             |             |
|             |             | > will be 5 |             |             |
|             |             | > different |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             | > neurons   |             |             |
|             |             | > all       |             |             |
|             |             | > looking   |             |             |
|             |             | > at the    |             |             |
|             |             | > same      |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 3           | 5           | > region in |             |             |
|             |             | > the input |             |             |
|             |             | > volume    |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Fei-Fei Li  | > Lecture 7 | > 27 Jan    |             |             |
| & Andrej    | > 52        | > 2016      |             |             |
| Karpathy &  |             |             |             |             |
| Justin      |             |             |             |             |
| Johnson     |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image198.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image199.jpeg){width="4.3284722222222225in"
height="0.14097222222222222in"}

![](media/image200.jpeg){width="10.0in" height="5.372222222222222in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 53 27 Jan 2016
>
> ![](media/image201.jpeg){width="9.663194444444445in"
> height="1.3923611111111112in"}

-   makes the representations smaller and more manageable

-   operates over each activation map independently:

![](media/image202.jpeg){width="10.0in" height="4.155555555555556in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 54 27 Jan 2016

> ![](media/image203.jpeg){width="4.694444444444445in"
> height="0.7520833333333333in"}

![](media/image204.jpeg){width="2.890277777777778in"
height="3.2354166666666666in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Single depth slice</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>x</td>
<td></td>
<td></td>
<td>1</td>
<td>1</td>
<td>2</td>
<td>4</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td>5</td>
<td>6</td>
<td>7</td>
<td>8</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td>3</td>
<td>2</td>
<td>1</td>
<td>0</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td>1</td>
<td>2</td>
<td>3</td>
<td>4</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image205.jpeg){width="5.208880139982502e-3in"
height="2.5854166666666667in"}

max pool with 2x2 filters and stride 2

![](media/image209.jpeg){width="2.222916666666667in"
height="5.208880139982502e-3in"}

-   8

> 3 4

![](media/image211.jpeg){width="1.3527777777777779in"
height="1.3527777777777779in"}

> y

![](media/image212.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 55 27 Jan 2016

![](media/image213.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 56        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image215.jpeg){width="3.3409722222222222in"
> height="3.453472222222222in"}

![](media/image216.jpeg){width="5.871527777777778in"
height="2.611111111111111in"}

> F = 2, S = 2
>
> F = 3, S = 2

![](media/image217.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 57 27 Jan 2016

> ![](media/image218.jpeg){width="9.663194444444445in"
> height="1.3923611111111112in"}

-   Contains neurons that connect to the entire input volume, as in
    > ordinary Neural Networks

![](media/image219.jpeg){width="10.0in" height="4.0625in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 58 27 Jan 2016

> ![](media/image220.jpeg){width="8.928472222222222in"
> height="2.5944444444444446in"}
>
> [[http://cs.stanford.edu/people/karpathy/convnetjs/demo/cifar10.html]{.underline}](http://cs.stanford.edu/people/karpathy/convnetjs/demo/cifar10.html)

![](media/image221.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 59 27 Jan 2016

![](media/image222.jpeg){width="8.627777777777778in"
height="1.1430555555555555in"}

> \[LeCun et al., 1998\]

![](media/image223.jpeg){width="9.48263888888889in"
height="3.0215277777777776in"}

> Conv filters were 5x5, applied at stride 1
>
> Subsampling (Pooling) layers were 2x2 applied at stride 2 i.e.
> architecture is \[CONV-POOL-CONV-POOL-CONV-FC\]

![](media/image224.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 60 27 Jan 2016
>
> ![](media/image225.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image226.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> **First layer** (CONV1): 96 11x11 filters applied at stride 4 =\>
>
> Q: what is the output volume size? Hint: (227-11)/4+1 = 55

![](media/image227.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 61 27 Jan 2016

> ![](media/image228.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image229.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> **First layer** (CONV1): 96 11x11 filters applied at stride 4 =\>
>
> Output volume **\[55x55x96\]**
>
> Q: What is the total number of parameters in this layer?

![](media/image230.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 62 27 Jan 2016

> ![](media/image231.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image232.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> **First layer** (CONV1): 96 11x11 filters applied at stride 4 =\>
>
> Output volume **\[55x55x96\]**
>
> Parameters: (11\*11\*3)\*96 = **35K**

![](media/image233.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 63 27 Jan 2016

> ![](media/image234.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image235.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> After CONV1: 55x55x96
>
> **Second layer** (POOL1): 3x3 filters applied at stride 2
>
> Q: what is the output volume size? Hint: (55-3)/2+1 = 27

![](media/image236.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 64 27 Jan 2016

> ![](media/image237.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image238.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> After CONV1: 55x55x96
>
> **Second layer** (POOL1): 3x3 filters applied at stride 2
>
> Output volume: 27x27x96
>
> Q: what is the number of parameters in this layer?

![](media/image239.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 65 27 Jan 2016

> ![](media/image240.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image241.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> After CONV1: 55x55x96
>
> **Second layer** (POOL1): 3x3 filters applied at stride 2
>
> Output volume: 27x27x96
>
> Parameters: 0!

![](media/image242.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 66 27 Jan 2016

> ![](media/image243.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image244.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> After CONV1: 55x55x96
>
> After POOL1: 27x27x96
>
> \...

![](media/image245.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 67 27 Jan 2016

> ![](media/image246.jpeg){width="9.830555555555556in"
> height="2.451388888888889in"}
>
> *\[Krizhevsky et al. 2012\]*
>
> Full (simplified) AlexNet architecture:
>
> \[227x227x3\] INPUT
>
> \[55x55x96\] CONV1: 96 11x11 filters at stride 4, pad 0
>
> \[27x27x96\] MAX POOL1: 3x3 filters at stride 2
>
> \[27x27x96\] NORM1: Normalization layer
>
> \[27x27x256\] CONV2: 256 5x5 filters at stride 1, pad 2
>
> \[13x13x256\] MAX POOL2: 3x3 filters at stride 2
>
> \[13x13x256\] NORM2: Normalization layer
>
> \[13x13x384\] CONV3: 384 3x3 filters at stride 1, pad 1
>
> \[13x13x384\] CONV4: 384 3x3 filters at stride 1, pad 1
>
> \[13x13x256\] CONV5: 256 3x3 filters at stride 1, pad 1
>
> \[6x6x256\] MAX POOL3: 3x3 filters at stride 2
>
> \[4096\] FC6: 4096 neurons
>
> \[4096\] FC7: 4096 neurons
>
> \[1000\] FC8: 1000 neurons (class scores)

![](media/image247.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 68 27 Jan 2016

> ![](media/image248.jpeg){width="9.911805555555556in"
> height="4.4125in"}
>
> *\[Krizhevsky et al. 2012\]*
>
> Full (simplified) AlexNet architecture:
>
> \[227x227x3\] INPUT
>
> \[55x55x96\] CONV1: 96 11x11 filters at stride 4, pad 0
>
> \[27x27x96\] MAX POOL1: 3x3 filters at stride 2
>
> \[27x27x96\] NORM1: Normalization layer
>
> \[27x27x256\] CONV2: 256 5x5 filters at stride 1, pad 2
>
> \[13x13x256\] MAX POOL2: 3x3 filters at stride 2
>
> \[13x13x256\] NORM2: Normalization layer
>
> \[13x13x384\] CONV3: 384 3x3 filters at stride 1, pad 1
>
> \[13x13x384\] CONV4: 384 3x3 filters at stride 1, pad 1
>
> \[13x13x256\] CONV5: 256 3x3 filters at stride 1, pad 1
>
> \[6x6x256\] MAX POOL3: 3x3 filters at stride 2
>
> \[4096\] FC6: 4096 neurons
>
> \[4096\] FC7: 4096 neurons
>
> \[1000\] FC8: 1000 neurons (class scores)

![](media/image249.jpeg){width="10.0in" height="0.5888888888888889in"}

**Details/Retrospectives:**

-   first use of ReLU

-   used Norm layers (not common anymore)

-   heavy data augmentation

-   dropout 0.5

-   batch size 128

-   SGD Momentum 0.9

-   Learning rate 1e-2, reduced by 10 manually when val accuracy
    plateaus

-   L2 weight decay 5e-4

-   7 CNN ensemble: 18.2% -\> 15.4%

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 69 27 Jan 2016

![](media/image250.jpeg){width="9.76875in"
height="3.0368055555555555in"}

+-------------------+---------------------------------+--+
| Case Study: ZFNet | > *\[Zeiler and Fergus, 2013\]* |  |
+-------------------+---------------------------------+--+
|                   |                                 |  |
+-------------------+---------------------------------+--+

![](media/image251.jpeg){width="9.50625in"
height="1.4590277777777778in"}

> AlexNet but:
>
> CONV1: change from (11x11 stride 4) to (7x7 stride 2)
>
> CONV3,4,5: instead of 384, 384, 256 filters use 512, 1024, 512
>
> ImageNet top 5 error: 15.4% -\> 14.8%

![](media/image252.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 70        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image253.jpeg){width="9.827083333333333in" height="5.625in"}

> Case Study: VGGNet
>
> *\[Simonyan and Zisserman, 2014\]*
>
> Only 3x3 CONV stride 1, pad 1 and 2x2 MAX POOL stride 2
>
> best model
>
> 11.2% top 5 error in ILSVRC 2013 -\>
>
> 7.3% top 5 error

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 71        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image254.jpeg){width="9.719444444444445in"
height="4.968055555555556in"}

+-----------------+-----------------+-----------------+-----------------+
| INPUT:          | > memory:       | > params: 0     | (not counting   |
| \[224x224x3\]   | > 224\*224\*3=1 |                 | biases)         |
|                 | 50K             |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*3)\*64 |                 |                 |
| memory:         | > = 1,728       |                 |                 |
| 224\*224\*64=3. |                 |                 |                 |
| 2M              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*64)\*6 |                 |                 |
| memory:         | 4               |                 |                 |
| 224\*224\*64=3. | > = 36,864      |                 |                 |
| 2M              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[112x112x64\]  |                 |                 |                 |
| memory:         |                 |                 |                 |
| 112\*112\*64=80 |                 |                 |                 |
| 0K              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*64)\*128 |                 |                 |
| memory:         | = 73,728        |                 |                 |
| 112\*112\*128=1 |                 |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*128)\*12 |                 |                 |
| memory:         | 8               |                 |                 |
| 112\*112\*128=1 | = 147,456       |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[56x56x128\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 56\*56\*128=400 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*128)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 294,912     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[28x28x256\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 28\*28\*256=200 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 1,179,648   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[14x14x512\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 14\*14\*512=100 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          |                 |                 |                 |
| \[7x7x512\]     |                 |                 |                 |
| memory:         |                 |                 |                 |
| 7\*7\*512=25K   |                 |                 |                 |
| params: 0       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

> FC: \[1x1x4096\] memory: 4096 params: 7\*7\*512\*4096 = 102,760,448
>
> FC: \[1x1x4096\] memory: 4096 params: 4096\*4096 = 16,777,216
>
> FC: \[1x1x1000\] memory: 1000 params: 4096\*1000 = 4,096,000

![](media/image255.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 72 27 Jan 2016

+-----------------+-----------------+-----------------+-----------------+
| INPUT:          | > memory:       | > params: 0     | (not counting   |
| \[224x224x3\]   | > 224\*224\*3=1 |                 | biases)         |
|                 | 50K             |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*3)\*64 |                 |                 |
| memory:         | > = 1,728       |                 |                 |
| 224\*224\*64=3. |                 |                 |                 |
| 2M              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*64)\*6 |                 |                 |
| memory:         | 4               |                 |                 |
| 224\*224\*64=3. | > = 36,864      |                 |                 |
| 2M              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[112x112x64\]  |                 |                 |                 |
| memory:         |                 |                 |                 |
| 112\*112\*64=80 |                 |                 |                 |
| 0K              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*64)\*128 |                 |                 |
| memory:         | = 73,728        |                 |                 |
| 112\*112\*128=1 |                 |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*128)\*12 |                 |                 |
| memory:         | 8               |                 |                 |
| 112\*112\*128=1 | = 147,456       |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[56x56x128\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 56\*56\*128=400 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*128)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 294,912     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[28x28x256\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 28\*28\*256=200 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 1,179,648   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[14x14x512\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 14\*14\*512=100 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          |                 |                 |                 |
| \[7x7x512\]     |                 |                 |                 |
| memory:         |                 |                 |                 |
| 7\*7\*512=25K   |                 |                 |                 |
| params: 0       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

> ![](media/image256.jpeg){width="9.719444444444445in"
> height="4.968055555555556in"}memory: 4096 params: 7\*7\*512\*4096 =
> 102,760,448
>
> FC: \[1x1x4096\] memory: 4096 params: 4096\*4096 = 16,777,216
>
> FC: \[1x1x1000\] memory: 1000 params: 4096\*1000 = 4,096,000
>
> TOTAL memory: 24M \* 4 bytes \~= 93MB / image (only forward! \~\*2 for
> bwd)
>
> TOTAL params: 138M parameters

![](media/image257.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 73 27 Jan 2016

+-----------------+-----------------+-----------------+-----------------+
| INPUT:          | > memory:       | > params: 0     | (not counting   |
| \[224x224x3\]   | > 224\*224\*3=1 |                 | biases)         |
|                 | 50K             |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*3)\*64 |                 |                 |
| memory:         | > = 1,728       |                 |                 |
| **224\*224\*64= |                 |                 |                 |
| 3.2M**          |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-64:       | > params:       |                 |                 |
| \[224x224x64\]  | > (3\*3\*64)\*6 |                 |                 |
| memory:         | 4               |                 |                 |
| **224\*224\*64= | > = 36,864      |                 |                 |
| 3.2M**          |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[112x112x64\]  |                 |                 |                 |
| memory:         |                 |                 |                 |
| 112\*112\*64=80 |                 |                 |                 |
| 0K              |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*64)\*128 |                 |                 |
| memory:         | = 73,728        |                 |                 |
| 112\*112\*128=1 |                 |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-128:      | params:         |                 |                 |
| \[112x112x128\] | (3\*3\*128)\*12 |                 |                 |
| memory:         | 8               |                 |                 |
| 112\*112\*128=1 | = 147,456       |                 |                 |
| .6M             |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[56x56x128\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 56\*56\*128=400 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*128)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 294,912     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-256:      | > params:       |                 |                 |
| \[56x56x256\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 256             |                 |                 |
| 56\*56\*256=800 | > = 589,824     |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[28x28x256\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 28\*28\*256=200 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*256)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 1,179,648   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[28x28x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 28\*28\*512=400 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          | > params: 0     |                 |                 |
| \[14x14x512\]   |                 |                 |                 |
| memory:         |                 |                 |                 |
| 14\*14\*512=100 |                 |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| CONV3-512:      | > params:       |                 |                 |
| \[14x14x512\]   | > (3\*3\*512)\* |                 |                 |
| memory:         | 512             |                 |                 |
| 14\*14\*512=100 | > = 2,359,296   |                 |                 |
| K               |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| POOL2:          |                 |                 |                 |
| \[7x7x512\]     |                 |                 |                 |
| memory:         |                 |                 |                 |
| 7\*7\*512=25K   |                 |                 |                 |
| params: 0       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

> ![](media/image258.jpeg){width="9.8875in"
> height="4.968055555555556in"}memory: 4096 params: 7\*7\*512\*4096 =
> **102,760,448**
>
> FC: \[1x1x4096\] memory: 4096 params: 4096\*4096 = 16,777,216
>
> FC: \[1x1x1000\] memory: 1000 params: 4096\*1000 = 4,096,000
>
> TOTAL memory: 24M \* 4 bytes \~= 93MB / image (only forward! \~\*2 for
> bwd)
>
> TOTAL params: 138M parameters

![](media/image259.jpeg){width="10.0in" height="0.5888888888888889in"}

Note:

Most memory is in early CONV

Most params are in late FC

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 74 27 Jan 2016

![](media/image260.jpeg){width="10.0in" height="5.552083333333333in"}

+-----------------------+------------------------------+--+
| Case Study: GoogLeNet | > *\[Szegedy et al., 2014\]* |  |
+-----------------------+------------------------------+--+
|                       |                              |  |
+-----------------------+------------------------------+--+

> Inception module
>
> ILSVRC 2014 winner (6.7% top 5 error)

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 75        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image261.jpeg){width="9.840277777777779in"
> height="4.618055555555555in"}
>
> Fun features:
>
> \- Only 5 million params! (Removes FC layers completely)
>
> **Compared to AlexNet:**
>
> \- 12X less params
>
> \- 2x more compute - 6.67% (vs. 16.4%)

![](media/image262.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 76 27 Jan 2016

> ![](media/image263.jpeg){width="8.847916666666666in"
> height="4.4319444444444445in"}*\[He et al., 2015\]*

ILSVRC 2015 winner (3.6% top 5 error)

![](media/image264.jpeg){width="8.675in" height="0.4583333333333333in"}

> Slide from Kaiming He's recent presentation
> [[https://www.youtube.com/watch?v=1PGLj-uKT1w]{.underline}](https://www.youtube.com/watch?v=1PGLj-uKT1w)

![](media/image265.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 77 27 Jan 2016

![](media/image266.jpeg){width="8.909722222222221in"
height="4.825694444444444in"}

> (slide from Kaiming He's recent presentation)

![](media/image267.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 78 27 Jan 2016

![](media/image268.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 7 79        | > 27 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image270.jpeg){width="9.136805555555556in"
> height="4.924305555555556in"}*\[He et al., 2015\]*
>
> ILSVRC 2015 winner (3.6% top 5 error)
>
> 2-3 weeks of training on 8 GPU machine
>
> at runtime: faster than a VGGNet! (even though it has 8x more layers)
>
> (slide from Kaiming He's recent presentation)

![](media/image271.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 80 27 Jan 2016

> ![](media/image272.jpeg){width="9.870138888888889in"
> height="4.813888888888889in"}

+-----------------------+---------------------+--+
| ResNet                | > 224x224x3         |  |
+-----------------------+---------------------+--+
|                       | > spatial dimension |  |
+-----------------------+---------------------+--+
| *\[He et al., 2015\]* |                     |  |
+-----------------------+---------------------+--+
|                       | > only 56x56!       |  |
+-----------------------+---------------------+--+
|                       |                     |  |
+-----------------------+---------------------+--+

![](media/image273.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 81 27 Jan 2016

+--------------------+-------------------------+--+
| Case Study: ResNet | > *\[He et al., 2015\]* |  |
+--------------------+-------------------------+--+
|                    |                         |  |
+--------------------+-------------------------+--+

![](media/image274.jpeg){width="8.675in" height="1.1118055555555555in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 82 27 Jan 2016

+--------------------+-------------------------+--+
| Case Study: ResNet | > *\[He et al., 2015\]* |  |
+--------------------+-------------------------+--+
|                    |                         |  |
+--------------------+-------------------------+--+

![](media/image277.jpeg){width="9.639583333333333in"
height="4.458333333333333in"}

-   Batch Normalization after every CONV layer

-   Xavier/2 initialization from He et al.

-   SGD + Momentum (0.9)

-   Learning rate: 0.1, divided by 10 when validation error plateaus

-   Mini-batch size 256

-   Weight decay of 1e-5

-   No dropout used

![](media/image278.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 83 27 Jan 2016

+--------------------+-------------------------+--+
| Case Study: ResNet | > *\[He et al., 2015\]* |  |
+--------------------+-------------------------+--+
|                    |                         |  |
+--------------------+-------------------------+--+

![](media/image279.jpeg){width="8.675in" height="4.104861111111111in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 84 27 Jan 2016

> ![](media/image281.jpeg){width="8.675in"
> height="1.1118055555555555in"} *\[He et al., 2015\]*

![](media/image282.jpeg){width="7.832638888888889in"
height="3.234722222222222in"}

> (this trick is also used in GoogLeNet)

![](media/image283.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 85 27 Jan 2016

> ![](media/image284.jpeg){width="10.0in" height="5.625in"}*\[He et al.,
> 2015\]*

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 86 27 Jan 2016

> ![](media/image285.jpeg){width="8.675in"
> height="1.1118055555555555in"}

![](media/image286.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 87 27 Jan 2016

![](media/image288.jpeg){width="9.527777777777779in"
height="4.738888888888889in"}

> **policy network:**
>
> \[19x19x48\] Input
>
> CONV1: 192 5x5 filters , stride 1, pad 2 =\> \[19x19x192\]
>
> CONV2..12: 192 3x3 filters, stride 1, pad 1 =\> \[19x19x192\]
>
> CONV: 1 1x1 filter, stride 1, pad 0 =\> \[19x19\] *(probability map of
> promising moves)*

![](media/image289.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 88 27 Jan 2016

> ![](media/image290.jpeg){width="9.264583333333333in"
> height="4.401388888888889in"}

-   ConvNets stack CONV,POOL,FC layers

-   Trend towards smaller filters and deeper architectures

-   Trend towards getting rid of POOL/FC layers (just CONV)

-   Typical architectures look like

> **\[(CONV-RELU)\*N-POOL?\]\*M-(FC-RELU)\*K,SOFTMAX** where N is
> usually up to \~5, M is large, 0 \<= K \<= 2.

-   but recent advances such as ResNet/GoogLeNet challenge this paradigm

![](media/image291.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 7 89 27 Jan 2016
