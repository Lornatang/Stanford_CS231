![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Lecture 3:

Loss functions and

Optimization

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 1 11 Jan 2016

> ![](media/image3.jpeg){width="8.472222222222221in"
> height="4.243055555555555in"}
>
> A1 is due Jan 20 (Wednesday). \~9 days left
>
> Warning: Jan 18 (Monday) is Holiday (no class/office hours)

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 2 11 Jan 2016

![](media/image5.jpeg){width="9.70625in"
height="0.8958333333333334in"}Challenges in Visual Recognition

> Camera pose Illumination Deformation Occlusion

![](media/image6.jpeg){width="8.804166666666667in" height="1.525in"}

> ~Background\ clutter~ Intraclass variation

![](media/image7.jpeg){width="10.0in" height="2.7104166666666667in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 3 11 Jan 2016

> ![](media/image8.jpeg){width="9.734027777777778in"
> height="4.685416666666667in"} data-driven approach, kNN
>
> the data NN classifier 5-NN classifier

![](media/image9.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 4 11 Jan 2016

> ![](media/image10.jpeg){width="9.4in" height="2.202777777777778in"}
> Linear classifier

+------------------+------------------------------+
| image parameters | > **10** numbers, indicating |
+------------------+------------------------------+
| > f(**x**,**W**) | > class scores               |
+------------------+------------------------------+

> **\[32x32x3\]**

![](media/image11.jpeg){width="3.7493055555555554in"
height="5.208880139982502e-3in"}

> array of numbers 0\...1

![](media/image12.jpeg){width="2.825in" height="2.079861111111111in"}

> (3072 numbers total)

![](media/image13.jpeg){width="10.0in" height="2.553472222222222in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 5 11 Jan 2016

> ![](media/image15.jpeg){width="10.0in"
> height="5.559722222222222in"}Going forward: Loss function/Optimization

![](media/image16.jpeg){width="5.208880139982502e-3in"
height="4.0055555555555555in"}

> -3.45 -0.51 3.42
>
> ^-8.87^ **6.04** 4.64
>
> ^0.09^ 5.31 2.65
>
> **^2.9^** -4.22 5.1
>
> ^4.48^ -4.19 2.64
>
> ^8.02^ 3.58 5.55
>
> ^3.78^ 4.49 **-4.34**
>
> ^1.06^ -4.37 -1.5
>
> ^-0.36^ -2.09 -4.79
>
> ^-0.72^ -2.93 6.14

TODO:

1.  Define a **loss function** that quantifies our unhappiness with the
    > scores across the training data.

2.  Come up with a way of efficiently finding the parameters that
    > minimize the loss function.

> **(optimization)**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 6 11 Jan 2016

> ![](media/image17.jpeg){width="8.20138888888889in"
> height="0.4166666666666667in"}
>
> With some W the scores ![](media/image18.jpeg){width="1.6125in"
> height="0.3125in"} are:

![](media/image19.jpeg){width="6.104861111111111in"
height="1.9305555555555556in"}

> cat

![](media/image20.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image21.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog
>
> **3.2** 1.3 2.2

![](media/image22.jpeg){width="4.435416666666667in"
height="0.4166666666666667in"}

> 5.1 **4.9** 2.5

![](media/image23.jpeg){width="4.352083333333334in"
height="0.4166666666666667in"}

-1.7 2.0 **-3.1**

![](media/image24.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 7 11 Jan 2016

> ![](media/image25.jpeg){width="9.870833333333334in"
> height="4.8694444444444445in"}
>
> With some W the scores ![](media/image26.jpeg){width="1.6125in"
> height="0.3125in"} are:

  ------ --------- --------- ----------
  cat    **3.2**   1.3       2.2
  car    5.1       **4.9**   2.5
  frog   -1.7      2.0       **-3.1**
  ------ --------- --------- ----------

![](media/image27.jpeg){width="10.0in" height="0.5888888888888889in"}

**Multiclass SVM loss:**

![](media/image28.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

> Given an example
>
> where is the image and where
> ![](media/image29.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image30.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}

the SVM loss has the form:

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 8 11 Jan 2016

![](media/image31.jpeg){width="9.9in" height="4.8694444444444445in"}

> Suppose: 3 training examples, 3 classes.
>
> With some W the scores ![](media/image32.jpeg){width="1.6125in"
> height="0.3125in"} are:

+---------+-----+---------+----------+--+
| > cat   |     | 1.3     | 2.2      |  |
+---------+-----+---------+----------+--+
| > car   |     | **4.9** | 2.5      |  |
+---------+-----+---------+----------+--+
| > frog  | 2.9 | 2.0     | **-3.1** |  |
+---------+-----+---------+----------+--+
| Losses: |     |         |          |  |
+---------+-----+---------+----------+--+

![](media/image33.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson

**Multiclass SVM loss:**

![](media/image34.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

> Given an example
>
> where is the image and where
> ![](media/image35.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image36.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}

the SVM loss has the form:

-   max(0, 5.1 - 3.2 + 1) +max(0, -1.7 - 3.2 + 1)

-   max(0, 2.9) + max(0, -3.9)

-   2.9 + 0

-   2.9

+-------------+---------------+
| Lecture 3 9 | > 11 Jan 2016 |
+-------------+---------------+
|             |               |
+-------------+---------------+

![](media/image37.jpeg){width="9.9in" height="4.8694444444444445in"}

> Suppose: 3 training examples, 3 classes.
>
> With some W the scores ![](media/image38.jpeg){width="1.6125in"
> height="0.3125in"} are:

+---------+---------+---+----------+
| > cat   | **3.2** |   | 2.2      |
+---------+---------+---+----------+
| > car   | 5.1     |   | 2.5      |
+---------+---------+---+----------+
| > frog  | -1.7    |   | **-3.1** |
+---------+---------+---+----------+
| Losses: | 2.9     | 0 |          |
+---------+---------+---+----------+

![](media/image39.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson

**Multiclass SVM loss:**

![](media/image40.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

> Given an example
>
> where is the image and where
> ![](media/image41.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image42.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}

the SVM loss has the form:

-   max(0, 1.3 - 4.9 + 1) +max(0, 2.0 - 4.9 + 1)

-   max(0, -2.6) + max(0, -1.9)

-   0 + 0

-   0

+--------------+---------------+
| Lecture 3 10 | > 11 Jan 2016 |
+--------------+---------------+
|              |               |
+--------------+---------------+

![](media/image43.jpeg){width="9.9in" height="4.8694444444444445in"}

> Suppose: 3 training examples, 3 classes.
>
> With some W the scores ![](media/image44.jpeg){width="1.6125in"
> height="0.3125in"} are:

+---------+---------+---------+------+--+
| > cat   | **3.2** | 1.3     |      |  |
+---------+---------+---------+------+--+
| > car   | 5.1     | **4.9** |      |  |
+---------+---------+---------+------+--+
| > frog  | -1.7    | 2.0     | 10.9 |  |
+---------+---------+---------+------+--+
| Losses: | 2.9     | 0       |      |  |
+---------+---------+---------+------+--+

![](media/image45.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> **Multiclass SVM loss:**

![](media/image46.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

> Given an example
>
> where is the image and where
> ![](media/image47.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image48.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:

-   max(0, 2.2 - (-3.1) + 1) +max(0, 2.5 - (-3.1) + 1)

-   max(0, 5.3) + max(0, 5.6)

-   5.3 + 5.6

-   10.9

+--------------+---------------+
| Lecture 3 11 | > 11 Jan 2016 |
+--------------+---------------+
|              |               |
+--------------+---------------+

> ![](media/image49.jpeg){width="9.9in" height="4.8694444444444445in"}
>
> With some W the scores ![](media/image50.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image51.jpeg){width="10.0in" height="0.5888888888888889in"}

> **Multiclass SVM loss:**

![](media/image52.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

> Given an example
>
> where is the image and where
> ![](media/image53.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image54.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:
>
> and the full training loss is the mean over all examples in the
> training data:

L = (2.9 + 0 + 10.9)/3

-   **4.6**

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 12 11 Jan 2016
>
> ![](media/image55.jpeg){width="5.208880139982502e-3in"
> height="4.855555555555555in"}
>
> With some W the scores ![](media/image57.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image58.jpeg){width="10.0in" height="0.5888888888888889in"}

**Multiclass SVM loss:**

> Given an example
>
> where is the image and where
> ![](media/image59.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image60.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:

Q.  what if the sum was instead over all classes?

> (including j = y\_i)
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 13 11 Jan 2016
>
> ![](media/image61.jpeg){width="5.208880139982502e-3in"
> height="4.855555555555555in"}
>
> With some W the scores ![](media/image63.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image64.jpeg){width="10.0in" height="0.5888888888888889in"}

**Multiclass SVM loss:**

> Given an example
>
> where is the image and where
> ![](media/image65.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image66.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:
>
> Q2: what if we used a mean instead of a sum here?
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 14 11 Jan 2016
>
> ![](media/image67.jpeg){width="5.208880139982502e-3in"
> height="4.855555555555555in"}
>
> With some W the scores ![](media/image69.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image70.jpeg){width="10.0in" height="0.5888888888888889in"}

**Multiclass SVM loss:**

> Given an example
>
> where is the image and where
> ![](media/image71.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image72.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:
>
> Q3: what if we used
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 15 11 Jan 2016
>
> ![](media/image73.jpeg){width="5.208880139982502e-3in"
> height="4.855555555555555in"}
>
> With some W the scores ![](media/image75.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image76.jpeg){width="10.0in" height="0.5888888888888889in"}

**Multiclass SVM loss:**

> Given an example
>
> where is the image and where
> ![](media/image77.jpeg){width="0.2902777777777778in"
> height="0.2916666666666667in"} is the (integer) label,
>
> and using the shorthand for the scores vector:
> ![](media/image78.jpeg){width="1.229861111111111in"
> height="0.23958333333333334in"}
>
> the SVM loss has the form:
>
> Q4: what is the min/max possible loss?
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 16 11 Jan 2016
>
> ![](media/image79.jpeg){width="9.9in" height="4.8694444444444445in"}
>
> With some W the scores ![](media/image80.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---------+----------+
| > cat     | **3.2** | 1.3     | 2.2      |
+-----------+---------+---------+----------+
| > car     | 5.1     | **4.9** | 2.5      |
+-----------+---------+---------+----------+
| > frog    | -1.7    | 2.0     | **-3.1** |
+-----------+---------+---------+----------+
|           |         |         |          |
+-----------+---------+---------+----------+
| > Losses: | 2.9     | 0       | 10.9     |
+-----------+---------+---------+----------+

![](media/image81.jpeg){width="10.0in" height="0.5888888888888889in"}

> **Multiclass SVM loss:**

![](media/image82.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

Given an example

where the image and

where ![](media/image83.jpeg){width="0.2902777777777778in"
height="0.3125in"} the (integer) label,

and using the shorthand for the scores vector:
![](media/image84.jpeg){width="1.229861111111111in"
height="0.23958333333333334in"}

the SVM loss has the form:

Q5: usually at initialization W are small numbers, so all s \~= 0. What
is the loss?

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 17 11 Jan 2016
>
> ![](media/image85.jpeg){width="5.9625in"
> height="0.5368055555555555in"}

![](media/image86.jpeg){width="10.0in" height="4.602083333333334in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 18 11 Jan 2016

![](media/image87.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 19        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image90.jpeg){width="8.991666666666667in"
> height="1.961111111111111in"}

![](media/image91.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 20 11 Jan 2016

> ![](media/image92.jpeg){width="8.991666666666667in"
> height="1.961111111111111in"}

![](media/image93.jpeg){width="9.36736111111111in"
height="2.270138888888889in"}

> E.g. Suppose that we found a W such that L = 0. Is this W unique?

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 21 11 Jan 2016

> ![](media/image95.jpeg){width="6.134027777777778in"
> height="4.8694444444444445in"}
>
> With some W the scores ![](media/image96.jpeg){width="1.6125in"
> height="0.3125in"} are:

+-----------+---------+---+----------+
| > cat     | **3.2** |   | 2.2      |
+-----------+---------+---+----------+
| > car     | 5.1     |   | 2.5      |
+-----------+---------+---+----------+
| > frog    | -1.7    |   | **-3.1** |
+-----------+---------+---+----------+
|           |         |   |          |
+-----------+---------+---+----------+
| > Losses: | 2.9     | 0 |          |
+-----------+---------+---+----------+

![](media/image97.jpeg){width="10.0in" height="0.5888888888888889in"}

**Before:**

![](media/image98.jpeg){width="5.208880139982502e-3in"
height="4.855555555555555in"}

-   max(0, 1.3 - 4.9 + 1) +max(0, 2.0 - 4.9 + 1)

-   max(0, -2.6) + max(0, -1.9)

-   0 + 0

-   0

![](media/image100.jpeg){width="3.520138888888889in"
height="1.5305555555555554in"}

**With W twice as large:**

-   max(0, 2.6 - 9.8 + 1) +max(0, 4.0 - 9.8 + 1)

-   max(0, -6.2) + max(0, -4.8)

-   0 + 0

-   0

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 22 11 Jan 2016
>
> Weight Regularization

![](media/image101.jpeg){width="9.027777777777779in"
height="1.0472222222222223in"}

\\lambda = regularization strength (hyperparameter)

![](media/image102.jpeg){width="9.830555555555556in"
height="1.492361111111111in"}

> In common use:
>
> **L2 regularization**
>
> L1 regularization
> ![](media/image103.jpeg){width="2.8152777777777778in"
> height="0.4270833333333333in"} Elastic net (L1 + L2)
> ![](media/image104.jpeg){width="4.163194444444445in"
> height="0.4791666666666667in"} Max norm regularization (might see
> later) Dropout (will see later)

![](media/image105.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 23 11 Jan 2016

> ![](media/image106.jpeg){width="8.688194444444445in"
> height="0.7340277777777777in"}

![](media/image107.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 24 11 Jan 2016

> ![](media/image111.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image112.jpeg){width="3.0215277777777776in"
height="1.9305555555555556in"}

> cat

![](media/image113.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image114.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog
>
> **3.2**

![](media/image115.jpeg){width="1.3520833333333333in"
height="0.4166666666666667in"}

> 5.1

![](media/image116.jpeg){width="1.3520833333333333in"
height="0.4166666666666667in"}

-1.7

![](media/image117.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 25 11 Jan 2016

> ![](media/image118.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image119.jpeg){width="9.782638888888888in"
height="3.7159722222222222in"}

**scores = unnormalized log probabilities of the classes.**

> cat
>
> car
>
> frog
>
> **3.2**
>
> 5.1

-1.7

![](media/image120.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 26 11 Jan 2016

> ![](media/image121.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image122.jpeg){width="9.782638888888888in"
height="3.7159722222222222in"}

**scores = unnormalized log probabilities of the classes.**

> where
>
> cat
>
> car
>
> frog
>
> **3.2**
>
> 5.1

-1.7

![](media/image123.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 27 11 Jan 2016

> ![](media/image124.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image125.jpeg){width="9.782638888888888in"
height="3.7159722222222222in"}

**scores = unnormalized log probabilities of the classes.**

> where
>
> cat
>
> car
>
> frog
>
> **3.2**
>
> 5.1

-1.7

Softmax function

![](media/image126.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 28 11 Jan 2016

> ![](media/image127.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image128.jpeg){width="9.782638888888888in"
height="3.7159722222222222in"}

> cat
>
> car
>
> frog

**scores = unnormalized log probabilities of the classes.**

+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       | > whe |       |       |       |       |
|       |       |       |       | re    |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| **3.2 | > Wan |       |       |       |       |       |       |       |
| **    | t     |       |       |       |       |       |       |       |
|       | > to  |       |       |       |       |       |       |       |
|       | > max |       |       |       |       |       |       |       |
|       | imize |       |       |       |       |       |       |       |
|       | > the |       |       |       |       |       |       |       |
|       | > log |       |       |       |       |       |       |       |
|       | > lik |       |       |       |       |       |       |       |
|       | eliho |       |       |       |       |       |       |       |
|       | od,   |       |       |       |       |       |       |       |
|       | > or  |       |       |       |       |       |       |       |
|       | > (fo |       |       |       |       |       |       |       |
|       | r     |       |       |       |       |       |       |       |
|       | > a   |       |       |       |       |       |       |       |
|       | > los |       |       |       |       |       |       |       |
|       | s     |       |       |       |       |       |       |       |
|       | > fun |       |       |       |       |       |       |       |
|       | ction |       |       |       |       |       |       |       |
|       | )     |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       | > min |       |       |       |       |       |       |
|       |       | imize |       |       |       |       |       |       |
|       |       | > the |       |       |       |       |       |       |
|       |       | > neg |       |       |       |       |       |       |
|       |       | ative |       |       |       |       |       |       |
|       |       | > log |       |       |       |       |       |       |
|       |       | > lik |       |       |       |       |       |       |
|       |       | eliho |       |       |       |       |       |       |
|       |       | od    |       |       |       |       |       |       |
|       |       | > of  |       |       |       |       |       |       |
|       |       | > the |       |       |       |       |       |       |
|       |       | > cor |       |       |       |       |       |       |
|       |       | rect  |       |       |       |       |       |       |
|       |       | > cla |       |       |       |       |       |       |
|       |       | ss:   |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+

> 5.1

-1.7

![](media/image129.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 29 11 Jan 2016

> ![](media/image130.jpeg){width="9.1125in"
> height="0.6722222222222223in"}(Multinomial Logistic Regression)

![](media/image131.jpeg){width="9.782638888888888in"
height="3.7159722222222222in"}

> cat
>
> car
>
> frog

**scores = unnormalized log probabilities of the classes.**

+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       | > whe |       |       |       |       |
|       |       |       |       | re    |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| **3.2 | > Wan |       |       |       |       |       |       |       |
| **    | t     |       |       |       |       |       |       |       |
|       | > to  |       |       |       |       |       |       |       |
|       | > max |       |       |       |       |       |       |       |
|       | imize |       |       |       |       |       |       |       |
|       | > the |       |       |       |       |       |       |       |
|       | > log |       |       |       |       |       |       |       |
|       | > lik |       |       |       |       |       |       |       |
|       | eliho |       |       |       |       |       |       |       |
|       | od,   |       |       |       |       |       |       |       |
|       | > or  |       |       |       |       |       |       |       |
|       | > (fo |       |       |       |       |       |       |       |
|       | r     |       |       |       |       |       |       |       |
|       | > a   |       |       |       |       |       |       |       |
|       | > los |       |       |       |       |       |       |       |
|       | s     |       |       |       |       |       |       |       |
|       | > fun |       |       |       |       |       |       |       |
|       | ction |       |       |       |       |       |       |       |
|       | )     |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       | > min |       |       |       |       |       |       |
|       |       | imize |       |       |       |       |       |       |
|       |       | > the |       |       |       |       |       |       |
|       |       | > neg |       |       |       |       |       |       |
|       |       | ative |       |       |       |       |       |       |
|       |       | > log |       |       |       |       |       |       |
|       |       | > lik |       |       |       |       |       |       |
|       |       | eliho |       |       |       |       |       |       |
|       |       | od    |       |       |       |       |       |       |
|       |       | > of  |       |       |       |       |       |       |
|       |       | > the |       |       |       |       |       |       |
|       |       | > cor |       |       |       |       |       |       |
|       |       | rect  |       |       |       |       |       |       |
|       |       | > cla |       |       |       |       |       |       |
|       |       | ss:   |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+

> 5.1

^-1.7^ in summary:

![](media/image132.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 30 11 Jan 2016

![](media/image133.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image134.jpeg){width="7.602777777777778in"
height="3.438888888888889in"}

> cat

![](media/image135.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image136.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog
>
> **3.2**
>
> 5.1

-1.7

![](media/image137.jpeg){width="3.7930555555555556in"
height="0.4166666666666667in"}

> unnormalized log probabilities

![](media/image138.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 31        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image139.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image140.jpeg){width="6.2034722222222225in"
height="1.4472222222222222in"}

> unnormalized probabilities

![](media/image141.jpeg){width="5.188194444444444in" height="1.88125in"}

> cat

![](media/image142.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image143.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog
>
> **3.2** **24.5**
>
> exp
>
> 5.1 ![](media/image144.jpeg){width="0.8215277777777777in"
> height="0.15208333333333332in"} 164.0

![](media/image145.jpeg){width="0.8097222222222222in"
height="5.208880139982502e-3in"}

-1.7 0.18

![](media/image146.jpeg){width="3.7930555555555556in"
height="0.4166666666666667in"}

> unnormalized log probabilities

![](media/image147.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 32        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image148.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image149.jpeg){width="6.2034722222222225in"
height="1.4472222222222222in"}

> unnormalized probabilities

![](media/image150.jpeg){width="7.688194444444444in" height="1.88125in"}

> cat

![](media/image151.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image152.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog
>
> **3.2** **24.5** **0.13**

  ----- ----- ----------- -- ------ --
        exp   normalize             
  5.1         164.0          0.87   
                                    
  ----- ----- ----------- -- ------ --

![](media/image153.jpeg){width="0.8097222222222222in"
height="5.208880139982502e-3in"}

-1.7 0.18 0.00

![](media/image155.jpeg){width="7.2444444444444445in"
height="0.4166666666666667in"}

+-----------------------+-----------------------+-----------------------+
| > unnormalized log    | probabilities         |                       |
| > probabilities       |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | Lecture 3 33          | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image156.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image157.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image158.jpeg){width="6.2034722222222225in"
height="1.4472222222222222in"}

> unnormalized probabilities

![](media/image159.jpeg){width="9.877083333333333in" height="1.88125in"}

> cat

![](media/image160.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image161.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog

  --------- ---------- ----------- -- ------ --
  **3.2**   **24.5**   **0.13**              
            exp        normalize             
  5.1                  164.0          0.87   
                                             
  --------- ---------- ----------- -- ------ --

![](media/image162.jpeg){width="0.8097222222222222in"
height="5.208880139982502e-3in"}

-1.7 0.18 0.00

![](media/image164.jpeg){width="7.2444444444444445in"
height="0.4166666666666667in"}

L\_i = -log(0.13)

![](media/image165.jpeg){width="0.24861111111111112in"
height="5.208880139982502e-3in"}

-   **0.89**

+-----------------------+-----------------------+-----------------------+
| > unnormalized log    | probabilities         |                       |
| > probabilities       |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | Lecture 3 34          | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image166.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image167.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image168.jpeg){width="6.988194444444445in"
height="1.6701388888888888in"}

> Q: What is the min/max possible loss L\_i?

![](media/image169.jpeg){width="1.275in" height="1.4041666666666666in"}

> unnormalized probabilities

![](media/image170.jpeg){width="9.877083333333333in" height="1.88125in"}

> cat

![](media/image171.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image172.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog

  --------- ---------- ----------- -- ------ --
  **3.2**   **24.5**   **0.13**              
            exp        normalize             
  5.1                  164.0          0.87   
                                             
  --------- ---------- ----------- -- ------ --

![](media/image173.jpeg){width="0.8097222222222222in"
height="5.208880139982502e-3in"}

-1.7 0.18 0.00

![](media/image175.jpeg){width="7.2444444444444445in"
height="0.4166666666666667in"}

L\_i = -log(0.13)

![](media/image176.jpeg){width="0.24861111111111112in"
height="5.208880139982502e-3in"}

-   **0.89**

+-----------------------+-----------------------+-----------------------+
| > unnormalized log    | probabilities         |                       |
| > probabilities       |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | Lecture 3 35          | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image177.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image178.jpeg){width="9.1125in" height="0.6722222222222223in"}

> **Softmax Classifier** (Multinomial Logistic Regression)

![](media/image179.jpeg){width="6.988194444444445in"
height="1.6701388888888888in"}

+----------------------------+------------------------------+--+
|                            | > Q5: usually at             |  |
+----------------------------+------------------------------+--+
|                            | > initialization W are small |  |
+----------------------------+------------------------------+--+
|                            | > numbers, so all s \~= 0.   |  |
+----------------------------+------------------------------+--+
| unnormalized probabilities | > What is the loss?          |  |
+----------------------------+------------------------------+--+
|                            |                              |  |
+----------------------------+------------------------------+--+

![](media/image180.jpeg){width="9.877083333333333in"
height="3.395138888888889in"}

> cat

![](media/image182.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> car

![](media/image183.jpeg){width="1.4652777777777777in"
height="0.32569444444444445in"}

> frog

  --------- ---------- ----------- -- ------ --
  **3.2**   **24.5**   **0.13**              
            exp        normalize             
  5.1                  164.0          0.87   
                                             
  --------- ---------- ----------- -- ------ --

![](media/image184.jpeg){width="0.8097222222222222in"
height="5.208880139982502e-3in"}

-1.7 0.18 0.00

![](media/image186.jpeg){width="7.2444444444444445in"
height="0.4166666666666667in"}

L\_i = -log(0.13)

![](media/image187.jpeg){width="0.24861111111111112in"
height="5.208880139982502e-3in"}

-   **0.89**

+-----------------------+-----------------------+-----------------------+
| > unnormalized log    | probabilities         |                       |
| > probabilities       |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | Lecture 3 36          | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image188.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image189.jpeg){width="9.78125in"
height="5.5993055555555555in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 37        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image190.jpeg){width="9.090277777777779in"
> height="1.707638888888889in"}

![](media/image191.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 38 11 Jan 2016

> ![](media/image192.jpeg){width="9.090277777777779in"
> height="1.707638888888889in"}

![](media/image193.jpeg){width="10.0in" height="2.832638888888889in"}

> assume scores: \[10, -2, 3\] \[10, 9, 9\]
>
> \[10, -100, -100\] and
> ![](media/image194.jpeg){width="1.1215277777777777in"
> height="0.4270833333333333in"}

Q.  Suppose I take a datapoint and I jiggle a bit (changing its score
    slightly). What happens to the loss in both cases?

![](media/image195.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 39 11 Jan 2016

> ![](media/image196.jpeg){width="8.7in" height="4.366666666666666in"}

![](media/image197.jpeg){width="6.386805555555555in"
height="0.3909722222222222in"}

[[http://vision.stanford.edu/teaching/cs231n/linear-classify-demo/]{.underline}](http://vision.stanford.edu/teaching/cs231n/linear-classify-demo/)

![](media/image198.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 40 11 Jan 2016

![](media/image199.jpeg){width="7.213888888888889in"
height="2.5104166666666665in"}

> Optimization

![](media/image200.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 41 11 Jan 2016

> ![](media/image201.jpeg){width="9.259722222222223in"
> height="0.7256944444444444in"}

![](media/image202.jpeg){width="9.52361111111111in"
height="3.8020833333333335in"}

> \- We have some dataset of (x,y) ~e.g.~

-   We have a **score function:**

-   We have a **loss function**:

> Softmax
>
> SVM
>
> ![](media/image203.jpeg){width="3.1333333333333333in"
> height="0.5854166666666667in"} Full loss

![](media/image204.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 42 11 Jan 2016

> ![](media/image205.jpeg){width="9.063888888888888in"
> height="0.8013888888888889in"}**Random search**

![](media/image206.jpeg){width="10.0in" height="4.658333333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 43 11 Jan 2016

> ![](media/image207.jpeg){width="9.14861111111111in"
> height="0.8430555555555556in"}

![](media/image208.jpeg){width="9.613888888888889in"
height="2.9715277777777778in"}

> 15.5% accuracy! not bad!
>
> (SOTA is \~95%)

![](media/image209.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 44 11 Jan 2016

![](media/image210.jpeg){width="9.602777777777778in"
height="5.596527777777778in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 45        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image211.jpeg){width="9.602777777777778in"
height="5.596527777777778in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 46        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image212.jpeg){width="9.063888888888888in"
> height="0.8013888888888889in"}**Follow the slope**

![](media/image213.jpeg){width="9.360416666666667in"
height="0.8013888888888889in"}

> In 1-dimension, the derivative of a function:

![](media/image214.jpeg){width="4.006944444444445in"
height="0.9652777777777778in"}

> In multiple dimensions, the **gradient** is the vector of (partial
> derivatives).

![](media/image216.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 47 11 Jan 2016

+------------------+--+--------------------+--+
| **current W:**   |  | > **gradient dW:** |  |
+------------------+--+--------------------+--+
|                  |  |                    |  |
+------------------+--+--------------------+--+
| \[0.34,          |  | > \[?,             |  |
+------------------+--+--------------------+--+
| -1.11,           |  | > ?,               |  |
+------------------+--+--------------------+--+
| 0.78,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| 0.12,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| 0.55,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| 2.81,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| -3.1,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| -1.5,            |  | > ?,               |  |
+------------------+--+--------------------+--+
| 0.33,...\]       |  | > ?,...\]          |  |
+------------------+--+--------------------+--+
| **loss 1.25347** |  |                    |  |
+------------------+--+--------------------+--+
|                  |  |                    |  |
+------------------+--+--------------------+--+

![](media/image217.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 48 11 Jan 2016

+------------------+------------------------------+
| **current W:**   | > **W + h** (first dim)**:** |
+------------------+------------------------------+
| \[0.34,          | > \[0.34 + **0.0001**,       |
+------------------+------------------------------+
| -1.11,           | > -1.11,                     |
+------------------+------------------------------+
| 0.78,            | > 0.78,                      |
+------------------+------------------------------+
| 0.12,            | > 0.12,                      |
+------------------+------------------------------+
| 0.55,            | > 0.55,                      |
+------------------+------------------------------+
| 2.81,            | > 2.81,                      |
+------------------+------------------------------+
| -3.1,            | > -3.1,                      |
+------------------+------------------------------+
| -1.5,            | > -1.5,                      |
+------------------+------------------------------+
| 0.33,...\]       | > 0.33,...\]                 |
+------------------+------------------------------+
| **loss 1.25347** | > **loss 1.25322**           |
+------------------+------------------------------+

![](media/image222.jpeg){width="6.490277777777778in"
height="4.906944444444444in"}

**gradient dW:**

![](media/image225.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

\[?,

?,

?,

?,

?,

?,

?,

?,

?,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 49 11 Jan 2016

+------------------+------------------------------+
| **current W:**   | > **W + h** (first dim)**:** |
+------------------+------------------------------+
| \[0.34,          | > \[0.34 + **0.0001**,       |
+------------------+------------------------------+
| -1.11,           | > -1.11,                     |
+------------------+------------------------------+
| 0.78,            | > 0.78,                      |
+------------------+------------------------------+
| 0.12,            | > 0.12,                      |
+------------------+------------------------------+
| 0.55,            | > 0.55,                      |
+------------------+------------------------------+
| 2.81,            | > 2.81,                      |
+------------------+------------------------------+
| -3.1,            | > -3.1,                      |
+------------------+------------------------------+
| -1.5,            | > -1.5,                      |
+------------------+------------------------------+
| 0.33,...\]       | > 0.33,...\]                 |
+------------------+------------------------------+
| **loss 1.25347** | > **loss 1.25322**           |
+------------------+------------------------------+

![](media/image226.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

> **gradient dW:**

![](media/image230.jpeg){width="6.9847222222222225in"
height="4.906944444444444in"}

> \[**-2.5**,
>
> ?,
>
> ?,

(1.25322 - 1.25347)/0.0001 = -2.5

> ?,
>
> ?,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 50 11 Jan 2016

+------------------+-------------------------------+
| **current W:**   | > **W + h** (second dim)**:** |
+------------------+-------------------------------+
| \[0.34,          | > \[0.34,                     |
+------------------+-------------------------------+
| -1.11,           | > -1.11 + **0.0001**,         |
+------------------+-------------------------------+
| 0.78,            | > 0.78,                       |
+------------------+-------------------------------+
| 0.12,            | > 0.12,                       |
+------------------+-------------------------------+
| 0.55,            | > 0.55,                       |
+------------------+-------------------------------+
| 2.81,            | > 2.81,                       |
+------------------+-------------------------------+
| -3.1,            | > -3.1,                       |
+------------------+-------------------------------+
| -1.5,            | > -1.5,                       |
+------------------+-------------------------------+
| 0.33,...\]       | > 0.33,...\]                  |
+------------------+-------------------------------+
| **loss 1.25347** | > **loss 1.25353**            |
+------------------+-------------------------------+

![](media/image231.jpeg){width="5.208880139982502e-3in"
height="4.809722222222222in"}

**gradient dW:**

![](media/image235.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

\[-2.5,

?,

?,

?,

?,

?,

?,

?,

?,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 51 11 Jan 2016

+------------------+-------------------------------+
| **current W:**   | > **W + h** (second dim)**:** |
+------------------+-------------------------------+
| \[0.34,          | > \[0.34,                     |
+------------------+-------------------------------+
| -1.11,           | > -1.11 + **0.0001**,         |
+------------------+-------------------------------+
| 0.78,            | > 0.78,                       |
+------------------+-------------------------------+
| 0.12,            | > 0.12,                       |
+------------------+-------------------------------+
| 0.55,            | > 0.55,                       |
+------------------+-------------------------------+
| 2.81,            | > 2.81,                       |
+------------------+-------------------------------+
| -3.1,            | > -3.1,                       |
+------------------+-------------------------------+
| -1.5,            | > -1.5,                       |
+------------------+-------------------------------+
| 0.33,...\]       | > 0.33,...\]                  |
+------------------+-------------------------------+
| **loss 1.25347** | > **loss 1.25353**            |
+------------------+-------------------------------+

![](media/image236.jpeg){width="5.208880139982502e-3in"
height="4.809722222222222in"}

> **gradient dW:**
>
> \[-2.5,
>
> **0.6**, ![](media/image240.jpeg){width="7.777777777777778e-2in"
> height="9.166666666666666e-2in"}
>
> ?,
>
> ?,

(1.25353 - 1.25347)/0.0001 = 0.6

> ?,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 52 11 Jan 2016

+------------------+------------------------------+
| **current W:**   | > **W + h** (third dim)**:** |
+------------------+------------------------------+
| \[0.34,          | > \[0.34,                    |
+------------------+------------------------------+
| -1.11,           | > -1.11,                     |
+------------------+------------------------------+
| 0.78,            | > 0.78 + **0.0001**,         |
+------------------+------------------------------+
| 0.12,            | > 0.12,                      |
+------------------+------------------------------+
| 0.55,            | > 0.55,                      |
+------------------+------------------------------+
| 2.81,            | > 2.81,                      |
+------------------+------------------------------+
| -3.1,            | > -3.1,                      |
+------------------+------------------------------+
| -1.5,            | > -1.5,                      |
+------------------+------------------------------+
| 0.33,...\]       | > 0.33,...\]                 |
+------------------+------------------------------+
| **loss 1.25347** | > **loss 1.25347**           |
+------------------+------------------------------+

![](media/image241.jpeg){width="5.208880139982502e-3in"
height="4.809722222222222in"}

**gradient dW:**

![](media/image245.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

\[-2.5,

0.6,

?,

?,

?,

?,

?,

?,

?,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 53 11 Jan 2016

+------------------+------------------------------+
| **current W:**   | > **W + h** (third dim)**:** |
+------------------+------------------------------+
| \[0.34,          | > \[0.34,                    |
+------------------+------------------------------+
| -1.11,           | > -1.11,                     |
+------------------+------------------------------+
| 0.78,            | > 0.78 + **0.0001**,         |
+------------------+------------------------------+
| 0.12,            | > 0.12,                      |
+------------------+------------------------------+
| 0.55,            | > 0.55,                      |
+------------------+------------------------------+
| 2.81,            | > 2.81,                      |
+------------------+------------------------------+
| -3.1,            | > -3.1,                      |
+------------------+------------------------------+
| -1.5,            | > -1.5,                      |
+------------------+------------------------------+
| 0.33,...\]       | > 0.33,...\]                 |
+------------------+------------------------------+
| **loss 1.25347** | > **loss 1.25347**           |
+------------------+------------------------------+

![](media/image246.jpeg){width="5.208880139982502e-3in"
height="4.809722222222222in"}

> **gradient dW:**

![](media/image249.jpeg){width="5.208880139982502e-3in"
height="4.840972222222222in"}

> \[-2.5,
>
> 0.6,
>
> **0**, ![](media/image250.jpeg){width="8.263888888888889e-2in"
> height="9.027777777777778e-2in"}
>
> ?,

(1.25347 - 1.25347)/0.0001 = 0

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 54 11 Jan 2016

![](media/image251.jpeg){width="9.808333333333334in"
height="5.002777777777778in"}

![](media/image252.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 55 11 Jan 2016

![](media/image253.jpeg){width="9.808333333333334in"
height="5.002777777777778in"}

-   approximate

-   very slow to evaluate

![](media/image254.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 56 11 Jan 2016
>
> ![](media/image255.jpeg){width="9.172222222222222in"
> height="4.628472222222222in"}
>
> want ![](media/image256.jpeg){width="0.9763888888888889in"
> height="0.4583333333333333in"}

![](media/image257.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 57 11 Jan 2016

> ![](media/image258.jpeg){width="9.372916666666667in"
> height="4.7659722222222225in"}
>
> want ![](media/image259.jpeg){width="0.9763888888888889in"
> height="0.4583333333333333in"}

![](media/image260.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 58 11 Jan 2016

> ![](media/image261.jpeg){width="9.469444444444445in"
> height="4.752777777777778in"}
>
> want ![](media/image262.jpeg){width="0.9763888888888889in"
> height="0.4583333333333333in"}
>
> Calculus

![](media/image263.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 59 11 Jan 2016

> ![](media/image264.jpeg){width="9.104861111111111in"
> height="4.628472222222222in"}
>
> ![](media/image265.jpeg){width="0.9763888888888889in"
> height="0.4583333333333333in"} = \...

![](media/image266.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 60 11 Jan 2016

> ![](media/image267.jpeg){width="5.208880139982502e-3in"
> height="4.809722222222222in"}
>
> \[0.34,
>
> -1.11,
>
> 0.78,
>
> 0.12,
>
> 0.55,
>
> 2.81,
>
> -3.1,
>
> -1.5,
>
> 0.33,...\] **loss 1.25347**

dW = \...

![](media/image269.jpeg){width="3.7784722222222222in"
height="3.410416666666667in"}

(some function

data and W)

![](media/image270.jpeg){width="10.0in" height="0.5888888888888889in"}

**gradient dW:**

![](media/image271.jpeg){width="2.6034722222222224in"
height="0.4583333333333333in"}

\[-2.5,

0.6,

0,

0.2,

0.7,

-0.5,

1.1,

1.3,

-2.1,...\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 61 11 Jan 2016

> ![](media/image272.jpeg){width="8.984027777777778in"
> height="4.1930555555555555in"}

-   Numerical gradient: approximate, slow, easy to write

-   Analytic gradient: exact, fast, error-prone

> =\>
>
> [In practice:]{.underline} Always use analytic gradient, but check
> implementation with numerical gradient. This is called a **gradient
> check.**

![](media/image273.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 62 11 Jan 2016

> ![](media/image274.jpeg){width="7.3694444444444445in"
> height="1.2354166666666666in"}

![](media/image275.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 63 11 Jan 2016

> ![](media/image277.jpeg){width="7.291666666666667in"
> height="4.3125in"}

![](media/image278.jpeg){width="2.1041666666666665in"
height="0.4583333333333333in"}

original W

![](media/image280.jpeg){width="1.8965277777777778in"
height="5.208880139982502e-3in"}

> W\_1
>
> negative gradient direction

![](media/image282.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 64 11 Jan 2016

> ![](media/image283.jpeg){width="8.822222222222223in"
> height="0.7694444444444445in"}

![](media/image284.jpeg){width="8.727777777777778in"
height="0.6256944444444444in"}

-   only use a small portion of the training set to compute the
    > gradient.

![](media/image285.jpeg){width="9.350694444444445in"
height="2.8520833333333333in"}

> Common mini-batch sizes are 32/64/128 examples e.g. Krizhevsky ILSVRC
> ConvNet used 256 examples

![](media/image286.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 65 11 Jan 2016

> ![](media/image287.jpeg){width="9.647916666666667in"
> height="3.8805555555555555in"}
>
> (Loss over mini-batches goes down over time.)

![](media/image288.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 66 11 Jan 2016

> ![](media/image289.jpeg){width="4.9527777777777775in"
> height="4.645138888888889in"}

![](media/image290.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 67 11 Jan 2016

![](media/image292.jpeg){width="8.822222222222223in"
height="0.7694444444444445in"}

> Mini-batch Gradient Descent

![](media/image293.jpeg){width="8.727777777777778in"
height="0.6256944444444444in"}

-   only use a small portion of the training set to compute the
    > gradient.

![](media/image294.jpeg){width="9.727083333333333in"
height="3.1638888888888888in"}

> Common mini-batch sizes are 32/64/128 examples e.g. Krizhevsky ILSVRC
> ConvNet used 256 examples

![](media/image295.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

we will look at more fancy update formulas (momentum, Adagrad, RMSProp,
Adam, ...)

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 3 68        | > 11 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image296.jpeg){width="9.810416666666667in"
> height="4.716666666666667in"}

(image credits to Alec Radford)

![](media/image297.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 69 11 Jan 2016

> ![](media/image298.jpeg){width="9.540972222222223in"
> height="0.6361111111111111in"}

![](media/image299.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 70 11 Jan 2016

> ![](media/image301.jpeg){width="6.279861111111111in"
> height="0.8722222222222222in"}

![](media/image302.jpeg){width="5.208880139982502e-3in"
height="2.8270833333333334in"}

> hue bins
>
> ![](media/image314.jpeg){width="0.15208333333333332in"
> height="0.17916666666666667in"} +1

![](media/image315.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 71 11 Jan 2016

> ![](media/image316.jpeg){width="6.279861111111111in"
> height="0.8722222222222222in"}

![](media/image317.jpeg){width="2.202777777777778in" height="0.56875in"}

> 8x8 pixel region, quantize the edge orientation into 9 bins

![](media/image318.jpeg){width="9.916666666666666in"
height="3.792361111111111in"}

*(image from vlfeat.org)*

![](media/image320.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 72 11 Jan 2016

> ![](media/image321.jpeg){width="6.279861111111111in"
> height="0.8722222222222222in"}

![](media/image322.jpeg){width="6.304861111111111in"
height="3.5208333333333335in"}

> 8x8 pixel region, quantize the edge orientation into 9 bins

![](media/image323.jpeg){width="3.361111111111111in"
height="3.361111111111111in"}

> Many more:
>
> GIST, LBP, Texton, SSIM, \...

![](media/image324.jpeg){width="2.4291666666666667in"
height="0.36041666666666666in"}

*(image from vlfeat.org)*

![](media/image325.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 73 11 Jan 2016

<table>
<tbody>
<tr class="odd">
<td>Example: Bag of Words</td>
<td><blockquote>
<p>histogram of</p>
</blockquote></td>
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
<td><blockquote>
<p>visual words</p>
</blockquote></td>
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
<td></td>
</tr>
<tr class="odd">
<td></td>
<td><blockquote>
<p>visual word vectors</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>learn k-means centroids</p>
</blockquote></td>
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
<td><blockquote>
<p>“vocabulary” of visual words</p>
</blockquote></td>
<td><blockquote>
<p>1000-d vector</p>
</blockquote></td>
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
<td></td>
</tr>
</tbody>
</table>

![](media/image326.jpeg){width="6.279861111111111in"
height="0.6666666666666666in"}

+-----+--+-----------------+--+
| 144 |  | > 1000-d vector |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+
|     |  |                 |  |
+-----+--+-----------------+--+

![](media/image329.jpeg){width="1.1861111111111111in"
height="5.208880139982502e-3in"}

> 1000-d vector

![](media/image339.jpeg){width="1.1861111111111111in"
height="5.208880139982502e-3in"}

> e.g. 1000 centroids

![](media/image347.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 74 11 Jan 2016

> ![](media/image349.jpeg){width="2.645138888888889in"
> height="0.28888888888888886in"}
>
> image statistics

![](media/image350.jpeg){width="5.208880139982502e-3in"
height="0.47847222222222224in"}

+------------+--+--+------------+------------------------------+--+----------------+--+
| Feature    |  |  | > f        | > **10** numbers, indicating |  |                |  |
+------------+--+--+------------+------------------------------+--+----------------+--+
| Extraction |  |  |            |                              |  | > class scores |  |
+------------+--+--+------------+------------------------------+--+----------------+--+
|            |  |  | > training |                              |  |                |  |
+------------+--+--+------------+------------------------------+--+----------------+--+
|            |  |  |            |                              |  |                |  |
+------------+--+--+------------+------------------------------+--+----------------+--+

![](media/image352.jpeg){width="0.7236111111111111in"
height="5.208880139982502e-3in"}

> **\[32x32x3\]**
>
> f
>
> **10** numbers, indicating class scores

![](media/image356.jpeg){width="4.061111111111111in"
height="5.208880139982502e-3in"}

> training
>
> **\[32x32x3\]**

![](media/image358.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 75 11 Jan 2016

![](media/image359.jpeg){width="9.515972222222222in"
height="1.351388888888889in"}

Becoming a backprop ninja

and

Neural Networks (part 1)

![](media/image360.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 3 76 11 Jan 2016
