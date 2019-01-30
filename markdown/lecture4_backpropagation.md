![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Backpropagation

and

Neural Networks part 1

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 1 13 Jan 2016

> ![](media/image3.jpeg){width="9.183333333333334in"
> height="4.215277777777778in"}
>
> A1 is due Jan 20 (Wednesday). \~150 hours left
>
> Warning: Jan 18 (Monday) is Holiday (no class/office hours)
>
> Also note:
>
> Lectures are non-exhaustive.
>
> Read course notes for completeness.
>
> I'll hold make up office hours on Wed Jan20, 5pm @ Gates 259

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 2 13 Jan 2016

> ![](media/image5.jpeg){width="7.652083333333334in"
> height="0.6409722222222223in"}

![](media/image6.jpeg){width="2.8777777777777778in"
height="0.4986111111111111in"}

> scores function

![](media/image8.jpeg){width="4.904861111111111in"
height="0.5506944444444445in"}

> SVM loss

![](media/image9.jpeg){width="8.786111111111111in"
height="0.6409722222222223in"}

data loss + regularization

![](media/image11.jpeg){width="1.9666666666666666in"
height="0.5527777777777778in"}

> want

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 3 13 Jan 2016

> ![](media/image13.jpeg){width="9.91388888888889in"
> height="4.584027777777778in"}
>
> (image credits to Alec Radford)

![](media/image14.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 4 13 Jan 2016

> ![](media/image15.jpeg){width="4.882638888888889in"
> height="0.8916666666666667in"}

![](media/image16.jpeg){width="4.006944444444445in"
height="0.9652777777777778in"}

> **Numerical gradient**: slow :(, approximate :(, easy to write :)
>
> **Analytic gradient**: fast :), exact :), error-prone :(
>
> In practice: Derive analytic gradient, check your implementation with
> numerical gradient

![](media/image18.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 5 13 Jan 2016

> ![](media/image19.jpeg){width="5.507638888888889in"
> height="0.5583333333333333in"}

![](media/image20.jpeg){width="8.011805555555556in"
height="1.2993055555555555in"}

> x

![](media/image21.jpeg){width="5.561805555555556in"
height="2.2305555555555556in"}

+----+------------------+----+-----+--+
| \* | > **s** (scores) |    | > L |  |
+----+------------------+----+-----+--+
|    | > hinge          | \+ |     |  |
+----+------------------+----+-----+--+
|    |                  |    |     |  |
+----+------------------+----+-----+--+
|    | > loss           |    |     |  |
+----+------------------+----+-----+--+
|    |                  |    |     |  |
+----+------------------+----+-----+--+

![](media/image23.jpeg){width="1.0486111111111112in" height="1.075in"}

> W

R

![](media/image28.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 6 13 Jan 2016

> ![](media/image29.jpeg){width="7.427777777777778in"
> height="4.873611111111111in"}
>
> input image
>
> weights

![](media/image30.jpeg){width="3.5965277777777778in"
height="0.6569444444444444in"}

> loss

![](media/image31.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 7 13 Jan 2016

> ![](media/image33.jpeg){width="9.051388888888889in"
> height="4.905555555555556in"}
>
> input tape

loss

![](media/image34.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 8 13 Jan 2016

![](media/image35.jpeg){width="10.0in" height="5.5777777777777775in"}

> 9 13 Jan 2016

![](media/image36.jpeg){width="9.605555555555556in"
height="2.277083333333333in"}

> e.g. x = -2, y = 5, z = -4

![](media/image37.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 10        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image38.jpeg){width="9.605555555555556in"
height="2.277083333333333in"}

> e.g. x = -2, y = 5, z = -4

![](media/image39.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image42.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 11        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image43.jpeg){width="9.605555555555556in"
height="3.1756944444444444in"}

> e.g. x = -2, y = 5, z = -4

![](media/image44.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image47.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 12        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image48.jpeg){width="9.605555555555556in"
height="3.1756944444444444in"}

> e.g. x = -2, y = 5, z = -4

![](media/image49.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image52.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 13        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image53.jpeg){width="9.605555555555556in"
height="3.2159722222222222in"}

> e.g. x = -2, y = 5, z = -4

![](media/image54.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image57.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 14        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image58.jpeg){width="9.605555555555556in"
height="3.2159722222222222in"}

> e.g. x = -2, y = 5, z = -4

![](media/image59.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image62.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 15        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image63.jpeg){width="9.605555555555556in"
height="3.342361111111111in"}

> e.g. x = -2, y = 5, z = -4

![](media/image64.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

> Want:

![](media/image67.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 16        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image68.jpeg){width="9.605555555555556in"
> height="3.342361111111111in"}

![](media/image69.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

Want:

![](media/image72.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 17 13 Jan 2016

> ![](media/image73.jpeg){width="9.605555555555556in"
> height="3.2069444444444444in"}

![](media/image74.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

Want:

![](media/image77.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 18 13 Jan 2016

> ![](media/image78.jpeg){width="3.9895833333333335in"
> height="1.1993055555555556in"}

![](media/image79.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

Want:

Chain rule:

![](media/image81.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 19 13 Jan 2016

> ![](media/image83.jpeg){width="9.605555555555556in"
> height="3.2069444444444444in"}

![](media/image84.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

Want:

![](media/image87.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 20 13 Jan 2016

> ![](media/image88.jpeg){width="3.9895833333333335in"
> height="1.1993055555555556in"}

![](media/image89.jpeg){width="4.595138888888889in"
height="1.8791666666666667in"}

Want:

Chain rule:

![](media/image91.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 21 13 Jan 2016

> ![](media/image93.jpeg){width="8.810416666666667in"
> height="4.404861111111111in"}

f

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 22 13 Jan 2016

> ![](media/image96.jpeg){width="8.810416666666667in"
> height="4.404861111111111in"}

"local gradient"

> f

![](media/image97.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 23 13 Jan 2016

> ![](media/image99.jpeg){width="9.235416666666667in"
> height="4.404861111111111in"}
>
> "local gradient"
>
> f

![](media/image100.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients

![](media/image102.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 24 13 Jan 2016

> ![](media/image103.jpeg){width="9.235416666666667in"
> height="4.404861111111111in"}
>
> "local gradient"
>
> f

![](media/image104.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients

![](media/image106.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 25 13 Jan 2016

> ![](media/image107.jpeg){width="9.235416666666667in"
> height="4.945833333333334in"}
>
> "local gradient"
>
> f

![](media/image108.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients

![](media/image110.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 26 13 Jan 2016

> ![](media/image111.jpeg){width="10.0in" height="5.625in"}
>
> "local gradient"
>
> f

![](media/image112.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 27 13 Jan 2016

![](media/image114.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image115.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 28        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image117.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image118.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 29        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image120.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image121.jpeg){width="9.76875in" height="4.7in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 30        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image122.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image123.jpeg){width="9.76875in" height="4.7in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 31        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image124.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image125.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 32        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image127.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image128.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 33        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image130.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image131.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 34        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image133.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image134.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 35        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image136.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image137.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 36        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image139.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image140.jpeg){width="7.231944444444444in"
height="2.636111111111111in"}

> (-1) \* (-0.20) = 0.20

![](media/image141.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 37        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image143.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image144.jpeg){width="9.76875in" height="4.7in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 38        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image145.jpeg){width="6.645138888888889in"
height="0.8090277777777778in"}

> Another example:

![](media/image146.jpeg){width="9.555555555555555in"
height="3.8722222222222222in"}

> \[local gradient\] x \[its gradient\]
>
> \[1\] x \[0.2\] = 0.2
>
> \[1\] x \[0.2\] = 0.2 (both inputs!)

![](media/image147.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 39        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image149.jpeg){width="8.559722222222222in"
height="3.4868055555555557in"}

> Another example:

![](media/image150.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 40        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image152.jpeg){width="8.746527777777779in"
height="3.4868055555555557in"}

> Another example:
>
> \[local gradient\] x \[its gradient\]
>
> x0: \[2\] x \[0.2\] = 0.4
>
> w0: \[-1\] x \[0.2\] = -0.2

![](media/image153.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 41        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image155.jpeg){width="9.040972222222223in"
> height="0.8090277777777778in"}

![](media/image156.jpeg){width="7.861111111111111in"
height="0.7465277777777778in"}

> sigmoid gate

![](media/image158.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 42 13 Jan 2016

![](media/image159.jpeg){width="9.040972222222223in"
height="0.8090277777777778in"}

> sigmoid function

![](media/image160.jpeg){width="7.861111111111111in"
height="0.7465277777777778in"}

> sigmoid gate
>
> (0.73) \* (1 - 0.73) = 0.2

![](media/image162.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 43        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image163.jpeg){width="4.217361111111111in"
> height="0.56875in"}

![](media/image164.jpeg){width="9.56875in"
height="3.4652777777777777in"}

**add** gate: gradient distributor

**max** gate: gradient router

**mul** gate: gradient... "switcher"?

![](media/image165.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 44 13 Jan 2016
>
> ![](media/image166.jpeg){width="7.8375in"
> height="4.689583333333333in"}
>
> \+

![](media/image167.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 45 13 Jan 2016

> ![](media/image169.jpeg){width="9.177777777777777in"
> height="0.6729166666666667in"}: forward/backward API

![](media/image170.jpeg){width="6.163194444444445in"
height="3.826388888888889in"}

Graph (or Net) object. *(Rough psuedo code)*

![](media/image171.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 46 13 Jan 2016

> ![](media/image173.jpeg){width="9.177777777777777in"
> height="0.6729166666666667in"}: forward/backward API

![](media/image174.jpeg){width="0.39305555555555555in"
height="0.27708333333333335in"}

> x

![](media/image176.jpeg){width="1.7340277777777777in"
height="1.1659722222222222in"}

\*

> y

z

![](media/image177.jpeg){width="3.004166666666667in"
height="0.42430555555555555in"}

> (x,y,z are scalars)

![](media/image179.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 47 13 Jan 2016

> ![](media/image180.jpeg){width="9.611805555555556in"
> height="4.861111111111111in"}: forward/backward API
>
> x

\*

> y

z

![](media/image181.jpeg){width="0.6673611111111111in"
height="5.208880139982502e-3in"}

> (x,y,z are scalars)

![](media/image182.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 48 13 Jan 2016

> ![](media/image183.jpeg){width="9.177777777777777in"
> height="0.5611111111111111in"}

![](media/image184.jpeg){width="10.0in" height="5.007638888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 49 13 Jan 2016

> ![](media/image185.jpeg){width="9.261111111111111in"
> height="4.990277777777778in"}
>
> =

![](media/image186.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 50 13 Jan 2016

**Example: Torch MulConstant**

![](media/image187.jpeg){width="7.825694444444444in" height="4.95in"}

> initialization

![](media/image188.jpeg){width="0.8923611111111112in"
height="0.25972222222222224in"} forward()

> ![](media/image189.jpeg){width="0.8909722222222223in"
> height="0.18680555555555556in"} backward()

![](media/image190.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 51 13 Jan 2016

> ![](media/image191.jpeg){width="9.177777777777777in"
> height="0.5611111111111111in"}

![](media/image192.jpeg){width="10.0in" height="5.009027777777778in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 52 13 Jan 2016

> ![](media/image193.jpeg){width="9.900694444444444in"
> height="4.907638888888889in"}
>
> ![](media/image194.jpeg){width="3.3319444444444444in"
> height="0.7465277777777778in"} \*top\_diff (chain rule)

![](media/image196.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 53 13 Jan 2016

![](media/image197.jpeg){width="9.235416666666667in"
height="4.904861111111111in"}^(x,y,z^ ^are\ now^

> vectors)
>
> "local gradient"
>
> f

![](media/image198.jpeg){width="10.0in" height="0.5888888888888889in"}

This is now the

**Jacobian matrix** (derivative of each element of z w.r.t. each element
of x)

![](media/image199.jpeg){width="2.4875in"
height="5.208880139982502e-3in"}

> gradients
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 54 13 Jan 2016
>
> ![](media/image200.jpeg){width="7.975in"
> height="0.6416666666666667in"}

![](media/image201.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> 4096-d input vector

![](media/image204.jpeg){width="0.7444444444444445in"
height="0.20416666666666666in"} f(x) = max(0,x)
![](media/image205.jpeg){width="0.7506944444444444in"
height="0.20416666666666666in"}

![](media/image206.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

*(elementwise)*

![](media/image212.jpeg){width="10.0in" height="0.5888888888888889in"}

4096-d

output vector

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 55 13 Jan 2016

> ![](media/image217.jpeg){width="8.647222222222222in" height="0.925in"}

![](media/image218.jpeg){width="2.0215277777777776in"
height="0.5402777777777777in"}

Jacobian matrix

![](media/image219.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> 4096-d

![](media/image222.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> input vector

![](media/image224.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

Q.  what is the size of the Jacobian matrix?

![](media/image227.jpeg){width="8.888888888888889e-2in"
height="0.20416666666666666in"} f(x) = max(0,x)
![](media/image228.jpeg){width="0.7506944444444444in"
height="0.20416666666666666in"}

![](media/image229.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> *(elementwise)*

![](media/image232.jpeg){width="10.0in" height="0.5888888888888889in"}

4096-d

output vector

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 56 13 Jan 2016

> ![](media/image235.jpeg){width="8.647222222222222in" height="0.925in"}

![](media/image236.jpeg){width="9.502777777777778in"
height="3.686111111111111in"}

> 4096-d

![](media/image237.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> input vector

![](media/image240.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

Q.  what is the size of the Jacobian matrix? \[4096 x 4096!\]

Jacobian matrix

![](media/image243.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

+-------------------+-----------------+
| f(x) = max(0,x)   | > 4096-d        |
+-------------------+-----------------+
| > *(elementwise)* | > output vector |
+-------------------+-----------------+

![](media/image244.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> Q2: what does it
>
> look like?

![](media/image249.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 57 13 Jan 2016

> ![](media/image250.jpeg){width="7.975in"
> height="0.6416666666666667in"}

![](media/image251.jpeg){width="9.854861111111111in"
height="3.734722222222222in"}

> in practice we process an entire minibatch (e.g. 100) of examples at
> one time:

![](media/image252.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

100. 4096-d input vectors

![](media/image253.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

+-------------------+------------------+
| f(x) = max(0,x)   | > 100 4096-d     |
+-------------------+------------------+
| > *(elementwise)* | > output vectors |
+-------------------+------------------+

![](media/image258.jpeg){width="0.7388888888888889in"
height="5.208880139982502e-3in"}

> i.e. Jacobian would technically be a \[409,600 x 409,600\] matrix :\\

![](media/image264.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 58 13 Jan 2016

> ![](media/image265.jpeg){width="9.881944444444445in"
> height="4.802083333333333in"}
>
> Stage your forward/backward computation!
>
> margins

![](media/image266.jpeg){width="5.208880139982502e-3in"
height="0.22777777777777777in"}

> E.g. for the SVM:

![](media/image267.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 59 13 Jan 2016

> ![](media/image269.jpeg){width="8.938888888888888in"
> height="4.419444444444444in"}

-   neural nets will be very large: no hope of writing down gradient
    > formula by hand for all parameters

-   **backpropagation** = recursive application of the chain rule along
    > a computational graph to compute the gradients of all
    > inputs/parameters/intermediates

-   implementations maintain a graph structure, where the nodes
    > implement the **forward**() / **backward**() API.

-   **forward**: compute result of an operation and save any
    > intermediates needed for gradient computation in memory

-   **backward**: apply the chain rule to compute the gradient of the
    > loss function with respect to the inputs.

![](media/image270.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 60 13 Jan 2016

![](media/image271.jpeg){width="9.602777777777778in"
height="5.481944444444444in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 61        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image272.jpeg){width="7.299305555555556in"
> height="0.8597222222222223in"}without the brain stuff

![](media/image273.jpeg){width="7.283333333333333in"
height="0.6111111111111112in"}

> (**Before**) Linear score function:

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 62 13 Jan 2016

> ![](media/image275.jpeg){width="7.299305555555556in"
> height="0.8597222222222223in"}without the brain stuff

![](media/image276.jpeg){width="7.283333333333333in"
height="0.6111111111111112in"}

> (**Before**) Linear score function:

![](media/image277.jpeg){width="9.239583333333334in" height="0.56875in"}

> (**Now**) 2-layer Neural Network

![](media/image278.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 63 13 Jan 2016

![](media/image279.jpeg){width="7.299305555555556in"
height="0.8597222222222223in"}

> Neural Network: without the brain stuff

![](media/image280.jpeg){width="7.283333333333333in"
height="0.6111111111111112in"}

> (**Before**) Linear score function:

![](media/image281.jpeg){width="9.239583333333334in" height="0.56875in"}

> (**Now**) 2-layer Neural Network

![](media/image282.jpeg){width="5.052083333333333in"
height="1.7986111111111112in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td><blockquote>
<p>x</p>
</blockquote></td>
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
<td>h</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td><blockquote>
<p>W1</p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p>W2</p>
</blockquote></td>
<td>s</td>
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
<td>10</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>3072</td>
<td></td>
<td></td>
<td>100</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Fei-Fei Li &amp; Andrej Karpathy &amp; Justin Johnson</td>
<td><blockquote>
<p>Lecture 4 64</p>
</blockquote></td>
<td><blockquote>
<p>13 Jan 2016</p>
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
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image283.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image284.jpeg){width="8.811805555555555in" height="1.85625in"}

> Neural Network: without the brain stuff
>
> (**Before**) Linear score function:

![](media/image285.jpeg){width="9.239583333333334in" height="0.56875in"}

> (**Now**) 2-layer Neural Network

![](media/image286.jpeg){width="5.052083333333333in"
height="1.7986111111111112in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td><blockquote>
<p>x</p>
</blockquote></td>
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
<td>h</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td><blockquote>
<p>W1</p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p>W2</p>
</blockquote></td>
<td>s</td>
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
<td>10</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>3072</td>
<td></td>
<td></td>
<td>100</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Fei-Fei Li &amp; Andrej Karpathy &amp; Justin Johnson</td>
<td><blockquote>
<p>Lecture 4 65</p>
</blockquote></td>
<td><blockquote>
<p>13 Jan 2016</p>
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
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image287.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image288.jpeg){width="7.299305555555556in"
> height="0.8597222222222223in"}without the brain stuff

![](media/image289.jpeg){width="7.283333333333333in"
height="0.6111111111111112in"}

> (**Before**) Linear score function:

![](media/image290.jpeg){width="9.239583333333334in" height="0.56875in"}

> (**Now**) 2-layer Neural Network or 3-layer Neural Network

![](media/image291.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 66 13 Jan 2016

> ![](media/image293.jpeg){width="9.420833333333333in"
> height="0.3541666666666667in"}

![](media/image294.jpeg){width="9.975694444444445in"
height="4.133333333333334in"}

> from \@iamtrask,
> http://iamtrask.github.io/2015/07/12/basic-python-network/

![](media/image295.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 67 13 Jan 2016

> ![](media/image296.jpeg){width="8.384027777777778in"
> height="0.9930555555555556in"}
>
> Stage your forward/backward computation!

![](media/image297.jpeg){width="10.0in" height="4.489583333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 68 13 Jan 2016

![](media/image298.jpeg){width="9.602777777777778in"
height="5.481944444444444in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 69        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image299.jpeg){width="9.602777777777778in"
height="5.503472222222222in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 70        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image300.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 71        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image302.jpeg){width="9.873611111111112in"
height="5.565972222222222in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 72        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image303.jpeg){width="9.747222222222222in"
height="4.878472222222222in"}

> **sigmoid activation**
>
> **function**

![](media/image304.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 73 13 Jan 2016

![](media/image305.jpeg){width="9.938888888888888in"
height="5.565972222222222in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 4 74        | > 13 Jan 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image306.jpeg){width="9.751388888888888in"
> height="4.905555555555556in"}
>
> **Biological Neurons:**

-   Many different types

-   Dendrites can perform complex non-linear computations

-   Synapses are not a single weight but a complex non-linear dynamical
    > system

-   Rate code may not be adequate

*\[Dendritic Computation. London and Hausser\]*

![](media/image307.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 75 13 Jan 2016

![](media/image308.jpeg){width="5.63125in"
height="0.8298611111111112in"}

> Activation Functions

![](media/image309.jpeg){width="1.832638888888889in"
height="1.1784722222222221in"}

**Leaky ReLU**

![](media/image311.jpeg){width="2.5277777777777777in"
height="0.5229166666666667in"}

max(0.1x, x)

![](media/image312.jpeg){width="2.4in" height="1.5527777777777778in"}

> **Sigmoid**

![](media/image313.jpeg){width="9.740277777777777in"
height="1.7826388888888889in"}

+------------------+--------------+--+
| **tanh** tanh(x) | > **Maxout** |  |
+------------------+--------------+--+
|                  | > **ELU**    |  |
+------------------+--------------+--+
|                  |              |  |
+------------------+--------------+--+

![](media/image315.jpeg){width="9.165277777777778in"
height="1.8743055555555554in"}

> **ReLU** max(0,x)

![](media/image317.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 76 13 Jan 2016

> ![](media/image318.jpeg){width="7.084027777777778in"
> height="0.5201388888888889in"}

![](media/image319.jpeg){width="5.208880139982502e-3in"
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

![](media/image321.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 77 13 Jan 2016
>
> ![](media/image322.jpeg){width="8.988194444444444in"
> height="0.7208333333333333in"}

![](media/image323.jpeg){width="8.565277777777778in"
height="2.654861111111111in"}

> We can efficiently evaluate an entire layer of neurons.

![](media/image324.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 78 13 Jan 2016

> ![](media/image325.jpeg){width="8.988194444444444in"
> height="3.111111111111111in"}

![](media/image326.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 79 13 Jan 2016

> ![](media/image328.jpeg){width="9.20625in"
> height="0.8597222222222223in"}

![](media/image329.jpeg){width="9.20625in" height="3.678472222222222in"}

more neurons = more capacity

![](media/image330.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 80 13 Jan 2016

> ![](media/image331.jpeg){width="9.82986111111111in"
> height="0.6222222222222222in"}

![](media/image332.jpeg){width="9.20625in" height="3.795138888888889in"}

> (you can play with this demo over at ConvNetJS:
> [[http://cs.stanford.]{.underline}](http://cs.stanford.edu/people/karpathy/convnetjs/demo/classify2d.html)
>
> [[edu/people/karpathy/convnetjs/demo/classify2d.html]{.underline}](http://cs.stanford.edu/people/karpathy/convnetjs/demo/classify2d.html))

![](media/image333.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 81 13 Jan 2016

> ![](media/image334.jpeg){width="8.909027777777778in"
> height="4.4631944444444445in"}

-   we arrange neurons into fully-connected layers

-   the abstraction of a **layer** has the nice property that it allows
    > us to use efficient vectorized code (e.g. matrix multiplies)

-   neural networks are not really *neural*

-   neural networks: bigger = better (but might have to regularize more
    > strongly)

![](media/image335.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 82 13 Jan 2016

> ![](media/image336.jpeg){width="8.23611111111111in"
> height="2.9784722222222224in"}
>
> More than you ever wanted to know about Neural Networks and how to
> train them.

![](media/image337.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 83 13 Jan 2016

> ![](media/image338.jpeg){width="4.389583333333333in"
> height="2.6881944444444446in"}

![](media/image339.jpeg){width="1.03125in" height="0.26875in"}

> outputs y

![](media/image340.jpeg){width="0.925in"
height="5.208880139982502e-3in"}

> ![](media/image346.jpeg){width="0.22708333333333333in"
> height="0.4166666666666667in"}complex graph

![](media/image347.jpeg){width="6.952083333333333in"
height="5.208880139982502e-3in"}

> reverse-mode differentiation (if you want effect of many things on one
> thing)
>
> for many different x

![](media/image361.jpeg){width="6.952083333333333in"
height="5.208880139982502e-3in"}

> forward-mode differentiation (if you want effect of one thing on many
> things)
>
> for many different y

![](media/image363.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 4 84 13 Jan 2016
