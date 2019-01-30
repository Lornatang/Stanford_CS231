![](media/image1.jpeg){width="10.0in" height="5.429166666666666in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 1 29 Feb 2016

> ![](media/image2.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image3.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Everyone should be done with Assignment 3 now

-   Milestone grades will go out soon

![](media/image4.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 2 29 Feb 2016

![](media/image5.jpeg){width="9.918055555555556in" height="2.7125in"}

Spatial Transformer

> Segmentation

![](media/image6.jpeg){width="3.7083333333333335in"
height="0.45694444444444443in"}

> Soft Attention

![](media/image7.jpeg){width="10.0in" height="2.35625in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 3 29 Feb 2016

![](media/image8.jpeg){width="1.9368055555555554in"
height="0.8597222222222223in"}

Videos

![](media/image9.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 4 29 Feb 2016

> ![](media/image10.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image11.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 5 29 Feb 2016

> ![](media/image13.jpeg){width="9.027777777777779in"
> height="2.7104166666666667in"}
>
> **Dense trajectories and motion boundary descriptors for action
> recognition** *Wang et al., 2013*
>
> **Action Recognition with Improved Trajectories**
>
> *Wang and Schmid, 2013*
>
> (code available!)

![](media/image14.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 6 29 Feb 2016

![](media/image16.jpeg){width="9.347222222222221in"
height="3.4868055555555557in"}

> **Dense trajectories and motion boundary descriptors for action
> recognition** *Wang et al., 2013*

![](media/image17.jpeg){width="9.154166666666667in"
height="0.8930555555555556in"}

+-----------+-----------+-----------+-----------+-----------+-----------+
| > detect  | > track   | > extract |           |           |           |
| > feature | > feature | > HOG/HOF |           |           |           |
| > points  | s         | /MBH      |           |           |           |
|           | > with    |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           | > feature |           |           |           |
|           |           | s         |           |           |           |
|           |           | > in the  |           |           |           |
|           |           | > (stabil |           |           |           |
|           |           | ized)     |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | > optical |           |           |           |           |
|           | > flow    |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           | > coordin |           |           |           |
|           |           | ate       |           |           |           |
|           |           | > system  |           |           |           |
|           |           | > of      |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           | > each    |           |           |           |
|           |           | > trackle |           |           |           |
|           |           | t         |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| > Fei-Fei | > Lecture | 7         | > 29 Feb  |           |           |
| > Li &    | > 14      |           | > 2016    |           |           |
| > Andrej  |           |           |           |           |           |
| > Karpath |           |           |           |           |           |
| y         |           |           |           |           |           |
| > &       |           |           |           |           |           |
| > Justin  |           |           |           |           |           |
| > Johnson |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+

![](media/image18.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image19.jpeg){width="9.370138888888889in" height="4.9in"}*Wang
et al., 2013*

> detected feature points
>
> \[J. Shi and C. Tomasi, "Good features to track," CVPR 1994\] \[Ivan
> Laptev 2005\]

![](media/image20.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 8 29 Feb 2016

![](media/image21.jpeg){width="8.74236111111111in"
height="0.8201388888888889in"}*Wang et al., 2013*

![](media/image22.jpeg){width="9.94375in" height="3.170138888888889in"}

> track each keypoint using **optical flow.**

![](media/image23.jpeg){width="9.624305555555555in"
height="0.4583333333333333in"}

> \[G. Farnebäck, "Two-frame motion estimation based on polynomial
> expansion," 2003\]
>
> \[T. Brox and J. Malik, "Large displacement optical flow: Descriptor
> matching in variational motion estimation," 2011\]

![](media/image24.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 9 29 Feb 2016

![](media/image25.jpeg){width="8.74236111111111in"
height="0.8201388888888889in"}*Wang et al., 2013*

![](media/image26.jpeg){width="8.796527777777778in"
height="3.2270833333333333in"}

+-----------------------+-----------------------+-----------------------+
| Extract features in   | > Accumulate into     |                       |
| the local coordinate  | > histograms,         |                       |
|                       | > separately          |                       |
+-----------------------+-----------------------+-----------------------+
|                       | > according to        |                       |
|                       | > multiple            |                       |
|                       | > spatio-temporal     |                       |
|                       | > layouts.            |                       |
+-----------------------+-----------------------+-----------------------+
| system of each        |                       |                       |
| tracklet.             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image27.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 10 29 Feb
> 2016
>
> ![](media/image28.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image29.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> **First layer** (CONV1): 96 11x11 filters applied at stride 4 =\>
>
> Output volume **\[55x55x96\]**
>
> Q: What if the input is now a small chunk of video? E.g.
> \[227x227x3x15\] ?

![](media/image30.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 11 29 Feb 2016

> ![](media/image31.jpeg){width="9.765972222222222in"
> height="1.9097222222222223in"}
>
> *\[Krizhevsky et al. 2012\]*

![](media/image32.jpeg){width="9.245138888888889in"
height="1.179861111111111in"}

> Input: 227x227x3 images
>
> **First layer** (CONV1): 96 11x11 filters applied at stride 4 =\>
>
> Output volume **\[55x55x96\]**
>
> Q: What if the input is now a small chunk of video? E.g.
> \[227x227x3x15\] ?

A.  Extend the convolutional filters in time, perform spatio-temporal
    > convolutions! E.g. can have 11x11xT filters, where T = 2..15.

![](media/image33.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 12 29 Feb 2016

> ![](media/image34.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image35.jpeg){width="10.0in" height="4.497222222222222in"}

\[3D Convolutional Neural Networks for Human Action Recognition, Ji et
al., 2010\]

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 13 29 Feb
> 2016
>
> ![](media/image36.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image37.jpeg){width="10.0in" height="4.649305555555555in"}

> Sequential Deep Learning for Human Action Recognition, Baccouche et
> al., 2011

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 14 29 Feb 2016

> ![](media/image38.jpeg){width="9.907638888888888in"
> height="1.0041666666666667in"} spatio-temporal convolutions; worked
> best.

![](media/image39.jpeg){width="9.328472222222222in"
height="3.6743055555555557in"}

> \[Large-scale Video Classification with Convolutional Neural Networks,
> Karpathy et al., 2014\]

![](media/image40.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 15 29 Feb 2016

> ![](media/image41.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image42.jpeg){width="8.238888888888889in"
height="3.3090277777777777in"}

> Learned filters on the first layer

![](media/image43.jpeg){width="8.36736111111111in" height="0.31875in"}

> \[Large-scale Video Classification with Convolutional Neural Networks,
> Karpathy et al., 2014\]

![](media/image44.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 16 29 Feb 2016

> ![](media/image45.jpeg){width="9.59375in"
> height="4.358333333333333in"}
>
> 1 million videos
>
> 487 sports classes

![](media/image46.jpeg){width="8.36736111111111in" height="0.31875in"}

> \[Large-scale Video Classification with Convolutional Neural Networks,
> Karpathy et al., 2014\]

![](media/image47.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 17 29 Feb 2016

> ![](media/image48.jpeg){width="9.027777777777779in"
> height="3.7756944444444445in"}

![](media/image49.jpeg){width="8.477083333333333in"
height="0.4583333333333333in"}

> The motion information didn't add all that much\...

![](media/image50.jpeg){width="8.36736111111111in" height="0.31875in"}

> \[Large-scale Video Classification with Convolutional Neural Networks,
> Karpathy et al., 2014\]

![](media/image51.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 18 29 Feb 2016

> ![](media/image52.jpeg){width="9.178472222222222in"
> height="4.8590277777777775in"}

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 19 29 Feb 2016

> ![](media/image54.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image55.jpeg){width="9.141666666666667in"
height="1.5361111111111112in"}

> 3D VGGNet, basically.

![](media/image57.jpeg){width="8.261111111111111in"
height="0.6840277777777778in"}

> \[Learning Spatiotemporal Features with 3D Convolutional Networks,
> Tran et al. 2015\]

![](media/image58.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 20 29 Feb 2016

> ![](media/image59.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image60.jpeg){width="10.0in" height="4.407638888888889in"}

> (of VGGNet fame)
>
> \[Two-Stream Convolutional Networks for Action Recognition in Videos,
> **Simonyan** and Zisserman 2014\]

\[T. Brox and J. Malik, "Large displacement optical flow: Descriptor
matching in variational motion estimation," 2011\]

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 21 29 Feb
> 2016
>
> ![](media/image61.jpeg){width="9.790277777777778in" height="1.4625in"}

![](media/image62.jpeg){width="7.819444444444445in"
height="0.9652777777777778in"}

> Two-stream version works much better than either alone.

![](media/image64.jpeg){width="10.0in" height="1.4652777777777777in"}

> \[Two-Stream Convolutional Networks for Action Recognition in Videos,
> **Simonyan** and Zisserman 2014\]

\[T. Brox and J. Malik, "Large displacement optical flow: Descriptor
matching in variational motion estimation," 2011\]

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 22 29 Feb
> 2016
>
> ![](media/image65.jpeg){width="9.027777777777779in"
> height="2.1145833333333335in"}
>
> All 3D ConvNets so far used local motion cues to get extra accuracy
> (e.g. half a second or so)

Q.  what if the temporal dependencies of interest are much much longer?
    > E.g. several seconds?

![](media/image66.jpeg){width="8.301388888888889in"
height="2.0597222222222222in"}

+--+--+--+-----------+--+-----------+--+--+
|  |  |  | > event 1 |  | > event 2 |  |  |
+--+--+--+-----------+--+-----------+--+--+
|  |  |  |           |  |           |  |  |
+--+--+--+-----------+--+-----------+--+--+
|  |  |  |           |  |           |  |  |
+--+--+--+-----------+--+-----------+--+--+
|  |  |  |           |  |           |  |  |
+--+--+--+-----------+--+-----------+--+--+
|  |  |  |           |  |           |  |  |
+--+--+--+-----------+--+-----------+--+--+

![](media/image67.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 23 29 Feb 2016

> ![](media/image72.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image73.jpeg){width="8.545833333333333in"
height="3.3618055555555557in"}

> (This paper was way ahead of its time. Cited 65 times.)

![](media/image74.jpeg){width="10.0in" height="1.145138888888889in"}

> Sequential Deep Learning for Human Action Recognition, Baccouche et
> al., **2011**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 24 29 Feb 2016

> ![](media/image75.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image76.jpeg){width="4.865277777777778in"
height="0.4583333333333333in"}

LSTM way before it was cool

![](media/image77.jpeg){width="7.350694444444445in"
height="2.071527777777778in"}

> (This paper was way ahead of its time. Cited 65 times.)

![](media/image79.jpeg){width="10.0in" height="1.145138888888889in"}

> Sequential Deep Learning for Human Action Recognition, Baccouche et
> al., **2011**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 25 29 Feb 2016

> ![](media/image80.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image81.jpeg){width="4.283333333333333in" height="3.01875in"}

> \[Long-term Recurrent Convolutional Networks for Visual Recognition
> and Description, Donahue et al., 2015\]

![](media/image83.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 26 29 Feb 2016

> ![](media/image84.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image85.jpeg){width="9.718055555555555in"
height="3.923611111111111in"}

> \[Beyond Short Snippets: Deep Networks for Video Classification, Ng et
> al., 2015\]

![](media/image86.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 27 29 Feb 2016

> ![](media/image87.jpeg){width="9.027777777777779in"
> height="4.552083333333333in"}
>
> We looked at two types of architectural patterns:

1.  Model temporal motion locally (3D CONV)

    2.  Model temporal motion globally (LSTM / RNN) + Fusions of both
        > approaches at the same time.

![](media/image88.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 28 29 Feb 2016

> ![](media/image89.jpeg){width="9.51388888888889in"
> height="4.552083333333333in"}
>
> We looked at two types of architectural patterns:

1.  Model temporal motion locally (3D CONV)

    2.  Model temporal motion globally (LSTM / RNN)

> \+ Fusions of both approaches at the same time.

There is another (cleaner) way!

![](media/image90.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 29 29 Feb 2016

![](media/image91.jpeg){width="2.3444444444444446in"
height="0.5909722222222222in"}

> RNN

![](media/image92.jpeg){width="0.9569444444444445in"
height="5.208880139982502e-3in"}

> 3D
>
> CONVNET

![](media/image94.jpeg){width="8.667361111111111in"
height="0.5159722222222223in"}

Infinite (in theory)

![](media/image95.jpeg){width="3.5875in" height="0.31875in"}

temporal extent

(neurons that are function

of all video frames in the past)

![](media/image96.jpeg){width="3.422222222222222in" height="0.31875in"}

> Finite temporal
>
> extent
>
> (neurons that are only
>
> a function of finitely many
>
> video frames in the past)
>
> video

![](media/image97.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 30 29 Feb 2016

> ![](media/image98.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image99.jpeg){width="3.817361111111111in"
height="3.4368055555555554in"}

> Beautiful:

![](media/image100.jpeg){width="5.717361111111111in" height="3.09375in"}

> All neurons in the ConvNet are recurrent.
>
> Only requires (existing) 2D CONV routines. No need for 3D
> spatio-temporal CONV.

![](media/image101.jpeg){width="9.155555555555555in"
height="0.39444444444444443in"}

> \[Delving Deeper into Convolutional Networks for Learning Video
> Representations, Ballas et al., 2016\]

![](media/image102.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 31 29 Feb 2016

> ![](media/image103.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image104.jpeg){width="3.761111111111111in"
height="0.39444444444444443in"}

> Normal ConvNet:

![](media/image105.jpeg){width="4.4222222222222225in"
height="1.7020833333333334in"}

> Convolution Layer

![](media/image106.jpeg){width="9.155555555555555in"
height="0.39444444444444443in"}

> \[Delving Deeper into Convolutional Networks for Learning Video
> Representations, Ballas et al., 2016\]

![](media/image108.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 32 29 Feb 2016

> ![](media/image109.jpeg){width="9.66875in" height="4.5125in"}
>
> layer N
>
> layer N+1 at previous timestep

CONV

![](media/image110.jpeg){width="2.01875in"
height="5.208880139982502e-3in"}

> RNN-like recurrence

![](media/image111.jpeg){width="0.8909722222222223in"
height="5.208880139982502e-3in"}

> (GRU)
>
> CONV

![](media/image112.jpeg){width="1.9701388888888889in"
height="5.208880139982502e-3in"}

layer N+1

![](media/image113.jpeg){width="9.155555555555555in"
height="0.39444444444444443in"}

> \[Delving Deeper into Convolutional Networks for Learning Video
> Representations, Ballas et al., 2016\]

![](media/image114.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 33 29 Feb 2016

> ![](media/image115.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image116.jpeg){width="9.447222222222223in"
height="1.1458333333333333in"}

> Recall: RNNs Vanilla RNN

![](media/image117.jpeg){width="8.88888888888889in"
height="1.7652777777777777in"}

> GRU LSTM

![](media/image118.jpeg){width="9.155555555555555in"
height="1.7631944444444445in"}

> \[Delving Deeper into Convolutional Networks for Learning Video
> Representations, Ballas et al., 2016\]

![](media/image120.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 34 29 Feb 2016

> ![](media/image121.jpeg){width="9.027777777777779in"
> height="0.9513888888888888in"}

![](media/image122.jpeg){width="6.122222222222222in"
height="1.4027777777777777in"}

> Recall: RNNs

![](media/image123.jpeg){width="4.815972222222222in"
height="1.8729166666666666in"}

> GRU

Matrix multiply

![](media/image124.jpeg){width="3.9618055555555554in"
height="1.4715277777777778in"}

=\>

CONV

![](media/image125.jpeg){width="9.155555555555555in"
height="0.39444444444444443in"}

> \[Delving Deeper into Convolutional Networks for Learning Video
> Representations, Ballas et al., 2016\]

![](media/image126.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 35 29 Feb 2016

![](media/image127.jpeg){width="2.3444444444444446in"
height="0.5909722222222222in"}

> RNN

![](media/image128.jpeg){width="0.9569444444444445in"
height="5.208880139982502e-3in"}

> 3D
>
> CONVNET

![](media/image130.jpeg){width="8.667361111111111in"
height="0.5159722222222223in"}

Infinite (in theory)

![](media/image131.jpeg){width="3.5875in" height="0.31875in"}

temporal extent

(neurons that are function

of all video frames in the past)

![](media/image132.jpeg){width="3.422222222222222in" height="0.31875in"}

> Finite temporal
>
> extent
>
> (neurons that are only
>
> a function of finitely many
>
> video frames in the past)
>
> video

![](media/image133.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 36 29 Feb 2016

> ![](media/image134.jpeg){width="6.073611111111111in"
> height="3.7305555555555556in"}
>
> RNN
>
> CONVNET

![](media/image135.jpeg){width="10.0in" height="0.5888888888888889in"}

Infinite (in theory)

![](media/image137.jpeg){width="3.3625in" height="0.31875in"}

temporal extent

(neurons that are function

of all video frames in the past)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 37 29 Feb 2016

> ![](media/image139.jpeg){width="9.027777777777779in"
> height="4.635416666666667in"}

-   You think you need a Spatio-Temporal Fancy Video ConvNet

-   STOP. Do you really?

-   Okay fine: do you want to model:

    -   [local motion?]{.underline} (use 3D CONV), or

    -   [global motion?]{.underline} (use LSTM).

-   Try out using Optical Flow in a second stream (can work better
    > sometimes)

-   Try out GRU-RCN! (imo best model)

![](media/image140.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 38 29 Feb 2016

![](media/image141.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

Unsupervised Learning

![](media/image142.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 39 29 Feb 2016

> ![](media/image143.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image144.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Definitions

-   Autoencoders

    -   Vanilla

    -   Variational

-   Adversarial Networks

![](media/image145.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 40 29 Feb 2016

> ![](media/image146.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Supervised Learning**
>
> **Data**: (x, y)
>
> x is data, y is label
>
> **Goal**: Learn a *function* to
>
> map x -\> y
>
> **Examples**: Classification,
>
> regression, object detection,
>
> semantic segmentation, image
>
> captioning, etc

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 41 29 Feb 2016

> ![](media/image147.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Supervised Learning Data**: (x, y)
>
> x is data, y is label
>
> **Goal**: Learn a *function* to map x -\> y
>
> **Examples**: Classification, regression, object detection, semantic
> segmentation, image captioning, etc

**Unsupervised Learning Data**: x

Just data, no labels!

**Goal**: Learn some *structure* of the data

**Examples**: Clustering, dimensionality reduction, feature learning,
generative models, etc.

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 42 29 Feb 2016

> ![](media/image148.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image149.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Autoencoders

    -   Traditional: feature learning

    -   Variational: generate samples

-   Generative Adversarial Networks: Generate samples

![](media/image150.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 43 29 Feb 2016

> ![](media/image151.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image152.jpeg){width="4.583333333333333in" height="1.7625in"}

Features

> Input data

**z**

![](media/image153.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Encoder

**x**

![](media/image155.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 44 29 Feb 2016

> ![](media/image156.jpeg){width="9.420833333333333in"
> height="1.7930555555555556in"}
>
> **Originally**: Linear + nonlinearity (sigmoid)
>
> **Later**: Deep, fully-connected
>
> **Later**: ReLU CNN

![](media/image157.jpeg){width="4.583333333333333in" height="2.71875in"}

Features

> Input data

**z**

![](media/image158.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Encoder

**x**

![](media/image160.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 45 29 Feb 2016

Autoencoders

> **z** usually smaller than **x** (dimensionality reduction)

**Originally**: Linear + nonlinearity (sigmoid)

![](media/image161.jpeg){width="9.420833333333333in" height="4.73125in"}

**Later**: Deep, fully-connected

**Later**: ReLU CNN

Features

> Input data

**z**

![](media/image162.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Encoder

**x**

![](media/image163.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 46 29 Feb 2016

> ![](media/image164.jpeg){width="9.2875in" height="4.73125in"}

+---------------+----------+--+
| Reconstructed |          |  |
+---------------+----------+--+
|               | > **xx** |  |
+---------------+----------+--+
| input data    |          |  |
+---------------+----------+--+
|               |          |  |
+---------------+----------+--+

![](media/image165.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Decoder

Features

> Input data

**z**

![](media/image166.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Encoder

**x**

![](media/image167.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 47 29 Feb 2016

+--------------+------------------------------------+--+
| Autoencoders | > **Originally**: Linear +         |  |
+--------------+------------------------------------+--+
|              | > nonlinearity (sigmoid)           |  |
+--------------+------------------------------------+--+
|              | > **Later**: Deep, fully-connected |  |
+--------------+------------------------------------+--+
|              | > **Later**: ReLU CNN (upconv)     |  |
+--------------+------------------------------------+--+

![](media/image168.jpeg){width="9.438194444444445in"
height="4.879861111111111in"}

+---------------+----------+--+
| Reconstructed |          |  |
+---------------+----------+--+
|               | > **xx** |  |
+---------------+----------+--+
| input data    |          |  |
+---------------+----------+--+
|               |          |  |
+---------------+----------+--+

![](media/image169.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> Decoder
>
> Features **z**

![](media/image170.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> Encoder

+------------+---------+
| Input data | > **x** |
+------------+---------+

![](media/image171.jpeg){width="10.0in" height="0.5888888888888889in"}

**Encoder**: 4-layer conv

**Decoder**: 4-layer upconv

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 48 29 Feb 2016

<table>
<tbody>
<tr class="odd">
<td></td>
<td></td>
<td><blockquote>
<p>Autoencoders</p>
</blockquote></td>
<td><blockquote>
<p><strong>Originally</strong>: Linear +</p>
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
<td><blockquote>
<p>nonlinearity (sigmoid)</p>
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
<td><blockquote>
<p><strong>Later</strong>: Deep, fully-connected</p>
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
<td><blockquote>
<p><strong>Later</strong>: ReLU CNN (upconv)</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td></td>
<td></td>
<td>Reconstructed</td>
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
<p><strong>xx</strong></p>
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
<td>input data</td>
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
<p>Decoder</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Encoder / decoder</td>
<td></td>
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
<td>sometimes share</td>
<td></td>
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
<td>weights</td>
<td><blockquote>
<p>Features</p>
</blockquote></td>
<td></td>
<td><blockquote>
<p><strong>z</strong></p>
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
</tr>
<tr class="even">
<td><em>Example<strong>:</strong></em></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>Encoder</p>
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
</tr>
<tr class="even">
<td>dim(<strong>x</strong>) = D</td>
<td></td>
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
<td>dim(<strong>z</strong>) = H</td>
<td></td>
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
<td><strong>w<sub>e</sub></strong>: H x D</td>
<td>data</td>
<td></td>
<td></td>
<td><blockquote>
<p><strong>x</strong></p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td><strong>w</strong></td>
<td><strong>d</strong></td>
<td>: D x H = <strong>w</strong> <strong><sup>T</sup></strong></td>
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
<td><blockquote>
<p><strong>e</strong></p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

![](media/image172.jpeg){width="9.71111111111111in"
height="4.9118055555555555in"}

Train for

reconstruction with no labels!

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 49 29 Feb 2016

> ![](media/image176.jpeg){width="9.2875in" height="4.73125in"} **Loss
> function**
>
> **(Often L2)**

+---------------+-----------+--+
| Reconstructed | > **xx**  |  |
+---------------+-----------+--+
| input data    |           |  |
+---------------+-----------+--+
|               |           |  |
+---------------+-----------+--+
|               | > Decoder |  |
+---------------+-----------+--+

![](media/image177.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> Features **z**

![](media/image178.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> Encoder

+------------+---------+
| Input data | > **x** |
+------------+---------+

![](media/image179.jpeg){width="10.0in" height="0.5888888888888889in"}

Train for

reconstruction

with no labels!

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 50 29 Feb 2016

> ![](media/image180.jpeg){width="9.71111111111111in" height="4.7625in"}

+-----------------+------------+--------+-------+-----------+--+--+--+
| Reconstructed   |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            | **xx** |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 | input data |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
| After training, |            |        |       | > Decoder |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
| throw away      |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
| decoder!        | > Features | **z**  |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       | > Encoder |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 |            |        |       |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+
|                 | data       |        | **x** |           |  |  |  |
+-----------------+------------+--------+-------+-----------+--+--+--+

![](media/image181.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 51 29 Feb 2016

+--------------------+---------------------+----------------------+--------------+--+--+--+
| > Autoencoders     | > **Loss function** |                      |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
|                    |                     | > **(Softmax, etc)** |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| > Predicted~Label~ | > **yy**            |                      | > **y**      |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| Use encoder to     |                     |                      |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| initialize a       |                     |                      | > Classifier |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| **supervised**     |                     |                      |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| model              |                     |                      |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
|                    |                     | > **z**              |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+
| > Features         |                     |                      |              |  |  |  |
+--------------------+---------------------+----------------------+--------------+--+--+--+

![](media/image184.jpeg){width="9.820833333333333in"
height="4.581944444444445in"}

> Encoder

+------------+---------+
| Input data | > **x** |
+------------+---------+

![](media/image188.jpeg){width="10.0in" height="0.5888888888888889in"}

> bird plane
>
> dog deer truck

+--------------+------------------------+
| Fine-tune    | > Train for final task |
+--------------+------------------------+
| encoder      | > (sometimes with      |
+--------------+------------------------+
| jointly with | > small data)          |
+--------------+------------------------+
| classifier   |                        |
+--------------+------------------------+

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 52 29 Feb 2016

> ![](media/image189.jpeg){width="9.3375in"
> height="4.518055555555556in"}
>
> In mid 2000s layer-wise pretraining with Restricted Boltzmann Machines
> (RBM) was common
>
> Training deep nets was hard in 2006!

![](media/image190.jpeg){width="10.0in" height="0.8784722222222222in"}

Hinton and Salakhutdinov, "Reducing the Dimensionality of Data with
Neural Networks", Science 2006

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 53 29 Feb
> 2016
>
> ![](media/image191.jpeg){width="9.753472222222221in"
> height="4.518055555555556in"}
>
> In mid 2000s layer-wise pretraining with Restricted Boltzmann Machines
> (RBM) was common
>
> Training deep nets was hard in 2006!

![](media/image192.jpeg){width="10.0in" height="0.8784722222222222in"}

Hinton and Salakhutdinov, "Reducing the Dimensionality of Data with
Neural Networks", Science 2006

Not common anymore

With ReLU, proper initialization, batchnorm, Adam, etc easily train from
scratch

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 54 29 Feb
> 2016
>
> ![](media/image193.jpeg){width="9.235416666666667in"
> height="4.516666666666667in"}

+---------------+----------+--+
| Reconstructed |          |  |
+---------------+----------+--+
|               | > **xx** |  |
+---------------+----------+--+
| input data    |          |  |
+---------------+----------+--+
|               |          |  |
+---------------+----------+--+

![](media/image194.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

Decoder

> Features **z**

![](media/image195.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> Encoder

+------------+---------+
| Input data | > **x** |
+------------+---------+

![](media/image196.jpeg){width="10.0in" height="0.5888888888888889in"}

Autoencoders can reconstruct data, and can learn features to initialize
a supervised model

Can we generate images from an autoencoder?

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 55 29 Feb 2016

> ![](media/image197.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image198.jpeg){width="10.0in" height="4.326388888888889in"}

> A Bayesian spin on an autoencoder - lets us generate data!
>
> Assume our data ![](media/image199.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"} is generated like this:

+--------------+---------+--------------------+--+---------+--+
|              |         | Sample from *true* |  |         |  |
+--------------+---------+--------------------+--+---------+--+
|              |         | *conditional*      |  |         |  |
+--------------+---------+--------------------+--+---------+--+
| Sample from  |         |                    |  |         |  |
+--------------+---------+--------------------+--+---------+--+
|              | > **z** |                    |  | > **x** |  |
+--------------+---------+--------------------+--+---------+--+
| *true prior* |         |                    |  |         |  |
+--------------+---------+--------------------+--+---------+--+
|              |         |                    |  |         |  |
+--------------+---------+--------------------+--+---------+--+
|              |         |                    |  |         |  |
+--------------+---------+--------------------+--+---------+--+

![](media/image200.jpeg){width="2.6527777777777777in"
height="5.208880139982502e-3in"}

> Kingma and Welling, "Auto-Encoding
>
> Variational Bayes", ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 56 29 Feb 2016

> ![](media/image201.jpeg){width="10.0in" height="5.413888888888889in"}
>
> A Bayesian spin on an autoencoder!
>
> Assume our data ![](media/image202.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"} is generated like this:
>
> Sample from *true*
>
> *conditional*

+--------------+---------+---------+--+
| Sample from  | > **z** | > **x** |  |
+--------------+---------+---------+--+
| *true prior* |         |         |  |
+--------------+---------+---------+--+

![](media/image203.jpeg){width="2.6527777777777777in"
height="5.208880139982502e-3in"}

> **Intuition**: **x** is an image, **z** gives class, orientation,
> attributes, etc

Kingma and Welling, "Auto-Encoding Variational Bayes", ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 57 29 Feb 2016

> ![](media/image204.jpeg){width="10.0in" height="5.413888888888889in"}
>
> A Bayesian spin on an autoencoder!
>
> Assume our data ![](media/image205.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"} is generated like this:

**Intuition**: **x** is an image, **z** gives class, orientation,
attributes, etc

+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        | Sample |        | > **Pr |        |        |        |
|        |        | from   |        | oblem* |        |        |        |
|        |        | *true* |        | *:     |        |        |        |
|        |        |        |        | > Esti |        |        |        |
|        |        |        |        | mate   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Sample |        | *condi |        | > with |        |        |        |
| from   |        | tional |        | out    |        |        |        |
|        |        | *      |        | > acce |        |        |        |
|        |        |        |        | ss     |        |        |        |
|        |        |        |        | > to   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        | > late | !      |        |
|        |        |        |        |        | nt     |        |        |
|        |        |        |        |        | > stat |        |        |
|        |        |        |        |        | es     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > **z* |        |        | > **x* |        |        |        |
|        | *      |        |        | *      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| *true  |        |        |        |        |        |        |        |
| prior* |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

![](media/image206.jpeg){width="2.6527777777777777in"
height="5.208880139982502e-3in"}

> Kingma and Welling, "Auto-Encoding
>
> Variational Bayes", ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 58 29 Feb 2016

> ![](media/image207.jpeg){width="9.340277777777779in"
> height="1.9104166666666667in"}
>
> **Prior**: Assume
> ![](media/image208.jpeg){width="0.9638888888888889in"
> height="0.4597222222222222in"}
>
> is a unit Gaussian

![](media/image209.jpeg){width="10.0in" height="0.9409722222222222in"}

Kingma and Welling, ICLR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 59 29 Feb
> 2016
>
> ![](media/image210.jpeg){width="9.340277777777779in"
> height="1.9104166666666667in"}
>
> **Prior**: Assume
> ![](media/image211.jpeg){width="0.9638888888888889in"
> height="0.4597222222222222in"}
>
> is a unit Gaussian

![](media/image212.jpeg){width="3.3645833333333335in" height="2.375in"}

> **Conditional**: Assume
>
> is a
>
> diagonal Gaussian,
>
> predict mean and
>
> variance with neural
>
> net

![](media/image213.jpeg){width="10.0in" height="0.9409722222222222in"}

Kingma and Welling, ICLR 2014

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 60 29 Feb
> 2016
>
> ![](media/image214.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Prior**: Assume
> ![](media/image215.jpeg){width="0.9638888888888889in"
> height="0.3645833333333333in"} is a unit Gaussian
>
> **Conditional**: Assume
>
> is a
>
> diagonal Gaussian,
>
> predict mean and
>
> variance with neural
>
> net

Kingma and Welling, ICLR 2014

> Mean and (diagonal) covariance of
> ![](media/image216.jpeg){width="1.5659722222222223in"
> height="0.4479166666666667in"}
>
> **x** **~Σ~x**
>
> Decoder network

with parameters

**z**

> Latent state
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 61 29 Feb
> 2016
>
> ![](media/image217.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Prior**: Assume
> ![](media/image218.jpeg){width="0.9638888888888889in"
> height="0.3645833333333333in"} is a unit Gaussian
>
> **Conditional**: Assume
>
> is a
>
> diagonal Gaussian,
>
> predict mean and
>
> variance with neural
>
> net

Kingma and Welling, ICLR 2014

> Mean and (diagonal) covariance of
> ![](media/image219.jpeg){width="1.5659722222222223in"
> height="0.4479166666666667in"}
>
> **x** **~Σ~x**
>
> Decoder network
>
> with parameters
>
> **z**

Fully-connected or

> Latent state
>
> upconvolutional
>
> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 62 29 Feb
> 2016
>
> ![](media/image220.jpeg){width="9.51388888888889in"
> height="2.517361111111111in"}
>
> By Bayes Rule the posterior is:

![](media/image221.jpeg){width="1.8701388888888888in"
height="0.4583333333333333in"}

Kingma and Welling,

ICLR 2014

![](media/image222.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 63 29 Feb
> 2016
>
> ![](media/image223.jpeg){width="9.51388888888889in"
> height="3.667361111111111in"}
>
> By Bayes Rule the posterior is:
>
> **Use decoder network =)**
>
> **Gaussian =)**
>
> **Intractible integral =(**

![](media/image224.jpeg){width="1.8701388888888888in"
height="0.4583333333333333in"}

Kingma and Welling,

ICLR 2014

![](media/image225.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 64 29 Feb
> 2016
>
> ![](media/image226.jpeg){width="10.0in" height="5.413888888888889in"}

<table>
<tbody>
<tr class="odd">
<td>By Bayes Rule the posterior is:</td>
<td><blockquote>
<p>Mean and (diagonal)</p>
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
<td><blockquote>
<p>covariance of</p>
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

+-----------------------------+-------------------+--+
| **Use decoder network =)**  | > Encoder network |  |
+-----------------------------+-------------------+--+
| **Gaussian =)**             |                   |  |
+-----------------------------+-------------------+--+
| **Intractible integral =(** | > with parameters |  |
+-----------------------------+-------------------+--+

Kingma and Welling,

ICLR 2014

**x**

Data point

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 65 29 Feb
> 2016
>
> ![](media/image227.jpeg){width="10.0in" height="5.413888888888889in"}

<table>
<tbody>
<tr class="odd">
<td>By Bayes Rule the posterior is:</td>
<td><blockquote>
<p>Mean and (diagonal)</p>
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
<td><blockquote>
<p>covariance of</p>
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

+-----------------------------+-------------------+--+
| **Use decoder network =)**  | > Encoder network |  |
+-----------------------------+-------------------+--+
| **Gaussian =)**             |                   |  |
+-----------------------------+-------------------+--+
| **Intractible integral =(** | > with parameters |  |
+-----------------------------+-------------------+--+

Kingma and Welling, ICLR 2014

+----------------------------+--------------+-------+--+--+
| Approximate posterior with |              | **x** |  |  |
+----------------------------+--------------+-------+--+--+
| **encoder network**        | > Data point |       |  |  |
+----------------------------+--------------+-------+--+--+
|                            |              |       |  |  |
+----------------------------+--------------+-------+--+--+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 66 29 Feb
> 2016
>
> ![](media/image228.jpeg){width="10.0in" height="5.413888888888889in"}

<table>
<tbody>
<tr class="odd">
<td>By Bayes Rule the posterior is:</td>
<td><blockquote>
<p>Mean and (diagonal)</p>
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
<td><blockquote>
<p>covariance of</p>
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
<td><blockquote>
<p>Fully-connected</p>
</blockquote></td>
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
<td><blockquote>
<p>or convolutional</p>
</blockquote></td>
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
</tbody>
</table>

+-----------------------------+-------------------+--+
| **Use decoder network =)**  | > Encoder network |  |
+-----------------------------+-------------------+--+
| **Gaussian =)**             |                   |  |
+-----------------------------+-------------------+--+
| **Intractible integral =(** | > with parameters |  |
+-----------------------------+-------------------+--+

Kingma and Welling, ICLR 2014

+----------------------------+--------------+-------+--+--+
| Approximate posterior with |              | **x** |  |  |
+----------------------------+--------------+-------+--+--+
| **encoder network**        | > Data point |       |  |  |
+----------------------------+--------------+-------+--+--+
|                            |              |       |  |  |
+----------------------------+--------------+-------+--+--+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 67 29 Feb
> 2016
>
> ![](media/image229.jpeg){width="9.027777777777779in"
> height="0.9270833333333334in"}

![](media/image230.jpeg){width="10.0in" height="1.1319444444444444in"}

+------------+---------+
| Data point | > **x** |
+------------+---------+

Kingma and Welling, ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 68 29 Feb 2016

> ![](media/image231.jpeg){width="9.027777777777779in"
> height="0.9270833333333334in"}

![](media/image232.jpeg){width="10.0in" height="2.2715277777777776in"}

+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        | > Mean |        |
|        |        |        |        |        |        | > and  |        |
|        |        |        |        |        |        | > (dia |        |
|        |        |        |        |        |        | gonal) |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        | > **z* |        | > **Σ^ |        |        |        |        |
|        | *      |        | z^**   |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        | > cova |        |        |        |
|        |        |        |        | riance |        |        |        |
|        |        |        |        | > of   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| Encode |        |        |        |        |        |        |        |
| r      |        |        |        |        |        |        |        |
| networ |        |        |        |        |        |        |        |
| k      |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| > Data |        | > **x* |        |        | > King |        |        |
| > poin |        | *      |        |        | ma     |        |        |
| t      |        |        |        |        | > and  |        |        |
|        |        |        |        |        | > Well |        |        |
|        |        |        |        |        | ing,   |        |        |
|        |        |        |        |        | > ICLR |        |        |
|        |        |        |        |        | > 2014 |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 69 29 Feb 2016

> ![](media/image233.jpeg){width="9.027777777777779in"
> height="0.9270833333333334in"}

![](media/image234.jpeg){width="10.0in" height="2.9715277777777778in"}

+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       | **z** |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       | > Sam |       |       | > Mea |       |       |       |       |
|       | ple   |       |       | n     |       |       |       |       |
|       | > fro |       |       | > and |       |       |       |       |
|       | m     |       |       | > (di |       |       |       |       |
|       |       |       |       | agona |       |       |       |       |
|       |       |       |       | l)    |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       | > **z |       |       | > **Σ |       |       |       |       |
|       | **    |       |       | ^z^** |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       | > cov |       |       |       |
|       |       |       |       |       | arian |       |       |       |
|       |       |       |       |       | ce    |       |       |       |
|       |       |       |       |       | > of  |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| Encod |       |       |       |       |       |       |       |       |
| er    |       |       |       |       |       |       |       |       |
| netwo |       |       |       |       |       |       |       |       |
| rk    |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| > Dat |       | **x** |       |       | > Kin |       |       |       |
| a     |       |       |       |       | gma   |       |       |       |
| > poi |       |       |       |       | > and |       |       |       |
| nt    |       |       |       |       | > Wel |       |       |       |
|       |       |       |       |       | ling, |       |       |       |
|       |       |       |       |       | > ICL |       |       |       |
|       |       |       |       |       | R     |       |       |       |
|       |       |       |       |       | > 201 |       |       |       |
|       |       |       |       |       | 4     |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 70 29 Feb 2016

> ![](media/image235.jpeg){width="9.027777777777779in"
> height="0.9270833333333334in"}

![](media/image236.jpeg){width="10.0in" height="3.823611111111111in"}

+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       | > **x |       |       | > **~ | > Mea |       |       |       |
|       | **    |       |       | Σ~x** | n     |       |       |       |
|       |       |       |       |       | > and |       |       |       |
|       |       |       |       |       | > (di |       |       |       |
|       |       |       |       |       | agona |       |       |       |
|       |       |       |       |       | l)    |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| Decod |       |       |       |       | > cov |       |       |       |
| er    |       |       |       |       | arian |       |       |       |
| netwo |       |       |       |       | ce    |       |       |       |
| rk    |       |       |       |       | > of  |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       | **z** |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       | > Sam |       |       | > Mea |       |       |       |       |
|       | ple   |       |       | n     |       |       |       |       |
|       | > fro |       |       | > and |       |       |       |       |
|       | m     |       |       | > (di |       |       |       |       |
|       |       |       |       | agona |       |       |       |       |
|       |       |       |       | l)    |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       | > **z |       |       | > **Σ |       |       |       |       |
|       | **    |       |       | ^z^** |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       | > cov |       |       |       |
|       |       |       |       |       | arian |       |       |       |
|       |       |       |       |       | ce    |       |       |       |
|       |       |       |       |       | > of  |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| > Enc |       |       |       |       |       |       |       |       |
| oder  |       |       |       |       |       |       |       |       |
| > net |       |       |       |       |       |       |       |       |
| work  |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
|       |       |       |       |       |       |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+
| > Dat |       | **x** |       |       | > Kin |       |       |       |
| a     |       |       |       |       | gma   |       |       |       |
| > poi |       |       |       |       | > and |       |       |       |
| nt    |       |       |       |       | > Wel |       |       |       |
|       |       |       |       |       | ling, |       |       |       |
|       |       |       |       |       | > ICL |       |       |       |
|       |       |       |       |       | R     |       |       |       |
|       |       |       |       |       | > 201 |       |       |       |
|       |       |       |       |       | 4     |       |       |       |
+-------+-------+-------+-------+-------+-------+-------+-------+-------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 71 29 Feb
> 2016
>
> ![](media/image237.jpeg){width="10.0in" height="5.625in"}

<table>
<tbody>
<tr class="odd">
<td>Reconstructed</td>
<td></td>
<td></td>
<td><strong>xx</strong></td>
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
<p>Sample from</p>
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
<td><blockquote>
<p><strong>x</strong></p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p><strong><sub>Σ</sub>x</strong></p>
</blockquote></td>
<td><blockquote>
<p>Mean and (diagonal)</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Decoder network</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>covariance of</p>
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
<td><strong>z</strong></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td></td>
<td><blockquote>
<p>Sample from</p>
</blockquote></td>
<td><blockquote>
<p>Mean and (diagonal)</p>
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
<td></td>
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
<p><strong>z</strong></p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p><strong>Σ<sup>z</sup></strong></p>
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
<td><blockquote>
<p>covariance of</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Encoder network</td>
<td></td>
<td></td>
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
<td><blockquote>
<p>Data point</p>
</blockquote></td>
<td></td>
<td></td>
<td><strong>x</strong></td>
<td></td>
<td><blockquote>
<p>Kingma and Welling, ICLR 2014</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 72 29 Feb
> 2016

73 29 Feb 2016

Kingma and Welling, ICLR 2014

> ![](media/image238.jpeg){width="10.0in" height="5.625in"}
>
> Reconstructed **xx**
>
> Sample from
>
> **x** **~Σ~x**

Decoder network![](media/image239.jpeg){width="0.2743055555555556in"
height="0.2375in"}

+-----------------+---------------+-------+------------+--+--+--+
|                 |               |       | **z**      |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
|                 | > Sample from |       |            |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
|                 |               |       |            |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
|                 | > **z**       |       | > **Σ^z^** |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
| Encoder network |               |       |            |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
|                 |               |       |            |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+
| > Data point    |               | **x** |            |  |  |  |
+-----------------+---------------+-------+------------+--+--+--+

> Training like a normal autoencoder: **reconstruction loss** at the
> end, **regularization toward prior** in middle
>
> Mean and (diagonal) covariance of
> ![](media/image240.jpeg){width="1.20625in"
> height="0.3958333333333333in"} **(should be close to data x)**

Mean and (diagonal) covariance of
![](media/image241.jpeg){width="1.20625in" height="0.28125in"} **(should
be close**

**to prior** ![](media/image242.jpeg){width="0.9506944444444444in"
height="0.4166666666666667in"}**)**

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14
>
> ![](media/image243.jpeg){width="9.747222222222222in"
> height="1.4145833333333333in"}
>
> After network is trained:

![](media/image244.jpeg){width="1.9131944444444444in"
height="0.9604166666666667in"}

> **z**
>
> Sample from
>
> prior

![](media/image245.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 74 29 Feb 2016

> ![](media/image246.jpeg){width="9.747222222222222in"
> height="1.4145833333333333in"}
>
> After network is trained:
>
> **x** **~Σ~x**

![](media/image247.jpeg){width="3.5659722222222223in"
height="2.0597222222222222in"}

> Decoder
>
> network
>
> **z**
>
> Sample from
>
> prior

![](media/image248.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 75 29 Feb 2016

> ![](media/image249.jpeg){width="9.747222222222222in"
> height="1.4145833333333333in"}
>
> After network is trained:

![](media/image250.jpeg){width="3.7256944444444446in"
height="3.0416666666666665in"}

Generated **xx**

> Sample from
>
> **x** **~Σ~x**
>
> Decoder
>
> network
>
> **z**
>
> Sample from
>
> prior

![](media/image251.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 76 29 Feb
> 2016
>
> ![](media/image252.jpeg){width="9.747222222222222in"
> height="1.4145833333333333in"}
>
> After network is trained:

![](media/image253.jpeg){width="7.083333333333333in"
height="3.223611111111111in"}

Generated **xx**

> Sample from
>
> **x** **~Σ~x**
>
> Decoder
>
> network
>
> **z**
>
> Sample from
>
> prior

![](media/image254.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 77 29 Feb
> 2016
>
> ![](media/image255.jpeg){width="9.940972222222221in"
> height="4.777777777777778in"}
>
> After network is trained:

Generated **xx**

> Sample from
>
> **x** **~Σ~x**
>
> Decoder
>
> network
>
> **z**
>
> Sample from
>
> prior

![](media/image256.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 78 29 Feb
> 2016
>
> ![](media/image257.jpeg){width="9.940972222222221in"
> height="4.777777777777778in"}
>
> After network is trained:
> ^Diagonal\ prior\ on\ **z**\ =\>\ independent\ latent\ variables^

Generated **xx**

> Sample from
>
> **x** **~Σ~x**
>
> Decoder
>
> network
>
> **z**
>
> Sample from
>
> prior

![](media/image258.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 79 29 Feb
> 2016
>
> Variational Autoencoder: Math Maximum Likelihood?

![](media/image259.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> Maximize likelihood of dataset
> ![](media/image261.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"}

![](media/image262.jpeg){width="10.0in" height="0.9715277777777778in"}

Kingma and Welling, ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 80 29 Feb 2016

> Variational Autoencoder: Math Maximum Likelihood?

![](media/image263.jpeg){width="9.043055555555556in"
height="3.571527777777778in"}

> Maximize likelihood of dataset
> ![](media/image264.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"}
>
> Maximize log-likelihood instead because sums are nicer

![](media/image265.jpeg){width="10.0in" height="0.9715277777777778in"}

Kingma and Welling, ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 81 29 Feb 2016

> Variational Autoencoder: Math Maximum Likelihood?

![](media/image266.jpeg){width="9.043055555555556in"
height="3.571527777777778in"}

> Maximize likelihood of dataset
> ![](media/image267.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"}
>
> Maximize log-likelihood instead because sums are nicer

![](media/image268.jpeg){width="10.0in" height="1.6868055555555554in"}

> Marginalize joint
>
> distribution

Kingma and Welling, ICLR 2014

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 82 29 Feb 2016

> Variational Autoencoder: Math Maximum Likelihood?

![](media/image269.jpeg){width="9.043055555555556in"
height="3.571527777777778in"}

> Maximize likelihood of dataset
> ![](media/image270.jpeg){width="1.5944444444444446in"
> height="0.5972222222222222in"}
>
> Maximize log-likelihood instead because sums are nicer

![](media/image271.jpeg){width="9.848611111111111in"
height="0.9652777777777778in"}

Intractible integral =(

![](media/image272.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 83 29 Feb 2016

![](media/image273.jpeg){width="9.01388888888889in" height="1.04375in"}

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 84 29 Feb
> 2016

![](media/image276.jpeg){width="9.925694444444444in" height="1.04375in"}

![](media/image277.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 85 29 Feb
> 2016

![](media/image279.jpeg){width="9.925694444444444in"
height="1.7548611111111112in"}

![](media/image280.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 86 29 Feb
> 2016

![](media/image282.jpeg){width="9.925694444444444in"
height="2.4805555555555556in"}

![](media/image283.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 87 29 Feb
> 2016

![](media/image285.jpeg){width="9.925694444444444in" height="3.11875in"}

![](media/image286.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 88 29 Feb
> 2016

![](media/image288.jpeg){width="9.946527777777778in"
height="4.004861111111111in"}

![](media/image289.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 89 29 Feb
> 2016

![](media/image290.jpeg){width="9.946527777777778in"
height="4.065277777777778in"}

> **"Elbow"**

![](media/image291.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 90 29 Feb
> 2016

![](media/image292.jpeg){width="9.925694444444444in"
height="4.065277777777778in"}

> **"Elbow"**

![](media/image293.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 91 29 Feb
> 2016

![](media/image294.jpeg){width="9.925694444444444in"
height="4.947222222222222in"}

> **"Elbow"**
>
> **Variational lower bound (elbow)**

![](media/image295.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 92 29 Feb
> 2016

![](media/image296.jpeg){width="9.925694444444444in" height="5.01875in"}

> Variational Autoencoder: Math
>
> **"Elbow"**

+-----------------------+-----------------------+-----------------------+
| > **Variational lower | > **Training:         |                       |
| > bound (elbow)**     | > Maximize lower      |                       |
|                       | > bound**             |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 14 93       | > 29 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image297.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image298.jpeg){width="9.925694444444444in" height="5.01875in"}

> Variational Autoencoder: Math
>
> **Reconstruct**
>
> **the input**
>
> **data**
>
> **"Elbow"**

+-----------------------+-----------------------+-----------------------+
| > **Variational lower | > **Training:         |                       |
| > bound (elbow)**     | > Maximize lower      |                       |
|                       | > bound**             |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 14 94       | > 29 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image299.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image300.jpeg){width="10.0in" height="5.01875in"}

+-------------------------------+---------------------+
| Variational Autoencoder: Math | > **Latent states** |
+-------------------------------+---------------------+
|                               | > **should follow** |
+-------------------------------+---------------------+
| > **Reconstruct**             | > **the prior**     |
+-------------------------------+---------------------+
| > **the input**               |                     |
+-------------------------------+---------------------+
| > **data**                    |                     |
+-------------------------------+---------------------+

> **"Elbow"**

+-----------------------+-----------------------+-----------------------+
| > **Variational lower | > **Training:         |                       |
| > bound (elbow)**     | > Maximize lower      |                       |
|                       | > bound**             |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 14 95       | > 29 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image301.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image302.jpeg){width="10.0in" height="5.01875in"}

> Variational Autoencoder: Math
>
> **Reconstruct**
>
> **the input**
>
> **data**
>
> **Sampling**
>
> **with**
>
> **reparam.**
>
> **trick**
>
> **(see paper)**
>
> **"Elbow"**

**Latent states should follow the prior**

+-----------------------+-----------------------+-----------------------+
| > **Variational lower | > **Training:         |                       |
| > bound (elbow)**     | > Maximize lower      |                       |
|                       | > bound**             |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 14 96       | > 29 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image303.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

![](media/image304.jpeg){width="10.0in" height="5.01875in"}

> Variational Autoencoder: Math
>
> **Reconstruct**
>
> **the input**
>
> **data**
>
> **Sampling**
>
> **with**
>
> **reparam.**
>
> **trick**
>
> **(see paper)**
>
> **"Elbow"**

**Latent states should follow the prior**

> **Everything is Gaussian, closed form solution!**

+-----------------------+-----------------------+-----------------------+
| > **Variational lower | > **Training:         |                       |
| > bound (elbow)**     | > Maximize lower      |                       |
|                       | > bound**             |                       |
+-----------------------+-----------------------+-----------------------+
| > Fei-Fei Li & Andrej | > Lecture 14 97       | > 29 Feb 2016         |
| > Karpathy & Justin   |                       |                       |
| > Johnson             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image305.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image306.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image307.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Traditional Autoencoders

    -   Try to reconstruct input

    -   Used to learn features, initialize supervised model

    -   Not used much anymore

-   Variational Autoencoders

    -   Bayesian meets deep learning

    -   Sample from model to generate images

![](media/image308.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 98 29 Feb 2016

![](media/image309.jpeg){width="9.474305555555556in" height="1.59375in"}

> Generative Adversarial Nets

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

Can we generate images with less math?

![](media/image310.jpeg){width="3.3625in" height="0.4583333333333333in"}

+--------------+---------+
| Random noise | > **z** |
+--------------+---------+

![](media/image311.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 99 29 Feb 2016

![](media/image312.jpeg){width="9.474305555555556in" height="1.59375in"}

> Generative Adversarial Nets

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

Can we generate images with less math?

![](media/image313.jpeg){width="3.857638888888889in" height="1.7625in"}

+------------+---------+
| Fake image | > **x** |
+------------+---------+

![](media/image314.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Generator**

+--------------+---------+
| Random noise | > **z** |
+--------------+---------+

![](media/image315.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 100 29 Feb 2016

![](media/image316.jpeg){width="9.63125in" height="4.531944444444444in"}

> Generative Adversarial Nets

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

Can we generate images with less math?

+---------------+---------+
| Real or fake? | > **y** |
+---------------+---------+

![](media/image317.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Discriminator**

+------------+---------+
| Fake image | > **x** |
+------------+---------+

![](media/image318.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Generator**

+--------------+---------+
| Random noise | > **z** |
+--------------+---------+

![](media/image319.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 101 29 Feb 2016

![](media/image320.jpeg){width="9.63125in" height="4.577083333333333in"}

> Generative Adversarial Nets

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

Can we generate images with less math?

+---------------+---------+
| Real or fake? | > **y** |
+---------------+---------+

![](media/image321.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Discriminator**

+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
| Fake image      |  | > **x** |  |  |                                 |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
| > **Generator** |  |         |  |  | > **x**                         | > Real image |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
|                 |  |         |  |  |                                 |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
|                 |  |         |  |  | > Fake examples: from generator |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
|                 |  |         |  |  |                                 |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
| > Random noise  |  | > **z** |  |  |                                 |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+
|                 |  |         |  |  | > Real examples: from dataset   |              |  |  |
+-----------------+--+---------+--+--+---------------------------------+--------------+--+--+

![](media/image322.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 102 29 Feb 2016

![](media/image324.jpeg){width="9.63125in" height="4.577083333333333in"}

> Generative Adversarial Nets

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

+---------------+---------+
| Real or fake? | > **y** |
+---------------+---------+

![](media/image325.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Discriminator**

+------------+---------+
| Fake image | > **x** |
+------------+---------+

![](media/image326.jpeg){width="5.208880139982502e-3in"
height="0.8743055555555556in"}

> **Generator**

+--------------+---------+
| Random noise | > **z** |
+--------------+---------+

Can we generate images with less math?

> Train generator and discriminator jointly After training, easy to
> generate images

+---------+--------------+
| > **x** | > Real image |
+---------+--------------+

> Fake examples: from generator
>
> Real examples: from dataset

![](media/image327.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 103 29 Feb 2016

![](media/image328.jpeg){width="10.0in" height="5.413888888888889in"}

> Generative Adversarial Nets

Generated samples

> Nearest neighbor from training set

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

![](media/image329.jpeg){width="5.770138888888889in"
height="0.5819444444444445in"} Lecture 14 104 29 Feb 2016

![](media/image330.jpeg){width="10.0in" height="5.413888888888889in"}

> Generative Adversarial Nets

Generated samples (CIFAR-10)

> Nearest neighbor from training set

Goodfellow et al, "Generative Adversarial Nets", NIPS 2014

![](media/image331.jpeg){width="5.770138888888889in"
height="0.5819444444444445in"} Lecture 14 105 29 Feb 2016

![](media/image332.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

![](media/image333.jpeg){width="10.0in" height="3.8965277777777776in"}

Denton et al, "Deep generative image models using a Laplacian pyramid of
adversarial networks", NIPS 2015

Generate low-res

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 106 29 Feb
> 2016

![](media/image334.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

![](media/image335.jpeg){width="10.0in" height="4.340972222222222in"}

Upsample

Denton et al, "Deep generative image models using a Laplacian pyramid of
adversarial networks", NIPS 2015

Generate low-res

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 107 29 Feb
> 2016

![](media/image336.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

![](media/image337.jpeg){width="10.0in" height="4.340972222222222in"}

Upsample

+-----------------------+-----------------------+-----------------------+
| > Generate            | > Generate            |                       |
+-----------------------+-----------------------+-----------------------+
| > delta, add          |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       | > low-res             |                       |
+-----------------------+-----------------------+-----------------------+
| Denton et al, "Deep   |                       |                       |
| generative image      |                       |                       |
| models using a        |                       |                       |
| Laplacian pyramid of  |                       |                       |
| adversarial           |                       |                       |
| networks", NIPS 2015  |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 108 29 Feb
> 2016

![](media/image338.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

![](media/image339.jpeg){width="10.0in" height="4.340972222222222in"}

> Upsample Upsample

+-----------------------+-----------------------+-----------------------+
| > Generate            | > Generate            |                       |
+-----------------------+-----------------------+-----------------------+
| > delta, add          |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       | > low-res             |                       |
+-----------------------+-----------------------+-----------------------+
| Denton et al, "Deep   |                       |                       |
| generative image      |                       |                       |
| models using a        |                       |                       |
| Laplacian pyramid of  |                       |                       |
| adversarial           |                       |                       |
| networks", NIPS 2015  |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 109 29 Feb
> 2016

![](media/image340.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

![](media/image341.jpeg){width="10.0in" height="4.340972222222222in"}

> Upsample Upsample

+-----------------+-----------------+-----------------+-----------------+
| > Generate      | > Generate      | > Generate      |                 |
+-----------------+-----------------+-----------------+-----------------+
| > delta, add    | > delta, add    |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | > low-res       |                 |
+-----------------+-----------------+-----------------+-----------------+
| Denton et al,   |                 |                 |                 |
| "Deep           |                 |                 |                 |
| generative      |                 |                 |                 |
| image models    |                 |                 |                 |
| using a         |                 |                 |                 |
| Laplacian       |                 |                 |                 |
| pyramid of      |                 |                 |                 |
| adversarial     |                 |                 |                 |
| networks", NIPS |                 |                 |                 |
| 2015            |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 110 29 Feb
> 2016

![](media/image342.jpeg){width="10.0in" height="5.413888888888889in"}

+----------+------------+------------+--+
| Upsample | > Upsample | > Upsample |  |
+----------+------------+------------+--+
|          |            |            |  |
+----------+------------+------------+--+

+-----------------+-----------------+-----------------+-----------------+
| > Generate      | > Generate      | > Generate      |                 |
+-----------------+-----------------+-----------------+-----------------+
| > delta, add    | > delta, add    |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 | > low-res       |                 |
+-----------------+-----------------+-----------------+-----------------+
| Denton et al,   |                 |                 |                 |
| "Deep           |                 |                 |                 |
| generative      |                 |                 |                 |
| image models    |                 |                 |                 |
| using a         |                 |                 |                 |
| Laplacian       |                 |                 |                 |
| pyramid of      |                 |                 |                 |
| adversarial     |                 |                 |                 |
| networks", NIPS |                 |                 |                 |
| 2015            |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+
|                 |                 |                 |                 |
+-----------------+-----------------+-----------------+-----------------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 111 29 Feb
> 2016

![](media/image343.jpeg){width="10.0in" height="5.413888888888889in"}

+-------+------------+------------+------------+--+
| Done! | > Upsample | > Upsample | > Upsample |  |
+-------+------------+------------+------------+--+
|       |            |            |            |  |
+-------+------------+------------+------------+--+

+-------------+-------------+-------------+-------------+-------------+
| > Generate  | > Generate  | > Generate  | > Generate  |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             | > delta,    |             |             |
|             |             | > add       |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > delta,    | > delta,    |             | > low-res   |             |
| > add       | > add       |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Denton et   | > pyramid   |             |             |             |
| al, "Deep   | > of        |             |             |             |
| generative  | > adversari |             |             |             |
| image       | al          |             |             |             |
| models      | > networks" |             |             |             |
|             | ,           |             |             |             |
|             | > NIPS 2015 |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 112 29 Feb
> 2016

![](media/image344.jpeg){width="10.0in" height="5.413888888888889in"}

> Discriminators work
>
> at every scale!

Denton et al, NIPS 2015

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 113 29 Feb
> 2016

![](media/image345.jpeg){width="9.979861111111111in"
height="5.413888888888889in"}

Generative Adversarial Nets: Multiscale

> Train separate model per-class on CIFAR-10
>
> Denton et al, NIPS 2015

+-----------------------+------+
| > Fei-Fei Li & Andrej | 2016 |
+-----------------------+------+
|                       |      |
+-----------------------+------+

> ![](media/image346.jpeg){width="9.291666666666666in"
> height="0.9652777777777778in"}

![](media/image347.jpeg){width="9.363888888888889in"
height="0.8826388888888889in"}

> Generator is an upsampling network with fractionally-strided
> convolutions Discriminator is a convolutional network

![](media/image348.jpeg){width="10.0in" height="3.509027777777778in"}

> Radford et al, "Unsupervised Representation Learning with Deep
> Convolutional Generative Adversarial Networks", ICLR 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 115 29 Feb 2016

> ![](media/image349.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Generator
>
> Radford et al, "Unsupervised Representation Learning with Deep
> Convolutional Generative Adversarial Networks", ICLR 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 116 29 Feb 2016

> ![](media/image350.jpeg){width="9.946527777777778in"
> height="4.822916666666667in"}
>
> Samples from the model look amazing!

Radford et al, ICLR 2016

![](media/image351.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 117 29 Feb
> 2016
>
> ![](media/image352.jpeg){width="9.842361111111112in"
> height="4.820833333333334in"}

Interpolating

between

random

points in latent

space

Radford et al, ICLR 2016

![](media/image353.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 118 29 Feb
> 2016
>
> Generative Adversarial Nets: Vector Math

![](media/image354.jpeg){width="9.55625in"
height="3.0416666666666665in"}

Smiling woman Neutral woman Neutral man

> Samples from the model

![](media/image355.jpeg){width="10.0in" height="0.5888888888888889in"}

Radford et al, ICLR 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 119 29 Feb 2016

> Generative Adversarial Nets: Vector Math

![](media/image356.jpeg){width="9.683333333333334in"
height="4.050694444444445in"}

> Radford et al, ICLR 2016
>
> Smiling woman Neutral woman Neutral man
>
> Samples from the model
>
> Average Z vectors, do arithmetic

![](media/image357.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 120 29 Feb 2016

> Generative Adversarial Nets: Vector Math

![](media/image358.jpeg){width="9.716666666666667in"
height="4.050694444444445in"}

> Smiling woman Neutral woman Neutral man

Radford et al, ICLR 2016

+----------+---------------+--+
| Samples  | > Smiling Man |  |
+----------+---------------+--+
|          |               |  |
+----------+---------------+--+
| from the |               |  |
+----------+---------------+--+
| model    |               |  |
+----------+---------------+--+

> Average Z vectors, do arithmetic

![](media/image359.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 121 29 Feb 2016

> ![](media/image360.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Glasses man No glasses man No glasses woman
>
> Radford et al, ICLR 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 122 29 Feb 2016

> ![](media/image361.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Glasses man No glasses man No glasses woman
>
> Woman with glasses
>
> Radford et al, ICLR 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 123 29 Feb 2016

![](media/image362.jpeg){width="9.463888888888889in"
height="1.1034722222222222in"}

> Putting everything together

![](media/image363.jpeg){width="4.0680555555555555in"
height="3.2680555555555557in"}

> Pixel loss

![](media/image364.jpeg){width="5.208880139982502e-3in"
height="0.75625in"}

> **xx**
>
> **x** **~Σ~x**
>
> Variational
>
> Autoencoder **z**
>
> **z** **~Σ~z**
>
> **x**

![](media/image367.jpeg){width="10.0in" height="0.5888888888888889in"}

Dosovitskiy and Brox, "Generating Images with Perceptual Similarity
Metrics based on Deep Networks", arXiv 2016

![](media/image368.jpeg){width="0.25972222222222224in"
height="0.25972222222222224in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 124 29 Feb 2016

![](media/image370.jpeg){width="9.542361111111111in"
height="4.842361111111111in"}

> Putting everything together
>
> Real or Generated

![](media/image371.jpeg){width="5.208880139982502e-3in"
height="0.6576388888888889in"}

Dosovitskiy and Brox, "Generating Images with Perceptual Similarity
Metrics based on Deep Networks", arXiv 2016

+---------------+--------------+--+
| Discriminator | > Pixel loss |  |
+---------------+--------------+--+
| network       | > **y**      |  |
+---------------+--------------+--+
|               |              |  |
+---------------+--------------+--+

![](media/image372.jpeg){width="5.208880139982502e-3in"
height="0.75625in"}

> **xx**
>
> **x** **~Σ~x**
>
> Variational
>
> Autoencoder **z**
>
> **z** **~Σ~z**
>
> **x**

![](media/image373.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 125 29 Feb 2016

> ![](media/image374.jpeg){width="9.542361111111111in"
> height="4.842361111111111in"}
>
> Images with Perceptual Similarity
>
> Putting everything together Metrics based on Deep Networks", arXiv
> 2016
>
> Real or Generated
>
> Pretrained AlexNet

![](media/image375.jpeg){width="5.208880139982502e-3in"
height="0.6576388888888889in"}

+---------------+--------------+--+
| Discriminator | > Pixel loss |  |
+---------------+--------------+--+
| network       | > **y**      |  |
+---------------+--------------+--+
|               |              |  |
+---------------+--------------+--+

![](media/image376.jpeg){width="5.208880139982502e-3in"
height="0.75625in"}

> **xx**
>
> **x** **~Σ~x**
>
> Variational
>
> Autoencoder **z**
>
> **z** **~Σ~z**
>
> **x**

![](media/image377.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 126 29 Feb 2016

> ![](media/image378.jpeg){width="9.593055555555555in"
> height="4.842361111111111in"}
>
> Images with Perceptual Similarity
>
> Putting everything together Metrics based on Deep Networks", arXiv
> 2016
>
> Real or Generated

+---------+---------+---------+---------+---------+---------+---------+
|         |         |         | > Pretr |         |         |         |
|         |         |         | ained   |         |         |         |
|         |         |         | > AlexN |         |         |         |
|         |         |         | et      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Discrim | > Pixel |         |         |         |         |         |
| inator  | > loss  |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| network | > **y** |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **xx* |         |         |         |         |         |
|         | *       |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Varia | > **x** | > **Σ^x |         |         | > Featu |         |
| tional  |         | ^**     |         |         | res     |         |
|         |         |         |         |         | > of    |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **z** |         | > Featu | > **xf* |         |         |
|         |         |         | res     | *       |         |         |
|         |         |         | > of    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Autoe |         |         |         |         | > **xxf |         |
| ncoder  |         |         |         |         | **      |         |
|         |         |         |         |         | > recon |         |
|         |         |         |         |         | structe |         |
|         |         |         |         |         | d       |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **z** | > **Σ^z | > real  |         | > image |         |
|         |         | ^**     | > image |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+

![](media/image379.jpeg){width="5.208880139982502e-3in"
height="0.6701388888888888in"}

> **x**

![](media/image383.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 127 29 Feb 2016

![](media/image384.jpeg){width="9.593055555555555in"
height="4.934027777777778in"}

> Dosovitskiy and Brox, "Generating
>
> Images with Perceptual Similarity
>
> Putting everything together Metrics based on Deep Networks", arXiv
> 2016
>
> Real or Generated

+---------+---------+---------+---------+---------+---------+---------+
|         |         |         | > Pretr |         |         |         |
|         |         |         | ained   |         |         |         |
|         |         |         | > AlexN |         |         |         |
|         |         |         | et      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Discr | > Pixel |         |         |         |         |         |
| iminato | > loss  |         |         |         |         |         |
| r       |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > netwo | > **y** |         |         |         |         |         |
| rk      |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **xx* |         |         |         |         |         |
|         | *       |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Varia | > **x** | > **Σ^x |         |         | > Featu |         |
| tional  |         | ^**     |         |         | res     |         |
|         |         |         |         |         | > of    |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **z** |         | > Featu | > **xf* |         |         |
|         |         |         | res     | *       |         |         |
|         |         |         | > of    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Autoe |         |         |         |         | > **xxf |         |
| ncoder  |         |         |         |         | **      |         |
|         |         |         |         |         | > recon |         |
|         |         |         |         |         | structe |         |
|         |         |         |         |         | d       |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **z** | > **Σ^z | > real  |         | > image |         |
|         |         | ^**     | > image |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > **x** |         |         | > L2    |         |         |
|         |         |         |         | > loss  |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Fei-Fei | > Lectu | > 29    |         |         |         |         |
| Li &    | re      | > Feb   |         |         |         |         |
| Andrej  | > 14    | > 2016  |         |         |         |         |
| Karpath | > 128   |         |         |         |         |         |
| y       |         |         |         |         |         |         |
| &       |         |         |         |         |         |         |
| Justin  |         |         |         |         |         |         |
| Johnson |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+

![](media/image385.jpeg){width="10.0in" height="0.5888888888888889in"}

![](media/image390.jpeg){width="10.0in" height="5.551388888888889in"}

> Putting everything together
>
> Samples from the model, trained on ImageNet

Dosovitskiy and Brox, "Generating Images with Perceptual Similarity
Metrics based on Deep Networks", arXiv 2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 129 29 Feb 2016

> ![](media/image391.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image392.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Videos

-   Unsupervised learning

    -   Autoencoders: Traditional / variational

    -   Generative Adversarial Networks

-   Next time: Guest lecture from Jeff Dean

![](media/image393.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 14 130 29 Feb 2016
