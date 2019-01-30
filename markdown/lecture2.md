![](media/image1.jpeg){width="9.73125in" height="1.9243055555555555in"}

Lecture 2:

Image Classification pipeline

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 1 6 Jan 2016

> ![](media/image3.jpeg){width="8.472222222222221in"
> height="4.243055555555555in"}
>
> First assignment will come out tonight (or tomorrow at worst)
>
> It is due **January 20** (i.e. in two weeks). Handed in through
> CourseWork It includes:

-   Write/train/evaluate a kNN classifier

-   Write/train/evaluate a Linear Classifier (SVM and Softmax)

-   Write/train/evaluate a 2-layer Neural Network (backpropagation!)

-   Requires writing numpy/Python code

> **Warning**: don't work on assignments from last year!
>
> Compute: Can use your own laptops, or Terminal.com

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 2 6 Jan 2016

> ![](media/image5.jpeg){width="7.840972222222222in"
> height="0.5284722222222222in"}

![](media/image6.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 3 6 Jan 2016

![](media/image9.jpeg){width="9.602777777777778in"
height="5.5680555555555555in"}

+-------------------------------------------------+---------------+--------------+
| > Fei-Fei Li & Andrej Karpathy & Justin Johnson | > Lecture 2 4 | > 6 Jan 2016 |
+-------------------------------------------------+---------------+--------------+
|                                                 |               |              |
+-------------------------------------------------+---------------+--------------+

![](media/image10.jpeg){width="9.602777777777778in"
height="5.555555555555555in"}

+-------------------------------------------------+---------------+--------------+
| > Fei-Fei Li & Andrej Karpathy & Justin Johnson | > Lecture 2 5 | > 6 Jan 2016 |
+-------------------------------------------------+---------------+--------------+
|                                                 |               |              |
+-------------------------------------------------+---------------+--------------+

> ![](media/image11.jpeg){width="9.210416666666667in"
> height="4.7625in"}: a core task in Computer Vision
>
> (assume given set of discrete labels)
>
> {dog, cat, truck, plane, \...}
>
> cat

![](media/image12.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 6 6 Jan 2016

> ![](media/image14.jpeg){width="9.849305555555556in"
> height="4.211111111111111in"}
>
> *semantic gap*
>
> Images are represented as 3D arrays of numbers, with integers between
> \[0, 255\].
>
> E.g.
>
> 300 x 100 x 3
>
> (3 for 3 color channels RGB)

![](media/image15.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 7 6 Jan 2016

> ![](media/image16.jpeg){width="7.2965277777777775in"
> height="0.8958333333333334in"}

![](media/image17.jpeg){width="10.0in" height="4.577083333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 8 6 Jan 2016

> ![](media/image18.jpeg){width="7.458333333333333in"
> height="4.725694444444445in"}

![](media/image19.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 9 6 Jan 2016

> ![](media/image20.jpeg){width="7.2965277777777775in"
> height="0.8958333333333334in"}

![](media/image21.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 10 6 Jan 2016

> ![](media/image23.jpeg){width="9.366666666666667in"
> height="4.7034722222222225in"}

![](media/image24.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 11 6 Jan 2016

> ![](media/image25.jpeg){width="7.388888888888889in"
> height="4.576388888888889in"}

![](media/image26.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 12 6 Jan 2016

> ![](media/image27.jpeg){width="7.534027777777778in"
> height="4.907638888888889in"}

![](media/image28.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 13 6 Jan 2016

> ![](media/image29.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image30.jpeg){width="5.506944444444445in"
height="0.8715277777777778in"}

> Unlike e.g. sorting a list of numbers,
>
> **no obvious way** to hard-code the algorithm for recognizing a cat,
> or other classes.

![](media/image32.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 14 6 Jan 2016

> ![](media/image33.jpeg){width="5.860416666666667in"
> height="0.5881944444444445in"}

![](media/image34.jpeg){width="2.032638888888889in"
height="0.3194444444444444in"}

> ???

![](media/image35.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 15 6 Jan 2016

> **Data-driven approach:**

![](media/image37.jpeg){width="9.5625in" height="0.9375in"}

1.  Collect a dataset of images and labels

2.  Use Machine Learning to train an image classifier

3.  Evaluate the classifier on a withheld set of test images

![](media/image38.jpeg){width="4.6875in" height="0.3680555555555556in"}

> **Example training set**

![](media/image39.jpeg){width="10.0in" height="3.127083333333333in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 16 6 Jan 2016

> ![](media/image40.jpeg){width="9.88125in"
> height="0.9513888888888888in"}**Nearest Neighbor Classifier**

![](media/image41.jpeg){width="4.269444444444445in"
height="0.5770833333333333in"}

> Remember all training images and their labels

![](media/image42.jpeg){width="9.29375in" height="1.9152777777777779in"}

> Predict the label of the most similar training image

![](media/image43.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 17 6 Jan 2016

> ![](media/image44.jpeg){width="9.354861111111111in"
> height="0.7701388888888889in"}**CIFAR-10**

10. labels

> **50,000** training images, each image is tiny: 32x32
>
> **10,000** test images.

![](media/image45.jpeg){width="10.0in" height="4.5777777777777775in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 18 6 Jan 2016

> ![](media/image46.jpeg){width="9.646527777777777in"
> height="1.2819444444444446in"}**CIFAR-10**

10. labels

> **50,000** training images

examples of nearest neighbors in rows

> **10,000** test images.

![](media/image47.jpeg){width="10.0in" height="4.334027777777778in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 19 6 Jan 2016

> ![](media/image48.jpeg){width="9.5in"
> height="0.7638888888888888in"}**distance metric**?

![](media/image49.jpeg){width="5.331944444444445in"
height="0.7638888888888888in"}

**L1 distance:**

![](media/image50.jpeg){width="9.674305555555556in"
height="2.777083333333333in"}

add

![](media/image51.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 20 6 Jan 2016

> ![](media/image52.jpeg){width="9.879861111111111in"
> height="4.895833333333333in"}

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 21 6 Jan 2016

> ![](media/image54.jpeg){width="9.886805555555556in"
> height="4.895833333333333in"}
>
> remember the training data

![](media/image55.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 22 6 Jan 2016

![](media/image56.jpeg){width="9.886805555555556in"
height="4.895833333333333in"}

> Nearest Neighbor classifier
>
> for every test image:
>
> \- find nearest train image with L1 distance
>
> \- predict the label of nearest training image

![](media/image57.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 2 23        | > 6 Jan 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image58.jpeg){width="9.886805555555556in"
> height="4.895833333333333in"}

![](media/image59.jpeg){width="2.9618055555555554in"
height="3.423611111111111in"}

Q.  **how does the classification speed depend on the size of the
    > training data?**

![](media/image60.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 24 6 Jan 2016

![](media/image61.jpeg){width="9.886805555555556in"
height="4.895833333333333in"}

> Nearest Neighbor classifier

![](media/image62.jpeg){width="2.9618055555555554in"
height="3.423611111111111in"}

> Q: how does the classification speed depend on the size of the
> training data? **linearly :(**
>
> This is **backwards**:
>
> \- test time performance is usually much more important in practice.
>
> \- CNNs flip this: expensive training, cheap test evaluation

![](media/image63.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 2 25        | > 6 Jan 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image64.jpeg){width="9.346527777777778in" height="0.9in"}

find approximate nearest neighbors quickly

![](media/image65.jpeg){width="10.0in" height="4.529166666666667in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 26 6 Jan 2016

> ![](media/image66.jpeg){width="9.522222222222222in"
> height="0.6541666666666667in"}**hyperparameter** common choices:

![](media/image67.jpeg){width="9.034722222222221in"
height="0.5993055555555555in"}

> L1 (Manhattan) distance L2 (Euclidean) distance

![](media/image68.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 27 6 Jan 2016

> ![](media/image71.jpeg){width="8.995138888888889in"
> height="0.9729166666666667in"}
>
> find the k nearest images, have them vote on the label

![](media/image72.jpeg){width="9.609027777777778in"
height="2.5194444444444444in"}

> the data NN classifier 5-NN classifier

![](media/image73.jpeg){width="6.5881944444444445in"
height="0.3902777777777778in"}

http://en.wikipedia.org/wiki/K-nearest\_neighbors\_algorithm

![](media/image74.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 28 6 Jan 2016

> ![](media/image75.jpeg){width="9.646527777777777in"
> height="1.2819444444444446in"}**CIFAR-10**

10. labels

> **50,000** training images

examples of nearest neighbors in rows

> **10,000** test images.

![](media/image76.jpeg){width="10.0in" height="4.334027777777778in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 29 6 Jan 2016

> ![](media/image77.jpeg){width="9.609027777777778in"
> height="2.5194444444444444in"} NN classifier 5-NN classifier

![](media/image78.jpeg){width="8.134027777777778in"
height="1.4013888888888888in"}

Q.  what is the accuracy of the nearest neighbor classifier on the
    > training data, when using the Euclidean distance?

![](media/image79.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 30 6 Jan 2016

> ![](media/image80.jpeg){width="9.609027777777778in"
> height="2.5194444444444444in"} NN classifier 5-NN classifier

![](media/image81.jpeg){width="8.134027777777778in"
height="1.4013888888888888in"}

> Q2: what is the accuracy of the **k-**nearest neighbor classifier on
> the training data?

![](media/image82.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 31 6 Jan 2016

> ![](media/image83.jpeg){width="8.5875in"
> height="3.5993055555555555in"}**distance** to use?
>
> What is the best value of **k** to use?
>
> i.e. how do we set the **hyperparameters**?

![](media/image84.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 32 6 Jan 2016

> ![](media/image85.jpeg){width="8.5875in"
> height="3.5993055555555555in"}**distance** to use?
>
> What is the best value of **k** to use?
>
> i.e. how do we set the **hyperparameters**?
>
> Very problem-dependent.
>
> Must try them all out and see what works best.

![](media/image86.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 33 6 Jan 2016

> ![](media/image87.jpeg){width="8.67013888888889in"
> height="0.38472222222222224in"}

![](media/image88.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 34 6 Jan 2016

> ![](media/image90.jpeg){width="8.67013888888889in"
> height="0.38472222222222224in"}
>
> Very bad idea. The test set is a proxy for the generalization
> performance! Use only **VERY SPARINGLY,** at the end.

![](media/image91.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 35 6 Jan 2016

![](media/image93.jpeg){width="8.98263888888889in"
height="2.7840277777777778in"}

> Validation data
>
> use to tune hyperparameters

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 36 6 Jan 2016

![](media/image95.jpeg){width="8.98263888888889in"
height="2.7840277777777778in"}

> **Cross-validation**
>
> cycle through the choice of which fold
>
> is the validation fold, average results.

![](media/image96.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 2 37        | > 6 Jan 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> ![](media/image97.jpeg){width="9.511111111111111in"
> height="4.711805555555555in"}**k.**
>
> Each point: single outcome.
>
> The line goes
>
> through the mean, bars indicated standard deviation
>
> (Seems that k \~= 7 works best for this data)

![](media/image98.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 38 6 Jan 2016

![](media/image99.jpeg){width="8.899305555555555in"
height="4.183333333333334in"}

> k-Nearest Neighbor on images **never used.**

-   terrible performance at test time

-   distance metrics on level of whole images can be very unintuitive

![](media/image100.jpeg){width="6.856944444444444in"
height="0.33541666666666664in"}

(all 3 images have same L2 distance to the one on the left)

![](media/image101.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 2 39        | > 6 Jan 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image102.jpeg){width="9.797222222222222in"
height="0.8076388888888889in"}

![](media/image103.jpeg){width="9.42361111111111in"
height="3.786111111111111in"}

-   **Image Classification:** We are given a **Training Set** of labeled
    > images, asked to predict labels on **Test Set**. Common to report
    > the **Accuracy** of predictions (fraction of correctly predicted
    > images)

-   We introduced the **k-Nearest Neighbor Classifier**, which predicts
    > the labels based on nearest images in the training set

-   We saw that the choice of distance and the value of k are
    > **hyperparameters** that are tuned using a **validation set**, or
    > through **cross-validation** if the size of the data is small.

-   Once the best set of hyperparameters is chosen, the classifier is
    > evaluated once on the test set, and reported as the performance of
    > kNN on that data.

![](media/image104.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 40 6 Jan 2016

![](media/image105.jpeg){width="7.557638888888889in"
height="3.308333333333333in"}

Linear Classification

![](media/image106.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 41 6 Jan 2016

![](media/image107.jpeg){width="5.208880139982502e-3in"
height="0.7138888888888889in"}

> language control

![](media/image109.jpeg){width="0.7138888888888889in"
height="5.208880139982502e-3in"}

> see

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 42 6 Jan 2016

> ![](media/image110.jpeg){width="5.002083333333333in"
> height="0.5444444444444444in"}

![](media/image111.jpeg){width="10.0in" height="4.813888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 43 6 Jan 2016

![](media/image112.jpeg){width="9.602777777777778in"
height="5.523611111111111in"}

+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 2 44        | > 6 Jan 2016          |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image113.jpeg){width="8.988194444444444in"
height="4.626388888888889in"}

> **CNN**

![](media/image114.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 45 6 Jan 2016

> ![](media/image115.jpeg){width="10.0in"
> height="5.530555555555556in"}**CIFAR-10**

10. labels

> **50,000** training images each image is **32x32x3**
>
> **10,000** test images.

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 46 6 Jan 2016

> ![](media/image116.jpeg){width="4.358333333333333in"
> height="0.8152777777777778in"}

![](media/image117.jpeg){width="3.3979166666666667in"
height="0.36736111111111114in"}

+--------------------+--------------------+
| > image parameters |                    |
+--------------------+--------------------+
| > f(**x**,**W**)   | > **10** numbers,  |
+--------------------+--------------------+
|                    | > indicating class |
+--------------------+--------------------+
|                    | > scores           |
+--------------------+--------------------+

![](media/image118.jpeg){width="9.239583333333334in"
height="1.7465277777777777in"}

> **\[32x32x3\]**
>
> array of numbers 0\...1
>
> (3072 numbers total)

![](media/image119.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 47 6 Jan 2016

> ![](media/image120.jpeg){width="8.94513888888889in"
> height="0.8152777777777778in"}**Linear classifier**

![](media/image121.jpeg){width="8.963888888888889in"
height="1.9708333333333334in"}

> **10** numbers,

![](media/image122.jpeg){width="3.7493055555555554in"
height="5.208880139982502e-3in"}

> indicating class
>
> scores

![](media/image124.jpeg){width="3.6680555555555556in"
height="0.36736111111111114in"}

> **\[32x32x3\]**
>
> array of numbers 0\...1

![](media/image125.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 48 6 Jan 2016

> ![](media/image126.jpeg){width="8.94513888888889in"
> height="0.8152777777777778in"}**Linear classifier**

![](media/image127.jpeg){width="9.239583333333334in"
height="3.6777777777777776in"}

> **3072x1**
>
> **10x1** **10x3072**
>
> **10** numbers,

![](media/image128.jpeg){width="3.7493055555555554in"
height="5.208880139982502e-3in"}

> indicating class
>
> scores
>
> **\[32x32x3\]**
>
> array of numbers 0\...1
>
> parameters, or "weights"

![](media/image129.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 49 6 Jan 2016

> ![](media/image130.jpeg){width="8.94513888888889in"
> height="0.8152777777777778in"}**Linear classifier**

![](media/image131.jpeg){width="9.39236111111111in"
height="3.6777777777777776in"}

> **3072x1**

**10x1**

> **10x1** **10x3072**
>
> **10** numbers,

![](media/image132.jpeg){width="3.7493055555555554in"
height="5.208880139982502e-3in"}

> indicating class
>
> scores
>
> **\[32x32x3\]**
>
> array of numbers 0\...1
>
> parameters, or "weights"

![](media/image133.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 50 6 Jan 2016

![](media/image134.jpeg){width="9.96875in"
height="0.5444444444444444in"}cat/dog/ship)

![](media/image135.jpeg){width="10.0in" height="4.529861111111111in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 51 6 Jan 2016
>
> ![](media/image136.jpeg){width="9.027777777777779in" height="0.875in"}

![](media/image137.jpeg){width="9.404166666666667in"
height="3.8152777777777778in"}

> Q: what does the linear classifier do, in English?

![](media/image138.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 52 6 Jan 2016

> ![](media/image139.jpeg){width="9.027777777777779in" height="0.875in"}

![](media/image140.jpeg){width="9.57986111111111in"
height="3.9694444444444446in"}

> Example trained weights of a linear classifier trained on CIFAR-10:

![](media/image141.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 53 6 Jan 2016

> ![](media/image142.jpeg){width="9.720138888888888in"
> height="4.878472222222222in"}
>
> **\[32x32x3\]**
>
> array of numbers 0\...1 (3072 numbers total)

![](media/image143.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 54 6 Jan 2016

> ![](media/image144.jpeg){width="9.027777777777779in" height="0.875in"}

![](media/image145.jpeg){width="9.720138888888888in"
height="3.8152777777777778in"}

> Q2: what would be a very hard set of classes for a linear classifier
> to distinguish?

![](media/image146.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 55 6 Jan 2016

![](media/image147.jpeg){width="9.027777777777779in"
height="2.1326388888888888in"}We defined a (linear) **[score
function]{.underline}:**![](media/image148.jpeg){width="2.4451388888888888in"
height="0.5in"}

![](media/image149.jpeg){width="10.0in" height="3.4868055555555557in"}

> Example class scores for 3 images, with a random W:
>
> -3.45 -0.51 3.42

^-8.87^ **6.04** 4.64

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

^-0.36^ -2.09 -4.79

^-0.72^ -2.93 6.14

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 56 6 Jan 2016

> Coming up:

-   Loss function

-   Optimization

-   ConvNets!

(quantifying what it means to have a "good" W)

![](media/image150.jpeg){width="9.66875in" height="4.729166666666667in"}

(start with random W and find a W that minimizes the loss)

(tweak the functional form of f)

![](media/image151.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 2 57 6 Jan 2016
