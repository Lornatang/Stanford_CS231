![](media/image1.jpeg){width="9.73125in" height="4.50625in"}

CNNs in Practice

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 1 17 Feb 2016

> ![](media/image3.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image4.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Midterms are graded!

    -   Pick up now

    -   Or in Andrej, Justin, Albert, or Serena's OH

-   Project milestone due today, 2/17 by midnight

    -   Turn in to Assignments tab on Coursework!

-   Assignment 2 grades soon

-   Assignment 3 released, due 2/24

![](media/image5.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 2 17 Feb 2016

> ![](media/image6.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image7.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Mean:** 75.0 **Median:** 76.3 **Standard Deviation:** 13.2
>
> **N:** 311 **Max:** 103.0

![](media/image8.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 3 17 Feb 2016

> ![](media/image9.jpeg){width="9.377083333333333in"
> height="3.4479166666666665in"}

\[We threw out TF3 and TF8\]

![](media/image10.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 4 17 Feb 2016

> ![](media/image11.jpeg){width="9.690277777777778in"
> height="4.657638888888889in"}

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 5 17 Feb 2016

> ![](media/image13.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image14.jpeg){width="9.946527777777778in"
height="3.683333333333333in"}

> **Bonus mean:** 0.8

![](media/image15.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 6 17 Feb 2016

> ![](media/image16.jpeg){width="9.027777777777779in"
> height="1.1409722222222223in"}

Vanilla RNNs

![](media/image17.jpeg){width="8.309027777777779in"
height="2.7666666666666666in"}

> LSTMs

![](media/image18.jpeg){width="2.310416666666667in"
height="1.4604166666666667in"}

> Recurrent neural networks
>
> for modeling sequences

![](media/image20.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 7 17 Feb 2016

![](media/image21.jpeg){width="9.027777777777779in"
height="4.180555555555555in"}

> Last Time

![](media/image22.jpeg){width="6.996527777777778in"
height="0.5194444444444445in"}

Sampling from RNN language models to generate text

![](media/image23.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 11 8        | > 17 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image24.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image25.jpeg){width="8.970138888888888in"
height="2.691666666666667in"}

+------------------+---------------------------+--+
| CNN + RNN for    | > Interpretable RNN cells |  |
+------------------+---------------------------+--+
| image captioning |                           |  |
+------------------+---------------------------+--+
|                  |                           |  |
+------------------+---------------------------+--+

![](media/image26.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 9 17 Feb 2016

> ![](media/image27.jpeg){width="9.027777777777779in"
> height="4.614583333333333in"}
>
> Working with CNNs in practice:

-   Making the most of your data

    -   Data augmentation

    -   Transfer learning

-   All about convolutions:

    -   How to arrange them

    -   How to compute them fast

-   "Implementation details"

    -   GPU / CPU, bottlenecks, distributed training

![](media/image28.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 10 17 Feb 2016

> Data Augmentation

![](media/image29.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 11 17 Feb 2016

> ![](media/image30.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image31.jpeg){width="7.932638888888889in" height="2.54375in"}

> Load image
>
> and label

![](media/image32.jpeg){width="0.8243055555555555in"
height="5.208880139982502e-3in"}

![](media/image33.jpeg){width="0.27361111111111114in"
height="0.24166666666666667in"} "cat"

![](media/image34.jpeg){width="1.3840277777777779in"
height="0.7979166666666667in"}

> Compute
>
> loss

CNN

![](media/image35.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 12 17 Feb 2016

> ![](media/image37.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image38.jpeg){width="7.932638888888889in"
height="2.9722222222222223in"}

> Load image
>
> and label

![](media/image39.jpeg){width="0.8243055555555555in"
height="5.208880139982502e-3in"}

![](media/image40.jpeg){width="0.27361111111111114in"
height="0.24166666666666667in"} "cat"

![](media/image41.jpeg){width="1.3840277777777779in"
height="0.7979166666666667in"}

> Compute
>
> loss
>
> CNN

![](media/image42.jpeg){width="0.5319444444444444in"
height="5.208880139982502e-3in"}

> Transform image

![](media/image44.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 13 17 Feb 2016

> ![](media/image45.jpeg){width="4.979166666666667in"
> height="0.85625in"}

![](media/image46.jpeg){width="4.784027777777778in" height="3.625in"}

> \- Change the pixels without changing the label

What the computer sees

-   Train on transformed data

-   VERY widely used

![](media/image47.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 14 17 Feb 2016

> ![](media/image48.jpeg){width="6.99375in" height="1.73125in"}

1\. Horizontal flips

![](media/image49.jpeg){width="10.0in" height="3.5597222222222222in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 15 17 Feb
> 2016
>
> ![](media/image50.jpeg){width="10.0in" height="5.560416666666667in"}
>
> 2\. Random crops/scales
>
> **Training**: sample random crops / scales

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 16 17 Feb 2016

> ![](media/image51.jpeg){width="10.0in" height="5.560416666666667in"}
>
> 2\. Random crops/scales
>
> **Training**: sample random crops / scales
>
> ResNet:

1.  Pick random L in range \[256, 480\]

2.  Resize training image, short side = L

3.  Sample random 224 x 224 patch

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 17 17 Feb 2016

> ![](media/image52.jpeg){width="10.0in" height="5.560416666666667in"}
>
> 2\. Random crops/scales
>
> **Training**: sample random crops / scales
>
> ResNet:

1.  Pick random L in range \[256, 480\]

2.  Resize training image, short side = L

3.  Sample random 224 x 224 patch

> **Testing**: average a fixed set of crops

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 18 17 Feb 2016

![](media/image53.jpeg){width="9.77361111111111in"
height="5.560416666666667in"}

> **Data Augmentation**
>
> 2\. Random crops/scales
>
> **Training**: sample random crops / scales
>
> ResNet:

1.  Pick random L in range \[256, 480\]

2.  Resize training image, short side = L

3.  Sample random 224 x 224 patch

> **Testing**: average a fixed set of crops
>
> ResNet:

1.  Resize image at 5 scales: {224, 256, 384, 480, 640}

2.  For each size, use 10 224 x 224 crops: 4 corners + center, + flips

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 11 19       | > 17 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image54.jpeg){width="10.0in" height="5.560416666666667in"}
>
> 3\. Color jitter
>
> **Simple**:
>
> Randomly jitter contrast

![](media/image55.jpeg){width="0.7611111111111111in"
height="5.208880139982502e-3in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 20 17 Feb 2016

> **Data Augmentation** 3. Color jitter
>
> **Simple**:
>
> Randomly jitter contrast

![](media/image56.jpeg){width="0.7611111111111111in"
height="5.208880139982502e-3in"}

> **Complex**:

![](media/image57.jpeg){width="10.0in" height="5.560416666666667in"}

1.  Apply PCA to all \[R, G, B\] pixels in training set

2.  Sample a "color offset" along principal component directions

3.  Add offset to all pixels of a training image

> (As seen in *\[Krizhevsky et al. 2012\],* ResNet, etc)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 21 17 Feb 2016

> ![](media/image58.jpeg){width="6.99375in" height="1.275in"}
>
> 4\. Get creative!

![](media/image59.jpeg){width="8.716666666666667in"
height="3.308333333333333in"}

> Random mix/combinations of :

-   translation

-   rotation

-   stretching

-   shearing,

-   lens distortions, ... (go crazy)

![](media/image60.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 22 17 Feb 2016

![](media/image61.jpeg){width="6.941666666666666in"
height="1.6881944444444446in"}

> **A general theme:**

1.  **Training**: Add random noise

2.  **Testing**: Marginalize over the noise

![](media/image62.jpeg){width="9.172222222222222in"
height="2.1173611111111112in"}

> Dropout DropConnect

![](media/image63.jpeg){width="2.51875in" height="0.5125in"}

> Data Augmentation

![](media/image64.jpeg){width="7.2375in" height="0.5465277777777777in"}

> Batch normalization, Model ensembles

![](media/image65.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 11 23       | > 17 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image66.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image67.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Simple to implement, use it

-   Especially useful for small datasets

-   Fits into framework of noise / marginalization

![](media/image68.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 24 17 Feb 2016

![](media/image69.jpeg){width="8.53125in" height="4.209722222222222in"}

"You need a lot of a data if you want to

train/use CNNs"

![](media/image70.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 25 17 Feb 2016

![](media/image71.jpeg){width="8.53125in" height="4.524305555555555in"}

> "You need a lot want to

![](media/image72.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 26 17 Feb 2016

> ![](media/image73.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image74.jpeg){width="3.0375in" height="3.932638888888889in"}

1.  Train on Imagenet

![](media/image75.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 27 17 Feb 2016

> ![](media/image76.jpeg){width="8.926388888888889in"
> height="4.679861111111111in"}
>
> 2\. Small dataset:
>
> 1\. Train on feature extractor
>
> Imagenet
>
> Freeze these
>
> ![](media/image77.jpeg){width="1.148611111111111in"
> height="0.41805555555555557in"} Train this

![](media/image79.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 28 17 Feb 2016

> ![](media/image81.jpeg){width="9.81875in"
> height="4.691666666666666in"}

+--------------+-------------------------+
|              | > 2\. Small dataset:    |
+--------------+-------------------------+
| 1\. Train on | > **feature extractor** |
+--------------+-------------------------+
| Imagenet     |                         |
+--------------+-------------------------+

> Freeze these
>
> ![](media/image82.jpeg){width="1.148611111111111in"
> height="0.41805555555555557in"} Train this

![](media/image84.jpeg){width="10.0in" height="0.5888888888888889in"}

3.  Medium dataset: **finetuning**

> more data = retrain more of the network (or all of it)
>
> Freeze these

![](media/image86.jpeg){width="0.6618055555555555in"
height="0.15208333333333332in"} Train this

![](media/image87.jpeg){width="0.6506944444444445in"
height="5.208880139982502e-3in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 29 17 Feb 2016

> ![](media/image88.jpeg){width="9.81875in"
> height="4.691666666666666in"}

+--------------+-------------------------+
|              | > 2\. Small dataset:    |
+--------------+-------------------------+
| 1\. Train on | > **feature extractor** |
+--------------+-------------------------+
| Imagenet     |                         |
+--------------+-------------------------+

> Freeze these
>
> ![](media/image89.jpeg){width="1.148611111111111in"
> height="0.41805555555555557in"} Train this

![](media/image91.jpeg){width="10.0in" height="0.5888888888888889in"}

3.  Medium dataset: **finetuning**

> more data = retrain more of the network (or all of it)
>
> Freeze these
>
> tip: use only \~1/10th of the original learning rate in finetuning top
> layer, and \~1/100th on intermediate layers

![](media/image93.jpeg){width="0.6618055555555555in"
height="0.15208333333333332in"} Train this

![](media/image94.jpeg){width="0.6506944444444445in"
height="5.208880139982502e-3in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 30 17 Feb 2016

> ![](media/image95.jpeg){width="10.0in" height="5.5368055555555555in"}

![](media/image96.jpeg){width="5.208880139982502e-3in"
height="4.126388888888889in"}

*DeCAF: A Deep*

*Convolutional Activation*

*Feature for Generic Visual*

*Recognition*

*\[Donahue\*, Jia\*, et al.,*

*2013\]*

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 31 17 Feb
> 2016

+-------------+-------------+-------------+-------------+-------------+
|             |             | > **very    | > **very    |             |
|             |             | > similar** | > different |             |
|             |             |             | **          |             |
+-------------+-------------+-------------+-------------+-------------+
| more        |             | > **dataset | > **dataset |             |
| generic     |             | **          | **          |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **very    | > ?         | > ?         |             |
|             | > little    |             |             |             |
|             | > data**    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > more      |             |             |             |             |
| > specific  |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **quite a | > ?         | > ?         |             |
|             | > lot of**  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **data**  |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image97.jpeg){width="3.222916666666667in"
height="4.876388888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 32 17 Feb 2016

+-------------+-------------+-------------+-------------+-------------+
|             |             | > **very    | > **very    |             |
|             |             | > similar** | > different |             |
|             |             |             | **          |             |
+-------------+-------------+-------------+-------------+-------------+
| more        |             | > **dataset | > **dataset |             |
| generic     |             | **          | **          |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **very    | > Use       | > ?         |             |
|             | > little    | > Linear    |             |             |
|             | > data**    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > more      |             | > Classifie |             |             |
| > specific  |             | r           |             |             |
|             |             | > on top    |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             | > layer     |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **quite a | > Finetune  | > ?         |             |
|             | > lot of**  | > a few     |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             | > **data**  | > layers    |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image99.jpeg){width="3.222916666666667in"
height="4.876388888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 33 17 Feb 2016

![](media/image101.jpeg){width="3.222916666666667in"
height="4.876388888888889in"}

> more generic
>
> more specific

+------------------------+---------------------+----------------------+
|                        | > **very similar**  | > **very different** |
+------------------------+---------------------+----------------------+
|                        | > **dataset**       | > **dataset**        |
+------------------------+---------------------+----------------------+
|                        |                     |                      |
+------------------------+---------------------+----------------------+
| > **very little data** | > Use Linear        | > You're in          |
+------------------------+---------------------+----------------------+
|                        | > Classifier on top | > trouble... Try     |
+------------------------+---------------------+----------------------+
|                        | > layer             | > linear classifier  |
+------------------------+---------------------+----------------------+
|                        |                     | > from different     |
+------------------------+---------------------+----------------------+
|                        |                     | > stages             |
+------------------------+---------------------+----------------------+
|                        |                     |                      |
+------------------------+---------------------+----------------------+
| > **quite a lot of**   | > Finetune a few    | > Finetune a         |
+------------------------+---------------------+----------------------+
| > **data**             | > layers            | > larger number of   |
+------------------------+---------------------+----------------------+
|                        |                     | > layers             |
+------------------------+---------------------+----------------------+
|                        |                     |                      |
+------------------------+---------------------+----------------------+

![](media/image102.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 34 17 Feb 2016

> ![](media/image103.jpeg){width="9.65625in"
> height="3.9881944444444444in"}
>
> (it's the norm, not an exception)

Image Captioning: CNN + RNN

> Object Detection
>
> (Faster R-CNN)

![](media/image104.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 35 17 Feb 2016

> ![](media/image105.jpeg){width="9.65625in"
> height="3.9881944444444444in"}
>
> (it's the norm, not an exception)

Image Captioning: CNN + RNN

> CNN pretrained on ImageNet
>
> Object Detection
>
> (Faster R-CNN)

![](media/image106.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 36 17 Feb 2016

![](media/image107.jpeg){width="9.65625in" height="4.8in"}

> Transfer learning with CNNs is pervasive...
>
> (it's the norm, not an exception)

Image Captioning: CNN + RNN

> CNN pretrained on ImageNet
>
> Object Detection
>
> (Faster R-CNN)
>
> Word vectors pretrained
> ![](media/image108.jpeg){width="0.6368055555555555in" height="0.5in"}
> from word2vec

![](media/image109.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 11 37       | > 17 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image110.jpeg){width="9.749305555555555in"
> height="4.377777777777778in"}
>
> Have some dataset of interest but it has \< \~1M images?

1.  Find a very large dataset that has similar data, train a big ConvNet
    > there.

2.  Transfer learn to your dataset

> Caffe ConvNet library has a **"Model Zoo"** of pretrained models:
>
> [[https://github.com/BVLC/caffe/wiki/Model-Zoo]{.underline}](https://github.com/BVLC/caffe/wiki/Model-Zoo)

![](media/image111.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 38 17 Feb 2016

![](media/image112.jpeg){width="5.926388888888889in"
height="1.5041666666666667in"}

All About Convolutions

![](media/image113.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 39 17 Feb 2016

![](media/image114.jpeg){width="5.926388888888889in"
height="1.5041666666666667in"}

All About Convolutions

Part I: How to stack them

![](media/image115.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 40 17 Feb 2016

![](media/image116.jpeg){width="8.926388888888889in"
height="0.6965277777777777in"}

> **The power of small filters**

![](media/image117.jpeg){width="9.286805555555556in"
height="1.3340277777777778in"}

> Suppose we stack two 3x3 conv layers (stride 1)
>
> Each neuron sees 3x3 region of previous activation map

![](media/image118.jpeg){width="8.329166666666667in"
height="2.5381944444444446in"}

+-----------------+-----------------+-----------------+-----------------+
| > Input         | > First Conv    | > Second Conv   |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11 41 | > 17 Feb 2016   |                 |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image119.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image120.jpeg){width="8.926388888888889in"
height="0.6965277777777777in"}

> **The power of small filters**

![](media/image121.jpeg){width="9.286805555555556in"
height="1.3340277777777778in"}

> **Question**: How big of a region in the input does a neuron on the
> second conv layer see?

![](media/image122.jpeg){width="8.329166666666667in"
height="2.5381944444444446in"}

+-----------------+-----------------+-----------------+-----------------+
| > Input         | > First Conv    | > Second Conv   |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11 42 | > 17 Feb 2016   |                 |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image123.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image124.jpeg){width="8.926388888888889in"
height="0.6965277777777777in"}

> **The power of small filters**

![](media/image125.jpeg){width="9.286805555555556in"
height="1.3340277777777778in"}

> **Question**: How big of a region in the input does a neuron on the
> second conv layer see?
>
> **Answer**: 5 x 5

![](media/image126.jpeg){width="8.329166666666667in"
height="2.5381944444444446in"}

+-----------------+-----------------+-----------------+-----------------+
| > Input         | > First Conv    | > Second Conv   |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11 43 | > 17 Feb 2016   |                 |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image127.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image128.jpeg){width="9.452083333333333in"
> height="1.9972222222222222in"}
>
> **Question**: If we stack **three** 3x3 conv layers, how big of an
> input region does a neuron in the third layer see?

![](media/image129.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 44 17 Feb 2016

> ![](media/image130.jpeg){width="9.452083333333333in"
> height="4.772222222222222in"}
>
> **Question**: If we stack **three** 3x3 conv layers, how big of an
> input region does a neuron in the third layer see?
>
> **Answer: 7 x 7**

X

![](media/image131.jpeg){width="0.8652777777777778in"
height="0.45694444444444443in"} X

![](media/image132.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 45 17 Feb 2016

> ![](media/image133.jpeg){width="9.452083333333333in"
> height="4.772222222222222in"}
>
> **Question**: If we stack **three** 3x3 conv layers, how big of an
> input region does a neuron in the third layer see?
>
> **Answer: 7 x 7**

X

![](media/image134.jpeg){width="0.8652777777777778in"
height="0.45694444444444443in"} X

![](media/image135.jpeg){width="10.0in" height="0.5888888888888889in"}

Three 3 x 3 conv

gives similar

representational

power as a single

7 x 7 convolution

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 46 17 Feb 2016

> ![](media/image136.jpeg){width="9.452083333333333in"
> height="1.7493055555555554in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)

![](media/image137.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 47 17 Feb 2016

> ![](media/image138.jpeg){width="9.676388888888889in"
> height="4.718055555555556in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters three CONV with 3 x 3 filters
>
> Number of weights: Number of weights:

![](media/image139.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 48 17 Feb 2016

> ![](media/image140.jpeg){width="9.676388888888889in"
> height="4.718055555555556in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters three CONV with 3 x 3 filters
>
> Number of weights: Number of weights:
>
> = C x (7 x 7 x C) = **49 C^2^** = 3 x C x (3 x 3 x C) = **27 C^2^**

![](media/image141.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 49 17 Feb 2016

> ![](media/image142.jpeg){width="9.676388888888889in"
> height="4.903472222222222in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters three CONV with 3 x 3 filters
>
> Number of weights: Number of weights:
>
> = C x (7 x 7 x C) = **49 C^2^** = 3 x C x (3 x 3 x C) = **27 C^2^**
>
> Fewer parameters, more nonlinearity = GOOD

![](media/image143.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 50 17 Feb 2016

> ![](media/image144.jpeg){width="9.676388888888889in"
> height="4.718055555555556in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters three CONV with 3 x 3 filters
>
> Number of weights: Number of weights:
>
> = C x (7 x 7 x C) = 49 C^2^ = 3 x C x (3 x 3 x C) = 27 C^2^
>
> Number of multiply-adds: Number of multiply-adds:

![](media/image145.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 51 17 Feb 2016

> ![](media/image146.jpeg){width="9.676388888888889in"
> height="4.718055555555556in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters
>
> Number of weights:
>
> = C x (7 x 7 x C) = 49 C^2^
>
> Number of multiply-adds:

-   (H x W x C) x (7 x 7 x C)

-   **49 HWC^2^**

three CONV with 3 x 3 filters

Number of weights:

= 3 x C x (3 x 3 x C) = 27 C^2^

Number of multiply-adds:

-   3 x (H x W x C) x (3 x 3 x C)

-   **27 HWC^2^**

![](media/image147.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 52 17 Feb 2016

> ![](media/image148.jpeg){width="9.676388888888889in"
> height="4.903472222222222in"}
>
> Suppose input is H x W x C and we use convolutions with C filters to
> preserve depth (stride 1, padding to preserve H, W)
>
> one CONV with 7 x 7 filters three CONV with 3 x 3 filters
>
> Number of weights: Number of weights:
>
> = C x (7 x 7 x C) = 49 C^2^ = 3 x C x (3 x 3 x C) = 27 C^2^
>
> Number of multiply-adds: Number of multiply-adds:
>
> = **49 HWC^2^** = **27
> HWC^2\ ^**![](media/image149.jpeg){width="0.6236111111111111in"
> height="0.5486111111111112in"}
>
> Less compute, more nonlinearity = GOOD

![](media/image150.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 53 17 Feb 2016

> ![](media/image151.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image152.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?

![](media/image153.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 54 17 Feb 2016

> ![](media/image154.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image155.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?

![](media/image156.jpeg){width="10.0in" height="4.060416666666667in"}

+-----------+-------------------------------+--+
| H x W x C | > 1\. "bottleneck" 1 x 1 conv |  |
+-----------+-------------------------------+--+
|           | > to reduce dimension         |  |
+-----------+-------------------------------+--+
|           |                               |  |
+-----------+-------------------------------+--+

> Conv 1x1, C/2 filters
>
> H x W x (C / 2)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 55 17 Feb 2016

> ![](media/image157.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image158.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?

![](media/image159.jpeg){width="10.0in" height="4.060416666666667in"}

> H x W x C
>
> Conv 1x1, C/2 filters
>
> H x W x (C / 2)
>
> Conv 3x3, C/2 filters

1.  "bottleneck" 1 x 1 conv to reduce dimension

2.  3 x 3 conv at reduced dimension

> H x W x (C / 2)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 56 17 Feb 2016

> ![](media/image160.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image161.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?

![](media/image162.jpeg){width="10.0in" height="4.060416666666667in"}

> H x W x C
>
> Conv 1x1, C/2 filters
>
> H x W x (C / 2)
>
> Conv 3x3, C/2 filters
>
> H x W x (C / 2)

![](media/image163.jpeg){width="5.208880139982502e-3in"
height="0.4951388888888889in"}

> Conv 1x1, C filters
>
> H x W x C

1.  "bottleneck" 1 x 1 conv to reduce dimension

2.  3 x 3 conv at reduced dimension

3.  Restore dimension with another 1 x 1 conv

\[Seen in Lin et al, "Network in Network", GoogLeNet, ResNet\]

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 57 17 Feb 2016

> ![](media/image164.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image165.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?

![](media/image166.jpeg){width="10.0in" height="3.952777777777778in"}

> H x W x C
>
> Conv 1x1, C/2 filters
>
> H x W x (C / 2)
>
> Conv 3x3, C/2 filters
>
> H x W x (C / 2)

![](media/image167.jpeg){width="5.208880139982502e-3in"
height="0.4951388888888889in"}

> Conv 1x1, C filters
>
> H x W x C

+----------------+-------------+--+
| **Bottleneck** | > H x W x C |  |
+----------------+-------------+--+
| **sandwich**   |             |  |
+----------------+-------------+--+

Conv 3x3, C filters

+----------------+-------------+--+
| **Single**     | > H x W x C |  |
+----------------+-------------+--+
| **3 x 3 conv** |             |  |
+----------------+-------------+--+

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 58 17 Feb 2016

> ![](media/image168.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image169.jpeg){width="10.0in" height="4.749305555555556in"}

> Why stop at 3 x 3 filters? Why not try 1 x 1?
>
> H x W x C

More nonlinearity,

> fewer params, less compute!

+-----------------------+------------------+-------------+--+
| Conv 1x1, C/2 filters | > **3.25 C^2^**  | > H x W x C |  |
+-----------------------+------------------+-------------+--+
|                       | > **parameters** |             |  |
+-----------------------+------------------+-------------+--+
|                       |                  |             |  |
+-----------------------+------------------+-------------+--+

> H x W x (C / 2)

+-----------------------+-----------------------+
| Conv 3x3, C/2 filters | > Conv 3x3, C filters |
+-----------------------+-----------------------+

+---------------------+------------+-------------+----------------+--+--+
| > H x W x (C / 2)   | **9 C^2^** | > H x W x C |                |  |  |
+---------------------+------------+-------------+----------------+--+--+
| Conv 1x1, C filters |            |             | **parameters** |  |  |
+---------------------+------------+-------------+----------------+--+--+
|                     |            |             |                |  |  |
+---------------------+------------+-------------+----------------+--+--+
|                     |            |             |                |  |  |
+---------------------+------------+-------------+----------------+--+--+
|                     |            |             |                |  |  |
+---------------------+------------+-------------+----------------+--+--+

![](media/image170.jpeg){width="5.208880139982502e-3in"
height="0.4951388888888889in"}

> H x W x C

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 59 17 Feb 2016

> ![](media/image171.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image172.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Still using 3 x 3 filters ... can we break it up?

![](media/image173.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 60 17 Feb 2016

> ![](media/image174.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image175.jpeg){width="9.609722222222222in"
height="0.6729166666666667in"}

> Still using 3 x 3 filters ... can we break it up?

![](media/image176.jpeg){width="3.6930555555555555in"
height="2.3868055555555556in"}

> H x W x C
>
> Conv 1x3, C filters
>
> H x W x C
>
> Conv 3x1, C filters
>
> H x W x C

![](media/image177.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 61 17 Feb 2016

> ![](media/image178.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image179.jpeg){width="9.609722222222222in"
height="1.1916666666666667in"}

> Still using 3 x 3 filters ... can we break it up?

![](media/image180.jpeg){width="9.827083333333333in"
height="2.620833333333333in"}

More nonlinearity,

> fewer params, less compute!

+---------------------+----------------+------------------+-----------------------+--+--+
| > H x W x C         | > **6 C^2^**   | > H x W x C      |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
| Conv 1x3, C filters |                |                  |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
|                     |                | > **parameters** |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
|                     |                |                  |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
| > H x W x C         |                |                  | > Conv 3x3, C filters |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
| Conv 3x1, C filters |                | **9 C^2^**       |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
|                     |                |                  | > H x W x C           |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+
| > H x W x C         | **parameters** |                  |                       |  |  |
+---------------------+----------------+------------------+-----------------------+--+--+

![](media/image181.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 62 17 Feb 2016

> ![](media/image182.jpeg){width="8.926388888888889in"
> height="0.6965277777777777in"}

![](media/image183.jpeg){width="9.609722222222222in"
height="3.5868055555555554in"}

> Latest version of GoogLeNet incorporates all these ideas

![](media/image184.jpeg){width="10.0in" height="1.038888888888889in"}

> Szegedy et al, "Rethinking the Inception Architecture for Computer
> Vision"

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 63 17 Feb 2016

> ![](media/image185.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image186.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Replace large convolutions (5 x 5, 7 x 7) with stacks of 3 x 3
    > convolutions

-   1 x 1 "bottleneck" convolutions are very efficient

-   Can factor N x N convolutions into 1 x N and N x 1

-   All of the above give fewer parameters, less compute, more
    > nonlinearity

![](media/image187.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 64 17 Feb 2016

![](media/image188.jpeg){width="6.966666666666667in"
height="1.5041666666666667in"}

All About Convolutions

Part II: How to compute them

![](media/image189.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 65 17 Feb 2016

> ![](media/image190.jpeg){width="9.027777777777779in"
> height="4.290972222222222in"}
>
> There are highly optimized matrix multiplication routines for just
> about every platform
>
> Can we turn convolution into matrix multiplication?

![](media/image191.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 66 17 Feb 2016

> ![](media/image192.jpeg){width="9.161805555555556in"
> height="2.6458333333333335in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image193.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image195.jpeg){width="9.274305555555555in"
> height="4.1618055555555555in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image196.jpeg){width="5.208880139982502e-3in"
height="0.4013888888888889in"}

> Reshape K x K x C
>
> receptive field to column
>
> with K^2^C elements

![](media/image197.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image198.jpeg){width="9.274305555555555in"
> height="4.1618055555555555in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image199.jpeg){width="4.384027777777778in"
height="0.5576388888888889in"}

> Repeat for all columns to get (K^2^C) x N matrix
>
> (N receptive field locations)

![](media/image201.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image202.jpeg){width="9.274305555555555in"
> height="4.1618055555555555in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image203.jpeg){width="5.208880139982502e-3in"
height="0.4013888888888889in"}

> Elements appearing in multiple
>
> receptive fields are duplicated; this
>
> uses a lot of memory

![](media/image204.jpeg){width="4.384027777777778in"
height="0.5576388888888889in"}

> Repeat for all columns to get (K^2^C) x N matrix
>
> (N receptive field locations)

![](media/image205.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image206.jpeg){width="9.274305555555555in"
> height="4.7375in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image207.jpeg){width="5.208880139982502e-3in"
height="0.4013888888888889in"}

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
<td></td>
<td></td>
<td></td>
<td></td>
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
<td>Reshape each filter to K<sup>2</sup>C row,</td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><blockquote>
<p>(K<sup>2</sup>C) x N matrix</p>
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
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>making D x (K<sup>2</sup>C) matrix</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image208.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image209.jpeg){width="9.321527777777778in"
> height="4.7375in"}
>
> Feature map: H x W x C Conv weights: D filters, each K x K x C

![](media/image210.jpeg){width="5.208880139982502e-3in"
height="0.4013888888888889in"}

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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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
<p>Matrix multiply</p>
</blockquote></td>
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
<td>D x (K<sup>2</sup>C) matrix</td>
<td></td>
<td></td>
<td></td>
<td>D x N result;</td>
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
<td><blockquote>
<p>(K<sup>2</sup>C) x N matrix</p>
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
<td>reshape to output tensor</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
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

![](media/image211.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 - 17 Feb 2016

> ![](media/image213.jpeg){width="9.747916666666667in"
> height="4.985416666666667in"}
>
> **CONV forward in Caffe library**
>
> im2col
>
> matrix multiply: call to cuBLAS
>
> ![](media/image214.jpeg){width="5.153472222222222in"
> height="0.65625in"} bias offset

![](media/image216.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 73 17 Feb 2016

> ![](media/image217.jpeg){width="8.7125in"
> height="4.904861111111111in"}
>
> **fast\_layers.py from HW**
>
> im2col
>
> matrix multiply:
>
> call np.dot
>
> (which calls BLAS)

![](media/image218.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 74 17 Feb 2016

> ![](media/image219.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image220.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Convolution Theorem:** The convolution of f and g is equal to the
> elementwise product of their Fourier Transforms:
>
> Using the **Fast Fourier Transform**, we can compute the Discrete
> Fourier transform of an N-dimensional vector in O (N log N) time (also
> extends to 2D images)

![](media/image221.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 75 17 Feb 2016

> ![](media/image222.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image223.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

1.  Compute FFT of weights: F(W)

2.  Compute FFT of image: F(X)

3.  Compute elementwise product: F(W) ○ F(X)

4.  Compute inverse FFT: Y = F^-1^(F(W) ○ F(X))

![](media/image224.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 76 17 Feb 2016

> ![](media/image225.jpeg){width="9.630555555555556in"
> height="4.514583333333333in"}
>
> FFT convolutions get a big speedup for larger filters Not much speedup
> for 3x3 filters =(
>
> Vasilache et al, Fast Convolutional Nets With fbfft: A GPU Performance
> Evaluation

![](media/image226.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 77 17 Feb 2016

> ![](media/image227.jpeg){width="9.554166666666667in"
> height="4.7972222222222225in"}
>
> **Naive matrix multiplication**: Computing product of two N x N
> matrices takes O(N^3^) operations
>
> **Strassen's Algorithm**: Use clever arithmetic to reduce complexity
> to O(N^log2(7)^) \~ O(N^2.81^)
>
> From Wikipedia

![](media/image228.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 78 17 Feb 2016

> ![](media/image229.jpeg){width="9.932638888888889in" height="4.775in"}
>
> Similar cleverness can be applied to convolutions
>
> Lavin and Gray (2015) work out special cases for 3x3 convolutions:
>
> Lavin and Gray, "Fast Algorithms for Convolutional Neural Networks",
> 2015

![](media/image230.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 79 17 Feb 2016

> ![](media/image231.jpeg){width="9.5in" height="0.9375in"}

![](media/image232.jpeg){width="8.99236111111111in"
height="3.214583333333333in"}

> Huge speedups on VGG for small batches:

![](media/image233.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 80 17 Feb 2016

> ![](media/image234.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image235.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   im2col: Easy to implement, but big memory overhead

-   FFT: Big speedups for small kernels

-   "Fast Algorithms" seem promising, not widely used yet

![](media/image236.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 81 17 Feb 2016

![](media/image237.jpeg){width="5.66875in"
height="0.7791666666666667in"}

> Implementation Details

![](media/image238.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 82 17 Feb 2016

![](media/image239.jpeg){width="9.646527777777777in"
height="5.514583333333333in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 11 83       | > 17 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image240.jpeg){width="9.46875in"
> height="4.872916666666667in"}

![](media/image241.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 84 17 Feb 2016

> ![](media/image242.jpeg){width="9.46875in"
> height="4.872916666666667in"}
>
> "central processing unit"

![](media/image243.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 85 17 Feb 2016

> ![](media/image244.jpeg){width="9.46875in"
> height="4.872916666666667in"}
>
> "graphics processing unit"

![](media/image245.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 86 17 Feb 2016

> ![](media/image246.jpeg){width="9.46875in"
> height="4.872916666666667in"}
>
> "graphics processing unit"

![](media/image247.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 87 17 Feb 2016

![](media/image250.jpeg){width="9.426388888888889in"
height="3.053472222222222in"}

VS

![](media/image251.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 88 17 Feb 2016

![](media/image252.jpeg){width="9.565277777777778in"
height="3.109027777777778in"}

> VS

![](media/image253.jpeg){width="5.228472222222222in"
height="1.2638888888888888in"}

> NVIDIA is much more
>
> common for deep learning

![](media/image254.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 89 17 Feb 2016

> ![](media/image255.jpeg){width="9.504166666666666in"
> height="4.565277777777778in"}
>
> Jen-Hsun Huang
>
> (Stanford EE Masters 1992)
>
> **GTC 2015:**
>
> Introduced new Titan X GPU by bragging about AlexNet benchmarks

![](media/image256.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 90 17 Feb 2016

> ![](media/image257.jpeg){width="8.991666666666667in"
> height="4.552777777777778in"}
>
> Few, fast cores (1 - 16)
>
> Good at sequential processing
>
> **GPU**
>
> Many, slower cores (thousands)
>
> Originally for graphics
>
> Good at parallel computation

![](media/image258.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 91 17 Feb 2016

> ![](media/image259.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image260.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   CUDA (NVIDIA only)

    -   Write C code that runs directly on the GPU

    -   Higher-level APIs: cuBLAS, cuFFT, cuDNN, etc

-   OpenCL

    -   Similar to CUDA, but runs on anything

    -   Usually slower :(

-   Udacity: Intro to Parallel Programming
    > [[https://www.udacity.]{.underline}](https://www.udacity.com/course/cs344)
    > [[com/course/cs344]{.underline}](https://www.udacity.com/course/cs344)

    -   For deep learning just use existing libraries

![](media/image261.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 92 17 Feb 2016

> ![](media/image262.jpeg){width="3.7583333333333333in"
> height="1.0347222222222223in"}
>
> at matrix multiplication:

![](media/image263.jpeg){width="8.327083333333333in"
height="2.8340277777777776in"}

> ![](media/image264.jpeg){width="0.6208333333333333in"
> height="0.22847222222222222in"} **GPU**: NVIDA Tesla K40

![](media/image265.jpeg){width="0.6041666666666666in"
height="5.208880139982502e-3in"}

> with cuBLAS

![](media/image266.jpeg){width="3.001388888888889in"
height="1.0930555555555554in"}

> **CPU**: Intel E5-2697 v2
>
> 12 core @ 2.7 Ghz

![](media/image267.jpeg){width="0.6041666666666666in"
height="5.208880139982502e-3in"}

> with MKL

![](media/image268.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 93 17 Feb 2016

> ![](media/image269.jpeg){width="9.092361111111112in"
> height="0.5777777777777777in"}

![](media/image270.jpeg){width="9.255555555555556in" height="2.55625in"}

> All comparisons are against a 12-core Intel E5-2679v2 CPU @ 2.4GHz
> running Caffe with Intel MKL 11.1.3.

![](media/image272.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 94 17 Feb 2016

> ![](media/image273.jpeg){width="9.377083333333333in"
> height="4.972916666666666in"}
>
> **VGG: \~**2-3 weeks training with 4 GPUs
>
> **ResNet 101:** 2-3 weeks with 4 GPUs
>
> NVIDIA Titan Blacks
>
> \~\$1K each
>
> ResNet reimplemented in Torch:
> [[http://torch.ch/blog/2016/02/04/resnets.html]{.underline}](http://torch.ch/blog/2016/02/04/resnets.html)

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 95 17 Feb 2016

> ![](media/image275.jpeg){width="9.027777777777779in"
> height="4.139583333333333in"}

![](media/image276.jpeg){width="7.3180555555555555in"
height="0.4583333333333333in"}

Alex Krizhevsky, "One weird trick for parallelizing convolutional neural
networks"

![](media/image277.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 96 17 Feb 2016

> ![](media/image278.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image279.jpeg){width="3.495138888888889in" height="2.8375in"}

> **Data parallelism**

![](media/image280.jpeg){width="5.822222222222222in"
height="0.4583333333333333in"}

*\[Large Scale Distributed Deep Networks, Jeff Dean et al., 2013\]*

![](media/image281.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 97 17 Feb 2016

> ![](media/image282.jpeg){width="9.027777777777779in"
> height="4.1715277777777775in"}

+----------------------+-------------------------+--+
| **Data parallelism** | > **Model parallelism** |  |
+----------------------+-------------------------+--+
|                      |                         |  |
+----------------------+-------------------------+--+

![](media/image283.jpeg){width="5.822222222222222in"
height="0.4583333333333333in"}

*\[Large Scale Distributed Deep Networks, Jeff Dean et al., 2013\]*

![](media/image284.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 98 17 Feb 2016

> ![](media/image285.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image286.jpeg){width="9.638194444444444in"
height="3.0069444444444446in"}

> *Abadi et al, "TensorFlow: Large-Scale Machine Learning on
> Heterogeneous Distributed Systems"*

![](media/image287.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 11 99 17 Feb 2016

![](media/image288.jpeg){width="4.508333333333334in"
height="0.5395833333333333in"}

> Bottlenecks
>
> to be aware of

![](media/image289.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 0               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image291.jpeg){width="9.122916666666667in"
height="4.395833333333333in"}

> **GPU - CPU communication is a bottleneck.** =\>
>
> **CPU** data prefetch+augment thread running
>
> while
>
> **GPU** performs forward/backward pass

![](media/image292.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 1               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image293.jpeg){width="9.438888888888888in"
height="4.985416666666667in"}

Moving parts lol

> **CPU - disk bottleneck**
>
> Hard disk is slow to read from
>
> =\> Pre-processed images
>
> stored contiguously in files, read as raw byte stream from SSD disk

![](media/image294.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 2               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image295.jpeg){width="9.122916666666667in"
height="4.395833333333333in"}

> **GPU memory bottleneck**
>
> Titan X: 12 GB \<- currently the max
>
> GTX 980 Ti: 6 GB
>
> e.g.
>
> AlexNet: \~3GB needed with batch size 256

![](media/image296.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 3               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image297.jpeg){width="6.51875in"
height="1.2652777777777777in"}

Floating Point Precision

![](media/image298.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 4               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image299.jpeg){width="9.027777777777779in"
height="4.635416666666667in"}

> Floating point precision

-   64 bit "double" precision is default in a lot of programming

-   32 bit "single" precision is typically used for CNNs for performance

![](media/image300.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 5               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image301.jpeg){width="9.447916666666666in"
height="4.635416666666667in"}

> Floating point precision

-   64 bit "double" precision is default in a lot of programming

-   32 bit "single" precision is typically used for CNNs for performance

    -   Including cs231n homework!

![](media/image302.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 6               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image303.jpeg){width="9.370833333333334in"
height="4.761111111111111in"}

> Floating point precision
>
> **Prediction**: 16 bit "half" precision will be the new standard

-   Already supported in cuDNN

-   Nervana fp16 kernels are the fastest right now

-   Hardware support in next-gen NVIDIA cards (Pascal)

-   Not yet supported in torch =(

![](media/image304.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

Benchmarks on Titan X, from
[[https://github.]{.underline}](https://github.com/soumith/convnet-benchmarks)

[[com/soumith/convnet-benchmarks]{.underline}](https://github.com/soumith/convnet-benchmarks)

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 7               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image305.jpeg){width="9.450694444444444in" height="4.8125in"}

> Floating point precision
>
> How low can we go?
>
> Gupta et al, 2015:
>
> Train with **16-bit fixed point** with stochastic rounding
>
> CNNs on MNIST

Gupta et al, "Deep Learning with Limited Numerical Precision", ICML 2015

![](media/image306.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 10              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 8               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image307.jpeg){width="9.285416666666666in"
height="4.635416666666667in"}

> Floating point precision
>
> How low can we go?
>
> Courbariaux et al, 2015:
>
> Train with **10-bit activations**, **12-bit parameter updates**

+-------------+-------------+-------------+-------------+-------------+
|             | Courbariaux |             |             |             |
|             | et al,      |             |             |             |
|             | "Training   |             |             |             |
|             | Deep Neural |             |             |             |
|             | Networks    |             |             |             |
|             | with Low    |             |             |             |
|             | Precision   |             |             |             |
|             | Multiplicat |             |             |             |
|             | ions",      |             |             |             |
|             | ICLR 2015   |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > Fei-Fei   | > Lecture   | 10          | > 17 Feb    |             |
| > Li &      | > 11        |             | > 2016      |             |
| > Andrej    |             |             |             |             |
| > Karpathy  |             |             |             |             |
| > & Justin  |             |             |             |             |
| > Johnson   |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             | 9           |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image308.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image309.jpeg){width="9.752083333333333in"
height="4.779166666666667in"}

> Floating point precision
>
> How low can we go?
>
> Courbariaux and Bengio, February 9 2016:

-   Train with **1-bit activations and weights**!

-   All activations and weights are +1 or -1

-   Fast multiplication with bitwise XNOR

-   (Gradients use higher precision)

> Courbariaux et al, "BinaryNet: Training Deep Neural Networks with
> Weights and Activations Constrained to +1 or -1", arXiv 2016

![](media/image310.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 11              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 0               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image311.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> Implementation details: Recap

![](media/image312.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   GPUs much faster than CPUs

-   Distributed training is sometimes used

    -   Not needed for small problems

-   Be aware of bottlenecks: CPU / GPU, CPU / disk

-   Low precison makes things faster and still works

    -   32 bit is standard now, 16 bit soon

    -   In the future: binary nets?

![](media/image313.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 11              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 1               |                 |
+-----------------+-----------------+-----------------+-----------------+

![](media/image314.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> Recap

![](media/image315.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Data augmentation: artificially expand your data

-   Transfer learning: CNNs without huge data

-   All about convolutions

-   Implementation details

![](media/image316.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------+-----------------+-----------------+-----------------+
| > Fei-Fei Li &  | > Lecture 11    | 11              | > 17 Feb 2016   |
| > Andrej        |                 |                 |                 |
| > Karpathy &    |                 |                 |                 |
| > Justin        |                 |                 |                 |
| > Johnson       |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | 2               |                 |
+-----------------+-----------------+-----------------+-----------------+
