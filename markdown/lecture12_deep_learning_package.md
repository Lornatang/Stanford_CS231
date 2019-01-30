![](media/image1.jpeg){width="9.73125in" height="4.50625in"}

Software Packages

Caffe / Torch / Theano / TensorFlow

![](media/image2.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 1 22 Feb 2016

> ![](media/image3.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image4.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   Milestones were due 2/17; looking at them this week

-   Assignment 3 due Wednesday 2/22

-   If you are using Terminal: BACK UP YOUR CODE!

![](media/image5.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 2 22 Feb 2016

Caffe

![](media/image6.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

[[http://caffe.berkeleyvision.org]{.underline}](http://caffe.berkeleyvision.org)

![](media/image7.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 3 22 Feb 2016

> ![](media/image8.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image9.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   From U.C. Berkeley

-   Written in C++

-   Has Python and MATLAB bindings

-   Good for training or finetuning feedforward models

![](media/image10.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 4 22 Feb 2016

> ![](media/image11.jpeg){width="10.0in" height="5.413888888888889in"}

Don't be afraid to read the code!

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 5 22 Feb 2016

+-----------------------+-----------------------+-----------------------+
| **Caffe: Main         | > SoftmaxLossLayer    |                       |
| classes**             |                       |                       |
+-----------------------+-----------------------+-----------------------+
|                       | > data                |                       |
+-----------------------+-----------------------+-----------------------+
|                       |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > **● Blob**: Stores  | > ^fc1^ diffs         |                       |
| > data and            |                       |                       |
+-----------------------+-----------------------+-----------------------+
| > derivatives         |                       |                       |
| > ([[header](https:// |                       |                       |
| github.com/BVLC/caffe |                       |                       |
| /blob/85bb397acfd383a |                       |                       |
| 676c125c75d877642d6b3 |                       |                       |
| 9ff6/include/caffe/bl |                       |                       |
| ob.hpp)               |                       |                       |
| > [source](https://gi |                       |                       |
| thub.com/BVLC/caffe/b |                       |                       |
| lob/85bb397acfd383a67 |                       |                       |
| 6c125c75d877642d6b39f |                       |                       |
| f6/src/caffe/blob.cpp |                       |                       |
| )]{.underline})       |                       |                       |
+-----------------------+-----------------------+-----------------------+

![](media/image12.jpeg){width="10.0in" height="5.58125in"}

-   **Layer**: Transforms bottom blobs to top blobs ([[header +
    > source]{.underline}](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/include/caffe/layer.hpp))

-   **Net**: Many layers; computes gradients via forward / backward
    > ([[header](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/include/caffe/net.hpp)
    > [source](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/src/caffe/net.cpp)]{.underline})

-   **Solver**: Uses gradients to update weights
    > ([[header](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/include/caffe/solver.hpp)
    > [source](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/src/caffe/solver.cpp)]{.underline})

**\
**

> InnerProductLayer

![](media/image13.jpeg){width="5.208880139982502e-3in"
height="0.3597222222222222in"}

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
<td><blockquote>
<p>W</p>
</blockquote></td>
<td><blockquote>
<p>data</p>
</blockquote></td>
<td></td>
<td></td>
<td><blockquote>
<p>X</p>
</blockquote></td>
<td></td>
<td>data</td>
<td></td>
<td></td>
<td><blockquote>
<p>y</p>
</blockquote></td>
<td><blockquote>
<p>data</p>
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
</tr>
<tr class="odd">
<td></td>
<td><blockquote>
<p>diffs</p>
</blockquote></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>diffs</td>
<td></td>
<td></td>
<td></td>
<td><blockquote>
<p>diffs</p>
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
</tr>
</tbody>
</table>

![](media/image14.jpeg){width="5.208880139982502e-3in"
height="0.3597222222222222in"}

> DataLayer

Fei Lecture 12 6 22 Feb 2016

> ![](media/image15.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image16.jpeg){width="10.0in" height="4.326388888888889in"}

-   "Typed JSON" from Google

-   Define "message types" in .proto files

**.proto file**

[[https://developers.google.com/protocol-buffers/]{.underline}](https://developers.google.com/protocol-buffers/)

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 7 22 Feb 2016
>
> ![](media/image17.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image18.jpeg){width="10.0in" height="4.326388888888889in"}

-   "Typed JSON" from Google

-   Define "message types" in .proto files

-   Serialize instances to text files (.prototxt)

> **.proto file**
>
> **.prototxt file**

**name: "John Doe"**

**id: 1234**

**email: "jdoe\@example.com"**

[[https://developers.google.com/protocol-buffers/]{.underline}](https://developers.google.com/protocol-buffers/)

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 8 22 Feb 2016
>
> ![](media/image19.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image20.jpeg){width="10.0in" height="4.326388888888889in"}

> **●** "Typed JSON"
>
> from Google
>
> ● Define "message
>
> types" in .proto files
>
> ● Serialize instances to

**.proto file** **Java class**

> text files (.prototxt)
>
> ● Compile classes for

**.prototxt file**

**name: "John Doe"**

**id: 1234**

**C++ class**

> different languages

**email: "jdoe\@example.com"**

[[https://developers.google.com/protocol-buffers/]{.underline}](https://developers.google.com/protocol-buffers/)

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 9 22 Feb 2016
>
> ![](media/image21.jpeg){width="9.489583333333334in"
> height="3.8652777777777776in"}

![](media/image22.jpeg){width="8.676388888888889in"
height="0.7152777777777778in"}

> [<https://github.com/BVLC/caffe/blob/master/src/caffe/proto/caffe.proto>]{.underline}
> \<- **All Caffe proto types defined here, good documentation!**

![](media/image23.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 10 22 Feb 2016

![](media/image24.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> **Caffe: Training / Finetuning**

![](media/image25.jpeg){width="9.602777777777778in"
height="4.326388888888889in"}

> No need to write code!

1.  Convert data (run a script)

2.  Define net (edit prototxt)

3.  Define solver (edit prototxt)

4.  Train (with pretrained weights) (run a script)

+-------+------+
| > Fei | 2016 |
+-------+------+
|       |      |
+-------+------+

![](media/image26.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> **Caffe Step 1: Convert Data**

![](media/image27.jpeg){width="9.602777777777778in"
height="4.326388888888889in"}

-   DataLayer reading from LMDB is the easiest

-   Create LMDB using
    > [[convert\_imageset]{.underline}](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/tools/convert_imageset.cpp)

-   Need text file where each line is

    -   "\[path/to/image.jpeg\] \[label\]"

-   Create HDF5 file yourself using h5py

+-------+------+
| > Fei | 2016 |
+-------+------+
|       |      |
+-------+------+

> ![](media/image28.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image29.jpeg){width="8.188194444444445in" height="2.85in"}

-   ImageDataLayer: Read from image files

-   WindowDataLayer: For detection

-   HDF5Layer: Read from HDF5 file

-   From memory, using Python interface

-   All of these are harder to use (except Python)

![](media/image30.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 13 22 Feb 2016

> ![](media/image31.jpeg){width="9.07986111111111in"
> height="4.954166666666667in"}

![](media/image32.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 14 22 Feb 2016

> ![](media/image33.jpeg){width="9.07986111111111in"
> height="4.954166666666667in"}
>
> ![](media/image34.jpeg){width="1.0486111111111112in"
> height="0.22847222222222222in"}Layers and Blobs

![](media/image35.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> often have same

![](media/image36.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> name!

![](media/image37.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 15 22 Feb 2016

> ![](media/image38.jpeg){width="9.07986111111111in"
> height="4.975694444444445in"}
>
> ![](media/image39.jpeg){width="1.0486111111111112in"
> height="0.22847222222222222in"}Layers and Blobs

![](media/image40.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> often have same

![](media/image41.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> name!

Learning rates

(weight + bias)

> Regularization
>
> (weight + bias)

![](media/image42.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 16 22 Feb 2016

> ![](media/image43.jpeg){width="9.45486111111111in"
> height="4.975694444444445in"}
>
> ![](media/image44.jpeg){width="1.0486111111111112in"
> height="0.22847222222222222in"}Layers and Blobs
> ![](media/image45.jpeg){width="1.0486111111111112in"
> height="0.22847222222222222in"}often have same name!

![](media/image46.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

Learning rates

(weight + bias)

> Regularization
>
> (weight + bias)

![](media/image48.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> Number of output
>
> classes

Lecture 12 17 22 Feb 2016

> ![](media/image49.jpeg){width="9.45486111111111in"
> height="4.975694444444445in"}
>
> ![](media/image50.jpeg){width="1.0486111111111112in"
> height="0.22847222222222222in"}Layers and Blobs

![](media/image51.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> often have same

![](media/image52.jpeg){width="1.03125in"
height="5.208880139982502e-3in"}

> name!
>
> Set these to 0 to
>
> freeze a layer

Number of output

classes

Learning rates

(weight + bias)

> Regularization
>
> (weight + bias)

![](media/image53.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 18 22 Feb 2016

> ![](media/image54.jpeg){width="10.0in" height="5.413888888888889in"}

-   .prototxt can get ugly for big models

-   ResNet-152 prototxt is 6775 lines long!

-   Not "compositional"; can't easily define a residual block and reuse

[[https://github.com/KaimingHe/deep-residual-networks/blob/master/prototxt/ResNet-152-deploy.prototxt]{.underline}](https://github.com/KaimingHe/deep-residual-networks/blob/master/prototxt/ResNet-152-deploy.prototxt)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 19 22 Feb 2016

> ![](media/image55.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Original prototxt:**
>
> **layer {**
>
> **name: \"fc7\"**
>
> **type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**
>
> **}**
>
> **}**
>
> **\[\... ReLU, Dropout\] layer {**
>
> **name: \"fc8\"**
>
> **type: \"InnerProduct\" inner\_product\_param { num\_output: 1000**
>
> **}**
>
> **}**

**Pretrained weights:**

**"fc7.weight": \[values\]**

**"fc7.bias": \[values\]**

**"fc8.weight": \[values\]**

**"fc8.bias": \[values\]**

**Modified prototxt:**

**layer {**

> **name: \"fc7\"**

**type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**

> **}**

**}**

**\[\... ReLU, Dropout\] layer {**

> **name: \"my-fc8\" type: \"InnerProduct\" inner\_product\_param {**
>
> **num\_output: 10**
>
> **}**

**}**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 20 22 Feb 2016

> ![](media/image56.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Original prototxt:**

**layer {**

**name:**

> **type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**
>
> **}**
>
> **}**
>
> **\[\... ReLU, Dropout\] layer {**
>
> **name: \"fc8\"**
>
> **type: \"InnerProduct\" inner\_product\_param { num\_output: 1000**
>
> **}**
>
> **}**
>
> Same name:
>
> weights copied

**Pretrained weights:**

**"fc8.weight": \[values\]**

**"fc8.bias": \[values\]**

**Modified prototxt:**

**layer {**

**name:**

**type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**

> **}**

**}**

**\[\... ReLU, Dropout\] layer {**

> **name: \"my-fc8\" type: \"InnerProduct\" inner\_product\_param {**
>
> **num\_output: 10**
>
> **}**

**}**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 21 22 Feb 2016

> ![](media/image57.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Original prototxt:**
>
> **layer {**
>
> **name: \"fc7\"**
>
> **type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**
>
> **}**
>
> **}**
>
> **\[\... ReLU, Dropout\] layer {**
>
> **name:**
>
> **type: \"InnerProduct\" inner\_product\_param { num\_output: 1000**
>
> **}**
>
> **}**
>
> Same name:
>
> weights copied
>
> **Pretrained weights:**
>
> **"fc7.weight": \[values\]**
>
> **"fc7.bias": \[values\]**

Different name:

weights reinitialized

**Modified prototxt:**

**layer {**

> **name: \"fc7\"**

**type: \"InnerProduct\" inner\_product\_param { num\_output: 4096**

> **}**

**}**

**\[\... ReLU, Dropout\] layer {**

> **name:**
>
> **type: \"InnerProduct\" inner\_product\_param {**

**num\_output: 10**

> **}**

**}**

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 22 22 Feb 2016

> ![](media/image58.jpeg){width="10.0in" height="5.413888888888889in"}

-   Write a prototxt file defining a
    > [[SolverParameter]{.underline}](https://github.com/BVLC/caffe/blob/85bb397acfd383a676c125c75d877642d6b39ff6/src/caffe/proto/caffe.proto#L92)

-   If finetuning, copy existing solver. prototxt file

    -   Change net to be your net

    -   Change snapshot\_prefix to your output

    -   Reduce base learning rate (divide by 100)

    -   Maybe change max\_iter and snapshot

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 23 22 Feb 2016

> ![](media/image59.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image60.jpeg){width="9.49375in" height="3.714583333333333in"}

> **./build/tools/caffe train \\ -gpu 0 \\**
>
> **-model path/to/trainval.prototxt \\ -solver path/to/solver.prototxt
> \\**
>
> **-weights path/to/pretrained\_weights.caffemodel**

[[https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp]{.underline}](https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp)

![](media/image61.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 24 22 Feb
> 2016
>
> ![](media/image62.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image63.jpeg){width="9.49375in" height="3.714583333333333in"}

> **./build/tools/caffe train \\**
>
> **-model path/to/trainval.prototxt \\ -solver path/to/solver.prototxt
> \\**

![](media/image64.jpeg){width="5.208880139982502e-3in"
height="1.3798611111111112in"}

> **-weights path/to/pretrained\_weights.caffemodel**
>
> **-gpu -1** ![](media/image65.jpeg){width="1.7395833333333333in"
> height="0.23680555555555555in"}

[[https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp]{.underline}](https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp)

![](media/image66.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 25 22 Feb
> 2016
>
> ![](media/image67.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image68.jpeg){width="9.49375in" height="3.714583333333333in"}

> **./build/tools/caffe train \\**
>
> **-model path/to/trainval.prototxt \\ -solver path/to/solver.prototxt
> \\**

![](media/image69.jpeg){width="5.208880139982502e-3in"
height="1.3798611111111112in"}

> **-weights path/to/pretrained\_weights.caffemodel**
>
> **-gpu all** ![](media/image70.jpeg){width="3.763888888888889in"
> height="0.2881944444444444in"}

[[https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp]{.underline}](https://github.com/BVLC/caffe/blob/master/tools/caffe.cpp)

![](media/image71.jpeg){width="10.0in" height="0.5888888888888889in"}

> Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 26 22 Feb
> 2016
>
> ![](media/image72.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image73.jpeg){width="9.400694444444444in"
height="3.714583333333333in"}

> AlexNet, VGG, GoogLeNet, ResNet, plus others

[[https://github.com/BVLC/caffe/wiki/Model-Zoo]{.underline}](https://github.com/BVLC/caffe/wiki/Model-Zoo)

![](media/image74.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 27 22 Feb 2016

> ![](media/image75.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image76.jpeg){width="9.027777777777779in"
height="3.408333333333333in"}

> Not much documentation...
>
> Read the code! Two most important files:

-   [[caffe/python/caffe/\_caffe.cpp]{.underline}](https://github.com/BVLC/caffe/blob/master/python/caffe/_caffe.cpp):

    -   Exports Blob, Layer, Net, and Solver classes

-   [[caffe/python/caffe/pycaffe.py]{.underline}](https://github.com/BVLC/caffe/blob/master/python/caffe/pycaffe.py)

    -   Adds extra methods to Net class

![](media/image77.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 28 22 Feb 2016

> ![](media/image78.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image79.jpeg){width="9.307638888888889in"
height="3.714583333333333in"}

> Good for:

-   Interfacing with numpy

-   Extract features: Run net forward

-   Compute gradients: Run net backward (DeepDream, etc)

-   Define layers in Python with numpy (CPU only)

![](media/image80.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 29 22 Feb 2016

> ![](media/image81.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image82.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   (+) Good for feedforward networks

-   (+) Good for finetuning existing networks

-   (+) Train models without writing any code!

-   (+) Python interface is pretty useful!

-   (-) Need to write C++ / CUDA for new GPU layers

-   (-) Not good for recurrent networks

-   (-) Cumbersome for big networks (GoogLeNet, ResNet)

![](media/image83.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 30 22 Feb 2016

Torch

![](media/image84.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

[[http://torch.ch]{.underline}](http://torch.ch)

![](media/image85.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 31 22 Feb 2016

> ![](media/image86.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image87.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   From NYU + IDIAP

-   Written in C and Lua

-   Used a lot a Facebook, DeepMind

![](media/image88.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 32 22 Feb 2016

![](media/image89.jpeg){width="9.027777777777779in"
height="4.944444444444445in"}

> Torch: Lua

+---------+---------+---------+---------+---------+---------+---------+
| > ●     |         |         |         |         |         |         |
| > High  |         |         |         |         |         |         |
| > level |         |         |         |         |         |         |
| > scrip |         |         |         |         |         |         |
| ting    |         |         |         |         |         |         |
| > langu |         |         |         |         |         |         |
| age,    |         |         |         |         |         |         |
| > easy  |         |         |         |         |         |         |
| > to    |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > inter |         |         |         |         |         |
|         | face    |         |         |         |         |         |
|         | > with  |         |         |         |         |         |
|         | > C     |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > ●     | > Simil |         |         |         |         |         |
|         | ar      |         |         |         |         |         |
|         | > to    |         |         |         |         |         |
|         | > Javas |         |         |         |         |         |
|         | cript:  |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     | > One   |         |         |         |         |
|         |         | > data  |         |         |         |         |
|         |         | > struc |         |         |         |         |
|         |         | ture:   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | > table |         |         |         |         |
|         |         | > == JS |         |         |         |         |
|         |         | > objec |         |         |         |         |
|         |         | t       |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     | > Proto |         |         |         |         |
|         |         | typical |         |         |         |         |
|         |         | > inher |         |         |         |         |
|         |         | itance  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | > metat |         |         |         |         |
|         |         | able    |         |         |         |         |
|         |         | > == JS |         |         |         |         |
|         |         | > proto |         |         |         |         |
|         |         | type    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     |         |         |         |         |         |
|         | > First |         |         |         |         |         |
|         | -class  |         |         |         |         |         |
|         | > funct |         |         |         |         |         |
|         | ions    |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > ●     | > Some  |         |         |         |         |         |
|         | > gotch |         |         |         |         |         |
|         | as:     |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     | > 1-ind |         |         |         |         |
|         |         | exed    |         |         |         |         |
|         |         | > =(    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     |         |         |         |         |         |
|         | > Varia |         |         |         |         |         |
|         | bles    |         |         |         |         |         |
|         | > globa |         |         |         |         |         |
|         | l       |         |         |         |         |         |
|         | > by    |         |         |         |         |         |
|         | > defau |         |         |         |         |         |
|         | lt      |         |         |         |         |         |
|         | > =(    |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         | > ○     | > Small |         | <http:/ |         |         |
|         |         | > stand |         | /tylern |         |         |
|         |         | ard     |         | eylon.c |         |         |
|         |         | > libra |         | om/a/le |         |         |
|         |         | ry      |         | arn-lua |         |         |
|         |         |         |         | />      |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| > Fei-F | > Lectu | > 22    |         |         |         |         |
| ei      | re      | > Feb   |         |         |         |         |
| > Li &  | > 12 33 | > 2016  |         |         |         |         |
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

![](media/image90.jpeg){width="9.602777777777778in"
height="0.5888888888888889in"}

> ![](media/image91.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Torch tensors are just like numpy arrays

![](media/image92.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 34 22 Feb 2016

> ![](media/image93.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Torch tensors are just like numpy arrays

![](media/image94.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 35 22 Feb 2016

> ![](media/image96.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Torch tensors are just like numpy arrays

![](media/image97.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 36 22 Feb 2016

> ![](media/image99.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Like numpy, can easily change data type:

![](media/image100.jpeg){width="10.0in" height="3.8513888888888888in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 37 22 Feb 2016

> ![](media/image101.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Unlike numpy, GPU is just a datatype away:

![](media/image102.jpeg){width="10.0in" height="3.8513888888888888in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 38 22 Feb 2016

> ![](media/image103.jpeg){width="9.074305555555556in"
> height="1.4006944444444445in"}
>
> Documentation on GitHub:

![](media/image104.jpeg){width="8.005555555555556in"
height="3.3041666666666667in"}

> [https://github.com/torch/torch7/blob/master/doc/tensor.md]{.underline}
> [~[https://github.com/torch/torch7/blob/master/doc/maths.md]{.underline}~](https://github.com/torch/torch7/blob/master/doc/maths.md)

![](media/image105.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 39 22 Feb 2016

> ![](media/image106.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

-   nn module lets you easily build and train neural nets

![](media/image107.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 40 22 Feb 2016

> ![](media/image108.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> Build a two-layer ReLU net

![](media/image109.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 41 22 Feb 2016

> ![](media/image110.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> Get weights and gradient for entire network

![](media/image111.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 42 22 Feb 2016

> ![](media/image112.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> Use a softmax loss function

![](media/image113.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 43 22 Feb 2016

> ![](media/image114.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> Generate random data
> ![](media/image115.jpeg){width="1.6305555555555555in"
> height="0.30416666666666664in"}

![](media/image117.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 44 22 Feb 2016

> ![](media/image118.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> **Forward pass**: compute scores and loss

![](media/image119.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 45 22 Feb 2016

> ![](media/image120.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> **Backward pass**: Compute
>
> gradients. Remember to set
>
> weight gradients to zero!

![](media/image121.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 46 22 Feb 2016

> ![](media/image122.jpeg){width="9.14236111111111in"
> height="4.8902777777777775in"}

n.  module lets you easily build and train neural nets

> **Update**: Make a gradient descent step

![](media/image123.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 47 22 Feb 2016

> ![](media/image124.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Running on GPU is easy:

![](media/image125.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 48 22 Feb 2016

> ![](media/image126.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Running on GPU is easy:
>
> Import a few new packages

![](media/image127.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 49 22 Feb 2016

> ![](media/image128.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Running on GPU is easy:
>
> Import a few new packages
>
> Cast network and criterion

![](media/image129.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 50 22 Feb 2016

> ![](media/image130.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Running on GPU is easy:
>
> Import a few new packages
>
> Cast network and criterion
>
> Cast data and labels

![](media/image131.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 51 22 Feb 2016

> ![](media/image132.jpeg){width="9.027777777777779in"
> height="4.971527777777778in"}
>
> optim package implements different update rules: momentum, Adam, etc

![](media/image133.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 52 22 Feb 2016

> ![](media/image134.jpeg){width="9.027777777777779in"
> height="4.971527777777778in"}
>
> optim package implements different update rules: momentum, Adam, etc
>
> Import optim package

![](media/image135.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 53 22 Feb 2016

> ![](media/image136.jpeg){width="9.027777777777779in"
> height="4.971527777777778in"}
>
> optim package implements different update rules: momentum, Adam, etc
>
> Import optim package
>
> Write a callback function that
> returns![](media/image137.jpeg){width="0.6854166666666667in"
> height="0.30694444444444446in"} loss and gradients

![](media/image138.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 54 22 Feb 2016

> ![](media/image139.jpeg){width="9.027777777777779in"
> height="4.971527777777778in"}
>
> optim package implements different update rules: momentum, Adam, etc
>
> Import optim package
>
> Write a callback function that returns loss and gradients
>
> state variable holds hyperparameters, cached values, etc; pass it to
> adam ![](media/image140.jpeg){width="0.7340277777777777in"
> height="0.30277777777777776in"}

![](media/image142.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 55 22 Feb 2016

> ![](media/image143.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image144.jpeg){width="4.5256944444444445in"
height="3.714583333333333in"}

> Caffe has Nets and Layers;
>
> Torch just has Modules

![](media/image145.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 56 22 Feb 2016

> ![](media/image146.jpeg){width="9.401388888888889in"
> height="4.802083333333333in"}
>
> Caffe has Nets and Layers; Torch just has Modules
>
> Modules are classes written in Lua; easy to read and write
>
> Forward / backward written in Lua
>
> using Tensor methods
>
> Same code runs on CPU / GPU

[[https://github.com/torch/nn/blob/master/Linear.lua]{.underline}](https://github.com/torch/nn/blob/master/Linear.lua)

![](media/image147.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 57 22 Feb 2016

> ![](media/image148.jpeg){width="9.401388888888889in"
> height="4.802083333333333in"}
>
> Caffe has Nets and Layers; Torch just has Modules
>
> Modules are classes written in Lua; easy to read and write
>
> **updateOutput**: Forward pass; compute output

[[https://github.com/torch/nn/blob/master/Linear.lua]{.underline}](https://github.com/torch/nn/blob/master/Linear.lua)

![](media/image149.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 58 22 Feb 2016

> ![](media/image150.jpeg){width="9.347222222222221in"
> height="0.9652777777777778in"}

![](media/image151.jpeg){width="9.347222222222221in" height="3.8in"}

> Caffe has Nets and Layers; Torch just has Modules
>
> Modules are classes written in Lua; easy to read and write
>
> **updateGradInput:** Backward; compute gradient of input

![](media/image152.jpeg){width="3.2944444444444443in"
height="0.3888888888888889in"}

[[https://github.com/torch/nn/blob/master/Linear.lua]{.underline}](https://github.com/torch/nn/blob/master/Linear.lua)

![](media/image153.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 59 22 Feb 2016

> ![](media/image154.jpeg){width="9.347222222222221in"
> height="0.9652777777777778in"}

![](media/image155.jpeg){width="4.5256944444444445in"
height="3.714583333333333in"}

> Caffe has Nets and Layers; Torch just has Modules

![](media/image156.jpeg){width="4.7659722222222225in"
height="1.9090277777777778in"}

> Modules are classes written in Lua; easy to read and write
>
> **accGradParameters:** Backward; compute gradient of weights

![](media/image157.jpeg){width="3.2944444444444443in"
height="0.3888888888888889in"}

[[https://github.com/torch/nn/blob/master/Linear.lua]{.underline}](https://github.com/torch/nn/blob/master/Linear.lua)

![](media/image158.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 60 22 Feb 2016

> ![](media/image159.jpeg){width="10.0in" height="5.413888888888889in"}
>
> Tons of built-in modules and loss functions
>
> [[https://github.com/torch/nn]{.underline}](https://github.com/torch/nn)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 61 22 Feb 2016

![](media/image160.jpeg){width="10.0in" height="5.625in"}

> Torch: Modules
>
> Tons of built-in modules and loss functions
>
> New ones all the time:
>
> [[https://github.com/torch/nn]{.underline}](https://github.com/torch/nn)

Added 2/19/2016

Added 2/16/2016

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 62 22 Feb 2016

> ![](media/image161.jpeg){width="9.027777777777779in"
> height="4.7756944444444445in"}
>
> Writing your own modules is easy!

![](media/image162.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 63 22 Feb 2016

> ![](media/image163.jpeg){width="9.307638888888889in"
> height="1.4027777777777777in"}
>
> *Container* modules allow you to combine multiple modules

![](media/image164.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 64 22 Feb 2016

> ![](media/image165.jpeg){width="9.572916666666666in"
> height="2.1597222222222223in"}
>
> *Container* modules allow you to combine multiple modules

![](media/image166.jpeg){width="0.9090277777777778in"
height="2.3256944444444443in"}

> x

![](media/image167.jpeg){width="5.208880139982502e-3in"
height="0.3284722222222222in"}

> mod1

![](media/image168.jpeg){width="5.208880139982502e-3in"
height="0.3284722222222222in"}

> mod2

![](media/image169.jpeg){width="5.208880139982502e-3in"
height="0.3284722222222222in"}

> out

![](media/image170.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 65 22 Feb 2016

![](media/image171.jpeg){width="9.572916666666666in"
height="2.1597222222222223in"}

> Torch: Modules
>
> *Container* modules allow you to combine multiple modules

![](media/image172.jpeg){width="2.5993055555555555in"
height="2.5840277777777776in"}

+-------------+-------------+-------------+-------------+-------------+
| x           |             | > x         |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| mod1        | > mod1      | > mod2      |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| mod2        |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| out         | > out\[1\]  | > out\[2\]  |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Fei-Fei Li  | > Lecture   |             |             |             |
| & Andrej    | > 12 66 22  |             |             |             |
| Karpathy &  | > Feb 2016  |             |             |             |
| Justin      |             |             |             |             |
| Johnson     |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image173.jpeg){width="10.0in" height="3.0868055555555554in"}

![](media/image177.jpeg){width="9.602777777777778in"
height="2.1597222222222223in"}

> Torch: Modules
>
> *Container* modules allow you to combine multiple modules

![](media/image178.jpeg){width="6.167361111111111in"
height="2.6458333333333335in"}

+-----------+-----------+-----------+-----------+-----------+-----------+
| x         |           | > x       | > x1      | x2        |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| mod1      | > mod1    | > mod2    | > mod1    | mod2      |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| mod2      |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| out       | > out\[1\ | > out\[2\ | > out\[1\ | out\[2\]  |           |
|           | ]         | ]         | ]         |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| Fei-Fei   | > Lecture | > 22 Feb  |           |           |           |
| Li &      | > 12 67   | > 2016    |           |           |           |
| Andrej    |           |           |           |           |           |
| Karpathy  |           |           |           |           |           |
| & Justin  |           |           |           |           |           |
| Johnson   |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+

![](media/image179.jpeg){width="10.0in" height="3.0868055555555554in"}

> ![](media/image187.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image188.jpeg){width="4.307638888888889in"
height="3.714583333333333in"}

> Use nngraph to build modules
>
> that combine their inputs in
>
> complex ways
>
> **Inputs**: x, y, z
>
> **Outputs**: c
>
> a = x + y
>
> b = a ☉ z
>
> c = a + b

![](media/image189.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 68 22 Feb 2016

+--------------------+----+-----+
| Torch: nngraph ^x^ | y  | > z |
+--------------------+----+-----+
|                    | \+ |     |
+--------------------+----+-----+

![](media/image190.jpeg){width="9.027777777777779in"
height="4.802083333333333in"}

> Use nngraph to build modules that combine their inputs in complex ways
>
> **Inputs**: x, y, z
>
> **Outputs**: c
>
> a = x + y
>
> b = a ☉ z
>
> c = a + b

a

![](media/image192.jpeg){width="10.0in" height="0.5888888888888889in"}

☉

![](media/image193.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

> b

![](media/image194.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

> \+

![](media/image195.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 69 22 Feb 2016

+--------------------+----+-----+
| Torch: nngraph ^x^ | y  | > z |
+--------------------+----+-----+
|                    | \+ |     |
+--------------------+----+-----+

![](media/image196.jpeg){width="9.370833333333334in"
height="4.802083333333333in"}

> Use nngraph to build modules that combine their inputs in complex ways
>
> **Inputs**: x, y, z
>
> **Outputs**: c
>
> a = x + y
>
> b = a ☉ z
>
> c = a + b

a

![](media/image198.jpeg){width="10.0in" height="0.5888888888888889in"}

☉

![](media/image199.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

b

![](media/image200.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

\+

![](media/image201.jpeg){width="5.208880139982502e-3in"
height="0.3104166666666667in"}

c

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 70 22 Feb 2016

> ![](media/image202.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image203.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **loadcaffe**: Load pretrained Caffe models: AlexNet, VGG, some others
>
> [[https://github.com/szagoruyko/loadcaffe]{.underline}](https://github.com/szagoruyko/loadcaffe)
>
> **GoogLeNet v1**:
> [[https://github.com/soumith/inception.torch]{.underline}](https://github.com/soumith/inception.torch)
>
> **GoogLeNet v3**:
> [[https://github.com/Moodstocks/inception-v3.torch]{.underline}](https://github.com/Moodstocks/inception-v3.torch)
>
> **ResNet**:
> [[https://github.com/facebook/fb.resnet.torch]{.underline}](https://github.com/facebook/fb.resnet.torch)

![](media/image204.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 71 22 Feb 2016

> ![](media/image205.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image206.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> After installing torch, use luarocks to install or update Lua packages
>
> (Similar to pip install from Python)

![](media/image207.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 72 22 Feb 2016

[[https://github.com/twitter/torch-autograd]{.underline}](https://github.com/twitter/torch-autograd)

[<https://github.com/hughperkins/cltorch>,
<https://github.com/hughperkins/clnn>]{.underline}

[[https://luarocks.org/modules/luarocks/lua-cjson]{.underline}](https://luarocks.org/modules/luarocks/lua-cjson)

[[https://github.com/deepmind/torch-hdf5]{.underline}](https://github.com/deepmind/torch-hdf5)

> ![](media/image208.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image209.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   **torch.cudnn**: Bindings for NVIDIA cuDNN kernels

> [[https://github.com/soumith/cudnn.torch]{.underline}](https://github.com/soumith/cudnn.torch)

-   **torch-hdf5**: Read and write HDF5 files from Torch

<!-- -->

-   **lua-cjson**: Read and write JSON files from Lua

<!-- -->

-   **cltorch, clnn**: OpenCL backend for Torch, and port of nn

<!-- -->

-   **torch-autograd**: Automatic differentiation; sort of like more
    > powerful

> nngraph, similar to Theano or TensorFlow

-   **fbcunn**: Facebook: FFT conv, multi-GPU (DataParallel,
    > ModelParallel)

> [[https://github.com/facebook/fbcunn]{.underline}](https://github.com/facebook/fbcunn)

![](media/image210.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 73 22 Feb 2016

> ![](media/image211.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image212.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Step 1**: Preprocess data; usually use a Python script to dump data
> to HDF5
>
> **Step 2**: Train a model in Lua / Torch; read from HDF5 datafile,
> save trained model to disk
>
> **Step 3:** Use trained model for something, often with an evaluation
> script

![](media/image213.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 74 22 Feb 2016

([[https://github.com/jcjohnson/torch-rnn/blob/master/sample.lua]{.underline}](https://github.com/jcjohnson/torch-rnn/blob/master/sample.lua))

([[https://github.com/jcjohnson/torch-rnn/blob/master/train.]{.underline}](https://github.com/jcjohnson/torch-rnn/blob/master/train.lua)

([[https://github.com/jcjohnson/torch-rnn/blob/master/scripts/preprocess.py]{.underline}](https://github.com/jcjohnson/torch-rnn/blob/master/scripts/preprocess.py))

![](media/image214.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> Torch: Typical Workflow

![](media/image215.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Example:**
> [[https://github.com/jcjohnson/torch-rnn]{.underline}](https://github.com/jcjohnson/torch-rnn)
>
> **Step 1**: Preprocess data; usually use a Python script to dump data
> to HDF5
>
> **Step 2**: Train a model in Lua / Torch; read from HDF5 datafile,
> save trained model to disk
>
> [[lua]{.underline}](https://github.com/jcjohnson/torch-rnn/blob/master/train.lua)
> )
>
> **Step 3:** Use trained model for something, often with an evaluation
> script

![](media/image216.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 75 22 Feb 2016

> ![](media/image217.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image218.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   (-) Lua

-   (-) Less plug-and-play than Caffe

    -   You usually write your own training code

-   (+) Lots of modular pieces that are easy to combine

-   (+) Easy to write your own layer types and run on GPU

-   (+) Most of the library code is in Lua, easy to read

-   (+) Lots of pretrained models!

-   (-) Not great for RNNs

![](media/image219.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 76 22 Feb 2016

Theano

![](media/image220.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

[[http://deeplearning.net/software/theano/]{.underline}](http://deeplearning.net/software/theano/)

![](media/image221.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 77 22 Feb 2016

> ![](media/image222.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image223.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> From Yoshua Bengio's group at University of Montreal
>
> Embracing computation graphs, symbolic computation
>
> High-level wrappers: Keras, Lasagne

![](media/image224.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 78 22 Feb 2016

> ![](media/image225.jpeg){width="9.395138888888889in"
> height="4.717361111111111in"}
>
> x y z
>
> \+

![](media/image226.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image227.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image228.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image229.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

![](media/image230.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 79 22 Feb 2016

> ![](media/image231.jpeg){width="10.0in" height="5.413888888888889in"}
>
> x y z
>
> \+

![](media/image232.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image233.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image234.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image235.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 80 22 Feb 2016

> ![](media/image236.jpeg){width="10.0in" height="5.413888888888889in"}

+---+------+-----+------------------------------+--+
| x | > y  | > z | > Define symbolic variables; |  |
+---+------+-----+------------------------------+--+
|   | > \+ |     | > these are inputs to the    |  |
+---+------+-----+------------------------------+--+
|   |      |     | > graph                      |  |
+---+------+-----+------------------------------+--+
|   |      |     |                              |  |
+---+------+-----+------------------------------+--+
|   | > a  |     |                              |  |
+---+------+-----+------------------------------+--+

![](media/image237.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> ☉

![](media/image238.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image239.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image240.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 81 22 Feb 2016

> ![](media/image241.jpeg){width="10.0in" height="5.413888888888889in"}
>
> x y z
>
> \+

![](media/image242.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image243.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image244.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image245.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> Compute intermediates and outputs symbolically

Lecture 12 82 22 Feb 2016

> ![](media/image246.jpeg){width="10.0in" height="5.413888888888889in"}
>
> x y z
>
> \+

![](media/image247.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image248.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image249.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image250.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> Compile a function that produces c from x, y, z (generates code)

Lecture 12 83 22 Feb 2016

> ![](media/image251.jpeg){width="10.0in" height="5.413888888888889in"}
>
> x y z
>
> \+

![](media/image252.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image253.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image254.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image255.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> Run the function, passing some numpy arrays (may run on GPU)

Lecture 12 84 22 Feb 2016

> ![](media/image256.jpeg){width="10.0in" height="5.413888888888889in"}
>
> x y z
>
> \+

![](media/image257.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> a
>
> ☉

![](media/image258.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> b

![](media/image259.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> \+

![](media/image260.jpeg){width="5.208880139982502e-3in"
height="0.28680555555555554in"}

> c

Fei-Fei Li & Andrej Karpathy & Justin Johnson

> Repeat the same computation using numpy operations (runs on CPU)

Lecture 12 85 22 Feb 2016

> ![](media/image261.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}

![](media/image262.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 86 22 Feb 2016

> ![](media/image263.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Define symbolic variables:
>
> x = data
>
> y = labels
>
> w1 = first-layer weights
>
> w2 = second-layer weights

![](media/image264.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 87 22 Feb 2016

> ![](media/image265.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> **Forward**: Compute scores (symbolically)

![](media/image266.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 88 22 Feb 2016

> ![](media/image267.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> **Forward**: Compute probs, loss (symbolically)

![](media/image268.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 89 22 Feb 2016

> ![](media/image269.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Compile a function that
>
> computes loss, scores

![](media/image270.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 90 22 Feb 2016

> ![](media/image271.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Stuff actual numpy arrays into the function

![](media/image272.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 91 22 Feb 2016

> ![](media/image273.jpeg){width="9.250694444444445in"
> height="4.5152777777777775in"}

![](media/image274.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 92 22 Feb 2016

> ![](media/image275.jpeg){width="9.322916666666666in"
> height="4.5680555555555555in"}
>
> Same as before: define variables, compute scores and loss symbolically

![](media/image276.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 93 22 Feb 2016

> ![](media/image277.jpeg){width="9.322916666666666in"
> height="4.5680555555555555in"}
>
> Theano computes gradients for
> ![](media/image278.jpeg){width="0.2048611111111111in"
> height="0.4375in"} us symbolically!

![](media/image279.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 94 22 Feb 2016

> ![](media/image280.jpeg){width="9.322916666666666in"
> height="4.5680555555555555in"}
>
> Now the function returns loss, scores, and gradients

![](media/image281.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 95 22 Feb 2016

> ![](media/image282.jpeg){width="9.677777777777777in"
> height="4.5680555555555555in"}
>
> Use the function to perform gradient descent!

![](media/image283.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 96 22 Feb 2016

> ![](media/image284.jpeg){width="9.660416666666666in"
> height="4.5680555555555555in"}
>
> **Problem**: Shipping weights and gradients to CPU on every iteration
> to update\...

![](media/image285.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 97 22 Feb 2016

> ![](media/image286.jpeg){width="9.709722222222222in"
> height="4.6722222222222225in"}
>
> Same as before: Define dimensions,
> ![](media/image287.jpeg){width="1.8333333333333333in"
> height="0.22847222222222222in"} define symbolic variables for x, y

![](media/image288.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 98 22 Feb 2016

> ![](media/image289.jpeg){width="9.709722222222222in"
> height="4.6722222222222225in"}
>
> Define weights as **shared variables** that persist in the graph
> between calls; initialize with numpy arrays

![](media/image290.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 99 22 Feb 2016

> ![](media/image291.jpeg){width="9.709722222222222in"
> height="4.6722222222222225in"}
>
> ![](media/image292.jpeg){width="0.33402777777777776in"
> height="0.5729166666666666in"}Same as before: Compute scores, loss,
> gradients symbolically

![](media/image293.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 100 22 Feb 2016

> ![](media/image294.jpeg){width="9.709722222222222in"
> height="4.673611111111111in"}
>
> Compiled function inputs are x and y; weights live in the graph

![](media/image295.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 101 22 Feb 2016

> ![](media/image296.jpeg){width="9.709722222222222in"
> height="4.673611111111111in"}
>
> Function includes an **update** that updates weights on every call

![](media/image297.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 102 22 Feb 2016

> ![](media/image298.jpeg){width="9.707638888888889in"
> height="4.6722222222222225in"}
>
> To train the net, just call function repeatedly!

![](media/image299.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 103 22 Feb 2016

> ![](media/image300.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image301.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Conditionals**: The **ifelse** and **switch** functions allow
> conditional control flow in the graph
>
> **Loops**: The **scan** function allows for (some types) of loops in
> the computational graph; good for RNNs
>
> **Derivatives**: Efficient Jacobian / vector products with R and L
> operators, symbolic hessians (gradient of gradient)
>
> **Sparse matrices, optimizations, etc**

![](media/image302.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 104 22 Feb 2016

> ![](media/image303.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image304.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Experimental model parallelism:
>
> [[http://deeplearning.net/software/theano/tutorial/using\_multi\_gpu.html]{.underline}](http://deeplearning.net/software/theano/tutorial/using_multi_gpu.html)
>
> Data parallelism using platoon:
>
> [[https://github.com/mila-udem/platoon]{.underline}](https://github.com/mila-udem/platoon)

![](media/image305.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 105 22 Feb 2016

> ![](media/image306.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> Lasagne gives layer abstractions, sets up weights for you, writes
> update rules for you

![](media/image307.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 106 22 Feb 2016

> ![](media/image308.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> Set up symbolic Theano variables for data, labels
> ![](media/image309.jpeg){width="1.5722222222222222in"
> height="0.3229166666666667in"}

![](media/image310.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 107 22 Feb 2016

> ![](media/image311.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> **Forward**: Use Lasagne layers to set up layers; don't set up weights
> explicitly ![](media/image312.jpeg){width="1.5722222222222222in"
> height="0.3229166666666667in"}

![](media/image313.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 108 22 Feb 2016

> ![](media/image314.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> **Forward**: Use Lasagne layers to compute loss
> ![](media/image315.jpeg){width="1.5722222222222222in"
> height="0.3229166666666667in"}

![](media/image316.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 109 22 Feb 2016

> ![](media/image317.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> Lasagne gets parameters, and
>
> writes the update rule for you
> ![](media/image318.jpeg){width="0.9194444444444444in"
> height="0.6166666666666667in"}

![](media/image319.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 110 22 Feb 2016

> ![](media/image320.jpeg){width="9.192361111111111in"
> height="4.802083333333333in"}
>
> Same as Theano: compile a function with updates, train model by
> calling function with arrays

![](media/image321.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 111 22 Feb 2016

> ![](media/image322.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image323.jpeg){width="4.5159722222222225in"
height="3.714583333333333in"}

> keras is a layer on top of Theano; makes common things easy to do

![](media/image324.jpeg){width="4.440972222222222in"
height="2.9194444444444443in"}

> (Also supports TensorFlow backend)

![](media/image325.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 112 22 Feb 2016

> ![](media/image326.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image327.jpeg){width="9.120138888888889in"
height="3.714583333333333in"}

> keras is a layer on top of Theano; makes common things easy to do
>
> Set up a two-layer ReLU net with softmax

![](media/image328.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 113 22 Feb 2016

> ![](media/image329.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image330.jpeg){width="9.121527777777779in"
height="3.714583333333333in"}

> keras is a layer on top of Theano; makes common things easy to do
>
> We will optimize the model using SGD with Nesterov momentum
> ![](media/image331.jpeg){width="0.4666666666666667in"
> height="0.12916666666666668in"}

![](media/image332.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 114 22 Feb 2016

> ![](media/image333.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image334.jpeg){width="4.5159722222222225in"
height="3.714583333333333in"}

> keras is a layer on top of Theano; makes common things easy to do

![](media/image335.jpeg){width="4.444444444444445in"
height="2.9208333333333334in"}

> Generate some random data and
>
> train the model

![](media/image336.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 115 22 Feb 2016

> ![](media/image337.jpeg){width="9.027777777777779in"
> height="4.753472222222222in"}
>
> **Problem**: It crashes, stack trace and error message not useful :(

![](media/image338.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 116 22 Feb 2016

> ![](media/image339.jpeg){width="9.289583333333333in"
> height="4.716666666666667in"}
>
> **Solution**: y should be one-hot
>
> (too much API for me ... )

![](media/image340.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 117 22 Feb 2016

[[https://github.com/kitofans/caffe-theano-conversion]{.underline}](https://github.com/kitofans/caffe-theano-conversion)

[[http://sklearn-theano.github.io]{.underline}](http://sklearn-theano.github.io)

![](media/image341.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

> Theano: Pretrained Models

![](media/image342.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> **Lasagne Model Zoo** has pretrained common architectures:
>
> [[https://github.com/Lasagne/Recipes/tree/master/modelzoo]{.underline}](https://github.com/Lasagne/Recipes/tree/master/modelzoo)
>
> **AlexNet with weights**:
> [[https://github.com/uoguelph-mlrg/theano\_alexnet]{.underline}](https://github.com/uoguelph-mlrg/theano_alexnet)
>
> **sklearn-theano**: Run OverFeat and GoogLeNet forward, but no
> fine-tuning?
>
> **caffe-theano-conversion**: CS 231n project from last year: load
> models and weights from caffe! Not sure if full-featured

![](media/image343.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 118 22 Feb 2016

[[https://github.com/kitofans/caffe-theano-conversion]{.underline}](https://github.com/kitofans/caffe-theano-conversion)

[[http://sklearn-theano.github.io]{.underline}](http://sklearn-theano.github.io)

![](media/image344.jpeg){width="9.429166666666667in"
height="4.802083333333333in"}

+--+---------------------------+---------------+--+--+--+
|  | Theano: Pretrained Models | > Best choice |  |  |  |
+--+---------------------------+---------------+--+--+--+
|  |                           |               |  |  |  |
+--+---------------------------+---------------+--+--+--+
|  |                           |               |  |  |  |
+--+---------------------------+---------------+--+--+--+
|  |                           |               |  |  |  |
+--+---------------------------+---------------+--+--+--+
|  |                           |               |  |  |  |
+--+---------------------------+---------------+--+--+--+

> **AlexNet with weights**:
> [[https://github.com/uoguelph-mlrg/theano\_alexnet]{.underline}](https://github.com/uoguelph-mlrg/theano_alexnet)
>
> **sklearn-theano**: Run OverFeat and GoogLeNet forward, but no
> fine-tuning?
>
> **caffe-theano-conversion**: CS 231n project from last year: load
> models and weights from caffe! Not sure if full-featured

![](media/image345.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 119 22 Feb 2016

> ![](media/image346.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image347.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   (+) Python + numpy

-   (+) Computational graph is nice abstraction

-   (+) RNNs fit nicely in computational graph

-   (-) Raw Theano is somewhat low-level

-   (+) High level wrappers (Keras, Lasagne) ease the pain

-   (-) Error messages can be unhelpful

-   (-) Large models can have long compile times

-   (-) Much "fatter" than Torch; more magic

-   (-) Patchy support for pretrained models

![](media/image348.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 120 22 Feb 2016

TensorFlow

![](media/image349.jpeg){width="9.027777777777779in"
height="0.9652777777777778in"}

[[https://www.tensorflow.org]{.underline}](https://www.tensorflow.org)

![](media/image350.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 121 22 Feb 2016

> ![](media/image351.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image352.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> From Google
>
> Very similar to Theano - all about computation graphs
>
> Easy visualizations (TensorBoard)
>
> Multi-GPU and multi-node training

![](media/image353.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 122 22 Feb 2016

> ![](media/image354.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}

![](media/image355.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 123 22 Feb 2016

> ![](media/image356.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}
>
> Create placeholders for data and labels: These will be fed to the
> graph

![](media/image357.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 124 22 Feb 2016

> ![](media/image358.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}
>
> Create Variables to hold
>
> weights; similar to Theano
>
> shared variables
>
> Initialize variables with numpy arrays

![](media/image359.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 125 22 Feb 2016

> ![](media/image360.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}
>
> **Forward**: Compute scores, probs, loss (symbolically)

![](media/image361.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 126 22 Feb 2016

> ![](media/image362.jpeg){width="9.11875in"
> height="4.802083333333333in"}
>
> Running train\_step will use SGD to minimize loss

![](media/image363.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 127 22 Feb 2016

> ![](media/image364.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}
>
> Create an artificial dataset; y is one-hot like Keras

![](media/image365.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 128 22 Feb 2016

> ![](media/image366.jpeg){width="9.116666666666667in"
> height="4.802083333333333in"}
>
> Actually train the model

![](media/image367.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 129 22 Feb 2016

> ![](media/image368.jpeg){width="9.178472222222222in"
> height="4.802083333333333in"}
>
> Tensorboard makes it easy to visualize what's happening inside your
> models

![](media/image369.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 130 22 Feb 2016

> ![](media/image370.jpeg){width="9.178472222222222in"
> height="4.802083333333333in"}
>
> Tensorboard makes it easy to visualize what's happening inside your
> models
>
> Same as before, but now we
> ![](media/image371.jpeg){width="1.4145833333333333in"
> height="0.22847222222222222in"} create summaries for loss and
>
> weights

![](media/image374.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 131 22 Feb 2016

> ![](media/image375.jpeg){width="9.178472222222222in"
> height="4.802083333333333in"}
>
> Tensorboard makes it easy to visualize what's happening inside your
> models
>
> Create a special "merged" variable and a SummaryWriter object

![](media/image376.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 132 22 Feb 2016

> ![](media/image377.jpeg){width="9.178472222222222in"
> height="4.802083333333333in"}
>
> Tensorboard makes it easy to visualize what's happening inside your
> models
>
> In the training loop, also run merged and pass its value to the writer

![](media/image378.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 133 22 Feb 2016

> ![](media/image379.jpeg){width="9.027777777777779in"
> height="4.802083333333333in"}
>
> Start Tensorboard server, and we get graphs!

![](media/image380.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 134 22 Feb 2016

> ![](media/image381.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image382.jpeg){width="10.0in" height="4.326388888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 135 22 Feb 2016

> ![](media/image383.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image384.jpeg){width="4.335416666666666in"
height="3.714583333333333in"}

> Add names to placeholders and

![](media/image385.jpeg){width="4.541666666666667in"
height="3.3743055555555554in"}

> variables

![](media/image386.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 136 22 Feb 2016

> ![](media/image387.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image388.jpeg){width="4.335416666666666in"
height="3.714583333333333in"}

> Add names to placeholders and variables

![](media/image389.jpeg){width="4.541666666666667in"
height="3.3743055555555554in"}

> Break up the forward pass with name scoping
> ![](media/image390.jpeg){width="2.509027777777778in"
> height="0.27291666666666664in"}

![](media/image391.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 137 22 Feb 2016

> ![](media/image392.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image393.jpeg){width="8.608333333333333in"
height="3.714583333333333in"}

> Tensorboard shows the graph!

![](media/image394.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 138 22 Feb 2016

> ![](media/image395.jpeg){width="9.449305555555556in"
> height="4.802083333333333in"}
>
> Tensorboard shows the graph!
>
> Name scopes expand to show individual operations

![](media/image396.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 139 22 Feb 2016

> ![](media/image397.jpeg){width="10.0in" height="5.413888888888889in"}
>
> **Data parallelism**:
>
> synchronous or asynchronous

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 140 22 Feb 2016

+-----------------------------+---------------------------+--+
| TensorFlow: Multi-GPU       |                           |  |
+-----------------------------+---------------------------+--+
| **Data parallelism**:       | > **Model parallelism**:  |  |
+-----------------------------+---------------------------+--+
| synchronous or asynchronous |                           |  |
+-----------------------------+---------------------------+--+
|                             | > Split model across GPUs |  |
+-----------------------------+---------------------------+--+
|                             |                           |  |
+-----------------------------+---------------------------+--+

![](media/image398.jpeg){width="10.0in" height="5.413888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 141 22 Feb 2016

> ![](media/image399.jpeg){width="9.027777777777779in"
> height="4.665972222222222in"}
>
> **Single machine**: **Many machines**:
>
> Like other frameworks Not open source (yet) =(

![](media/image400.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 142 22 Feb 2016

> ![](media/image401.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image402.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> You can get a pretrained version of Inception here:
>
> [[https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/android/README.md]{.underline}](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/android/README.md)
>
> (In an Android example?? Very well-hidden)
>
> The only one I could find =(

![](media/image403.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 143 22 Feb 2016

> ![](media/image404.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image405.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

-   (+) Python + numpy

-   (+) Computational graph abstraction, like Theano; great for RNNs

-   (+) Much faster compile times than Theano

-   (+) Slightly more convenient than raw Theano?

-   (+) TensorBoard for visualization

-   (+) Data AND model parallelism; best of all frameworks

-   (+/-) Distributed models, but not open-source yet

-   (-) Slower than other frameworks right now

-   (-) Much "fatter" than Torch; more magic

-   (-) Not many pretrained models

![](media/image406.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 144 22 Feb 2016

> ![](media/image407.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

+-------------+-------------+-------------+-------------+-------------+
|             | > **Caffe** | > **Torch** | > **Theano* | > **TensorF |
|             |             |             | *           | low**       |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Languag | > C++,      | > Lua       | > Python    | > Python    |
| e**         | > Python    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Pretrai | > Yes ++    | > Yes ++    | > Yes       | > Inception |
| ned**       |             |             | > (Lasagne) |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Multi-G | > Yes       | > Yes cunn. | > Yes       | > Yes       |
| PU:**       |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Data    |             | > DataParal | > platoon   |             |
| > parallel* |             | lelTable    |             |             |
| *           |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Multi-G | > No        | > Yes       | > Experimen | > Yes       |
| PU:**       |             |             | tal         | > (best)    |
+-------------+-------------+-------------+-------------+-------------+
| > **Model   |             | > fbcunn.Mo |             |             |
| > parallel* |             | delParallel |             |             |
| *           |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Readabl | > Yes (C++) | > Yes (Lua) | > No        | > No        |
| e**         |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **source  |             |             |             |             |
| > code**    |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| > **Good at | > No        | > Mediocre  | > Yes       | > Yes       |
| > RNN**     |             |             |             | > (best)    |
+-------------+-------------+-------------+-------------+-------------+
|             |             |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

![](media/image408.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 145 22 Feb 2016

> ![](media/image409.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image410.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Extract AlexNet or VGG features?

![](media/image411.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 146 22 Feb 2016

> ![](media/image412.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image413.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Extract AlexNet or VGG features? **Use Caffe**

![](media/image414.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 147 22 Feb 2016

> ![](media/image415.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image416.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Fine-tune AlexNet for new classes?

![](media/image417.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 148 22 Feb 2016

> ![](media/image418.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image419.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Fine-tune AlexNet for new classes? **Use Caffe**

![](media/image420.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 149 22 Feb 2016

> ![](media/image421.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image422.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Image Captioning with finetuning?

![](media/image423.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 150 22 Feb 2016

> ![](media/image424.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image425.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Image Captioning with finetuning?
>
> -\> Need pretrained models (Caffe, Torch, Lasagne)
>
> -\> Need RNNs (Torch or Lasagne)
>
> -\> **Use Torch or Lasagna**

![](media/image426.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 151 22 Feb 2016

> ![](media/image427.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image428.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Segmentation? (Classify every pixel)

![](media/image429.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 152 22 Feb 2016

> ![](media/image430.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image431.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Segmentation? (Classify every pixel)
>
> -\> Need pretrained model (Caffe, Torch, Lasagna)
>
> -\> Need funny loss function
>
> -\> If loss function exists in Caffe: **Use Caffe**
>
> -\> If you want to write your own loss: **Use Torch**

![](media/image432.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 153 22 Feb 2016

> ![](media/image433.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image434.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Object Detection?

![](media/image435.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 154 22 Feb 2016

> ![](media/image436.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image437.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Object Detection?
>
> -\> Need pretrained model (Torch, Caffe, Lasagne)
>
> -\> Need lots of custom imperative code (NOT Lasagne) -\> Use **Caffe
> + Python** or **Torch**

![](media/image438.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 155 22 Feb 2016

> ![](media/image439.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image440.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Language modeling with new RNN structure?

![](media/image441.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 156 22 Feb 2016

> ![](media/image442.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image443.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Language modeling with new RNN structure?
>
> -\> Need easy recurrent nets (NOT Caffe, Torch)
>
> -\> No need for pretrained models
>
> -\> **Use Theano or TensorFlow**

![](media/image444.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 157 22 Feb 2016

> ![](media/image445.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image446.jpeg){width="9.20486111111111in"
height="3.714583333333333in"}

> Implement BatchNorm?
>
> -\> Don't want to derive gradient? **Theano** or **TensorFlow** -\>
> Implement efficient backward pass? **Use Torch**

![](media/image447.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 158 22 Feb 2016

> ![](media/image448.jpeg){width="9.027777777777779in"
> height="0.9652777777777778in"}

![](media/image449.jpeg){width="9.027777777777779in"
height="3.714583333333333in"}

> Feature extraction / finetuning existing models: Use Caffe
>
> Complex uses of pretrained models: Use Lasagne or Torch
>
> Write your own layers: Use Torch
>
> Crazy RNNs: Use Theano or Tensorflow
>
> Huge model, need model parallelism: Use TensorFlow

![](media/image450.jpeg){width="10.0in" height="0.5888888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 159 22 Feb 2016

![](media/image451.jpeg){width="10.0in" height="5.413888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 160 22 Feb 2016

![](media/image452.jpeg){width="10.0in" height="5.413888888888889in"}

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 161 22 Feb 2016

> ![](media/image453.jpeg){width="9.295833333333333in"
> height="1.6777777777777778in"}

![](media/image454.jpeg){width="10.0in" height="3.765972222222222in"}

> [[https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 162 22 Feb 2016

> ![](media/image455.jpeg){width="10.0in" height="5.580555555555556in"}
>
> ● N-dimensional array for
>
> storing activations and
>
> weights

[[https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 163 22 Feb 2016

> ![](media/image456.jpeg){width="10.0in" height="5.604166666666667in"}

-   N-dimensional array for storing activations and weights

-   Template over datatype

[[https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 164 22 Feb 2016

> ![](media/image457.jpeg){width="10.0in" height="5.580555555555556in"}

-   N-dimensional array for storing activations and weights

-   Template over datatype

-   Two parallel tensors:

    -   **data**: values

    -   **diffs**: gradients

[[https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 165 22 Feb 2016

> ![](media/image458.jpeg){width="10.0in" height="5.580555555555556in"}

-   N-dimensional array for storing activations and weights

-   Template over datatype

-   Two parallel tensors:

    -   **data**: values

    -   **diffs**: gradients

-   Stores CPU / GPU versions of each tensor

[[https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/blob.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 166 22 Feb 2016

> ![](media/image459.jpeg){width="10.0in" height="5.413888888888889in"}

-   A small unit of computation

> [[https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 167 22 Feb 2016

> ![](media/image460.jpeg){width="10.0in" height="5.413888888888889in"}

-   A small unit of computation

> ● **Forward**: Use "bottom" data to compute "top" data
>
> [[https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 168 22 Feb 2016

> ![](media/image461.jpeg){width="10.0in" height="5.413888888888889in"}

-   A small unit of computation

-   **Forward**: Use "bottom" data to compute "top" data

-   **Backward**: Use "top"

> diffs to compute
>
> "bottom" diffs
>
> [[https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 169 22 Feb 2016

> ![](media/image462.jpeg){width="10.0in" height="5.413888888888889in"}
>
> ● A small unit of computation

-   **Forward**: Use "bottom" data to compute "top" data

> **● Backward**: Use "top" diffs to compute "bottom" diffs

-   Separate **CPU** / **GPU** implementations

> [[https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/layer.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 170 22 Feb 2016

> ![](media/image463.jpeg){width="10.0in" height="5.545138888888889in"}
>
> ● Tons of different layer types:

\...

[[https://github.com/BVLC/caffe/tree/master/src/caffe/layers]{.underline}](https://github.com/BVLC/caffe/tree/master/src/caffe/layers)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 171 22 Feb 2016

> ![](media/image464.jpeg){width="10.0in" height="5.545138888888889in"}

-   Tons of different layer types:

    -   **batch norm**

    -   **convolution**

    -   **cuDNN convolution**

> \...

-   **.cpp:** CPU implementation

-   **.cu**: GPU implementation

[[https://github.com/BVLC/caffe/tree/master/src/caffe/layers]{.underline}](https://github.com/BVLC/caffe/tree/master/src/caffe/layers)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 172 22 Feb 2016

> ![](media/image465.jpeg){width="9.330555555555556in"
> height="1.1569444444444446in"}

![](media/image466.jpeg){width="10.0in" height="4.326388888888889in"}

-   Collects layers into a DAG

-   Run all or part of the net **forward** and **backward**

> [[https://github.com/BVLC/caffe/blob/master/include/caffe/net.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/net.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 173 22 Feb 2016

> ![](media/image467.jpeg){width="10.0in" height="5.483333333333333in"}
>
> [[https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 174 22 Feb 2016

> ![](media/image468.jpeg){width="10.0in" height="5.483333333333333in"}
>
> ● Trains a Net by running it forward / backward, updating weights

[[https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 175 22 Feb 2016

> ![](media/image469.jpeg){width="10.0in" height="5.483333333333333in"}

-   Trains a Net by running it forward / backward, updating weights

-   Handles snapshotting,
    > ![](media/image470.jpeg){width="0.6326388888888889in"
    > height="0.27361111111111114in"} restoring from snapshots

[[https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/solver.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 176 22 Feb 2016

> ![](media/image471.jpeg){width="10.0in" height="5.483333333333333in"}

-   Trains a Net by running it forward / backward, updating weights

-   Handles snapshotting,

> restoring from snapshots

-   Subclasses implement different update rules
    > ![](media/image472.jpeg){width="0.6131944444444445in"
    > height="0.22361111111111112in"}

[[https://github.com/BVLC/caffe/blob/master/include/caffe/sgd\_solvers.hpp]{.underline}](https://github.com/BVLC/caffe/blob/master/include/caffe/sgd_solvers.hpp)

Fei-Fei Li & Andrej Karpathy & Justin Johnson Lecture 12 177 22 Feb 2016
