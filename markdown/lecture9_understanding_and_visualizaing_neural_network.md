![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

> Understanding and Visualizing Convolutional Neural Networks

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 1 3 Feb 2016

> ![](media/image3.jpeg){width="9.7625in" height="4.167361111111111in"}

-   A1 is graded. We'll send out grades tonight (or so)

-   A2 is due Feb 5 (this Friday!): **submit in Assignments tab** on
    > CourseWork (not Dropbox)

-   Midterm is Feb 10 (next Wednesday)

-   Oh and pretrained ResNets were released today

> (152-layer ILSVRC 2015 winning ConvNets)
>
> [[https://github.com/KaimingHe/deep-residual-networks]{.underline}](https://github.com/KaimingHe/deep-residual-networks)

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 2 3 Feb 2016

![](media/image5.jpeg){width="9.881944444444445in"
height="5.520833333333333in"}

+-------------------------------------------------+---------------+--------------+
| > Fei-Fei Li & Andrej Karpathy & Justin Johnson | > Lecture 9 3 | > 3 Feb 2016 |
+-------------------------------------------------+---------------+--------------+
|                                                 |               |              |
+-------------------------------------------------+---------------+--------------+

> ![](media/image6.jpeg){width="10.0in" height="5.625in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 4 3

> ![](media/image7.jpeg){width="8.450694444444444in"
> height="0.7173611111111111in"}

![](media/image8.jpeg){width="9.586805555555555in"
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

![](media/image9.jpeg){width="9.582638888888889in"
height="0.4583333333333333in"}

> CAT CAT CAT, DOG, DUCK CAT, DOG, DUCK

![](media/image10.jpeg){width="10.0in" height="1.448611111111111in"}

> Single object Multiple objects

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 5 3 Feb 2016

> ![](media/image11.jpeg){width="9.302777777777777in"
> height="4.418055555555555in"}

-   Visualize patches that maximally activate neurons

-   Visualize the weights

-   Visualize the representation space (e.g. with t-SNE)

-   Occlusion experiments

-   Human experiment comparisons

-   Deconv approaches (single backward pass)

-   Optimization over image approaches (optimization)

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 6 3 Feb 2016

> ![](media/image13.jpeg){width="10.0in" height="5.625in"}
>
> *Rich feature hierarchies for accurate object detection and semantic
> segmentation \[Girshick, Donahue, Darrell, Malik\]*

one-stream AlexNet

pool5

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 7 3 Feb 2016

> ![](media/image14.jpeg){width="9.89861111111111in" height="4.95625in"}

one-stream AlexNet

conv1

> only interpretable on the first layer :(

![](media/image15.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 8 3 Feb 2016

![](media/image16.jpeg){width="2.3673611111111112in"
height="0.6388888888888888in"}

> Visualize the filters/kernels (raw weights)

![](media/image17.jpeg){width="2.142361111111111in"
height="0.4652777777777778in"}

> you can still do it for higher layers, it's just not that interesting
>
> (these are taken from ConvNetJS CIFAR-10 demo)

![](media/image19.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

layer 1 weights

![](media/image20.jpeg){width="2.0in" height="0.27152777777777776in"}

> layer 2 weights

![](media/image22.jpeg){width="7.235416666666667in"
height="2.327777777777778in"}

> layer 3 weights

+-------------------------------------------------+---------------+--------------+
| > Fei-Fei Li & Andrej Karpathy & Justin Johnson | > Lecture 9 9 | > 3 Feb 2016 |
+-------------------------------------------------+---------------+--------------+
|                                                 |               |              |
+-------------------------------------------------+---------------+--------------+

> ![](media/image23.jpeg){width="9.843055555555555in"
> height="4.993055555555555in"}

![](media/image24.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 10 3 Feb 2016

![](media/image25.jpeg){width="5.069444444444445in"
height="0.5194444444444445in"}

![](media/image26.jpeg){width="2.497916666666667in"
height="4.552083333333333in"}

fc7 layer

![](media/image27.jpeg){width="5.444444444444445in"
height="2.5145833333333334in"}

> 4096-dimensional "code" for an image (layer immediately before the
> classifier)
>
> can collect the code for many images

![](media/image28.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 11 3 Feb 2016

![](media/image29.jpeg){width="9.713888888888889in" height="5.025in"}

> **Visualizing the representation**
>
> t-SNE visualization
>
> *\[van der Maaten & Hinton\]*
>
> Embed high-dimensional points so that locally, pairwise distances are
> conserved
>
> i.e. similar things end up in similar places. dissimilar things end up
> wherever
>
> **Right**: Example embedding of MNIST digits (0-9) in 2D

![](media/image30.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 12        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image31.jpeg){width="9.759722222222223in"
> height="4.954166666666667in"}
>
> two images are placed nearby if their CNN codes are close. See more:
>
> [[http://cs.stanford.](http://cs.stanford.edu/people/karpathy/cnnembed/)
> [edu/people/karpathy/cnnembed/](http://cs.stanford.edu/people/karpathy/cnnembed/)]{.underline}

![](media/image32.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 13 3 Feb 2016

> ![](media/image33.jpeg){width="9.89861111111111in"
> height="5.007638888888889in"}
>
> \[Zeiler & Fergus 2013\]
>
> (as a function of the
>
> position of the
>
> square of zeros in
>
> the original image)

![](media/image34.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 14 3 Feb 2016

> ![](media/image35.jpeg){width="9.89861111111111in"
> height="5.007638888888889in"}
>
> \[Zeiler & Fergus 2013\]
>
> (as a function of the
>
> position of the
>
> square of zeros in
>
> the original image)

![](media/image36.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 15 3 Feb 2016

> ![](media/image37.jpeg){width="9.57986111111111in" height="4.93125in"}
>
> [[http://yosinski.com/deepvis]{.underline}](http://yosinski.com/deepvis)
>
> YouTube video
>
> [[https://www.youtube.com/watch?v=AgkfIQ4IGaM]{.underline}](https://www.youtube.com/watch?v=AgkfIQ4IGaM)
>
> (4min)

![](media/image38.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 16 3 Feb 2016

> ![](media/image39.jpeg){width="9.1875in"
> height="0.9666666666666667in"}

1.  Feed image into net

    Q.  how can we compute the gradient of any arbitrary neuron in the
        > network w.r.t. the image?

![](media/image40.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 17 3 Feb 2016

> ![](media/image43.jpeg){width="9.1875in"
> height="0.9666666666666667in"}

1.  Feed image into net

![](media/image44.jpeg){width="10.0in" height="4.51875in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 18 3 Feb 2016

> ![](media/image45.jpeg){width="9.1875in"
> height="0.9666666666666667in"}

1.  Feed image into net

![](media/image46.jpeg){width="0.5138888888888888in"
height="5.208880139982502e-3in"}

2.  Pick a layer, set the gradient there to be all zero except for one 1
    > for some neuron of interest

3.  Backprop to image:

![](media/image48.jpeg){width="10.0in" height="2.4743055555555555in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 19 3 Feb 2016

**"Guided**

**backpropagation:"** instead

![](media/image49.jpeg){width="9.1875in" height="0.9666666666666667in"}

> Deconv approaches

1.  Feed image into net

![](media/image50.jpeg){width="0.5138888888888888in"
height="5.208880139982502e-3in"}

> 2\. Pick a layer, set the gradient there to be all zero except for one 1
> for

![](media/image52.jpeg){width="5.988888888888889in"
height="1.9819444444444445in"}

> some neuron of interest
>
> 3\. Backprop to image:

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 20 3 Feb 2016

> ![](media/image54.jpeg){width="9.780555555555555in"
> height="0.9944444444444445in"}
>
> *\[Visualizing and Understanding Convolutional Networks, Zeiler and
> Fergus 2013\]*
>
> *\[Deep Inside Convolutional Networks: Visualising Image
> Classification Models and Saliency Maps, Simonyan et al., 2014\]*
>
> *\[Striving for Simplicity: The all convolutional net, Springenberg,
> Dosovitskiy, et al., 2015\]*

![](media/image55.jpeg){width="10.0in" height="4.381944444444445in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 21 3 Feb 2016

> ![](media/image56.jpeg){width="9.780555555555555in"
> height="0.9944444444444445in"}
>
> *\[Visualizing and Understanding Convolutional Networks, Zeiler and
> Fergus 2013\]*
>
> *\[Deep Inside Convolutional Networks: Visualising Image
> Classification Models and Saliency Maps, Simonyan et al., 2014\]*
>
> *\[Striving for Simplicity: The all convolutional net, Springenberg,
> Dosovitskiy, et al., 2015\]*

![](media/image57.jpeg){width="9.622916666666667in"
height="3.7270833333333333in"}

> ![](media/image58.jpeg){width="8.888888888888889e-2in"
> height="0.43333333333333335in"} Backward pass for a ReLU (will be
> changed in Guided Backprop)

![](media/image59.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 22 3 Feb 2016

> ![](media/image60.jpeg){width="9.780555555555555in"
> height="0.9944444444444445in"}
>
> *\[Visualizing and Understanding Convolutional Networks, Zeiler and
> Fergus 2013\]*
>
> *\[Deep Inside Convolutional Networks: Visualising Image
> Classification Models and Saliency Maps, Simonyan et al., 2014\]*
>
> *\[Striving for Simplicity: The all convolutional net, Springenberg,
> Dosovitskiy, et al., 2015\]*

![](media/image61.jpeg){width="10.0in" height="4.381944444444445in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 23 3 Feb 2016

![](media/image62.jpeg){width="10.0in"
height="5.5569444444444445in"}**conv6** (top) and layer **conv9**
(bottom) of the network trained on ImageNet.

Each row corresponds to one filter.

The visualization using "guided backpropagation" is based on the top 10
image patches activating this filter taken from the ImageNet dataset.

> *\[Striving for Simplicity: The all convolutional net, Springenberg,
> Dosovitskiy, et al., 2015\]*
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 24 3 Feb 2016
>
> ![](media/image63.jpeg){width="9.780555555555555in"
> height="0.9944444444444445in"}
>
> *\[Visualizing and Understanding Convolutional Networks, Zeiler and
> Fergus 2013\]*
>
> *\[Deep Inside Convolutional Networks: Visualising Image
> Classification Models and Saliency Maps, Simonyan et al., 2014\]*
>
> *\[Striving for Simplicity: The all convolutional net, Springenberg,
> Dosovitskiy, et al., 2015\]*

![](media/image64.jpeg){width="9.240972222222222in"
height="3.7263888888888888in"}

> bit weird

![](media/image65.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 25 3 Feb 2016

> ![](media/image66.jpeg){width="9.844444444444445in"
> height="4.78125in"}
>
> *Zeiler & Fergus, 2013*
>
> Visualizing arbitrary neurons along the way to the top\...

![](media/image67.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 26 3 Feb 2016

> ![](media/image68.jpeg){width="9.457638888888889in"
> height="0.5979166666666667in"}

![](media/image69.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 27 3 Feb 2016

![](media/image71.jpeg){width="9.797222222222222in"
height="4.895138888888889in"}

![](media/image72.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 28 3 Feb 2016

> ![](media/image73.jpeg){width="6.355555555555555in"
> height="0.8722222222222222in"}

![](media/image74.jpeg){width="7.120833333333334in"
height="3.439583333333333in"}

Q.  can we find an image that maximizes some class score?

![](media/image75.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 29 3 Feb 2016

![](media/image76.jpeg){width="9.556944444444444in" height="1.00625in"}

> Optimization to Image
>
> score for class c (before Softmax)

![](media/image77.jpeg){width="7.120833333333334in"
height="3.439583333333333in"}

Q.  can we find an image that maximizes some class score?

![](media/image78.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 30        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image79.jpeg){width="6.355555555555555in"
> height="0.8722222222222222in"}

![](media/image80.jpeg){width="8.152777777777779in"
height="1.5777777777777777in"}

1.  feed in zeros.

zero image

![](media/image81.jpeg){width="0.5138888888888888in"
height="5.208880139982502e-3in"}

> 2\. set the gradient of the scores vector to be \[0,0,\....1,\....,0\],
> then backprop to image

![](media/image84.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 31 3 Feb 2016

![](media/image85.jpeg){width="6.355555555555555in"
height="0.8722222222222222in"}

> Optimization to Image

![](media/image86.jpeg){width="8.152777777777779in"
height="1.5777777777777777in"}

1.  feed in zeros.

> zero image

![](media/image87.jpeg){width="0.5138888888888888in"
height="5.208880139982502e-3in"}

2.  set the gradient of the scores vector to be \[0,0,\....1,\....,0\],
    > then backprop to image

3.  do a small "image update"

4.  forward the image through the network.

![](media/image90.jpeg){width="3.995833333333333in"
height="0.8930555555555556in"}

> 5\. go back to 2.

score for class c (before Softmax)

![](media/image91.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 32        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image92.jpeg){width="9.78888888888889in"
> height="0.5111111111111111in"}

![](media/image93.jpeg){width="9.213194444444444in"
height="4.246527777777778in"}

> 1\. Find images that maximize some class score:

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 33 3 Feb 2016

> ![](media/image95.jpeg){width="9.78888888888889in"
> height="0.5111111111111111in"}

![](media/image96.jpeg){width="9.213194444444444in" height="4.2125in"}

> 1\. Find images that maximize some class score:

![](media/image97.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 34 3 Feb 2016

![](media/image98.jpeg){width="9.78888888888889in"
height="4.936805555555556in"}

> *Deep Inside Convolutional Networks: Visualising Image Classification
> Models and Saliency Maps Karen Simonyan, Andrea Vedaldi, Andrew
> Zisserman, 2014*

2.  Visualize the Data gradient:

+------------------------------+---------+--+
| (note that the gradient on   | > M = ? |  |
+------------------------------+---------+--+
| data has three channels.     |         |  |
+------------------------------+---------+--+
|                              |         |  |
+------------------------------+---------+--+
| Here they visualize M, s.t.: |         |  |
+------------------------------+---------+--+

> (at each pixel take abs val, and max over channels)

![](media/image99.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 35        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image100.jpeg){width="9.78888888888889in"
height="4.936805555555556in"}

> *Deep Inside Convolutional Networks: Visualising Image Classification
> Models and Saliency Maps Karen Simonyan, Andrea Vedaldi, Andrew
> Zisserman, 2014*

2.  Visualize the Data gradient:

> (note that the gradient on data has three channels. Here they
> visualize M, s.t.:
>
> (at each pixel take abs val, and max over channels)

![](media/image101.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 36        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image102.jpeg){width="9.78888888888889in"
> height="0.5111111111111111in"}

![](media/image103.jpeg){width="9.655555555555555in"
height="4.283333333333333in"}

-   Use **grabcut** for segmentation

![](media/image104.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 37 3 Feb 2016

> ![](media/image105.jpeg){width="9.814583333333333in"
> height="3.1618055555555555in"}

![](media/image106.jpeg){width="9.18125in"
height="1.0152777777777777in"}

> **Repeat:**

1.  Forward an image

2.  Set activations in layer of interest to all zero, except for a 1.0
    > for a neuron of interest

3.  Backprop to image

4.  Do an "image update"

![](media/image107.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 38 3 Feb 2016

> ![](media/image108.jpeg){width="9.86875in"
> height="2.2631944444444443in"}
>
> Proposed a different form of regularizing the image

![](media/image109.jpeg){width="8.229861111111111in"
height="1.9118055555555555in"}

> More explicit scheme:
>
> **Repeat:**

-   Update the image **x** with gradient from some unit of interest

-   Blur x a bit

-   Take any pixel with small norm to zero (to encourage sparsity)

![](media/image110.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 39 3 Feb 2016

> ![](media/image111.jpeg){width="9.01388888888889in"
> height="4.93125in"}
>
> [[http://yosinski.com/deepvis]{.underline}](http://yosinski.com/deepvis)

![](media/image112.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 40 3 Feb 2016

![](media/image113.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 41        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image115.jpeg){width="9.906944444444445in"
height="5.356944444444444in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 42        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image116.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 43        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image118.jpeg){width="8.810416666666667in"
> height="1.6659722222222222in"}code, is it possible to reconstruct the
> original image?

![](media/image119.jpeg){width="10.0in" height="3.152083333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 44 3 Feb 2016

> ![](media/image120.jpeg){width="9.35625in"
> height="0.8354166666666667in"}

-   Its code is similar to a given code

-   It "looks natural" (image prior regularization)

![](media/image121.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 45 3 Feb 2016

> ![](media/image124.jpeg){width="9.640972222222222in"
> height="0.7444444444444445in"}

![](media/image125.jpeg){width="7.592361111111111in" height="3.94375in"}

> original image

![](media/image126.jpeg){width="2.0819444444444444in"
height="0.8472222222222222in"}

> reconstructions from the 1000 log probabilities for ImageNet (ILSVRC)
> classes

![](media/image127.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 46 3 Feb 2016

> ![](media/image128.jpeg){width="9.47638888888889in"
> height="0.6138888888888889in"}

![](media/image129.jpeg){width="10.0in" height="4.309722222222222in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 47 3 Feb 2016

> ![](media/image130.jpeg){width="9.745138888888889in"
> height="2.0069444444444446in"}

![](media/image131.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 48 3 Feb 2016

> ![](media/image133.jpeg){width="9.847222222222221in"
> height="1.7951388888888888in"}

![](media/image134.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 49 3 Feb 2016

![](media/image136.jpeg){width="10.0in" height="5.58125in"}

> DeepDream
> [[https://github.com/google/deepdream]{.underline}](https://github.com/google/deepdream)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 50 3 Feb 2016

![](media/image137.jpeg){width="9.602777777777778in"
height="5.427777777777778in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 51        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image138.jpeg){width="9.352777777777778in"
> height="4.684027777777778in"}

jitter regularizer

> "image update"

![](media/image139.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 52 3 Feb 2016

![](media/image140.jpeg){width="3.4652777777777777in"
height="0.37916666666666665in"}

> inception\_4c/output

![](media/image141.jpeg){width="9.921527777777778in"
height="2.8666666666666667in"}

> DeepDream modifies the image in a way that "boosts" all activations,
> at any layer
>
> this creates a [feedback loop]{.underline}: e.g. any slightly detected
> dog face will be made more and more dog like over time

![](media/image142.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 53        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image143.jpeg){width="3.4652777777777777in"
> height="0.37916666666666665in"}

![](media/image144.jpeg){width="0.3972222222222222in"
height="5.208880139982502e-3in"}

> DeepDream any layer

![](media/image146.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 54 3 Feb 2016

> ![](media/image147.jpeg){width="3.6347222222222224in"
> height="0.40694444444444444in"}

![](media/image148.jpeg){width="9.921527777777778in"
height="3.033333333333333in"}

> DeepDream modifies the image in a way that "boosts" all activations,
> at any layer

![](media/image149.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 55 3 Feb 2016

> ![](media/image150.jpeg){width="9.777083333333334in"
> height="0.9798611111111111in"}
>
> Deep Dream Grocery Trip
> [[https://www.youtube.com/watch?v=DgPaCWJL7XI]{.underline}](https://www.youtube.com/watch?v=DgPaCWJL7XI)
>
> Deep Dreaming Fear & Loathing in Las Vegas: the Great San Francisco
> Acid Wave
> [[https://www.youtube.com/watch?v=oyxSerkkP4o]{.underline}](https://www.youtube.com/watch?v=oyxSerkkP4o)

![](media/image151.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 56 3 Feb 2016

> ![](media/image152.jpeg){width="9.683333333333334in"
> height="4.894444444444445in"}

-   *A Neural Algorithm of Artistic Style by Leon A. Gatys, Alexander S.
    > Ecker, and Matthias Bethge, 2015\]* **good implementation by
    > Justin in Torch:
    > [[https://github.com/jcjohnson/neural-style]{.underline}](https://github.com/jcjohnson/neural-style)**

![](media/image153.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 57 3 Feb 2016

![](media/image154.jpeg){width="9.972222222222221in"
height="4.893055555555556in"}

> make your own easily on [deepart.io]{.underline}

![](media/image155.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 58        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image156.jpeg){width="7.4527777777777775in"
> height="0.8916666666666667in"}**content targets** (ConvNet activations
> of all layers for the given content image)

![](media/image157.jpeg){width="9.234027777777778in"
height="3.2840277777777778in"}

> content activations
>
> e.g.
>
> at CONV5\_1 layer we would have a \[14x14x512\] array of target
> activations

![](media/image158.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 59 3 Feb 2016

![](media/image159.jpeg){width="7.4527777777777775in"
height="0.8916666666666667in"}

> Step 2: Extract **style targets** (Gram matrices of ConvNet
> activations of all layers for the given style image)

![](media/image160.jpeg){width="9.234027777777778in"
height="3.1152777777777776in"}

> style gram matrices
>
> e.g. ![](media/image161.jpeg){width="1.1180555555555556in"
> height="0.3958333333333333in"} at CONV1 layer (with \[224x224x64\]
> activations) would give a \[64x64\] Gram matrix of all pairwise
> activation covariances (summed across spatial locations)

![](media/image162.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 60        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image163.jpeg){width="9.207638888888889in"
> height="0.8916666666666667in"}

-   The **content** of the content image (activations match content)

-   The **style** of the style image (Gram matrices of activations match
    > style)

![](media/image164.jpeg){width="10.0in" height="1.0902777777777777in"}

(+Total Variation regularization (maybe))

![](media/image165.jpeg){width="8.266666666666667in" height="2.40625in"}

> match content

![](media/image166.jpeg){width="1.1in" height="1.0145833333333334in"}

> match style

![](media/image167.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 61 3 Feb 2016

> ![](media/image168.jpeg){width="9.686805555555555in"
> height="1.6659722222222222in"}
>
> Question: Can we use this to "fool" ConvNets?

![](media/image169.jpeg){width="10.0in" height="1.4902777777777778in"}

> spoiler alert: yeah

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 62 3 Feb 2016

> *\[Intriguing properties of neural networks, Szegedy et al., 2013\]*

![](media/image170.jpeg){width="9.275in" height="4.678472222222222in"}

+---------+---------+---------+---------+---------+---------+---------+
| > corre | > +dist | > ostri | > corre | > +dist | > ostri |         |
| ct      | ort     | ch      | ct      | ort     | ch      |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Fei-F | > Lectu |         | > 3 Feb |         |         |         |
| ei      | re      |         | > 2016  |         |         |         |
| > Li &  | > 9 63  |         |         |         |         |         |
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

![](media/image171.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image172.jpeg){width="9.290277777777778in"
> height="4.700694444444444in"}
>
> \>99.6% confidences

![](media/image173.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 64 3 Feb 2016

> ![](media/image174.jpeg){width="9.290277777777778in"
> height="4.645138888888889in"}
>
> \>99.6% confidences

![](media/image175.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 65 3 Feb 2016

> ![](media/image176.jpeg){width="9.465972222222222in"
> height="0.7006944444444444in"}
>
> *\[Exploring the Representation Capabilities of the HOG Descriptor,
> Tatu et al., 2011\]*

![](media/image177.jpeg){width="8.588194444444444in"
height="2.6118055555555557in"}

> Identical HOG represention

![](media/image178.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 66 3 Feb 2016

> ![](media/image179.jpeg){width="9.066666666666666in"
> height="1.1083333333333334in"}
>
> "primary cause of neural networks' vulnerability to adversarial
> perturbation is their **linear nature**"

![](media/image180.jpeg){width="10.0in" height="3.9590277777777776in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 67 3 Feb 2016

> ![](media/image181.jpeg){width="9.315277777777778in"
> height="2.2333333333333334in"}
>
> (logistic regression)

![](media/image182.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 68 3 Feb 2016

> ![](media/image184.jpeg){width="7.91875in"
> height="0.5194444444444445in"}

![](media/image185.jpeg){width="6.540972222222222in" height="1.075in"}

<table>
<tbody>
<tr class="odd">
<td>x</td>
<td>2</td>
<td>-1</td>
<td>3</td>
<td>-2</td>
<td>2</td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>-4</p>
</blockquote></td>
<td><blockquote>
<p>5</p>
</blockquote></td>
<td>1</td>
<td></td>
</tr>
<tr class="even">
<td>w</td>
<td></td>
<td></td>
<td></td>
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
<td>1</td>
<td>-1</td>
<td>1</td>
<td>-1</td>
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
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
</tr>
</tbody>
</table>

![](media/image186.jpeg){width="10.0in" height="0.5888888888888889in"}

> input example

![](media/image191.jpeg){width="2.145138888888889in"
height="1.1770833333333333in"}

weights

![](media/image192.jpeg){width="4.88125in"
height="0.7111111111111111in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 69 3 Feb 2016

> ![](media/image193.jpeg){width="7.91875in"
> height="0.5194444444444445in"}

![](media/image194.jpeg){width="6.540972222222222in" height="1.075in"}

<table>
<tbody>
<tr class="odd">
<td>x</td>
<td>2</td>
<td>-1</td>
<td>3</td>
<td>-2</td>
<td>2</td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>-4</p>
</blockquote></td>
<td><blockquote>
<p>5</p>
</blockquote></td>
<td>1</td>
<td></td>
</tr>
<tr class="even">
<td>w</td>
<td></td>
<td></td>
<td></td>
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
<td>1</td>
<td>-1</td>
<td>1</td>
<td>-1</td>
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
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
</tr>
</tbody>
</table>

![](media/image195.jpeg){width="0.425in"
height="5.208880139982502e-3in"}

> class 1 score = dot product:
>
> = -2 + 1 + 3 + 2 + 2 - 2 + 1 - 4 - 5 + 1 = -3
>
> =\> probability of class 1 is 1/(1+e\^(-(-3))) = 0.0474
>
> i.e. the classifier is **95%** certain that this is class 0 example.

![](media/image200.jpeg){width="10.0in" height="0.5888888888888889in"}

> input example

![](media/image201.jpeg){width="2.145138888888889in"
height="1.1770833333333333in"}

weights

![](media/image202.jpeg){width="4.88125in"
height="0.7111111111111111in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 70 3 Feb 2016

> ![](media/image203.jpeg){width="7.91875in"
> height="0.5194444444444445in"}

![](media/image204.jpeg){width="6.540972222222222in" height="1.075in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>x</p>
</blockquote></td>
<td>2</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>3</td>
<td><blockquote>
<p>-2</p>
</blockquote></td>
<td>2</td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>-4</p>
</blockquote></td>
<td><blockquote>
<p>5</p>
</blockquote></td>
<td>1</td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>w</p>
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
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td>1</td>
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
</tr>
<tr class="even">
<td>adversarial x</td>
<td>?</td>
<td><blockquote>
<p>?</p>
</blockquote></td>
<td>?</td>
<td><blockquote>
<p>?</p>
</blockquote></td>
<td>?</td>
<td><blockquote>
<p>?</p>
</blockquote></td>
<td>?</td>
<td><blockquote>
<p>?</p>
</blockquote></td>
<td><blockquote>
<p>?</p>
</blockquote></td>
<td>?</td>
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
</tr>
</tbody>
</table>

![](media/image205.jpeg){width="0.425in"
height="5.208880139982502e-3in"}

> class 1 score = dot product:
>
> = -2 + 1 + 3 + 2 + 2 - 2 + 1 - 4 - 5 + 1 = -3
>
> =\> probability of class 1 is 1/(1+e\^(-(-3))) = 0.0474
>
> i.e. the classifier is **95%** certain that this is class 0 example.

![](media/image211.jpeg){width="10.0in" height="0.5888888888888889in"}

> input example

![](media/image212.jpeg){width="2.145138888888889in"
height="1.1770833333333333in"}

weights

![](media/image213.jpeg){width="3.7534722222222223in"
height="0.5527777777777778in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 71 3 Feb 2016

![](media/image214.jpeg){width="7.91875in"
height="0.5194444444444445in"}

> Lets fool a binary linear classifier:

![](media/image215.jpeg){width="9.879861111111111in"
height="3.220833333333333in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>x</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>3</p>
</blockquote></td>
<td><blockquote>
<p>-2</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-4</p>
</blockquote></td>
<td><blockquote>
<p>5</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>w</p>
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
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
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
</tr>
<tr class="even">
<td>adversarial x</td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>-1.5</p>
</blockquote></td>
<td><blockquote>
<p>3.5</p>
</blockquote></td>
<td><blockquote>
<p>-2.5</p>
</blockquote></td>
<td><blockquote>
<p>2.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>-3.5</p>
</blockquote></td>
<td><blockquote>
<p>4.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
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
</tr>
</tbody>
</table>

![](media/image216.jpeg){width="0.425in"
height="5.208880139982502e-3in"}

> input example

weights

> class 1 score before:
>
> -2 + 1 + 3 + 2 + 2 - 2 + 1 - 4 - 5 + 1 = -3
>
> =\> probability of class 1 is 1/(1+e\^(-(-3))) = 0.0474

![](media/image218.jpeg){width="5.860416666666667in"
height="5.208880139982502e-3in"}

> -1.5+1.5+3.5+2.5+2.5-1.5+1.5-3.5-4.5+1.5 = 2
>
> =\> probability of class 1 is now 1/(1+e\^(-(2))) = 0.88
>
> **i.e. we improved the class 1 probability from 5% to 88%**

![](media/image219.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 72        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image220.jpeg){width="7.91875in"
height="0.5194444444444445in"}

> Lets fool a binary linear classifier:

![](media/image221.jpeg){width="9.963194444444444in" height="3.7in"}

<table>
<tbody>
<tr class="odd">
<td><blockquote>
<p>x</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>3</p>
</blockquote></td>
<td><blockquote>
<p>-2</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>2</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-4</p>
</blockquote></td>
<td><blockquote>
<p>5</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>w</p>
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
<td>1</td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
</blockquote></td>
<td><blockquote>
<p>-1</p>
</blockquote></td>
<td><blockquote>
<p>1</p>
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
</tr>
<tr class="even">
<td>adversarial x</td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>-1.5</p>
</blockquote></td>
<td><blockquote>
<p>3.5</p>
</blockquote></td>
<td><blockquote>
<p>-2.5</p>
</blockquote></td>
<td><blockquote>
<p>2.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
</blockquote></td>
<td><blockquote>
<p>-3.5</p>
</blockquote></td>
<td><blockquote>
<p>4.5</p>
</blockquote></td>
<td><blockquote>
<p>1.5</p>
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
</tr>
</tbody>
</table>

![](media/image222.jpeg){width="0.425in"
height="5.208880139982502e-3in"}

> input example

weights

> class 1 score before:
>
> -2 + 1 + 3 + 2 + 2 - 2 + 1 - 4 - 5 + 1 = -3
>
> =\> probability of class 1 is 1/(1+e\^(-(-3))) = 0.0474

![](media/image224.jpeg){width="5.860416666666667in"
height="5.208880139982502e-3in"}

> -1.5+1.5+3.5+2.5+2.5-1.5+1.5-3.5-4.5+1.5 = 2
>
> =\> probability of class 1 is now 1/(1+e\^(-(2))) = 0.88
>
> **i.e. we improved the class 1 probability from 5% to 88%**

![](media/image225.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

image has 150,528.

(It's significantly easier with more numbers, need smaller nudge for
each)

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 73        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image226.jpeg){width="7.735416666666667in"
> height="0.6888888888888889in"}

![](media/image227.jpeg){width="9.165277777777778in"
height="0.6541666666666667in"}

> Recall CIFAR-10 linear classifiers:

![](media/image228.jpeg){width="9.688888888888888in"
height="3.217361111111111in"}

> ImageNet classifiers:

![](media/image229.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 74 3 Feb 2016

![](media/image230.jpeg){width="3.334722222222222in"
height="0.4583333333333333in"}

> mix in a tiny bit of
>
> Goldfish classifier weights

![](media/image231.jpeg){width="9.551388888888889in"
height="3.0131944444444443in"}

> \+ ~=~

![](media/image232.jpeg){width="0.6972222222222222in"
height="0.38055555555555554in"}

> **100% Goldfish**

![](media/image234.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 75        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image235.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 76        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image237.jpeg){width="9.602777777777778in" height="5.5125in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 9 77        | > 3 Feb 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image238.jpeg){width="9.665277777777778in"
> height="2.0590277777777777in"}
>
> "primary cause of neural networks' vulnerability to adversarial
> perturbation is their **linear nature**"
>
> (and very high-dimensional, sparsely-populated input spaces)
>
> In particular, this is not a problem with Deep Learning, and has
> little to do with ConvNets specifically. Same issue would come up with
> Neural Nets in any other modalities.

![](media/image239.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 78 3 Feb 2016

> Summary

![](media/image240.jpeg){width="9.417361111111111in" height="1.0875in"}

> Backpropping to the image is powerful. It can be used for:

-   **Understanding** (e.g. visualize optimal stimuli for arbitrary
    > neurons)

-   **Segmenting** objects in the image (kind of)

-   **Inverting** codes and introducing privacy concerns

-   **Fun** (NeuralStyle/DeepDream)

-   **Confusion and chaos** (Adversarial examples)

![](media/image241.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 79 3 Feb 2016

> ![](media/image242.jpeg){width="9.419444444444444in"
> height="4.864583333333333in"}
>
> Image Captioning Recurrent Neural Networks RNN Language Models

![](media/image243.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 80 3 Feb 2016

> ![](media/image244.jpeg){width="0.5305555555555556in"
> height="0.38958333333333334in"} ReLU W2 ReLU

![](media/image248.jpeg){width="9.105555555555556in" height="3.14375in"}

> 5 ![](media/image249.jpeg){width="1.1895833333333334in"
> height="0.12222222222222222in"} 2
> ![](media/image250.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 2
> ![](media/image251.jpeg){width="1.1895833333333334in"
> height="0.12222222222222222in"} 4
> ![](media/image252.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 4

![](media/image253.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

> W3
>
> -2 ![](media/image257.jpeg){width="1.1854166666666666in"
> height="0.1527777777777778in"} 3
> ![](media/image258.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 3
> ![](media/image259.jpeg){width="1.1854166666666666in"
> height="0.15347222222222223in"} -2
> ![](media/image260.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 0
> ![](media/image261.jpeg){width="0.8493055555555555in"
> height="0.1625in"} 5

![](media/image262.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

> 1 ![](media/image267.jpeg){width="1.1895833333333334in"
> height="0.12222222222222222in"} -2
> ![](media/image268.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 0
> ![](media/image269.jpeg){width="1.1895833333333334in"
> height="0.12222222222222222in"} -3
> ![](media/image270.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 0

![](media/image271.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 81 3 Feb 2016

> ![](media/image276.jpeg){width="9.093055555555555in"
> height="0.4583333333333333in"}: all +ve and -ve paths of influence
> through the graph interfere

![](media/image277.jpeg){width="9.105555555555556in"
height="3.411111111111111in"}

> W1 ReLU W2 ReLU
>
> 5 ![](media/image278.jpeg){width="1.2034722222222223in"
> height="0.24444444444444444in"} 2
> ![](media/image279.jpeg){width="0.4597222222222222in"
> height="0.15208333333333332in"} 2
> ![](media/image280.jpeg){width="1.2034722222222223in"
> height="0.24444444444444444in"} 4
> ![](media/image281.jpeg){width="0.4597222222222222in"
> height="0.15208333333333332in"} 4

![](media/image282.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

> W3
>
> -2 ![](media/image286.jpeg){width="1.1958333333333333in"
> height="0.30625in"} 3
> ![](media/image287.jpeg){width="0.4597222222222222in"
> height="0.15208333333333332in"} 3
> ![](media/image288.jpeg){width="1.1854166666666666in"
> height="0.15347222222222223in"} -2
> ![](media/image289.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 0
> ![](media/image290.jpeg){width="0.8611111111111112in"
> height="0.24375in"} 5

![](media/image291.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

-   ![](media/image296.jpeg){width="1.1895833333333334in"
    > height="0.12222222222222222in"} -2
    > ![](media/image297.jpeg){width="0.45416666666666666in"
    > height="7.63888888888889e-2in"} 0
    > ![](media/image298.jpeg){width="1.1895833333333334in"
    > height="0.12222222222222222in"} -3
    > ![](media/image299.jpeg){width="0.45416666666666666in"
    > height="7.63888888888889e-2in"} 0 positive gradient, negative
    > gradient, zero gradient

![](media/image300.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 82 3 Feb 2016

> ![](media/image306.jpeg){width="9.093055555555555in"
> height="0.4583333333333333in"}: cancel out -ve paths of influence at
> each step (i.e. we only keep positive paths of influence)

![](media/image307.jpeg){width="9.105555555555556in"
height="3.411111111111111in"}

> W1 ReLU W2 ReLU
>
> 5 ![](media/image308.jpeg){width="1.2034722222222223in"
> height="0.24444444444444444in"} 2
> ![](media/image309.jpeg){width="0.4597222222222222in"
> height="0.15208333333333332in"} 2
> ![](media/image310.jpeg){width="1.2034722222222223in"
> height="0.24444444444444444in"} 4
> ![](media/image311.jpeg){width="0.4597222222222222in"
> height="0.15208333333333332in"} 4

![](media/image312.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

> W3
>
> -2 ![](media/image316.jpeg){width="1.1854166666666666in"
> height="0.1527777777777778in"} 3 **X**
> ![](media/image317.jpeg){width="8.888888888888889e-2in"
> height="7.63888888888889e-2in"} 3
> ![](media/image318.jpeg){width="1.1854166666666666in"
> height="0.15347222222222223in"} -2
> ![](media/image319.jpeg){width="0.45416666666666666in"
> height="7.63888888888889e-2in"} 0
> ![](media/image320.jpeg){width="0.8611111111111112in"
> height="0.24375in"} 5

![](media/image321.jpeg){width="1.1756944444444444in"
height="5.208880139982502e-3in"}

-   ![](media/image326.jpeg){width="1.1895833333333334in"
    > height="0.12222222222222222in"} -2
    > ![](media/image327.jpeg){width="0.45416666666666666in"
    > height="7.63888888888889e-2in"} 0
    > ![](media/image328.jpeg){width="1.1895833333333334in"
    > height="0.12222222222222222in"} -3
    > ![](media/image329.jpeg){width="0.45416666666666666in"
    > height="7.63888888888889e-2in"} 0 positive gradient, negative
    > gradient, zero gradient

![](media/image330.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 9 83 3 Feb 2016
