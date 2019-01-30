![](media/image1.jpeg){width="9.73125in" height="4.50625in"}

Segmentation and Attention

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 1 24 Feb 2016

> ![](media/image3.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image4.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Assignment 3 due tonight!

-   We are reading your milestones

![](media/image5.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 2 24 Feb 2016

> ![](media/image6.jpeg){width="9.672222222222222in"
> height="4.752777777777778in"}
>
> **Caffe**

**Lasagne**

> **Torch**
>
> **Theano**
>
> **TensorFlow**

**Keras**

![](media/image7.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 3 24 Feb 2016

> ![](media/image8.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image9.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Segmentation

    -   Semantic Segmentation

    -   Instance Segmentation

-   (Soft) Attention

    -   Discrete locations

    -   Continuous locations (Spatial Transformers)

![](media/image10.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 4 24 Feb 2016

> ![](media/image11.jpeg){width="9.027777777777779in"
> height="4.557638888888889in"}

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 5 24 Feb 2016

> ![](media/image13.jpeg){width="10.0in" height="5.413888888888889in"}

New ImageNet Record today!

Szegedy et al, Inception-v4, Inception-ResNet and the Impact of Residual
Connections on Learning, arXiv 2016

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 6 24 Feb 2016
>
> ![](media/image14.jpeg){width="9.278472222222222in"
> height="4.427777777777778in"}
>
> 1x7, 7x1 filters
>
> Strided convolution AND max pooling
>
> V = Valid convolutions (no padding)
>
> 9 layers

![](media/image15.jpeg){width="10.0in" height="0.9354166666666667in"}

Szegedy et al, Inception-v4, Inception-ResNet and the Impact of Residual
Connections on Learning, arXiv 2016

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 7 24 Feb 2016
>
> ![](media/image16.jpeg){width="9.027777777777779in"
> height="4.427777777777778in"}
>
> 3 layers
>
> x4
>
> 4 x 3 layers
>
> 9 layers

![](media/image17.jpeg){width="10.0in" height="0.9354166666666667in"}

Szegedy et al, Inception-v4, Inception-ResNet and the Impact of Residual
Connections on Learning, arXiv 2016

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 8 24 Feb 2016
>
> ![](media/image18.jpeg){width="10.0in" height="5.413888888888889in"}
>
> 4 layers

+--------------+------+
| 5 x 7 layers | > x7 |
+--------------+------+

> 3 layers
>
> 4 x 3 layers
>
> 9 layers

Szegedy et al, Inception-v4, Inception-ResNet and the Impact of Residual
Connections on Learning, arXiv 2016

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 9 24 Feb 2016
>
> ![](media/image19.jpeg){width="9.47638888888889in"
> height="4.427777777777778in"}
>
> x3

  -------- -------------- --
           3 x 4 layers   
           4 layers       
  75       5 x 7 layers   
           3 layers       
  layers                  
           4 x 3 layers   
           9 layers       
  -------- -------------- --

![](media/image20.jpeg){width="10.0in" height="0.9354166666666667in"}

Szegedy et al, Inception-v4, Inception-ResNet and the Impact of Residual
Connections on Learning, arXiv 2016

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 10 24 Feb
> 2016
>
> ![](media/image22.jpeg){width="9.027777777777779in"
> height="4.7131944444444445in"}
>
> 9 layers

![](media/image23.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 11 24 Feb 2016

> ![](media/image24.jpeg){width="9.027777777777779in"
> height="4.74375in"}

3 layers

> 5 x 4 layers
>
> 9 layers

x7

![](media/image25.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 12 24 Feb 2016

> ![](media/image26.jpeg){width="9.027777777777779in"
> height="4.7131944444444445in"}
>
> 3 layers

+---------------+-------+--+
| 10 x 4 layers | > x10 |  |
+---------------+-------+--+
|               |       |  |
+---------------+-------+--+
| 3 layers      |       |  |
+---------------+-------+--+

> 5 x 4 layers
>
> 9 layers

![](media/image27.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 13 24 Feb 2016

> ![](media/image28.jpeg){width="9.51388888888889in"
> height="4.7131944444444445in"}

+------------------+-------+--+
| 5 x 4 layers     | > x 5 |  |
+------------------+-------+--+
|                  |       |  |
+------------------+-------+--+
| 3 layers         |       |  |
+------------------+-------+--+
| 75 10 x 4 layers |       |  |
+------------------+-------+--+

layers

> 3 layers
>
> 5 x 3 layers
>
> 9 layers

![](media/image29.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 14 24 Feb
> 2016
>
> ![](media/image30.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image31.jpeg){width="4.333333333333333in"
height="3.308333333333333in"}

> Residual and non-residual converge to
>
> similar value, but residual learns faster

![](media/image32.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 15 24 Feb 2016

> ![](media/image33.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image34.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Segmentation

    -   Semantic Segmentation

    -   Instance Segmentation

-   (Soft) Attention

    -   Discrete locations

    -   Continuous locations (Spatial Transformers)

![](media/image35.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 16 24 Feb 2016

![](media/image36.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

Segmentation

![](media/image37.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 17 24 Feb 2016

> ![](media/image38.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image39.jpeg){width="9.586805555555555in"
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
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
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

![](media/image40.jpeg){width="9.582638888888889in"
height="0.4583333333333333in"}

> CAT CAT CAT, DOG, DUCK CAT, DOG, DUCK

![](media/image41.jpeg){width="10.0in" height="1.448611111111111in"}

> Single object Multiple objects

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 1818 24 Feb
2016

> ![](media/image42.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image43.jpeg){width="9.586805555555555in"
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
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
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

![](media/image44.jpeg){width="4.733333333333333in"
height="0.9159722222222222in"}

Lecture 8

![](media/image45.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 1919 24 Feb
2016

> ![](media/image46.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image47.jpeg){width="9.586805555555555in"
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
<tr class="even">
<td></td>
<td><blockquote>
<p><strong>+ Localization</strong></p>
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

![](media/image48.jpeg){width="2.111111111111111in"
height="0.5201388888888889in"}

> Today

![](media/image49.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 2020 24 Feb
2016

> ![](media/image50.jpeg){width="9.355555555555556in"
> height="4.476388888888889in"}
>
> Label every pixel!
>
> Don't differentiate instances (cows)
>
> Classic computer vision problem

![](media/image51.jpeg){width="10.0in" height="0.9013888888888889in"}

Figure credit: Shotton et al, "TextonBoost for Image Understanding:
Multi-Class Object Recognition and Segmentation by Jointly Modeling
Texture, Layout, and Context", IJCV 2007

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 21 24 Feb
> 2016
>
> ![](media/image52.jpeg){width="9.640972222222222in"
> height="4.463888888888889in"}
>
> Detect instances, give category, label pixels
>
> "simultaneous detection and segmentation" (SDS)

![](media/image53.jpeg){width="0.7986111111111112in"
height="5.208880139982502e-3in"}

> Lots of recent work
>
> (MS-COCO)

![](media/image54.jpeg){width="10.0in" height="0.9236111111111112in"}

> Figure credit: Dai et al, "Instance-aware Semantic Segmentation via
> Multi-task Network Cascades", arXiv 2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 22 24 Feb 2016

![](media/image55.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

Semantic Segmentation

![](media/image56.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 23 24 Feb 2016

> ![](media/image57.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image58.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 24 24 Feb 2016

> ![](media/image60.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image61.jpeg){width="1.8347222222222221in"
height="0.7479166666666667in"}

> Extract
>
> patch

![](media/image62.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 25 24 Feb 2016

> ![](media/image64.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image65.jpeg){width="3.7555555555555555in"
height="0.7479166666666667in"}

> Extract Run through
>
> patch a CNN

![](media/image66.jpeg){width="6.566666666666666in"
height="1.9458333333333333in"}

> CNN

![](media/image67.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 26 24 Feb 2016

> ![](media/image70.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image71.jpeg){width="5.729166666666667in"
height="0.7479166666666667in"}

> Extract Run through Classify
>
> patch a CNN center pixel

![](media/image72.jpeg){width="8.477777777777778in"
height="1.9458333333333333in"}

> CNN ![](media/image73.jpeg){width="0.6138888888888889in"
> height="0.22847222222222222in"} COW

![](media/image74.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 27 24 Feb 2016

> ![](media/image78.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image79.jpeg){width="5.729166666666667in"
height="0.7479166666666667in"}

> Extract Run through Classify
>
> patch a CNN center pixel

![](media/image80.jpeg){width="8.477777777777778in"
height="1.9458333333333333in"}

> CNN ![](media/image81.jpeg){width="0.6138888888888889in"
> height="0.22847222222222222in"} COW

![](media/image82.jpeg){width="4.477777777777778in"
height="2.3541666666666665in"}

> Repeat for
>
> every pixel

![](media/image84.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 28 24 Feb 2016

> ![](media/image85.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image86.jpeg){width="3.895138888888889in"
height="0.9652777777777778in"}

Run "fully convolutional" network

to get all pixels at once

![](media/image87.jpeg){width="9.420833333333333in"
height="1.8833333333333333in"}

Smaller output

+-----+------------------+--+
| CNN | > due to pooling |  |
+-----+------------------+--+
|     |                  |  |
+-----+------------------+--+

![](media/image88.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 29 24 Feb 2016

> ![](media/image93.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image94.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 30 24 Feb
> 2016
>
> ![](media/image96.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image97.jpeg){width="4.227777777777778in"
height="2.214583333333333in"}

> Resize image to
>
> multiple scales

![](media/image98.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 31 24 Feb
> 2016
>
> ![](media/image99.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image100.jpeg){width="6.735416666666667in"
height="2.3048611111111112in"}

+-----------------+---------------+--+
| Resize image to | > Run one CNN |  |
+-----------------+---------------+--+
|                 | > per scale   |  |
+-----------------+---------------+--+
| multiple scales |               |  |
+-----------------+---------------+--+
|                 |               |  |
+-----------------+---------------+--+

![](media/image101.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 32 24 Feb
> 2016
>
> ![](media/image102.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image103.jpeg){width="6.735416666666667in"
height="2.3048611111111112in"}

+-----------------+-------------------+--+
| Resize image to | > Run one CNN     |  |
+-----------------+-------------------+--+
|                 | > per scale       |  |
+-----------------+-------------------+--+
| multiple scales |                   |  |
+-----------------+-------------------+--+
|                 | > Upscale outputs |  |
+-----------------+-------------------+--+
|                 |                   |  |
+-----------------+-------------------+--+
|                 | > and concatenate |  |
+-----------------+-------------------+--+

![](media/image104.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 33 24 Feb
> 2016
>
> ![](media/image105.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image106.jpeg){width="7.473611111111111in"
height="3.2465277777777777in"}

+-----------------+-------------------+--+
| Resize image to | > Run one CNN     |  |
+-----------------+-------------------+--+
|                 | > per scale       |  |
+-----------------+-------------------+--+
| multiple scales |                   |  |
+-----------------+-------------------+--+
|                 | > Upscale outputs |  |
+-----------------+-------------------+--+
|                 |                   |  |
+-----------------+-------------------+--+
|                 | > and concatenate |  |
+-----------------+-------------------+--+

> External "bottom-up"
>
> segmentation

![](media/image107.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 34 24 Feb
> 2016
>
> ![](media/image108.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image109.jpeg){width="9.70625in"
height="3.2465277777777777in"}

+-----------------+-------------------+----------------------+--+
| Resize image to | > Run one CNN     |                      |  |
+-----------------+-------------------+----------------------+--+
|                 | > per scale       |                      |  |
+-----------------+-------------------+----------------------+--+
| multiple scales |                   |                      |  |
+-----------------+-------------------+----------------------+--+
|                 | > Upscale outputs |                      |  |
+-----------------+-------------------+----------------------+--+
|                 |                   |                      |  |
+-----------------+-------------------+----------------------+--+
|                 | > and concatenate | > Combine everything |  |
+-----------------+-------------------+----------------------+--+
|                 |                   | > for final outputs  |  |
+-----------------+-------------------+----------------------+--+

> External "bottom-up"
>
> segmentation

![](media/image110.jpeg){width="10.0in" height="0.9354166666666667in"}

Farabet et al, "Learning Hierarchical Features for Scene Labeling,"
TPAMI 2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 35 24 Feb
> 2016
>
> ![](media/image111.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image112.jpeg){width="3.077777777777778in"
height="2.0930555555555554in"}

> Apply CNN once to get labels

![](media/image113.jpeg){width="10.0in" height="0.9354166666666667in"}

Pinheiro and Collobert, "Recurrent Convolutional Neural Networks for
Scene Labeling", ICML 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 36 24 Feb
> 2016
>
> ![](media/image114.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image115.jpeg){width="3.1375in" height="3.0083333333333333in"}

> Apply CNN once to get labels
>
> Apply AGAIN to
>
> refine labels

![](media/image116.jpeg){width="10.0in" height="0.9354166666666667in"}

Pinheiro and Collobert, "Recurrent Convolutional Neural Networks for
Scene Labeling", ICML 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 37 24 Feb
> 2016
>
> ![](media/image117.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image118.jpeg){width="10.0in" height="4.386111111111111in"}

> Apply CNN once to get labels
>
> Apply AGAIN to
>
> refine labels
>
> And again!

Pinheiro and Collobert, "Recurrent Convolutional Neural Networks for
Scene Labeling", ICML 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 38 24 Feb
> 2016
>
> ![](media/image119.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Same CNN weights:
>
> **recurrent convolutional network**
>
> Apply CNN once to get labels
>
> Apply AGAIN to
>
> refine labels
>
> And again!

Pinheiro and Collobert, "Recurrent Convolutional Neural Networks for
Scene Labeling", ICML 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 39 24 Feb
> 2016
>
> ![](media/image120.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Same CNN weights:
>
> **recurrent convolutional network**
>
> Apply CNN once to get labels
>
> Apply AGAIN to
>
> refine labels
>
> And again! ![](media/image121.jpeg){width="5.379861111111111in"
> height="0.22847222222222222in"} More iterations improve results

![](media/image122.jpeg){width="5.363194444444445in"
height="5.208880139982502e-3in"}

Pinheiro and Collobert, "Recurrent Convolutional Neural Networks for
Scene Labeling", ICML 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 40 24 Feb
> 2016
>
> ![](media/image123.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image124.jpeg){width="10.0in" height="0.9354166666666667in"}

Long, Shelhamer, and Darrell, "Fully Convolutional Networks for Semantic
Segmentation", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 41 24 Feb
> 2016
>
> ![](media/image126.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image127.jpeg){width="5.405555555555556in"
height="3.2993055555555557in"}

> Learnable upsampling!

![](media/image128.jpeg){width="10.0in" height="0.9354166666666667in"}

Long, Shelhamer, and Darrell, "Fully Convolutional Networks for Semantic
Segmentation", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 42 24 Feb
> 2016
>
> ![](media/image129.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image130.jpeg){width="10.0in" height="0.9354166666666667in"}

Long, Shelhamer, and Darrell, "Fully Convolutional Networks for Semantic
Segmentation", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 43 24 Feb
> 2016
>
> ![](media/image132.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image133.jpeg){width="7.332638888888889in"
height="3.1319444444444446in"}

> "skip
>
> connections"

![](media/image134.jpeg){width="10.0in" height="0.9354166666666667in"}

Long, Shelhamer, and Darrell, "Fully Convolutional Networks for Semantic
Segmentation", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 44 24 Feb
> 2016
>
> ![](media/image135.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image136.jpeg){width="9.224305555555556in" height="3.35625in"}

> "skip
>
> connections"
>
> Skip connections = Better results

![](media/image137.jpeg){width="10.0in" height="0.9354166666666667in"}

Long, Shelhamer, and Darrell, "Fully Convolutional Networks for Semantic
Segmentation", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 45 24 Feb
> 2016
>
> ![](media/image138.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, stride 1 pad 1

![](media/image139.jpeg){width="5.383333333333334in"
height="2.188888888888889in"}

> Input: 4 x 4 Output: 4 x 4

![](media/image140.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 46 24 Feb 2016

> ![](media/image141.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, stride 1 pad 1

![](media/image142.jpeg){width="5.804166666666666in"
height="2.1284722222222223in"}

> Dot product
>
> between filter
>
> and input

![](media/image143.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 4 x 4 Output: 4 x 4

![](media/image145.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 47 24 Feb 2016

> ![](media/image146.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, stride 1 pad 1

![](media/image147.jpeg){width="5.804166666666666in"
height="2.1284722222222223in"}

> Dot product
>
> between filter
>
> and input

![](media/image148.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 4 x 4 Output: 4 x 4

![](media/image150.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 48 24 Feb 2016

> ![](media/image151.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, **stride 2** pad 1

![](media/image152.jpeg){width="5.383333333333334in"
height="2.1694444444444443in"}

> Input: 4 x 4 Output: 2 x 2

![](media/image153.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 49 24 Feb 2016

> ![](media/image154.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, stride 2 pad 1

![](media/image155.jpeg){width="5.385416666666667in"
height="2.1284722222222223in"}

> Dot product
>
> between filter
>
> and input

![](media/image156.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 4 x 4 Output: 2 x 2

![](media/image158.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 50 24 Feb 2016

> ![](media/image159.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> Typical 3 x 3 convolution, stride 2 pad 1

![](media/image160.jpeg){width="5.39375in"
height="2.1284722222222223in"}

> Dot product
>
> between filter
>
> and input

![](media/image161.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 4 x 4 Output: 2 x 2

![](media/image163.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 51 24 Feb 2016

> ![](media/image164.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> 3 x 3 "deconvolution", stride 2 pad 1

![](media/image165.jpeg){width="0.8479166666666667in"
height="0.86875in"}

> Input: 2 x 2 Output: 4 x 4

![](media/image168.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 52 24 Feb 2016

> ![](media/image169.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> 3 x 3 "deconvolution", stride 2 pad 1

![](media/image170.jpeg){width="4.955555555555556in"
height="2.1479166666666667in"}

> Input gives
>
> weight for
>
> filter

![](media/image171.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 2 x 2 Output: 4 x 4

![](media/image173.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 53 24 Feb 2016

> ![](media/image174.jpeg){width="9.027777777777779in"
> height="1.3597222222222223in"}
>
> 3 x 3 "deconvolution", stride 2 pad 1

![](media/image175.jpeg){width="4.971527777777778in"
height="2.1479166666666667in"}

> Input gives
>
> weight for
>
> filter

![](media/image176.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 2 x 2 Output: 4 x 4

![](media/image178.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 54 24 Feb 2016

> ![](media/image179.jpeg){width="9.027777777777779in"
> height="3.759027777777778in"}

+---------------------------------------+-------------------+--+
| 3 x 3 "deconvolution", stride 2 pad 1 | > Sum where       |  |
+---------------------------------------+-------------------+--+
|                                       | > output overlaps |  |
+---------------------------------------+-------------------+--+
|                                       |                   |  |
+---------------------------------------+-------------------+--+

![](media/image180.jpeg){width="1.5888888888888888in"
height="5.208880139982502e-3in"}

> Input gives
>
> weight for
>
> filter

![](media/image181.jpeg){width="1.7027777777777777in"
height="0.4215277777777778in"}

> Input: 2 x 2 Output: 4 x 4

![](media/image183.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 55 24 Feb 2016

> ![](media/image184.jpeg){width="9.468055555555555in"
> height="4.802777777777778in"}

+---------------------------------------+-------------------+--+
| 3 x 3 "deconvolution", stride 2 pad 1 | > Sum where       |  |
+---------------------------------------+-------------------+--+
|                                       | > output overlaps |  |
+---------------------------------------+-------------------+--+
|                                       |                   |  |
+---------------------------------------+-------------------+--+

> Same as backward pass for
>
> normal convolution!

![](media/image185.jpeg){width="1.5888888888888888in"
height="5.208880139982502e-3in"}

> Input gives
>
> weight for
>
> filter
>
> Input: 2 x 2 Output: 4 x 4

![](media/image186.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 56 24 Feb 2016

> ![](media/image187.jpeg){width="9.468055555555555in"
> height="4.802777777777778in"}

<table>
<tbody>
<tr class="odd">
<td></td>
<td></td>
<td><blockquote>
<p>3 x 3 “deconvolution”, stride 2 pad 1</p>
</blockquote></td>
<td><blockquote>
<p>Sum where</p>
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
<td><blockquote>
<p>output overlaps</p>
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
<p>Same as backward pass for</p>
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
<p>normal convolution!</p>
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
<p>“Deconvolution” is a bad</p>
</blockquote></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Input gives</p>
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
<td><blockquote>
<p>weight for</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>name, already defined as</p>
</blockquote></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>filter</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>“inverse of convolution”</p>
</blockquote></td>
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
<p><strong>Better names:</strong></p>
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
<p>convolution transpose,</p>
</blockquote></td>
<td></td>
</tr>
<tr class="odd">
<td>Input: 2 x 2</td>
<td><blockquote>
<p>Output: 4 x 4</p>
</blockquote></td>
<td><blockquote>
<p>backward strided convolution,</p>
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

![](media/image188.jpeg){width="1.5888888888888888in"
height="5.208880139982502e-3in"}

> 1/2 strided convolution,
>
> upconvolution

![](media/image189.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 57 24 Feb 2016

> ![](media/image190.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image191.jpeg){width="9.01736111111111in"
height="3.453472222222222in"}

> Im et al, "Generating images with recurrent adversarial networks",
> arXiv 2016

![](media/image192.jpeg){width="6.897916666666666in"
height="0.7326388888888888in"}

> Radford et al, "Unsupervised Representation Learning with Deep
>
> Convolutional Generative Adversarial Networks", ICLR 2016

![](media/image194.jpeg){width="10.0in" height="0.5888888888888889in"}

"Deconvolution" is a bad name, already defined as "inverse of
convolution"

**Better names:** convolution transpose, backward strided convolution,
1/2 strided convolution, upconvolution

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 58 24 Feb 2016

> ![](media/image195.jpeg){width="9.720833333333333in"
> height="4.802777777777778in"}
>
> Im et al, "Generating images with recurrent adversarial networks",
> arXiv 2016
>
> Radford et al, "Unsupervised Representation Learning with Deep
> Convolutional Generative Adversarial Networks", ICLR 2016

![](media/image196.jpeg){width="10.0in" height="0.5888888888888889in"}

Great explanation

in appendix

> "Deconvolution" is a bad name, already defined as "inverse of
> convolution"
>
> **Better names:** convolution transpose, backward strided convolution,
> 1/2 strided convolution, upconvolution

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 59 24 Feb 2016

> ![](media/image197.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image198.jpeg){width="7.6125in" height="2.020138888888889in"}

Noh et al, "Learning Deconvolution Network for Semantic Segmentation",
ICCV 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 60 24 Feb
> 2016
>
> ![](media/image200.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image201.jpeg){width="5.208880139982502e-3in"
height="0.6256944444444444in"}

> Normal VGG "Upside down" VGG

![](media/image204.jpeg){width="10.0in" height="1.0361111111111112in"}

Noh et al, "Learning Deconvolution Network for Semantic Segmentation",
ICCV 2015

6 days of training on Titan X...

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 61 24 Feb
> 2016

![](media/image205.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

Instance Segmentation

![](media/image206.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 62 24 Feb 2016

> ![](media/image207.jpeg){width="9.640972222222222in"
> height="4.463888888888889in"}
>
> Detect instances, give category, label pixels
>
> "simultaneous detection and segmentation" (SDS)

![](media/image208.jpeg){width="0.7986111111111112in"
height="5.208880139982502e-3in"}

> Lots of recent work
>
> (MS-COCO)

![](media/image209.jpeg){width="10.0in" height="0.9236111111111112in"}

> Figure credit: Dai et al, "Instance-aware Semantic Segmentation via
> Multi-task Network Cascades", arXiv 2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 63 24 Feb 2016

> ![](media/image210.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image211.jpeg){width="10.0in" height="0.9354166666666667in"}

Similar to R-CNN, but

with segments

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 64 24 Feb
> 2016

+-----------------------+-------------------------+
| Instance Segmentation | > with segments         |
+-----------------------+-------------------------+
|                       | > Similar to R-CNN, but |
+-----------------------+-------------------------+

![](media/image213.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> External
>
> Segment
>
> proposals

![](media/image215.jpeg){width="10.0in" height="0.9354166666666667in"}

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 65 24 Feb
> 2016

+-----------------------+-------------------------+
| Instance Segmentation | > with segments         |
+-----------------------+-------------------------+
|                       | > Similar to R-CNN, but |
+-----------------------+-------------------------+

![](media/image216.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> External
>
> Segment
>
> proposals

![](media/image218.jpeg){width="10.0in" height="0.9354166666666667in"}

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 66 24 Feb
> 2016

+-----------------------+-------------------------+
| Instance Segmentation | > with segments         |
+-----------------------+-------------------------+
|                       | > Similar to R-CNN, but |
+-----------------------+-------------------------+

![](media/image219.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> External
>
> Segment
>
> proposals
>
> Mask out background
>
> with mean image

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 67 24 Feb
> 2016

+-----------------------+-------------------------+
| Instance Segmentation | > with segments         |
+-----------------------+-------------------------+
|                       | > Similar to R-CNN, but |
+-----------------------+-------------------------+

![](media/image221.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> External
>
> Segment
>
> proposals
>
> Mask out background
>
> with mean image

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 68 24 Feb
> 2016

+-----------------------+-------------------------+
| Instance Segmentation | > with segments         |
+-----------------------+-------------------------+
|                       | > Similar to R-CNN, but |
+-----------------------+-------------------------+

![](media/image223.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> External
>
> Segment
>
> proposals
>
> Mask out background
>
> with mean image

Hariharan et al, "Simultaneous Detection and Segmentation", ECCV 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 69 24 Feb
> 2016
>
> ![](media/image225.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image226.jpeg){width="10.0in" height="0.9354166666666667in"}

Hariharan et al, "Hypercolumns for Object Segmentation and Fine-grained
Localization", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 70 24 Feb
> 2016
>
> ![](media/image228.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image229.jpeg){width="10.0in" height="4.324305555555555in"}

Hariharan et al, "Hypercolumns for Object Segmentation and Fine-grained
Localization", CVPR 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 71 24 Feb
> 2016
>
> ![](media/image230.jpeg){width="9.414583333333333in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN
>
> Won COCO 2015
>
> challenge
>
> (with ResNet)

![](media/image231.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 72 24 Feb
> 2016
>
> ![](media/image232.jpeg){width="9.414583333333333in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN
>
> Won COCO 2015
>
> challenge
>
> (with ResNet)

![](media/image233.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 73 24 Feb
> 2016
>
> ![](media/image234.jpeg){width="9.414583333333333in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN

Region proposal network (RPN)

> Won COCO 2015
>
> challenge
>
> (with ResNet)

![](media/image235.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 74 24 Feb
> 2016
>
> ![](media/image236.jpeg){width="9.414583333333333in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN

Region proposal network (RPN)

> Reshape boxes to
>
> fixed size,
>
> figure / ground
>
> logistic regression
>
> Won COCO 2015
>
> challenge
>
> (with ResNet)

![](media/image237.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 75 24 Feb
> 2016
>
> ![](media/image238.jpeg){width="9.414583333333333in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN
>
> Won COCO 2015 challenge (with ResNet)

Region proposal network (RPN)

> Reshape boxes to
>
> fixed size,
>
> figure / ground
>
> logistic regression
>
> Mask out background,
>
> predict object class

![](media/image239.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 76 24 Feb
> 2016
>
> ![](media/image240.jpeg){width="9.473611111111111in"
> height="4.389583333333333in"}
>
> Similar to
>
> Faster R-CNN
>
> Won COCO 2015 challenge (with ResNet)

Region proposal network (RPN)

Reshape boxes to Learn entire model

> fixed size, end-to-end!
>
> figure / ground
>
> logistic regression
>
> Mask out background,
>
> predict object class

![](media/image241.jpeg){width="10.0in" height="0.9354166666666667in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 77 24 Feb
> 2016
>
> ![](media/image242.jpeg){width="10.0in" height="5.413888888888889in"}

Dai et al, "Instance-aware Semantic Segmentation via Multi-task Network
Cascades", arXiv 2015

**Predictions** **Ground truth**

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 78 24 Feb
> 2016
>
> ![](media/image243.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image244.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Semantic segmentation

    -   Classify all pixels

    -   Fully convolutional models, downsample then upsample

    -   Learnable upsampling: fractionally strided convolution

    -   Skip connections can help

-   Instance Segmentation

    -   Detect instance, generate mask

    -   Similar pipelines to object detection

![](media/image245.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 79 24 Feb 2016

![](media/image246.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

Attention Models

![](media/image247.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 80 24 Feb 2016

> ![](media/image248.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image249.jpeg){width="1.2375in" height="1.8875in"}

Image:

> H x W x 3

![](media/image250.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 81 24 Feb 2016

> ![](media/image251.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image252.jpeg){width="2.847916666666667in" height="1.8875in"}

> CNN

![](media/image253.jpeg){width="1.1076388888888888in" height="0.7125in"}

> ^Image:^ Features:
>
> H x W x 3 ~D~

![](media/image254.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 82 24 Feb 2016

> ![](media/image255.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image256.jpeg){width="4.254166666666666in" height="1.8875in"}

> CNN h0

![](media/image257.jpeg){width="2.4972222222222222in" height="1.45in"}

+-----------+-------------+-----------------+
| Image:    | > Features: | > Hidden state: |
+-----------+-------------+-----------------+
| H x W x 3 | > D         | > H             |
+-----------+-------------+-----------------+

![](media/image259.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 83 24 Feb 2016

> ![](media/image260.jpeg){width="9.027777777777779in"
> height="1.3722222222222222in"}
>
> Distribution
>
> over vocab

![](media/image261.jpeg){width="0.44722222222222224in"
height="0.5875in"}

> d1

![](media/image262.jpeg){width="2.4055555555555554in" height="1.8875in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<tr class="even">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>h0</td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
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
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Image:</td>
<td></td>
<td></td>
<td></td>
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
<td>Features:</td>
<td>Hidden state:</td>
<td></td>
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
<td>H x W x 3</td>
<td>D</td>
<td></td>
<td>H</td>
<td></td>
<td><blockquote>
<p>y1</p>
</blockquote></td>
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

![](media/image265.jpeg){width="3.495833333333333in"
height="2.3027777777777776in"}

> First
>
> word

![](media/image267.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 84 24 Feb 2016

> ![](media/image268.jpeg){width="9.027777777777779in"
> height="1.3722222222222222in"}
>
> Distribution
>
> over vocab

![](media/image269.jpeg){width="0.44722222222222224in"
height="0.5875in"}

> d1 d2

![](media/image271.jpeg){width="2.4055555555555554in" height="1.8875in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td>h0</td>
<td></td>
<td></td>
<td></td>
<td>h1</td>
<td></td>
<td></td>
<td></td>
<td>h2</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Image:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td>Features:</td>
<td>Hidden state:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>H x W x 3</td>
<td>D</td>
<td></td>
<td>H</td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td>First</td>
<td></td>
<td></td>
<td><blockquote>
<p>Second</p>
</blockquote></td>
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
<td>word</td>
<td></td>
<td></td>
<td></td>
<td>word</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image276.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 85 24 Feb 2016

> ![](media/image279.jpeg){width="9.2875in"
> height="1.3722222222222222in"}
>
> Distribution
>
> over vocab

![](media/image280.jpeg){width="0.44722222222222224in"
height="0.5875in"}

> d1 d2

![](media/image282.jpeg){width="2.4055555555555554in" height="1.8875in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td>h0</td>
<td></td>
<td></td>
<td></td>
<td>h1</td>
<td></td>
<td></td>
<td></td>
<td>h2</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Image:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td>Features:</td>
<td>Hidden state:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>H x W x 3</td>
<td>D</td>
<td></td>
<td>H</td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td>First</td>
<td></td>
<td></td>
<td><blockquote>
<p>Second</p>
</blockquote></td>
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
<td>word</td>
<td></td>
<td></td>
<td></td>
<td>word</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image287.jpeg){width="10.0in" height="0.5888888888888889in"}

RNN only looks at whole image, once

![](media/image290.jpeg){width="0.13055555555555556in"
height="0.13055555555555556in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 86 24 Feb 2016

> ![](media/image291.jpeg){width="9.2875in"
> height="1.3722222222222222in"}
>
> Distribution
>
> over vocab

![](media/image292.jpeg){width="0.44722222222222224in"
height="0.5875in"}

> d1 d2

![](media/image294.jpeg){width="2.4055555555555554in" height="1.8875in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td>h0</td>
<td></td>
<td></td>
<td></td>
<td>h1</td>
<td></td>
<td></td>
<td></td>
<td>h2</td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Image:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td>Features:</td>
<td>Hidden state:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>H x W x 3</td>
<td>D</td>
<td></td>
<td>H</td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td>First</td>
<td></td>
<td></td>
<td><blockquote>
<p>Second</p>
</blockquote></td>
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
<td>word</td>
<td></td>
<td></td>
<td></td>
<td>word</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image299.jpeg){width="10.0in" height="0.5888888888888889in"}

RNN only looks at whole image, once

![](media/image302.jpeg){width="0.13055555555555556in"
height="0.13055555555555556in"}

What if the RNN looks at different parts of the image at each timestep?

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 87 24 Feb 2016

> ![](media/image304.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image305.jpeg){width="3.3006944444444444in" height="1.8875in"}

> CNN
>
> Features:
>
> Image: ~L\ x\ D~
>
> H x W x 3

![](media/image306.jpeg){width="2.173611111111111in" height="0.6125in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image307.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 88 24 Feb
> 2016
>
> ![](media/image308.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image309.jpeg){width="4.254166666666666in" height="1.8875in"}

> CNN ![](media/image310.jpeg){width="0.4263888888888889in"
> height="0.15555555555555556in"} h0

![](media/image312.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Features:
>
> Image: ~L\ x\ D~
>
> H x W x 3

![](media/image314.jpeg){width="2.173611111111111in" height="0.6125in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image315.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 89 24 Feb
> 2016
>
> ![](media/image316.jpeg){width="9.027777777777779in"
> height="1.3472222222222223in"}
>
> L locations

![](media/image317.jpeg){width="0.44722222222222224in"
height="1.6916666666666667in"}

> a1

![](media/image318.jpeg){width="3.3006944444444444in" height="1.8875in"}

> CNN ![](media/image320.jpeg){width="0.4263888888888889in"
> height="0.15555555555555556in"} h0

![](media/image322.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Features:
>
> Image: ~L\ x\ D~
>
> H x W x 3

![](media/image324.jpeg){width="2.173611111111111in" height="0.6125in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image325.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 90 24 Feb
> 2016
>
> ![](media/image326.jpeg){width="9.027777777777779in"
> height="1.3472222222222223in"}
>
> L locations

![](media/image327.jpeg){width="5.301388888888889in"
height="3.3993055555555554in"}

CNN

Image:

> H x W x 3

Xu et al, "Show, Attend and Tell: Neural Image Caption Generation with
Visual Attention", ICML 2015

> a1

![](media/image328.jpeg){width="5.208880139982502e-3in"
height="0.43125in"}

> h0

![](media/image331.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

Features:

> L x D
>
> Weighted

z1

> features: D

Weighted

combination

of features

![](media/image332.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 91 24 Feb
> 2016
>
> ![](media/image333.jpeg){width="9.027777777777779in"
> height="1.3472222222222223in"}
>
> L locations

![](media/image334.jpeg){width="6.228472222222222in"
height="3.3993055555555554in"}

CNN

Image:

> H x W x 3

Xu et al, "Show, Attend and Tell: Neural Image Caption Generation with
Visual Attention", ICML 2015

> a1

![](media/image335.jpeg){width="5.208880139982502e-3in"
height="0.43125in"}

+----+------+
| h0 | > h1 |
+----+------+

![](media/image338.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

+---------------+------+------------+--+----+--+--+
| Features:     |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
| L x D         |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
|               |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
| > Weighted    | > z1 |            |  | y1 |  |  |
+---------------+------+------------+--+----+--+--+
| > features: D |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
|               |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
| Weighted      |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
|               |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+
| combination   |      | First word |  |    |  |  |
+---------------+------+------------+--+----+--+--+
| of features   |      |            |  |    |  |  |
+---------------+------+------------+--+----+--+--+

![](media/image340.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 92 24 Feb
> 2016
>
> ![](media/image341.jpeg){width="9.51388888888889in"
> height="4.764583333333333in"}

+-------------+----+----------------+------+--+------+--+--+
| L locations |    | > Distribution |      |  |      |  |  |
+-------------+----+----------------+------+--+------+--+--+
|             |    | > over vocab   |      |  |      |  |  |
+-------------+----+----------------+------+--+------+--+--+
|             |    |                |      |  |      |  |  |
+-------------+----+----------------+------+--+------+--+--+
|             | a1 |                | > a2 |  | > d1 |  |  |
+-------------+----+----------------+------+--+------+--+--+
|             |    |                |      |  |      |  |  |
+-------------+----+----------------+------+--+------+--+--+

![](media/image342.jpeg){width="5.208880139982502e-3in"
height="0.5451388888888888in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td><blockquote>
<p>h0</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Image:</td>
<td>Features:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>L x D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>H x W x 3</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Weighted</td>
<td></td>
<td><blockquote>
<p>z1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y1</td>
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
<td><blockquote>
<p>features: D</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td><blockquote>
<p>Weighted</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Xu et al, “Show, Attend and Tell: Neural</td>
<td><blockquote>
<p>combination</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>First word</p>
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
<td>Image Caption Generation with Visual</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>of features</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Attention”, ICML 2015</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image343.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 93 24 Feb
> 2016
>
> ![](media/image348.jpeg){width="10.0in" height="5.413888888888889in"}

+-------------+------+----------------+--+
| L locations |      | > Distribution |  |
+-------------+------+----------------+--+
|             |      | > over vocab   |  |
+-------------+------+----------------+--+
| a1          | > a2 | > d1           |  |
+-------------+------+----------------+--+

![](media/image349.jpeg){width="5.208880139982502e-3in"
height="0.5451388888888888in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td><blockquote>
<p>h0</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Image:</td>
<td>Features:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>L x D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>H x W x 3</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Weighted</td>
<td></td>
<td><blockquote>
<p>z1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y1</td>
<td></td>
<td><blockquote>
<p>z2</p>
</blockquote></td>
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
<td><blockquote>
<p>features: D</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>Weighted</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Xu et al, “Show, Attend and Tell: Neural</td>
<td><blockquote>
<p>combination</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>First word</p>
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
<td></td>
</tr>
<tr class="even">
<td>Image Caption Generation with Visual</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>of features</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Attention”, ICML 2015</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image350.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 94 24 Feb
> 2016
>
> ![](media/image354.jpeg){width="10.0in" height="5.413888888888889in"}

+-------------+------+----------------+--+
| L locations |      | > Distribution |  |
+-------------+------+----------------+--+
|             |      | > over vocab   |  |
+-------------+------+----------------+--+
| a1          | > a2 | > d1           |  |
+-------------+------+----------------+--+

![](media/image355.jpeg){width="5.208880139982502e-3in"
height="0.5451388888888888in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td></td>
<td></td>
<td></td>
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
<td><blockquote>
<p>h0</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h2</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Features:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>L x D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>H x W x 3</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Weighted</td>
<td></td>
<td><blockquote>
<p>z1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td><blockquote>
<p>z2</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td><blockquote>
<p>features: D</p>
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
<td></td>
<td></td>
<td></td>
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
<p>Weighted</p>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Xu et al, “Show, Attend and Tell: Neural</td>
<td><blockquote>
<p>combination</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>First word</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Image Caption Generation with Visual</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>of features</p>
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
<td></td>
<td></td>
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
<td>Attention”, ICML 2015</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image356.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 95 24 Feb
> 2016
>
> ![](media/image361.jpeg){width="10.0in" height="5.413888888888889in"}

+-------------+------+----------------+------+------+--+
| L locations |      | > Distribution |      |      |  |
+-------------+------+----------------+------+------+--+
|             |      | > over vocab   |      |      |  |
+-------------+------+----------------+------+------+--+
| a1          | > a2 | > d1           | > a3 | > d2 |  |
+-------------+------+----------------+------+------+--+

![](media/image362.jpeg){width="5.208880139982502e-3in"
height="0.5451388888888888in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td></td>
<td></td>
<td></td>
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
<td><blockquote>
<p>h0</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h2</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Features:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>L x D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>H x W x 3</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Weighted</td>
<td></td>
<td><blockquote>
<p>z1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td><blockquote>
<p>z2</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td><blockquote>
<p>features: D</p>
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
<td></td>
<td></td>
<td></td>
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
<p>Weighted</p>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Xu et al, “Show, Attend and Tell: Neural</td>
<td><blockquote>
<p>combination</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>First word</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Image Caption Generation with Visual</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>of features</p>
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
<td></td>
<td></td>
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
<td>Attention”, ICML 2015</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image363.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 96 24 Feb
> 2016
>
> ![](media/image368.jpeg){width="10.0in" height="5.413888888888889in"}

<table>
<tbody>
<tr class="odd">
<td>Guess which framework</td>
<td><blockquote>
<p>L locations</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>Distribution</p>
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
<td>was used to implement?</td>
<td></td>
<td></td>
<td><blockquote>
<p>over vocab</p>
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
<td>a1</td>
<td></td>
<td><blockquote>
<p>a2</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>d1</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>a3</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p>d2</p>
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
<td></td>
</tr>
</tbody>
</table>

![](media/image369.jpeg){width="5.208880139982502e-3in"
height="0.5451388888888888in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>CNN</p>
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
<td></td>
<td></td>
<td></td>
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
<td><blockquote>
<p>h0</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>h2</p>
</blockquote></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Features:</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>L x D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>H x W x 3</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Weighted</td>
<td></td>
<td><blockquote>
<p>z1</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y1</td>
<td></td>
<td></td>
<td><blockquote>
<p>z2</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td>y2</td>
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
<td><blockquote>
<p>features: D</p>
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
<td></td>
<td></td>
<td></td>
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
<p>Weighted</p>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
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
<td>Xu et al, “Show, Attend and Tell: Neural</td>
<td><blockquote>
<p>combination</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>First word</p>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Image Caption Generation with Visual</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>of features</p>
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
<td></td>
<td></td>
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
<td>Attention”, ICML 2015</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image370.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 97 24 Feb
> 2016
>
> ![](media/image375.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Guess which framework was used to implement?
>
> Crazy RNN = **Theano**
>
> CNN

Image:

> H x W x 3

Xu et al, "Show, Attend and Tell: Neural Image Caption Generation with
Visual Attention", ICML 2015

+-------------+------+----------------+------+------+--+
| L locations |      | > Distribution |      |      |  |
+-------------+------+----------------+------+------+--+
|             |      | > over vocab   |      |      |  |
+-------------+------+----------------+------+------+--+
| a1          | > a2 | > d1           | > a3 | > d2 |  |
+-------------+------+----------------+------+------+--+

![](media/image376.jpeg){width="5.208880139982502e-3in"
height="0.43125in"}

+----+------+------+
| h0 | > h1 | > h2 |
+----+------+------+

![](media/image379.jpeg){width="0.5659722222222222in"
height="5.208880139982502e-3in"}

+---------------+------+------------+------+------+--+
| Features:     |      |            |      |      |  |
+---------------+------+------------+------+------+--+
| L x D         |      |            |      |      |  |
+---------------+------+------------+------+------+--+
| > Weighted    | > z1 | y1         | > z2 | > y2 |  |
+---------------+------+------------+------+------+--+
| > features: D |      |            |      |      |  |
+---------------+------+------------+------+------+--+
|               |      |            |      |      |  |
+---------------+------+------------+------+------+--+
| Weighted      |      |            |      |      |  |
+---------------+------+------------+------+------+--+
| combination   |      | First word |      |      |  |
+---------------+------+------------+------+------+--+
| of features   |      |            |      |      |  |
+---------------+------+------------+------+------+--+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 98 24 Feb
> 2016
>
> ![](media/image382.jpeg){width="9.311111111111112in"
> height="2.829861111111111in"}
>
> Image:
>
> H x W x 3
>
> From
>
> RNN:
>
> a b

CNN

> c d

Grid of features

(Each D-

dimensional)

![](media/image383.jpeg){width="4.219444444444444in"
height="1.7430555555555556in"}

> p~a~ p~b~
>
> p~c~ p~d~

+------------------------------------------+---------------------------------+--+
|                                          | > Distribution over             |  |
+------------------------------------------+---------------------------------+--+
| Xu et al, "Show, Attend and Tell: Neural | > grid locations                |  |
+------------------------------------------+---------------------------------+--+
| Image Caption Generation with Visual     | > p~a~ + p~b~ + p~c~ + p~c~ = 1 |  |
+------------------------------------------+---------------------------------+--+
|                                          |                                 |  |
+------------------------------------------+---------------------------------+--+
| Attention", ICML 2015                    |                                 |  |
+------------------------------------------+---------------------------------+--+

![](media/image384.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 99 24 Feb
> 2016
>
> ![](media/image385.jpeg){width="9.51388888888889in"
> height="4.764583333333333in"}

+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > CNN  |        |        | a      | b      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        | c      | d      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Image: | Grid   |        |        |        |        |        |        |
|        | of     |        |        |        |        |        |        |
|        | featur |        |        |        |        |        |        |
|        | es     |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        | (Each  |        |        |        |        |
|        |        |        | D-     |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| H x W  |        | dimens |        |        |        |        |        |
| x 3    |        | ional) |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| From   |        |        | p~a~   | p~b~   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| > RNN: |        |        |        | p~c~   | p~d~   |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        | Distri |        |        |        |        |        |
|        |        | bution |        |        |        |        |        |
|        |        | over   |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Xu et  |        | grid   |        |        |        |        |        |
| al,    |        | locati |        |        |        |        |        |
| "Show, |        | ons    |        |        |        |        |        |
| Attend |        |        |        |        |        |        |        |
| and    |        |        |        |        |        |        |        |
| Tell:  |        |        |        |        |        |        |        |
| Neural |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

+--------------------------------------+---------------------------------+--+
| Image Caption Generation with Visual | > p~a~ + p~b~ + p~c~ + p~c~ = 1 |  |
+--------------------------------------+---------------------------------+--+
|                                      |                                 |  |
+--------------------------------------+---------------------------------+--+
| Attention", ICML 2015                |                                 |  |
+--------------------------------------+---------------------------------+--+

Context vector z

> (D-dimensional)

![](media/image386.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 100 24 Feb
> 2016
>
> ![](media/image387.jpeg){width="9.654861111111112in"
> height="4.764583333333333in"}
>
> **Soft attention:**

+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > CNN  |        |        | a      | b      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        | c      | d      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Image: | Grid   |        |        |        |        |        |        |
|        | of     |        |        |        |        |        |        |
|        | featur |        |        |        |        |        |        |
|        | es     |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        | (Each  |        |        |        |        |
|        |        |        | D-     |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| H x W  |        | dimens |        |        |        |        |        |
| x 3    |        | ional) |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| From   |        |        | p~a~   | p~b~   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| > RNN: |        |        |        | p~c~   | p~d~   |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        | Distri |        |        |        |        |        |
|        |        | bution |        |        |        |        |        |
|        |        | over   |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Xu et  |        | grid   |        |        |        |        |        |
| al,    |        | locati |        |        |        |        |        |
| "Show, |        | ons    |        |        |        |        |        |
| Attend |        |        |        |        |        |        |        |
| and    |        |        |        |        |        |        |        |
| Tell:  |        |        |        |        |        |        |        |
| Neural |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

+--------------------------------------+---------------------------------+--+
| Image Caption Generation with Visual | > p~a~ + p~b~ + p~c~ + p~c~ = 1 |  |
+--------------------------------------+---------------------------------+--+
|                                      |                                 |  |
+--------------------------------------+---------------------------------+--+
| Attention", ICML 2015                |                                 |  |
+--------------------------------------+---------------------------------+--+

Context vector z

> (D-dimensional)

![](media/image388.jpeg){width="10.0in" height="0.5888888888888889in"}

Summarize ALL locations

z = p~a~a+ p~b~b + p~c~c + p~d~d

Derivative dz/dp is nice!

Train with gradient descent

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 101 24 Feb
> 2016
>
> ![](media/image389.jpeg){width="9.791666666666666in"
> height="4.7972222222222225in"}
>
> **Soft attention:**

+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > CNN  |        |        | a      | b      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        | c      | d      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Image: | Grid   |        |        |        |        |        |        |
|        | of     |        |        |        |        |        |        |
|        | featur |        |        |        |        |        |        |
|        | es     |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        | (Each  |        |        |        |        |
|        |        |        | D-     |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| H x W  |        | dimens |        |        |        |        |        |
| x 3    |        | ional) |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| From   |        |        | p~a~   | p~b~   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| > RNN: |        |        |        | p~c~   | p~d~   |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        | Distri |        |        |        |        |        |
|        |        | bution |        |        |        |        |        |
|        |        | over   |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Xu et  |        | grid   |        |        |        |        |        |
| al,    |        | locati |        |        |        |        |        |
| "Show, |        | ons    |        |        |        |        |        |
| Attend |        |        |        |        |        |        |        |
| and    |        |        |        |        |        |        |        |
| Tell:  |        |        |        |        |        |        |        |
| Neural |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

+--------------------------------------+---------------------------------+--+
| Image Caption Generation with Visual | > p~a~ + p~b~ + p~c~ + p~c~ = 1 |  |
+--------------------------------------+---------------------------------+--+
|                                      |                                 |  |
+--------------------------------------+---------------------------------+--+
| Attention", ICML 2015                |                                 |  |
+--------------------------------------+---------------------------------+--+

Context vector z

> (D-dimensional)

![](media/image390.jpeg){width="10.0in" height="0.5888888888888889in"}

Summarize ALL locations

z = p~a~a+ p~b~b + p~c~c + p~d~d

Derivative dz/dp is nice!

Train with gradient descent

**Hard attention**:

Sample ONE location

according to p, z = that vector

With argmax, dz/dp is zero

almost everywhere ...

> Can't use gradient descent; need reinforcement learning
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 102 24 Feb
> 2016
>
> ![](media/image391.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image392.jpeg){width="9.761805555555556in" height="2.075in"}

> Soft attention
>
> Hard attention

![](media/image393.jpeg){width="2.173611111111111in" height="0.6125in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image394.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 103 24 Feb
> 2016
>
> ![](media/image395.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image396.jpeg){width="8.550694444444444in"
height="3.6819444444444445in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image397.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 104 24 Feb
> 2016

<table>
<tbody>
<tr class="odd">
<td>Soft Attention for Captioning</td>
<td><blockquote>
<p>Attention constrained to</p>
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
<td></td>
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
<p>fixed grid! We’ll come</p>
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
<td></td>
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
<p>back to this ….</p>
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
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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
<td></td>
<td></td>
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

![](media/image398.jpeg){width="9.315277777777778in"
height="1.0895833333333333in"}

Xu et al, "Show, Attend and Tell: Neural

Image Caption Generation with Visual

Attention", ICML 2015

![](media/image472.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 105 24 Feb
> 2016
>
> ![](media/image473.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image474.jpeg){width="9.839583333333334in"
height="3.714583333333333in"}

> "Mi gato es el mejor" -\> "My cat is the best"

Bahdanau et al, "Neural Machine Translation by

Jointly Learning to Align and Translate", ICLR 2015

![](media/image475.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 106 24 Feb
> 2016
>
> ![](media/image476.jpeg){width="9.839583333333334in"
> height="4.802083333333333in"}

Distribution over

input words

![](media/image477.jpeg){width="5.208880139982502e-3in"
height="0.8916666666666667in"}

> "Mi gato es el mejor" -\> "My cat is the best"

Bahdanau et al, "Neural Machine Translation by

Jointly Learning to Align and Translate", ICLR 2015

![](media/image482.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 107 24 Feb
> 2016
>
> ![](media/image483.jpeg){width="9.839583333333334in"
> height="4.802083333333333in"}

Distribution over

input words

![](media/image484.jpeg){width="5.208880139982502e-3in"
height="0.16458333333333333in"}

> "Mi gato es el mejor" -\> "My cat is the best"

Bahdanau et al, "Neural Machine Translation by

Jointly Learning to Align and Translate", ICLR 2015

![](media/image489.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 108 24 Feb
> 2016
>
> ![](media/image490.jpeg){width="9.839583333333334in"
> height="4.802083333333333in"}

Distribution over

input words

![](media/image491.jpeg){width="5.208880139982502e-3in"
height="0.16458333333333333in"}

> "Mi gato es el mejor" -\> "My cat is the best"

Bahdanau et al, "Neural Machine Translation by

Jointly Learning to Align and Translate", ICLR 2015

![](media/image496.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 109 24 Feb
> 2016
>
> ![](media/image497.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image498.jpeg){width="9.907638888888888in"
height="3.5395833333333333in"}

> **Machine Translation, attention over input:**
>
> \- Luong et al, "Effective Approaches to Attention-based Neural
> Machine Translation," EMNLP 2015
>
> **Speech recognition, attention over input sounds:**

-   Chan et al, "Listen, Attend, and Spell", arXiv 2015

-   Chorowski et al, "Attention-based models for Speech Recognition",
    > NIPS 2015

**Video captioning,**

**attention over input frames:**

-   Yao et al, "Describing Videos by Exploiting Temporal Structure",
    ICCV 2015

![](media/image499.jpeg){width="10.0in" height="0.5888888888888889in"}

**Image, question to answer, attention over image:**

-   Xu and Saenko, "Ask, Attend and Answer: Exploring Question-Guided
    Spatial Attention for Visual Question Answering", arXiv 2015

-   Zhu et al, "Visual7W: Grounded Question Answering in Images", arXiv
    2015

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 110 24 Feb 2016

> ![](media/image500.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image501.jpeg){width="5.208880139982502e-3in"
height="1.0618055555555554in"}

> Features:

![](media/image513.jpeg){width="1.0618055555555554in"
height="5.208880139982502e-3in"}

> Image: ~L\ x\ D~
>
> H x W x 3

![](media/image514.jpeg){width="6.795138888888889in" height="0.58125in"}

> Attention mechanism from Show, Attend, and Tell only lets us softly
> attend to fixed grid positions ... can we do better?

![](media/image515.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 111 24 Feb 2016

> ![](media/image516.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image517.jpeg){width="4.480555555555555in"
height="0.9652777777777778in"}

-   Read text, generate handwriting using an RNN

-   Attend to arbitrary regions of the **output** by predicting params
    > of a mixture model

![](media/image518.jpeg){width="10.0in" height="3.3916666666666666in"}

Graves, "Generating Sequences with Recurrent Neural Networks", arXiv
2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 112 24 Feb
> 2016
>
> ![](media/image519.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image520.jpeg){width="4.480555555555555in"
height="0.9652777777777778in"}

-   Read text, generate handwriting using an RNN

-   Attend to arbitrary regions of the **output** by predicting params
    > of a mixture model

![](media/image521.jpeg){width="10.0in" height="3.3916666666666666in"}

Which are real and which are generated?

![](media/image522.jpeg){width="4.480555555555555in"
height="2.995833333333333in"}

Graves, "Generating Sequences with Recurrent Neural Networks", arXiv
2013

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 113 24 Feb
> 2016
>
> ![](media/image524.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image525.jpeg){width="10.0in" height="4.402777777777778in"}

-   Read text, generate handwriting using an RNN

-   Attend to arbitrary regions of the **output** by predicting params
    > of a mixture model

Which are real and which are generated?

> **REAL**

Graves, "Generating Sequences with Recurrent Neural Networks", arXiv
2013

**GENERATED**

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 114 24 Feb
> 2016
>
> ![](media/image526.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Classify** images by attending to
>
> arbitrary regions of the *input*

Gregor et al, "DRAW: A Recurrent Neural Network For Image Generation",
ICML 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 115 24 Feb
> 2016
>
> ![](media/image527.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Classify** images by attending to
>
> arbitrary regions of the *input*

**Generate** images by attending to arbitrary regions of the *output*

Gregor et al, "DRAW: A Recurrent Neural Network For Image Generation",
ICML 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 116 24 Feb
> 2016

![](media/image528.jpeg){width="10.0in" height="5.370833333333334in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 117 24 Feb 2016

> ![](media/image529.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}
>
> Spatial Transformer Networks

![](media/image530.jpeg){width="9.027777777777779in"
height="1.6743055555555555in"}

> Attention mechanism similar to DRAW, but easier to explain

![](media/image531.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image532.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 118 24 Feb
> 2016
>
> ![](media/image533.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image534.jpeg){width="4.6in" height="2.8472222222222223in"}

> Input image:
>
> H x W x 3 Cropped and
>
> rescaled image:

X x Y x 3

![](media/image535.jpeg){width="1.8916666666666666in"
height="0.6291666666666667in"}

Box Coordinates:

> (xc, yc, w, h)

![](media/image536.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image537.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 119 24 Feb
> 2016
>
> ![](media/image538.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image539.jpeg){width="4.124305555555556in"
height="1.6736111111111112in"}

Can we make this

function differentiable?

![](media/image540.jpeg){width="4.4319444444444445in"
height="1.867361111111111in"}

> Input image:
>
> H x W x 3 Cropped and
>
> rescaled image:

X x Y x 3

![](media/image542.jpeg){width="1.8916666666666666in"
height="0.6291666666666667in"}

Box Coordinates:

> (xc, yc, w, h)

![](media/image543.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image544.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 120 24 Feb
> 2016
>
> ![](media/image545.jpeg){width="9.027777777777779in"
> height="4.334722222222222in"}
>
> Can we make this
>
> function differentiable?
>
> Input image:
>
> H x W x 3 Cropped and rescaled image:
>
> X x Y x 3

Box Coordinates:

> (xc, yc, w, h)

![](media/image546.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

**Idea**: Function mapping *pixel coordinates* (xt, yt) of output to
*pixel coordinates* (xs, ys) of input

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image547.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 121 24 Feb
> 2016
>
> ![](media/image548.jpeg){width="9.027777777777779in"
> height="4.334722222222222in"}

+--------------+--------------------------+
| (x^s^, y^s^) | Can we make this         |
+--------------+--------------------------+
|              | function differentiable? |
+--------------+--------------------------+
|              | > (x^t^, y^t^)           |
+--------------+--------------------------+

> Input image:
>
> H x W x 3 Cropped and rescaled image:
>
> X x Y x 3

Box Coordinates:

> (xc, yc, w, h)

![](media/image549.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

**Idea**: Function mapping *pixel coordinates* (xt, yt) of output to
*pixel coordinates* (xs, ys) of input

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image550.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 122 24 Feb
> 2016
>
> ![](media/image551.jpeg){width="9.027777777777779in"
> height="4.334722222222222in"}
>
> (x^s^, y^s^)
>
> Input image:
>
> H x W x 3
>
> Box Coordinates:
>
> (xc, yc, w, h)

![](media/image552.jpeg){width="3.9611111111111112in"
height="0.3104166666666667in"}

Can we make this

function differentiable?

> (x^t^, y^t^)
>
> Cropped and
>
> rescaled image:
>
> X x Y x 3

**Idea**: Function mapping *pixel coordinates* (xt, yt) of output to
*pixel coordinates* (xs, ys) of input

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image553.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 123 24 Feb
> 2016
>
> ![](media/image554.jpeg){width="9.975694444444445in"
> height="4.813194444444444in"}
>
> Can we make this
>
> function differentiable?

**Idea**: Function mapping

*pixel coordinates* (xt, yt) of

output to *pixel coordinates*

(xs, ys) of input

+-----------------+-----------------+-----------------+-----------------+
| Input image:    |                 | > Repeat for    |                 |
|                 |                 | > all pixels    |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 | Cropped and     | > in *output*   |                 |
|                 |                 | > to get a      |                 |
+-----------------+-----------------+-----------------+-----------------+
| H x W x 3       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 | rescaled image: | > **sampling    |                 |
|                 |                 | > grid**        |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 | X x Y x 3       |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Box             |                 |                 |                 |
| Coordinates:    |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| (xc, yc, w, h)  |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| Jaderberg et    |                 |                 |                 |
| al, "Spatial    |                 |                 |                 |
| Transformer     |                 |                 |                 |
| Networks", NIPS |                 |                 |                 |
| 2015            |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image555.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 124 24 Feb
> 2016
>
> ![](media/image556.jpeg){width="9.975694444444445in"
> height="4.813194444444444in"}
>
> Can we make this
>
> function differentiable?

**Idea**: Function mapping

*pixel coordinates* (xt, yt) of

output to *pixel coordinates*

(xs, ys) of input

+--------------+-----------------+-------------------------+--+
| Input image: |                 | > Repeat for all pixels |  |
+--------------+-----------------+-------------------------+--+
|              | Cropped and     | > in *output* to get a  |  |
+--------------+-----------------+-------------------------+--+
| H x W x 3    |                 |                         |  |
+--------------+-----------------+-------------------------+--+
|              | rescaled image: | > **sampling grid**     |  |
+--------------+-----------------+-------------------------+--+
|              | X x Y x 3       |                         |  |
+--------------+-----------------+-------------------------+--+

Then use **bilinear**

> Box Coordinates:
>
> **interpolation** to
>
> (xc, yc, w, h)
>
> compute output

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image557.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 125 24 Feb
> 2016
>
> ![](media/image558.jpeg){width="9.975694444444445in"
> height="4.813194444444444in"}
>
> Can we make this
>
> function differentiable?
>
> Input image:
>
> H x W x 3 Cropped and rescaled image:
>
> X x Y x 3

Box Coordinates:

> (xc, yc, w, h)

+---------------------------------+--------------+--+
| **Idea**: Function mapping      | > Network    |  |
+---------------------------------+--------------+--+
|                                 | > attends to |  |
+---------------------------------+--------------+--+
| *pixel coordinates* (xt, yt) of |              |  |
+---------------------------------+--------------+--+
|                                 | > input by   |  |
+---------------------------------+--------------+--+
| output to *pixel coordinates*   |              |  |
+---------------------------------+--------------+--+
|                                 | > predicting |  |
+---------------------------------+--------------+--+
| (xs, ys) of input               |              |  |
+---------------------------------+--------------+--+
|                                 |              |  |
+---------------------------------+--------------+--+

Repeat for all pixels in *output* to get a **sampling grid**

Then use **bilinear**

> **interpolation** to compute output

Jaderberg et al, "Spatial Transformer Networks", NIPS 2015

![](media/image559.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 126 24 Feb
> 2016
>
> ![](media/image560.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image561.jpeg){width="7.654166666666667in"
height="1.9868055555555555in"}

  ------------ -----------------------
  **Input**:   **Output:** Region of
  Full image   interest from input
  ------------ -----------------------

![](media/image562.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 127 24 Feb 2016

> ![](media/image563.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image564.jpeg){width="7.70625in"
height="2.6881944444444446in"}

-   small

> **Localization network**
>
> predicts transform

  ------------ -----------------------
  **Input**:   **Output:** Region of
  Full image   interest from input
  ------------ -----------------------

![](media/image565.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 128 24 Feb 2016

> ![](media/image566.jpeg){width="9.027777777777779in"
> height="3.904861111111111in"}
>
> **Grid generator** uses to
>
> compute sampling grid

-   small

> **Localization network**
>
> predicts transform

  ------------ -----------------------
  **Input**:   **Output:** Region of
  Full image   interest from input
  ------------ -----------------------

![](media/image567.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 129 24 Feb 2016

> ![](media/image568.jpeg){width="9.027777777777779in"
> height="4.773611111111111in"}
>
> **Grid generator** uses to
>
> compute sampling grid

-   small

> **Localization network**
>
> predicts transform

  ------------ -----------------------
  **Input**:   **Output:** Region of
  Full image   interest from input
  ------------ -----------------------

**Sampler** uses

bilinear interpolation

to produce output

![](media/image569.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 130 24 Feb 2016

> ![](media/image570.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image571.jpeg){width="4.395833333333333in"
height="2.748611111111111in"}

> Insert spatial transformers into a
>
> classification network and it learns
>
> to attend and transform the input

![](media/image572.jpeg){width="2.3833333333333333in"
height="0.6131944444444445in"}

> Differentiable "attention /
>
> transformation" module

![](media/image573.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 131 24 Feb 2016

![](media/image575.jpeg){width="10.0in" height="5.583333333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 132 24 Feb 2016

> ![](media/image576.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image577.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Soft attention:

    -   Easy to implement: produce distribution over input locations,
        > reweight features and feed as input

    -   Attend to arbitrary input locations using spatial transformer
        > networks

-   Hard attention:

    -   Attend to a single input location

    -   Can't use gradient descent!

    -   Need **reinforcement learning!**

![](media/image578.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 13 133 24 Feb 2016
