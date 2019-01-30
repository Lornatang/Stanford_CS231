![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Spatial Localization and

Detection

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 1 1 Feb 2016

> ![](media/image3.jpeg){width="9.7625in" height="4.215277777777778in"}

-   Project Proposals were due on Saturday

-   Homework 2 due Friday 2/5

-   Homework 1 grades out this week

-   Midterm will be in-class on Wednesday 2/10

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 2 1 Feb 2016

> ![](media/image5.jpeg){width="8.689583333333333in"
> height="4.770833333333333in"}
>
> 32
>
> 32
>
> 3

![](media/image6.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 3 1 Feb 2016

> **Pooling**

  ------- ------- --- -------
  1       1       2   4
                      
  5       **6**   7   **8**
                      
  **3**   2       1   0
                      
  1       2       3   **4**
                      
  ------- ------- --- -------

![](media/image7.jpeg){width="5.208880139982502e-3in"
height="1.3333333333333333in"}

> 2x2 max
>
> pooling

-   8

> 3 4

![](media/image9.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 4 1 Feb 2016

> ![](media/image10.jpeg){width="7.4743055555555555in"
> height="1.9631944444444445in"}
>
> LeNet
>
> (1998)

![](media/image11.jpeg){width="6.384722222222222in"
height="1.4048611111111111in"}

> AlexNet
>
> (2012)

![](media/image12.jpeg){width="1.3423611111111111in" height="1.0625in"}

> ZFNet

![](media/image13.jpeg){width="4.89375in" height="1.175in"}

> (2013)

![](media/image14.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 5 1 Feb 2016

![](media/image15.jpeg){width="9.621527777777779in"
height="4.934027777777778in"}

> **Case Studies**
>
> ^VGG^ GoogLeNet ResNet
>
> ^(2014)^ (2014) (2015)

![](media/image16.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 6 1 Feb 2016

> ![](media/image17.jpeg){width="10.0in" height="5.625in"}

Results from Faster R-CNN, Ren et al 2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 7 1 Feb 2016

> ![](media/image18.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image19.jpeg){width="9.586805555555555in"
height="2.8090277777777777in"}

<table>
<tbody>
<tr class="odd">
<td><strong>Classification</strong></td>
<td><blockquote>
<p><strong>Classification</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Object Detection</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Instance</strong></p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
</blockquote></td>
<td></td>
<td><blockquote>
<p><strong>Segmentation</strong></p>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image20.jpeg){width="9.582638888888889in"
height="0.4583333333333333in"}

> CAT CAT CAT, DOG, DUCK CAT, DOG, DUCK

![](media/image21.jpeg){width="10.0in" height="1.448611111111111in"}

> Single object Multiple objects

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 8 1 Feb 2016

> ![](media/image22.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image23.jpeg){width="9.586805555555555in"
height="2.8090277777777777in"}

<table>
<tbody>
<tr class="odd">
<td><strong>Classification</strong></td>
<td><blockquote>
<p><strong>Classification</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Object Detection</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Instance</strong></p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
</blockquote></td>
<td></td>
<td><blockquote>
<p><strong>Segmentation</strong></p>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image24.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 9 1 Feb 2016

![](media/image25.jpeg){width="8.450694444444444in"
height="0.7173611111111111in"}

> Classification + Localization: Task

![](media/image26.jpeg){width="9.625in" height="4.018055555555556in"}

> **Classification**: C classes
>
> **Input:** Image
>
> **Output:** Class label
>
> **Evaluation metric:** Accuracy
>
> **Localization**:
>
> **Input:** Image
>
> **Output**: Box in the image (x, y, w, h)
>
> **Evaluation metric:** Intersection over Union
>
> **Classification + Localization**: Do both

![](media/image27.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

CAT

![](media/image28.jpeg){width="1.0048611111111112in"
height="5.208880139982502e-3in"}

> ![](media/image29.jpeg){width="1.0215277777777778in"
> height="0.22847222222222222in"} (x, y, w, h)

![](media/image30.jpeg){width="1.0048611111111112in"
height="5.208880139982502e-3in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 8 10        | > 1 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image31.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image32.jpeg){width="10.0in" height="4.789583333333334in"}

> 1000 classes (same as classification)
>
> Each image has 1 class, at least one bounding box
>
> \~800 training images per class
>
> Algorithm produces 5 (class, box) guesses
>
> Example is correct if at least one one guess has correct class AND
> bounding box at least 0.5 intersection over union (IoU)

Krizhevsky et. al. 2012

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 11 1 Feb 2016

![](media/image33.jpeg){width="8.450694444444444in"
height="0.7173611111111111in"}

> Idea \#1: Localization as Regression

![](media/image34.jpeg){width="2.222916666666667in"
height="0.4222222222222222in"}

> **Input**: image

![](media/image35.jpeg){width="7.561111111111111in"
height="1.8493055555555555in"}

+--------------+---------------+-------------------+--+
| > Neural Net | > **Output**: |                   |  |
+--------------+---------------+-------------------+--+
|              |               | > Box coordinates |  |
+--------------+---------------+-------------------+--+
|              |               |                   |  |
+--------------+---------------+-------------------+--+
|              |               | > (4 numbers)     |  |
+--------------+---------------+-------------------+--+

![](media/image36.jpeg){width="1.3944444444444444in"
height="5.208880139982502e-3in"}

> **Correct output**:
>
> box coordinates

![](media/image39.jpeg){width="2.911111111111111in"
height="0.8263888888888888in"}

> Only one object, (4 numbers)
>
> simpler than detection

![](media/image40.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> **Loss**:

![](media/image41.jpeg){width="1.78125in" height="0.8708333333333333in"}

L2 distance

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 8 12        | > 1 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image42.jpeg){width="9.77361111111111in"
> height="1.6041666666666667in"}
>
> **Step 1**: Train (or download) a classification model (AlexNet, VGG,
> GoogLeNet)

![](media/image43.jpeg){width="7.977777777777778in"
height="2.4430555555555555in"}

> Convolution
>
> ~and\ Pooling~ Fully-connected
>
> layers
>
> Softmax loss

![](media/image44.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+----------------+--+--+--+
|       | > Final conv  |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               | > Class scores |  |  |  |
+-------+---------------+----------------+--+--+--+
| Image | > feature map |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               |                |  |  |  |
+-------+---------------+----------------+--+--+--+

![](media/image49.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 13 1 Feb 2016

> ![](media/image50.jpeg){width="9.77361111111111in"
> height="4.824305555555555in"}
>
> **Step 2**: Attach new fully-connected "regression head" to the
> network
>
> Convolution
>
> and Pooling

![](media/image51.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+--+
|       | > Final conv  |  |
+-------+---------------+--+
| Image | > feature map |  |
+-------+---------------+--+
|       |               |  |
+-------+---------------+--+

Fully-connected

layers

> "Classification head"

![](media/image53.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Class scores

Fully-connected

layers

"Regression head"

![](media/image54.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Box coordinates

![](media/image55.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 14 1 Feb 2016

> ![](media/image56.jpeg){width="9.77361111111111in"
> height="3.0076388888888888in"}
>
> **Step 3**: Train the regression head only with SGD and L2 loss
>
> Fully-connected
>
> layers

![](media/image57.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Convolution
>
> and Pooling

![](media/image58.jpeg){width="7.660416666666666in"
height="1.7972222222222223in"}

Class scores

> Fully-connected
>
> layers

![](media/image59.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

L2 loss

![](media/image61.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Final conv

+-------+---------------+-------------------+--+
| Image | > feature map | > Box coordinates |  |
+-------+---------------+-------------------+--+
|       |               |                   |  |
+-------+---------------+-------------------+--+

![](media/image63.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 15 1 Feb 2016

> ![](media/image64.jpeg){width="9.77361111111111in"
> height="1.6555555555555554in"}
>
> **Step 4**: At test time use both heads

![](media/image65.jpeg){width="6.950694444444444in"
height="3.0416666666666665in"}

> Convolution
>
> and Pooling

![](media/image66.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+--+
|       | > Final conv  |  |
+-------+---------------+--+
| Image | > feature map |  |
+-------+---------------+--+
|       |               |  |
+-------+---------------+--+

Fully-connected

layers

![](media/image68.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Class scores

Fully-connected

layers

![](media/image69.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

Box coordinates

![](media/image70.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 16 1 Feb 2016

> ![](media/image71.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image72.jpeg){width="9.446527777777778in"
height="3.823611111111111in"}

> Assume classification
>
> over C classes:
>
> Convolution

and Pooling

<table>
<tbody>
<tr class="odd">
<td>Fully-connected</td>
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
<td></td>
</tr>
<tr class="even">
<td></td>
<td>layers</td>
<td><blockquote>
<p><strong>Classification head</strong>:</p>
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
<td><blockquote>
<p>C numbers</p>
</blockquote></td>
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
<td><blockquote>
<p>(one per class)</p>
</blockquote></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Class</p>
</blockquote></td>
<td></td>
<td>scores</td>
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
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image73.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

+-------+---------------+--+
|       | > Final conv  |  |
+-------+---------------+--+
| Image | > feature map |  |
+-------+---------------+--+
|       |               |  |
+-------+---------------+--+

![](media/image74.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

Fully-connected

layers

![](media/image76.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

Box coordinates

![](media/image77.jpeg){width="10.0in" height="0.5888888888888889in"}

**Class agnostic:**

-   numbers (one box)

**Class specific:** C x 4 numbers (one box per class)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 17 1 Feb 2016

> ![](media/image78.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image79.jpeg){width="8.63125in" height="3.7in"}

**After conv layers**: **After last FC layer**:

> ![](media/image80.jpeg){width="0.2659722222222222in"
> height="0.23958333333333334in"} Overfeat, VGG
> ![](media/image81.jpeg){width="0.27569444444444446in"
> height="0.22430555555555556in"} DeepPose, R-CNN
>
> Convolution
>
> ~and\ Pooling~ Fully-connected
>
> layers
>
> Softmax loss

![](media/image82.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+----------------+--+--+--+
|       | > Final conv  |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               | > Class scores |  |  |  |
+-------+---------------+----------------+--+--+--+
| Image | > feature map |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               |                |  |  |  |
+-------+---------------+----------------+--+--+--+

![](media/image87.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 18 1 Feb 2016

> ![](media/image88.jpeg){width="9.621527777777779in"
> height="4.824305555555555in"}
>
> Want to localize **exactly** K objects in each image
>
> (e.g. whole cat, cat head, cat left ear, cat right ear for K=4)
>
> Convolution
>
> and Pooling

![](media/image89.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+--+
|       | > Final conv  |  |
+-------+---------------+--+
| Image | > feature map |  |
+-------+---------------+--+
|       |               |  |
+-------+---------------+--+

Fully-connected

layers

![](media/image91.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> Class scores

Fully-connected

layers

> K x 4 numbers

![](media/image92.jpeg){width="0.25277777777777777in"
height="5.208880139982502e-3in"}

> (one box per object)
>
> Box coordinates

![](media/image93.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 19 1 Feb 2016

> ![](media/image94.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image95.jpeg){width="10.0in" height="4.830555555555556in"}

> Represent a person by K joints
>
> Regress (x, y) for each joint from last fully-connected layer of
> AlexNet
>
> (Details: Normalized coordinates, iterative refinement)

Toshev and Szegedy, "DeepPose: Human Pose Estimation via Deep Neural
Networks", CVPR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 20 1 Feb 2016
>
> ![](media/image96.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image97.jpeg){width="8.450694444444444in"
height="2.104861111111111in"}

> Very simple
>
> Think if you can use this for projects

![](media/image98.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 21 1 Feb 2016

> ![](media/image99.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image100.jpeg){width="4.159027777777778in"
height="3.7222222222222223in"}

-   Run classification + regression network at multiple locations on a
    > high-resolution image

-   Convert fully-connected layers into convolutional layers for
    > efficient computation

-   Combine classifier and

> regressor predictions across all scales for final prediction

![](media/image101.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 22 1 Feb 2016

> ![](media/image102.jpeg){width="10.0in" height="5.5625in"}

<table>
<tbody>
<tr class="odd">
<td>Winner of ILSVRC 2013</td>
<td>4096</td>
<td>4096</td>
<td>Class scores:</td>
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
<td>1000</td>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td>localization challenge</td>
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
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td>FC</td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>Softmax</p>
</blockquote></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>Convolution</p>
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
<td><blockquote>
<p>loss</p>
</blockquote></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>+ pooling</p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p>FC</p>
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
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image103.jpeg){width="0.5819444444444445in"
height="5.208880139982502e-3in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td><blockquote>
<p>Feature map:</p>
</blockquote></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>Euclidean</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Image:</td>
<td><blockquote>
<p>1024 x 5 x 5</p>
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
<td></td>
<td><blockquote>
<p>loss</p>
</blockquote></td>
<td></td>
</tr>
<tr class="odd">
<td>3 x 221 x 221</td>
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
<td>1024</td>
<td></td>
<td>Boxes:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Sermanet et al, “Integrated Recognition, Localization and</td>
<td>4096</td>
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
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>1000 x 4</td>
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
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image105.jpeg){width="0.5819444444444445in"
height="5.208880139982502e-3in"}

Detection using Convolutional Networks", ICLR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 23 1 Feb 2016
>
> ![](media/image107.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image108.jpeg){width="4.834027777777778in"
height="2.2756944444444445in"}

> Network input:

![](media/image109.jpeg){width="1.7513888888888889in"
height="0.5951388888888889in"}

> 3 x 221 x 221 Larger image:
>
> 3 x 257 x 257

![](media/image110.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 24 1 Feb 2016

> ![](media/image111.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image112.jpeg){width="7.752777777777778in"
height="1.8493055555555555in"}

> 0.5

![](media/image113.jpeg){width="1.7513888888888889in"
height="0.5951388888888889in"}

+----------------+-----------------+--------------------------+--+
| Network input: | > Larger image: | > Classification scores: |  |
+----------------+-----------------+--------------------------+--+
| 3 x 221 x 221  |                 |                          |  |
+----------------+-----------------+--------------------------+--+
|                | > 3 x 257 x 257 | > P(cat)                 |  |
+----------------+-----------------+--------------------------+--+

![](media/image114.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 25 1 Feb 2016

> ![](media/image116.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image117.jpeg){width="7.752777777777778in"
height="1.8493055555555555in"}

> 0.5 0.75

![](media/image118.jpeg){width="1.7513888888888889in"
height="0.5951388888888889in"}

+----------------+-----------------+--------------------------+--+
| Network input: | > Larger image: | > Classification scores: |  |
+----------------+-----------------+--------------------------+--+
| 3 x 221 x 221  |                 |                          |  |
+----------------+-----------------+--------------------------+--+
|                | > 3 x 257 x 257 | > P(cat)                 |  |
+----------------+-----------------+--------------------------+--+

![](media/image119.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 26 1 Feb 2016

> ![](media/image121.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image122.jpeg){width="1.9916666666666667in"
height="1.8423611111111111in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>0.5</td>
<td>0.75</td>
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
<td>0.6</td>
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
<td>Network input:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Classification scores:</p>
</blockquote></td>
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
<td><blockquote>
<p>Larger image:</p>
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
<td>3 x 221 x 221</td>
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
<td><blockquote>
<p>3 x 257 x 257</p>
</blockquote></td>
<td></td>
<td>P(cat)</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image123.jpeg){width="10.0in" height="3.557638888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 27 1 Feb 2016

> ![](media/image124.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image125.jpeg){width="2.002083333333333in"
height="1.8423611111111111in"}

+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          | 0.5 | 0.75 |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          | 0.6 | 0.8  |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
| Network input: |                 |  |  | > Classification scores: |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                | > Larger image: |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
| 3 x 221 x 221  |                 |  |  |                          |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+
|                | > 3 x 257 x 257 |  |  | P(cat)                   |     |      |  |  |
+----------------+-----------------+--+--+--------------------------+-----+------+--+--+

![](media/image126.jpeg){width="10.0in" height="3.557638888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 28 1 Feb 2016

> ![](media/image127.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image128.jpeg){width="1.9916666666666667in"
height="1.8423611111111111in"}

<table>
<tbody>
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
<td>0.5</td>
<td>0.75</td>
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
<td>0.6</td>
<td>0.8</td>
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
<td>Network input:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Classification scores:</p>
</blockquote></td>
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
<td><blockquote>
<p>Larger image:</p>
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
<tr class="odd">
<td>3 x 221 x 221</td>
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
<td><blockquote>
<p>3 x 257 x 257</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>P(cat)</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image129.jpeg){width="10.0in" height="3.557638888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 29 1 Feb 2016

> ![](media/image130.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image131.jpeg){width="2.5875in" height="0.7173611111111111in"}

> Greedily merge boxes and
>
> scores (details in paper)

![](media/image132.jpeg){width="7.509027777777778in"
height="1.8493055555555555in"}

> 0.8

![](media/image133.jpeg){width="1.7513888888888889in"
height="0.5951388888888889in"}

+----------------+-----------------+---------+---------------------------+--+
| Network input: |                 |         | > Classification score: P |  |
+----------------+-----------------+---------+---------------------------+--+
|                | > Larger image: |         |                           |  |
+----------------+-----------------+---------+---------------------------+--+
| 3 x 221 x 221  |                 |         |                           |  |
+----------------+-----------------+---------+---------------------------+--+
|                | > 3 x 257 x 257 | > (cat) |                           |  |
+----------------+-----------------+---------+---------------------------+--+

![](media/image134.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 30 1 Feb 2016

> ![](media/image136.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image137.jpeg){width="4.45in" height="0.9145833333333333in"}

> In practice use many sliding window locations and multiple scales
>
> Window positions + score maps ~Box\ regression\ outputs~ Final
> Predictions

![](media/image138.jpeg){width="9.280555555555555in"
height="1.9326388888888888in"}

Sermanet et al, "Integrated Recognition, Localization and Detection
using Convolutional Networks", ICLR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 31 1 Feb 2016
>
> ![](media/image140.jpeg){width="8.450694444444444in"
> height="0.9659722222222222in"}
>
> Image:
>
> 3 x 221 x 221

<table>
<tbody>
<tr class="odd">
<td>4096</td>
<td>4096</td>
<td><blockquote>
<p>Class scores:</p>
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
<td>1000</td>
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
<td>FC</td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image141.jpeg){width="7.174305555555556in" height="3.05625in"}

Convolution

![](media/image142.jpeg){width="0.5819444444444445in"
height="5.208880139982502e-3in"}

\+ pooling

> FC

![](media/image144.jpeg){width="0.14444444444444443in"
height="1.3840277777777779in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td><blockquote>
<p>FC</p>
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
<td>Feature map:</td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p>FC</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>1024 x 5 x 5</td>
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

![](media/image145.jpeg){width="2.5458333333333334in"
height="1.7027777777777777in"}

+------+------+------------+--+
| 4096 | 1024 | > Boxes:   |  |
+------+------+------------+--+
|      |      | > 1000 x 4 |  |
+------+------+------------+--+
|      |      |            |  |
+------+------+------------+--+

![](media/image147.jpeg){width="10.0in" height="1.1305555555555555in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 32 1 Feb 2016

> ![](media/image148.jpeg){width="9.175694444444444in"
> height="4.3597222222222225in"}
>
> Efficient sliding window by converting fully-connected layers into
> convolutions

+--------------+----------------+-----------------+--+
| 4096 x 1 x 1 | > 1024 x 1 x 1 | > Class scores: |  |
+--------------+----------------+-----------------+--+
|              |                | > 1000 x 1 x 1  |  |
+--------------+----------------+-----------------+--+

> Convolution
>
> \+ pooling
>
> Feature map:
>
> ~Image:~ 1024 x 5 x 5 3 x 221 x 221

+-----------+-----------+-----------+-----------+-----------+-----------+
| > 1 x 1   | > 1 x 1   |           |           |           |           |
| > conv    | > conv    |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 5 x 5     |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > conv    |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > 5 x 5   |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > conv    |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > 1 x 1   | > 1 x 1   |           |           |           |           |
| > conv    | > conv    |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > 4096 x  |           | > 1024 x  |           |           |           |
| > 1 x 1   |           | > 1 x 1   |           |           |           |
|           |           | > Box     |           |           |           |
|           |           | > coordin |           |           |           |
|           |           | ates:     |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           | > (4 x    |
|           |           |           |           |           | > 1000) x |
|           |           |           |           |           | > 1 x 1   |
+-----------+-----------+-----------+-----------+-----------+-----------+

![](media/image149.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 33 1 Feb 2016

> ![](media/image154.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image155.jpeg){width="8.654861111111112in"
height="3.688888888888889in"}

> **Training time:** Small image, 1 x 1 classifier output
>
> **Test time:** Larger image, 2 x 2 classifier output, only extra
> compute at yellow regions

![](media/image156.jpeg){width="10.0in" height="0.9395833333333333in"}

Sermanet et al, "Integrated Recognition, Localization and Detection
using Convolutional Networks", ICLR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 34 1 Feb 2016
>
> ![](media/image157.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image158.jpeg){width="9.209027777777777in"
height="3.892361111111111in"}

> **AlexNet**: Localization method not published
>
> **Overfeat**: Multiscale convolutional regression
>
> with box merging
>
> **VGG**: Same as Overfeat, but fewer scales
>
> and locations; simpler method, gains all due
>
> to deeper features
>
> **ResNet:** Different localization method (RPN)
>
> and much deeper features

![](media/image159.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 35 1 Feb 2016

> ![](media/image160.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image161.jpeg){width="9.586805555555555in"
height="2.8090277777777777in"}

<table>
<tbody>
<tr class="odd">
<td><strong>Classification</strong></td>
<td><blockquote>
<p><strong>Classification</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Object Detection</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Instance</strong></p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
</blockquote></td>
<td></td>
<td><blockquote>
<p><strong>Segmentation</strong></p>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image162.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 36 1 Feb 2016

> ![](media/image163.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image164.jpeg){width="9.586805555555555in"
height="2.8090277777777777in"}

<table>
<tbody>
<tr class="odd">
<td><strong>Classification</strong></td>
<td><blockquote>
<p><strong>Classification</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Object Detection</strong></p>
</blockquote></td>
<td><blockquote>
<p><strong>Instance</strong></p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
</blockquote></td>
<td></td>
<td><blockquote>
<p><strong>Segmentation</strong></p>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image165.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 37 1 Feb 2016

> ![](media/image166.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image167.jpeg){width="2.813888888888889in"
height="2.6569444444444446in"}

> DOG, (x, y, w, h)

![](media/image168.jpeg){width="2.463888888888889in"
height="1.854861111111111in"}

> CAT, (x, y, w, h)
>
> CAT, (x, y, w, h)

![](media/image169.jpeg){width="2.1930555555555555in"
height="0.30416666666666664in"}

DUCK (x, y, w, h)

![](media/image170.jpeg){width="2.1708333333333334in"
height="5.208880139982502e-3in"}

> = 16 numbers

![](media/image171.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 38 1 Feb 2016

> ![](media/image172.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image173.jpeg){width="2.813888888888889in"
height="2.6569444444444446in"}

DOG, (x, y, w, h)

![](media/image174.jpeg){width="2.94375in"
height="1.9680555555555554in"}

> CAT, (x, y, w, h)

![](media/image175.jpeg){width="2.1930555555555555in"
height="0.30416666666666664in"}

> = 8 numbers

![](media/image176.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 39 1 Feb 2016

> ![](media/image178.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image179.jpeg){width="2.813888888888889in"
height="2.6569444444444446in"}

> CAT, (x, y, w, h)

![](media/image180.jpeg){width="3.3645833333333335in"
height="2.0708333333333333in"}

> CAT, (x, y, w, h)
>
> ....

![](media/image181.jpeg){width="2.1930555555555555in"
height="0.30416666666666664in"}

> CAT (x, y, w, h)

![](media/image182.jpeg){width="2.1708333333333334in"
height="5.208880139982502e-3in"}

= many numbers

> Need variable sized outputs

![](media/image183.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 40 1 Feb 2016

> ![](media/image184.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image185.jpeg){width="8.061111111111112in"
height="2.8305555555555557in"}

> **CAT? NO**

**DOG? NO**

![](media/image186.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 41 1 Feb 2016

> ![](media/image187.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image188.jpeg){width="8.061111111111112in"
height="2.8305555555555557in"}

**CAT? YES!**

> **DOG? NO**

![](media/image189.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 42 1 Feb 2016

> ![](media/image190.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image191.jpeg){width="8.061111111111112in"
height="2.8305555555555557in"}

> **CAT? NO**

**DOG? NO**

![](media/image192.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 43 1 Feb 2016

> ![](media/image193.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image194.jpeg){width="8.19513888888889in"
height="3.5416666666666665in"}

> **Problem**: Need to test many positions and scales
>
> **Solution:** If your classifier is fast enough, just do it

![](media/image195.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 44 1 Feb 2016

> ![](media/image196.jpeg){width="8.450694444444444in"
> height="4.572916666666667in"}

![](media/image197.jpeg){width="10.0in" height="0.9756944444444444in"}

Dalal and Triggs, "Histograms of Oriented Gradients for Human
Detection", CVPR 2005 Slide credit: Ross Girshick

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 45 1 Feb 2016
>
> ![](media/image198.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image199.jpeg){width="10.0in" height="4.590277777777778in"}

Felzenszwalb et al, "Object Detection with Discriminatively

Trained Part Based Models", PAMI 2010

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 46 1 Feb 2016
>
> ![](media/image200.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image201.jpeg){width="9.777777777777779in"
height="2.0569444444444445in"}

Girschick et al, "Deformable Part Models are Convolutional Neural
Networks", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 47 1 Feb 2016
>
> ![](media/image203.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image204.jpeg){width="9.3875in" height="3.5416666666666665in"}

> **Problem**: Need to test many positions and scales, and use a
> computationally demanding classifier (CNN)
>
> **Solution:** Only look at a tiny subset of possible positions

![](media/image205.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 48 1 Feb 2016

> ![](media/image206.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image207.jpeg){width="7.732638888888889in" height="1.06875in"}

-   Find "blobby" image regions that are likely to contain objects

-   "Class-agnostic" object detector

-   Look for "blob-like" regions

![](media/image208.jpeg){width="10.0in" height="3.123611111111111in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 49 1 Feb 2016

> ![](media/image209.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image210.jpeg){width="7.1305555555555555in"
height="0.41041666666666665in"}

Bottom-up segmentation, merging regions at multiple scales

![](media/image211.jpeg){width="1.1430555555555555in"
height="5.208880139982502e-3in"}

> Convert

![](media/image214.jpeg){width="5.208880139982502e-3in"
height="0.3284722222222222in"}

> regions
>
> to boxes

![](media/image217.jpeg){width="10.0in" height="0.9048611111111111in"}

> Uijlings et al, "Selective Search for Object Recognition", IJCV 2013

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 50 1 Feb 2016

> ![](media/image218.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image219.jpeg){width="9.261805555555556in" height="3.15in"}

> Hosang et al, "What makes for effective detection proposals?", PAMI
> 2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 51 1 Feb 2016

> ![](media/image221.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image222.jpeg){width="10.0in" height="0.9048611111111111in"}

> Hosang et al, "What makes for effective detection proposals?", PAMI
> 2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 52 1 Feb 2016

> ![](media/image224.jpeg){width="9.769444444444444in"
> height="4.947916666666667in"}
>
> Girschick et al, "Rich feature hierarchies for accurate object
> detection and semantic segmentation", CVPR 2014
>
> Slide credit: Ross Girschick

![](media/image225.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 53 1 Feb 2016

> ![](media/image226.jpeg){width="9.472222222222221in"
> height="1.6041666666666667in"}
>
> **Step 1**: Train (or download) a classification model for ImageNet
> (AlexNet)

![](media/image227.jpeg){width="7.977777777777778in"
height="2.4763888888888888in"}

> Convolution
>
> ~and\ Pooling~ Fully-connected
>
> layers
>
> Softmax loss

![](media/image228.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+----------------+--+--+--+
|       | > Final conv  |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               | > Class scores |  |  |  |
+-------+---------------+----------------+--+--+--+
| Image | > feature map |                |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               | > 1000 classes |  |  |  |
+-------+---------------+----------------+--+--+--+
|       |               |                |  |  |  |
+-------+---------------+----------------+--+--+--+

![](media/image233.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 54 1 Feb 2016

> ![](media/image234.jpeg){width="9.472222222222221in"
> height="4.858333333333333in"}
>
> **Step 2**: Fine-tune model for detection

-   Instead of 1000 ImageNet classes, want 20 object classes +
    > background

-   Throw away final fully-connected layer, reinitialize from scratch

-   Keep training model using positive / negative regions from detection
    > images

+---------------+-------------------+-----------------------------+--+
| Convolution   |                   | > Re-initialize this layer: |  |
+---------------+-------------------+-----------------------------+--+
|               | > Fully-connected | > was 4096 x 1000,          |  |
+---------------+-------------------+-----------------------------+--+
| > and Pooling |                   | > now will be 4096 x 21     |  |
+---------------+-------------------+-----------------------------+--+
|               | > layers          |                             |  |
+---------------+-------------------+-----------------------------+--+
|               |                   |                             |  |
+---------------+-------------------+-----------------------------+--+

> Softmax loss

![](media/image235.jpeg){width="0.3284722222222222in"
height="5.208880139982502e-3in"}

+-------+---------------+-----------------+--+--+--+
|       | > Final conv  |                 |  |  |  |
+-------+---------------+-----------------+--+--+--+
|       |               | > Class scores: |  |  |  |
+-------+---------------+-----------------+--+--+--+
| Image | > feature map |                 |  |  |  |
+-------+---------------+-----------------+--+--+--+
|       |               | > 21 classes    |  |  |  |
+-------+---------------+-----------------+--+--+--+
|       |               |                 |  |  |  |
+-------+---------------+-----------------+--+--+--+

![](media/image240.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 55 1 Feb 2016

> ![](media/image241.jpeg){width="9.472222222222221in"
> height="2.361111111111111in"}
>
> **Step 3**: Extract features

-   Extract region proposals for all images

-   For each region: warp to CNN input size, run forward through CNN,
    > save pool5 features to disk

-   Have a big hard drive: features are \~200GB for PASCAL dataset!

![](media/image242.jpeg){width="1.5993055555555555in"
height="0.6256944444444444in"}

> Convolution
>
> and Pooling

![](media/image243.jpeg){width="9.620138888888889in"
height="1.8368055555555556in"}

> pool5 features

![](media/image245.jpeg){width="5.473611111111111in"
height="0.43472222222222223in"}

> ^Image^ Region Proposals Crop + Warp Forward pass Save to disk

![](media/image246.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 56 1 Feb 2016

> ![](media/image247.jpeg){width="9.472222222222221in"
> height="1.2381944444444444in"}
>
> **Step 4**: Train one binary SVM per class to classify region features

![](media/image248.jpeg){width="9.20138888888889in"
height="1.0256944444444445in"}

> Training image regions

![](media/image249.jpeg){width="8.7in" height="1.0131944444444445in"}

> Cached region features

![](media/image250.jpeg){width="7.006944444444445in" height="1.0in"}

Positive samples for cat SVM Negative samples for cat SVM

![](media/image251.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 57 1 Feb 2016

> ![](media/image252.jpeg){width="9.472222222222221in"
> height="1.2381944444444444in"}
>
> **Step 4**: Train one binary SVM per class to classify region features

![](media/image253.jpeg){width="9.20138888888889in"
height="1.0256944444444445in"}

> Training image regions

![](media/image254.jpeg){width="8.7in" height="1.0131944444444445in"}

> Cached region features

![](media/image255.jpeg){width="7.00625in" height="1.0in"}

Negative samples for dog SVM Positive samples for dog SVM

![](media/image256.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 58 1 Feb 2016

> ![](media/image257.jpeg){width="9.881944444444445in"
> height="1.3916666666666666in"}
>
> **Step 5** (bbox regression): For each class, train a linear
> regression model to map from cached features to offsets to GT boxes to
> make up for "slightly wrong" proposals

![](media/image258.jpeg){width="8.28125in"
height="1.0263888888888888in"}

> Training image regions

![](media/image259.jpeg){width="2.2618055555555556in"
height="0.41805555555555557in"}

> Cached region features

![](media/image263.jpeg){width="8.709722222222222in" height="0.93125in"}

+------------------------+------------------+----------------+---------------------+
| Regression targets     | (0, 0, 0, 0)     | (.25, 0, 0, 0) | > (0, 0, -0.125, 0) |
+------------------------+------------------+----------------+---------------------+
| (dx, dy, dw, dh)       | Proposal is good | Proposal too   | > Proposal too      |
+------------------------+------------------+----------------+---------------------+
| Normalized coordinates |                  | far to left    | > wide              |
+------------------------+------------------+----------------+---------------------+

![](media/image264.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 59 1 Feb 2016

> ![](media/image265.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

+------------------+--------+---------------+-----------+--+
|                  | PASCAL | ImageNet      | > MS-COCO |  |
+------------------+--------+---------------+-----------+--+
|                  | VOC    | Detection     |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               | (2014)    |  |
+------------------+--------+---------------+-----------+--+
|                  | (2010) | (ILSVRC 2014) |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
| Number of        | 20     | **200**       | 80        |  |
+------------------+--------+---------------+-----------+--+
| classes          |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
| Number of        |        | **\~470k**    |           |  |
+------------------+--------+---------------+-----------+--+
| images (train +  | \~20k  |               | \~120k    |  |
+------------------+--------+---------------+-----------+--+
| val)             |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
| Mean objects per | 2.4    | 1.1           | **7.2**   |  |
+------------------+--------+---------------+-----------+--+
| image            |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+
|                  |        |               |           |  |
+------------------+--------+---------------+-----------+--+

![](media/image266.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 60 1 Feb 2016

> ![](media/image267.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image268.jpeg){width="5.790277777777778in"
height="4.039583333333334in"}

> We use a metric called "mean average precision" (mAP)
>
> Compute average precision (AP) separately for each class, then average
> over classes
>
> A detection is a true positive if it has IoU with a ground-truth box
> greater than some threshold (usually 0.5) (mAP\@0.5)
>
> Combine all detections from all test images to draw a precision /
> recall curve for each class; AP is area under the curve
>
> TL;DR mAP is a number from 0 to 100; high is good

![](media/image269.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 61 1 Feb 2016

> ![](media/image270.jpeg){width="8.450694444444444in"
> height="4.580555555555556in"}

![](media/image271.jpeg){width="10.0in" height="0.9048611111111111in"}

> Wang et al, "Regionlets for Generic Object Detection", ICCV 2013

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 62 1 Feb 2016

+---------------+----------------------------+--+
| R-CNN Results | > Big improvement compared |  |
+---------------+----------------------------+--+
|               |                            |  |
+---------------+----------------------------+--+
|               | > to pre-CNN methods       |  |
+---------------+----------------------------+--+

![](media/image272.jpeg){width="8.450694444444444in"
height="4.580555555555556in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 63 1 Feb 2016

+---------------+---------------------------+--+
| R-CNN Results | > Bounding box regression |  |
+---------------+---------------------------+--+
|               |                           |  |
+---------------+---------------------------+--+
|               | > helps a bit             |  |
+---------------+---------------------------+--+

![](media/image274.jpeg){width="8.450694444444444in"
height="4.580555555555556in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 64 1 Feb 2016

+---------------+--------------------------+--+
| R-CNN Results | > Features from a deeper |  |
+---------------+--------------------------+--+
|               |                          |  |
+---------------+--------------------------+--+
|               | > network help a lot     |  |
+---------------+--------------------------+--+

![](media/image276.jpeg){width="8.450694444444444in"
height="4.580555555555556in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 65 1 Feb 2016

> ![](media/image278.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image279.jpeg){width="8.525694444444444in"
height="3.9159722222222224in"}

1.  Slow at test-time: need to run full forward pass of CNN for each
    > region proposal

2.  SVMs and regressors are post-hoc: CNN features not updated in
    > response to SVMs and regressors

3.  Complex multistage training pipeline

![](media/image280.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 66 1 Feb 2016

![](media/image281.jpeg){width="9.850694444444445in"
height="4.975694444444445in"}

> Girschick, "Fast R-CNN", ICCV 2015
>
> Slide credit: Ross Girschick

![](media/image282.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 67 1 Feb 2016

> ![](media/image283.jpeg){width="9.893055555555556in"
> height="4.975694444444445in"}: Slow at test-time due to independent
> forward passes of the CNN

![](media/image284.jpeg){width="2.779166666666667in"
height="2.372916666666667in"}

> **Solution:**
>
> Share computation of convolutional layers between proposals for an
> image

![](media/image285.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 68 1 Feb 2016

> ![](media/image286.jpeg){width="9.654861111111112in"
> height="4.990972222222222in"}: Post-hoc training: CNN not updated in
> response to final classifiers and regressors
>
> **R-CNN Problem \#3:**
>
> Complex training pipeline
>
> **Solution:**
>
> Just train the whole system end-to-end all at once!
>
> Slide credit: Ross Girschick

![](media/image287.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 69 1 Feb 2016

> ![](media/image288.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image289.jpeg){width="4.483333333333333in"
height="2.073611111111111in"}

+---------------+-------------------+--+--------+--+--+--+--+--+
| Convolution   | > Fully-connected |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
| > and Pooling |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  | layers |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+
|               |                   |  |        |  |  |  |  |  |
+---------------+-------------------+--+--------+--+--+--+--+--+

![](media/image291.jpeg){width="9.540277777777778in"
height="2.3555555555555556in"}

Hi-res input image:

3 x 800 x 600

with region

proposal

+-----------------------+--------------------------------+
| Hi-res conv features: | > **Problem**: Fully-connected |
+-----------------------+--------------------------------+
| C x H x W             | > layers expect low-res conv   |
+-----------------------+--------------------------------+
| with region proposal  | > features: C x h x w          |
+-----------------------+--------------------------------+

![](media/image292.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 70 1 Feb 2016

> ![](media/image293.jpeg){width="9.345833333333333in"
> height="3.129166666666667in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td><blockquote>
<p>Project region proposal</p>
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
<td>Convolution</td>
<td><blockquote>
<p>onto conv feature map</p>
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
<tr class="odd">
<td></td>
<td></td>
<td><blockquote>
<p>Fully-connected</p>
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
<td><blockquote>
<p>and Pooling</p>
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
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td>layers</td>
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

![](media/image294.jpeg){width="9.540277777777778in" height="1.05in"}

Hi-res input image:

3 x 800 x 600

with region

proposal

+-----------------------+--------------------------------+
| Hi-res conv features: | > **Problem**: Fully-connected |
+-----------------------+--------------------------------+
| C x H x W             | > layers expect low-res conv   |
+-----------------------+--------------------------------+
| with region proposal  | > features: C x h x w          |
+-----------------------+--------------------------------+

![](media/image295.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 71 1 Feb 2016

> ![](media/image296.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image297.jpeg){width="6.7965277777777775in"
height="2.167361111111111in"}

<table>
<tbody>
<tr class="odd">
<td>Convolution</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Divide projected</p>
</blockquote></td>
<td><blockquote>
<p>Fully-connected</p>
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
<td></td>
<td><blockquote>
<p>region into h x w grid</p>
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
<tr class="odd">
<td><blockquote>
<p>and Pooling</p>
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
<td>layers</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image298.jpeg){width="9.540277777777778in"
height="3.0902777777777777in"}

Hi-res input image:

3 x 800 x 600

with region

proposal

+-----------------------+--------------------------------+
| Hi-res conv features: | > **Problem**: Fully-connected |
+-----------------------+--------------------------------+
| C x H x W             | > layers expect low-res conv   |
+-----------------------+--------------------------------+
| with region proposal  | > features: C x h x w          |
+-----------------------+--------------------------------+

![](media/image307.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 72 1 Feb 2016

> ![](media/image308.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image309.jpeg){width="6.605555555555555in"
height="2.338888888888889in"}

+---------------+-------------------+--+
|               | > Max-pool within |  |
+---------------+-------------------+--+
| Convolution   | > each grid cell  |  |
+---------------+-------------------+--+
| > and Pooling | > Fully-connected |  |
+---------------+-------------------+--+
|               | > layers          |  |
+---------------+-------------------+--+
|               |                   |  |
+---------------+-------------------+--+

![](media/image310.jpeg){width="9.540277777777778in"
height="3.0902777777777777in"}

Hi-res input image:

3 x 800 x 600

with region

proposal

Hi-res conv features:

C x H x W

with region proposal

RoI conv features:

C x h x w

for region proposal

![](media/image312.jpeg){width="10.0in" height="0.5888888888888889in"}

Fully-connected layers expect low-res conv features: C x h x w

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 73 1 Feb 2016

> ![](media/image313.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image314.jpeg){width="6.9534722222222225in"
height="2.338888888888889in"}

+---------------+--------------------------+--+
|               | > Can back propagate     |  |
+---------------+--------------------------+--+
| Convolution   | > similar to max pooling |  |
+---------------+--------------------------+--+
| > and Pooling | > Fully-connected        |  |
+---------------+--------------------------+--+
|               | > layers                 |  |
+---------------+--------------------------+--+
|               |                          |  |
+---------------+--------------------------+--+

![](media/image315.jpeg){width="9.540277777777778in"
height="3.0902777777777777in"}

Hi-res input image:

3 x 800 x 600

with region

proposal

Hi-res conv features:

C x H x W

with region proposal

RoI conv features:

C x h x w

for region proposal

![](media/image317.jpeg){width="10.0in" height="0.5888888888888889in"}

Fully-connected layers expect low-res conv features: C x h x w

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 74 1 Feb 2016

> ![](media/image318.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

+---------+------------------+-------------+------------------+--+
|         |                  | > **R-CNN** | > **Fast R-CNN** |  |
+---------+------------------+-------------+------------------+--+
|         |                  |             |                  |  |
+---------+------------------+-------------+------------------+--+
| Faster! | > Training Time: | > 84 hours  | > **9.5 hours**  |  |
+---------+------------------+-------------+------------------+--+
|         |                  |             |                  |  |
+---------+------------------+-------------+------------------+--+
|         | > (Speedup)      | > 1x        | > **8.8x**       |  |
+---------+------------------+-------------+------------------+--+
|         |                  |             |                  |  |
+---------+------------------+-------------+------------------+--+
|         |                  |             |                  |  |
+---------+------------------+-------------+------------------+--+

![](media/image319.jpeg){width="10.0in" height="0.9972222222222222in"}

Using VGG-16 CNN on Pascal VOC 2007 dataset

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 75 1 Feb 2016

> ![](media/image321.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

+-----------+-----------------------+--------------+--------------------+--+
|           |                       | > **R-CNN**  | > **Fast R-CNN**   |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
| > Faster! | > Training Time:      | > 84 hours   | > **9.5 hours**    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           | > (Speedup)           | > 1x         | > **8.8x**         |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
| FASTER!   | > Test time per image | > 47 seconds | > **0.32 seconds** |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           | > (Speedup)           | > 1x         | > **146x**         |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+

![](media/image322.jpeg){width="10.0in" height="0.9972222222222222in"}

Using VGG-16 CNN on Pascal VOC 2007 dataset

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 76 1 Feb 2016

> ![](media/image325.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

+-----------+-----------------------+--------------+--------------------+--+
|           |                       | > **R-CNN**  | > **Fast R-CNN**   |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
| > Faster! | > Training Time:      | > 84 hours   | > **9.5 hours**    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           | > (Speedup)           | > 1x         | > **8.8x**         |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
| FASTER!   | > Test time per image | > 47 seconds | > **0.32 seconds** |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           | > (Speedup)           | > 1x         | > **146x**         |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+
| > Better! | > mAP (VOC 2007)      | > 66.0       | > **66.9**         |  |
+-----------+-----------------------+--------------+--------------------+--+
|           |                       |              |                    |  |
+-----------+-----------------------+--------------+--------------------+--+

![](media/image326.jpeg){width="10.0in" height="3.328472222222222in"}

Using VGG-16 CNN on Pascal VOC 2007 dataset

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 77 1 Feb 2016

> ![](media/image327.jpeg){width="8.450694444444444in"
> height="1.1472222222222221in"}
>
> Test-time speeds don't include region proposals

+-------------------------+--------------+--------------------+--+
|                         | > **R-CNN**  | > **Fast R-CNN**   |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > Test time per image   | > 47 seconds | > **0.32 seconds** |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > (Speedup)             | > 1x         | > **146x**         |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > Test time per image   | > 50 seconds | > **2 seconds**    |  |
+-------------------------+--------------+--------------------+--+
| > with Selective Search |              |                    |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > (Speedup)             | > 1x         | > **25x**          |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+

![](media/image328.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 78 1 Feb 2016

> ![](media/image329.jpeg){width="8.450694444444444in"
> height="1.40625in"}~~Problem~~ Solution:
>
> Test-time speeds don't include region proposals Just make the CNN do
> region proposals too!

+-------------------------+--------------+--------------------+--+
|                         | > **R-CNN**  | > **Fast R-CNN**   |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > Test time per image   | > 47 seconds | > **0.32 seconds** |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > (Speedup)             | > 1x         | > **146x**         |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > Test time per image   | > 50 seconds | > **2 seconds**    |  |
+-------------------------+--------------+--------------------+--+
| > with Selective Search |              |                    |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+
| > (Speedup)             | > 1x         | > **25x**          |  |
+-------------------------+--------------+--------------------+--+
|                         |              |                    |  |
+-------------------------+--------------+--------------------+--+

![](media/image330.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 79 1 Feb 2016

> Faster R-CNN:
>
> Insert a **Region Proposal** **Network (RPN)** after the last
> convolutional layer

![](media/image331.jpeg){width="9.838194444444444in"
height="4.948611111111111in"}

> RPN trained to produce region proposals directly; no need for external
> region proposals!
>
> After RPN, use RoI Pooling and an upstream classifier and bbox
> regressor just like Fast R-CNN

Ren et al, "Faster R-CNN: Towards Real-Time Object Detection with Region
Proposal Networks", NIPS 2015

Slide credit: Ross Girschick

![](media/image332.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 80 1 Feb 2016

> ![](media/image333.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image334.jpeg){width="9.338888888888889in"
height="3.807638888888889in"}

> Slide a small window on the feature map

+-----------------+-----------------+-----------------+-----------------+
| Build a small   |                 |                 |                 |
| network for:    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| • classifying   | > 1 x 1 conv    | > 1 x 1 conv    |                 |
| object or       |                 |                 |                 |
| not-object, and |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| • regressing    |                 |                 |                 |
| bbox locations  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Position of the |                 | > 1 x 1 conv    |                 |
| sliding window  |                 |                 |                 |
| provides        |                 |                 |                 |
| localization    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| information     |                 |                 |                 |
| with reference  |                 |                 |                 |
| to the image    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Box regression  |                 |                 |                 |
| provides finer  |                 |                 |                 |
| localization    |                 |                 |                 |
| information     |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| with reference  |                 |                 |                 |
| to this sliding |                 |                 |                 |
| window          |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image335.jpeg){width="10.0in" height="0.9631944444444445in"}

Slide credit: Kaiming He

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 81 1 Feb 2016
>
> ![](media/image336.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image337.jpeg){width="9.26875in" height="3.73125in"}

> Use **N anchor boxes** at each location
>
> Anchors are **translation invariant**: use the same ones at every
> location

Regression gives offsets from anchor boxes

> Classification gives the probability that each (regressed) anchor
> shows an object

![](media/image338.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 82 1 Feb 2016

> ![](media/image339.jpeg){width="10.0in" height="5.5625in"}
>
> In the paper: Ugly pipeline

-   Use alternating optimization to train RPN, then Fast R-CNN with RPN
    > proposals, etc.

-   More complex than it has to be

> Since publication: Joint training!
>
> One network, four losses

-   RPN classification (anchor good / bad)

-   RPN regression (anchor -\> proposal)

-   Fast R-CNN classification (over classes)

-   Fast R-CNN regression (proposal -\> box)

Slide credit: Ross Girschick

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 83 1 Feb 2016
>
> ![](media/image340.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

+--------------------+--------------+------------------+--------------------+
|                    | > **R-CNN**  | > **Fast R-CNN** | > **Faster R-CNN** |
+--------------------+--------------+------------------+--------------------+
|                    |              |                  |                    |
+--------------------+--------------+------------------+--------------------+
| > Test time per    | > 50 seconds | > 2 seconds      | > **0.2 seconds**  |
+--------------------+--------------+------------------+--------------------+
| > image            |              |                  |                    |
+--------------------+--------------+------------------+--------------------+
| > (with proposals) |              |                  |                    |
+--------------------+--------------+------------------+--------------------+
|                    |              |                  |                    |
+--------------------+--------------+------------------+--------------------+
| > (Speedup)        | > 1x         | > 25x            | > **250x**         |
+--------------------+--------------+------------------+--------------------+
|                    |              |                  |                    |
+--------------------+--------------+------------------+--------------------+
| > mAP (VOC 2007)   | > 66.0       | > **66.9**       | > **66.9**         |
+--------------------+--------------+------------------+--------------------+
|                    |              |                  |                    |
+--------------------+--------------+------------------+--------------------+

![](media/image341.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 84 1 Feb 2016

> ![](media/image342.jpeg){width="8.450694444444444in"
> height="1.23125in"}
>
> ResNet 101 + Faster R-CNN + some extras

![](media/image343.jpeg){width="7.254166666666666in"
height="2.5618055555555554in"}

He et. al, "Deep Residual Learning for Image Recognition", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 85 1 Feb 2016
>
> ![](media/image345.jpeg){width="8.450694444444444in"
> height="4.854166666666667in"}

![](media/image346.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 86 1 Feb 2016

> ![](media/image347.jpeg){width="9.879861111111111in"
> height="4.888194444444444in"}
>
> Divide image into S x S grid
>
> Within each grid cell predict:
>
> B Boxes: 4 coordinates + confidence
>
> Class scores: C numbers
>
> Regression from image to 7 x 7 x (5 \* B + C) tensor
>
> Direct prediction using a CNN
>
> Redmon et al, "You Only Look Once:
>
> Unified, Real-Time Object Detection", arXiv 2015

![](media/image348.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 87 1 Feb 2016

> ![](media/image349.jpeg){width="9.547916666666667in"
> height="4.888194444444444in"}
>
> Faster than Faster R-CNN, but not as good
>
> Redmon et al, "You Only Look Once:
>
> Unified, Real-Time Object Detection", arXiv 2015

![](media/image350.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 88 1 Feb 2016

> ![](media/image351.jpeg){width="8.854166666666666in"
> height="4.730555555555555in"}
>
> **R-CNN**
>
> (Cafffe + MATLAB):
> [[https://github.com/rbgirshick/rcnn]{.underline}](https://github.com/rbgirshick/rcnn)
> Probably don't use this; too slow
>
> **Fast R-CNN**
>
> (Caffe + MATLAB):
> [[https://github.com/rbgirshick/fast-rcnn]{.underline}](https://github.com/rbgirshick/fast-rcnn)
>
> **Faster R-CNN**
>
> (Caffe + MATLAB):
> [[https://github.com/ShaoqingRen/faster\_rcnn]{.underline}](https://github.com/ShaoqingRen/faster_rcnn)
>
> (Caffe + Python):
> [[https://github.com/rbgirshick/py-faster-rcnn]{.underline}](https://github.com/rbgirshick/py-faster-rcnn)
>
> **YOLO**
>
> [[http://pjreddie.com/darknet/yolo/]{.underline}](http://pjreddie.com/darknet/yolo/)
>
> Maybe try this for projects?

![](media/image352.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 8 89 1 Feb 2016

![](media/image353.jpeg){width="9.657638888888888in"
height="4.930555555555555in"}

> Recap
>
> **Localization**:

-   Find a fixed number of objects (one or many)

-   L2 regression from CNN features to box coordinates

-   Much simpler than detection; consider it for your projects!

-   Overfeat: Regression + efficient sliding window with FC -\> conv
    > conversion

-   Deeper networks do better

<!-- -->

-   Find a variable number of objects by classifying image regions

-   Before CNNs: dense multiscale sliding window (HoG, DPM)

-   Avoid dense sliding window with region proposals

-   R-CNN: Selective Search + CNN classification / regression

-   Fast R-CNN: Swap order of convolutions and region extraction

-   Faster R-CNN: Compute region proposals within the network

-   Deeper networks do better

![](media/image354.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 8 90        | > 1 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
