# Neural networks

## Notes

* Neural Networks are great identifying patterns in data. As a classic example, if you wanted to predict housing prices, you could build a data set that maps features about houses \(square feet, location, proximity to Caltrain, etc\) onto their actual price, and then train a network to recognize the complex relationship between features and pricing. Training happens by feeding the network features, letting it make a guess about the price, and then correcting the guess \(backpropagation\).
  * Convolutional Neural Networks work similarly, but with images. Instead of giving a CNN discrete features, you'll usually just use the pixels of the image itself. Through a series of layers, the CNN is able to build features itself \(traditionally things like edges, corners\) and learn patterns in image data. For example, a CNN might be trained on a dataset that maps images onto labels, and learn how to label new images on its own.

## Links

* [But what is a Neural Network? \| Deep learning, chapter 1 \(2017\)](https://www.youtube.com/watch?v=aircAruvnKk)
* [A Neural Network Playground](https://playground.tensorflow.org)
* \[A Beginner's Guide To Understanding Convolutional Neural Networks\]\([https://adeshpande3.github.io/adeshpande3.github.io/A-Beginner's-Guide-To-Understanding-Convolutional-Neural-Networks/](https://adeshpande3.github.io/adeshpande3.github.io/A-Beginner's-Guide-To-Understanding-Convolutional-Neural-Networks/)\)
* [Capsule Networks \(CapsNets\) – Tutorial](https://www.youtube.com/watch?v=pPN8d0E3900)
* [Chris Olah explains neural nets](https://www.youtube.com/watch?v=vdqu6fvjc5c)
* [How I Shipped a Neural Network on iOS with CoreML, PyTorch, and React Native](https://attardi.org/pytorch-and-coreml) - Detailed and awesome article.
* [Generative Adversarial Networks \(GANs\) in 50 lines of code \(PyTorch\)](https://medium.com/@devnag/generative-adversarial-networks-gans-in-50-lines-of-code-pytorch-e81b79659e3f)
* [Neural Networks, Types, and Functional Programming](http://colah.github.io/posts/2015-09-NN-Types-FP/)
* [Recurrent Neural Networks lecture by Yoshua Bengio](http://videolectures.net/deeplearning2016_bengio_neural_networks/)
* [Practical Advice for Building Deep Neural Networks](https://pcc.cs.byu.edu/2017/10/02/practical-advice-for-building-deep-neural-networks/)
* [Differentiable Architecture Search](https://github.com/quark0/darts) - Code for [DARTS: Differentiable Architecture Search](https://arxiv.org/abs/1806.09055) paper.
* [TensorSpace.js](https://github.com/tensorspace-team/tensorspace) - Neural network 3D visualization framework, build interactive and intuitive model in browsers, support pre-trained deep learning models from TensorFlow, Keras, TensorFlow.js
* [UIS-RNN](https://github.com/google/uis-rnn) - Library for the Unbounded Interleaved-State Recurrent Neural Network \(UIS-RNN\) algorithm, corresponding to the paper Fully Supervised Speaker Diarization.
* [ONNX](https://github.com/onnx/onnx) - Open Neural Network Exchange. \([Scoring ONNX ML Models with Scala](https://www.youtube.com/watch?v=HyYpMJNVoVk)\)
* [DyNet](https://github.com/clab/dynet) - Dynamic Neural Network Toolkit.
* [gonn](https://github.com/sausheong/gonn) - Building a simple neural network in Go.
* [Neural Ordinary Differential Equations \(2018\)](https://arxiv.org/abs/1806.07366) - [Video explanation](https://www.youtube.com/watch?v=AD3K8j12EIE) \| [Notes](https://github.com/llSourcell/Neural_Differential_Equations/blob/master/Neural_Ordinary_Differential_Equations.ipynb)
* [MindsDB](https://github.com/mindsdb/mindsdb) - Framework to streamline use of neural networks.
* [Neural Network framework in 25 LOC](https://gist.github.com/macournoyer/620a8ba4a2ecd6d6feaf)
* [Learning and Processing over Networks \(2019\)](https://github.com/rodrigo-pena/amld2019-graph-workshop) - Workshop presented by Michaël Defferrard and Rodrigo Pena at the Applied Machine Learning Days in January 2019.
* [The Next Generation of Neural Networks by Geoffrey Hinton \(2007\)](https://www.youtube.com/watch?v=AyzOUbkUf3M)
* [Who Invented Backpropagation? \(2014\)](http://people.idsia.ch/~juergen/who-invented-backpropagation.html)
* [Deep Learning in Neural Networks: An Overview \(2015\)](http://people.idsia.ch/~juergen/deep-learning-overview.html)
* [Neural Networks \(E01: introduction\) \(2018\)](https://www.youtube.com/watch?v=bVQUSndDllU) - This series is intended as a light introduction to neural networks, with a focus on the task of classifying handwritten digits.
* [Machine Learning for Beginners: An Introduction to Neural Networks \(2019\)](https://victorzhou.com/blog/intro-to-neural-networks/)
* [A Recipe for Training Neural Networks \(2019\)](https://karpathy.github.io/2019/04/25/recipe/)
* [Exploring Neural Networks with Activation Atlases \(2019\)](https://distill.pub/2019/activation-atlas/)
* [Curated list of neural architecture search and related resources](https://github.com/D-X-Y/Awesome-NAS)
* [Weight Agnostic Neural Networks \(2019\)](https://weightagnostic.github.io/) \([HN](https://news.ycombinator.com/item?id=20160693)\)
* [Geoffrey Hinton explains the evolution of neural networks \(2019\)](https://www.wired.com/story/ai-pioneer-explains-evolution-neural-networks/)
* [Evolved Turing neural networks](http://compucology.net/evolved)
* [Intelligent Machinery paper by Alan Turing](https://weightagnostic.github.io/papers/turing1948.pdf)
* [SRU](https://github.com/taolei87/sru) - Training RNNs as Fast as CNNs.
* [ODIN](https://github.com/facebookresearch/odin) - Out-of-Distribution Detector for Neural Networks.
* [Ask HN: What Neural Networks/Deep Learning Books Should I Read? \(2019\)](https://news.ycombinator.com/item?id=20674745)
* [Python vs Rust for Neural Networks \(2019\)](https://ngoldbaum.github.io/posts/python-vs-rust-nn/) \([HN](https://news.ycombinator.com/item?id=20728288)\)
* [Exploring Weight Agnostic Neural Networks \(2019\)](https://ai.googleblog.com/2019/08/exploring-weight-agnostic-neural.html) \([HN](https://news.ycombinator.com/item?id=20817083)\)
* [Neural Networks, Types, and Functional Programming \(2015\)](https://colah.github.io/posts/2015-09-NN-Types-FP/)
* [Glow](https://github.com/pytorch/glow) - Compiler for Neural Network hardware accelerators.
* [Go Neural Net Sandbox](https://github.com/lightvector/GoNN) - Sandbox for personal experimentation in Go neural net training and Go AI.
* [layer](https://github.com/cloudkj/layer) - Neural network inference the Unix way.
* [XNNPACK](https://github.com/google/XNNPACK) - Highly optimized library of floating-point neural network inference operators for ARM, WebAssembly, and x86 \(SSE2 level\) platforms.
* [LSTM implementation explained \(2015\)](http://apaszke.github.io/lstm-explained.html)
* [The Neural Process Family](https://github.com/deepmind/neural-processes) - Contains notebook implementations of the following Neural Process variants: Conditional Neural Processes \(CNPs\), Neural Processes \(NPs\), Attentive Neural Processes \(ANPs\).
* [Notes on Neural Nets](https://wiki.kourouklides.com/wiki/Artificial_Neural_Network)
* [RNNoise](https://github.com/xiph/rnnoise) - Recurrent neural network for audio noise reduction.
* [Hacking Neural Networks](https://github.com/Kayzaks/HackingNeuralNetworks) - Short introduction on methods that use neural networks in an offensive manner.
* [Distilling knowledge from Neural Networks to build smaller and faster models \(2019\)](https://blog.floydhub.com/knowledge-distillation/)
* [Neural Network Processing Neural Networks: An efficient way to learn higher order functions \(2019\)](https://arxiv.org/abs/1911.05640)
* [Building a neural net from scratch in Go \(2017\)](https://datadan.io/neural-net-with-go)
* [SparseConvNet](https://github.com/btgraham/SparseConvNet) - Spatially-sparse convolutional neural network.
* [Norse](https://github.com/electronicvisions/norse) - Library to do deep learning with spiking neural networks.
* [Tensor Programs I: Wide Feedforward or Recurrent Neural Networks of Any Architecture are Gaussian Processes \(2019\)](https://arxiv.org/abs/1910.12478)
* [Single Headed Attention RNN: Stop Thinking With Your Head \(2019\)](https://arxiv.org/abs/1911.11423) \([HN](https://news.ycombinator.com/item?id=21647804)\)
* [Visualizing the Loss Landscape of Neural Nets](https://github.com/tomgoldstein/loss-landscape)
* [primitiv](https://github.com/primitiv/primitiv) - Neural Network Toolkit.
* [On the Relationship between Self-Attention and Convolutional Layers \(2019\)](https://openreview.net/forum?id=HJlnC1rKPB) \([Code](https://github.com/epfml/attention-cnn)\) \([Reddit](https://www.reddit.com/r/MachineLearning/comments/en2ywu/r_on_the_relationship_between_selfattention_and/)\)
* [Implementation of a deep learning library in Futhark](https://futhark-lang.org/student-projects/duc-bsc-thesis.pdf)
* [Single Headed Attention RNN: Stop Thinking With Your Head \(2019\)](https://arxiv.org/abs/1911.11423)
* [Using neural networks to solve advanced mathematics equations \(2020\)](https://ai.facebook.com/blog/using-neural-networks-to-solve-advanced-mathematics-equations/)
* [AlphaFold](https://github.com/deepmind/deepmind-research/tree/master/alphafold_casp13) - Provides an implementation of the contact prediction network, associated model weights and CASP13 dataset as published in Nature. \([Paper](https://www.nature.com/articles/s41586-019-1923-7)\)
* [Go Perceptron](https://github.com/made2591/go-perceptron-go) - Single / multi layer / recurrent neural network written in Golang.
* [Temperature Scaling](https://github.com/gpleiss/temperature_scaling) - Simple way to calibrate your neural network.
* [Recurrent Geometric Networks for end-to-end differentiable learning of protein structure](https://github.com/aqlaboratory/rgn)
* [FixMatch: Simplifying Semi-Supervised Learning with Consistency and Confidence \(2020\)](https://arxiv.org/abs/2001.07685) \([Tweet](https://twitter.com/D_Berthelot_ML/status/1219823580654948353)\)
* [kapre](https://github.com/keunwoochoi/kapre) - Keras Audio Preprocessors.
* [Putting An End to End-to-End: Gradient-Isolated Learning of Representations \(2019\)](https://arxiv.org/pdf/1905.11786.pdf)
* [Memory-Augmented Neural Networks for Machine Translation \(2019\)](https://arxiv.org/abs/1909.08314)
* [Have there been any important developments on content addressable memory since hopfield network? \(neural networkish\) \(2020\)](https://www.reddit.com/r/MachineLearning/comments/esrroh/d_have_there_been_any_important_developments_on/)
* [G-Bert](https://github.com/jshang123/G-Bert) - Pre-training of Graph Augmented Transformers for Medication Recommendation.
* [Two strange useless things to do with neural nets: a demonstration](https://github.com/howonlee/twostrangethings)
* [Understanding the Neural Tangent Kernel \(2019\)](https://rajatvd.github.io/NTK/)
* [Cutting out the Middle-Man: Training and Evaluating Energy-Based Models without Sampling](https://arxiv.org/abs/2002.05616) \([Tweet](https://twitter.com/wgrathwohl/status/1228144635010322440)\)
* [Haiku](https://github.com/deepmind/haiku) - JAX-based neural network library.
* [Convolution in one dimension for neural networks \(2020\)](https://e2eml.school/convolution_one_d.html)
* [Lucid](https://github.com/tensorflow/lucid) - Collection of infrastructure and tools for research in neural network interpretability.
* [Minkowski Engine](https://github.com/StanfordVL/MinkowskiEngine) - Auto-diff convolutional neural network library for high-dimensional sparse tensors.
* [Generating MIDI melody from lyrics using LSTM-GANs](https://github.com/yy1lab/Lyrics-Conditioned-Neural-Melody-Generation) \([HN](https://news.ycombinator.com/item?id=22524176)\)
* [Zoom In: An Introduction to Circuits \(2020\)](https://distill.pub/2020/circuits/zoom-in/)
* [Lagrangian Neural Networks \(2020\)](https://greydanus.github.io/2020/03/10/lagrangian-nns/) \([HN](https://news.ycombinator.com/item?id=22552790)\)
* [Neural Tangents](https://github.com/google/neural-tangents) - Fast and Easy Infinite Neural Networks in Python.
* [A Survey of Long-Term Context in Transformers \(2020\)](https://www.pragmatic.ml/a-survey-of-methods-for-incorporating-long-term-context/)
* [OpenNMT-py](https://github.com/OpenNMT/OpenNMT-py) - Open Source Neural Machine Translation in PyTorch.
* [Deep Learning for Symbolic Mathematics](https://github.com/facebookresearch/SymbolicMathematics)
* [Google Brain AutoML](https://github.com/google/automl)
* [Physics Informed Neural Networks](https://github.com/maziarraissi/PINNs) - Data-driven Solutions and Discovery of Nonlinear Partial Differential Equations.
* [An introduction to Bayesian neural networks \(2020\)](https://papercup.dev/posts/bayesian-neural-nets/)
* [PyTorch Neural Turing Machine](https://github.com/loudinthecloud/pytorch-ntm)
* [PyTorch Neural Turing Machine 2](https://github.com/vlgiitr/ntm-pytorch)
* [Learning DAGs with Continuous Optimization \(2020\)](https://blog.ml.cmu.edu/2020/04/10/learning-dags-with-continuous-optimization/)
* [Early Vision \(2020\)](https://distill.pub/2020/circuits/early-vision/) - Guided tour of the first five layers of InceptionV1, taxonomized into “neuron groups.”.
* [micrograd](https://github.com/karpathy/micrograd) - Tiny autograd engine and a neural net library on top of it, potentially for educational purposes.
* [MiniGrad](https://github.com/kennysong/minigrad) - Minimal implementation of reverse-mode automatic differentiation \(a.k.a. autograd / backpropagation\) in pure Python.
* [Learning from Small Neural Networks \(2020\)](https://medium.com/make-computer-science-fun-again/learning-from-small-neural-networks-6bc5ffc2f3d3)
* [Neural Game Engine](https://github.com/Bam4d/Neural-Game-Engine) - Code to reproduce Neural Game Engine experiments and pre-trained models.
* [Graph Convolutional Neural Network Approach to Antibiotic Discovery \(2020\)](https://www.welcometothejungle.com/en/articles/btc-covid19-convolutional-neural-network) \([HN](https://news.ycombinator.com/item?id=22898551)\)
* [KPNNs](https://github.com/epigen/KPNN) - Knowledge-primed neural networks.
* [ResNeSt](https://github.com/zhanghang1989/ResNeSt) - Split-Attention Network.
* [Shortcut Learning in Deep Neural Networks \(2020\)](https://github.com/rgeirhos/shortcut-perspective)
* [Discourse-Aware Attention Model for Abstractive Summarization of Long Documents](https://github.com/armancohan/long-summarization)
* [Perovskite neural trees \(2020\)](https://www.nature.com/articles/s41467-020-16105-y) \([HN](https://news.ycombinator.com/item?id=23107722)\)
* [RigNet: Neural Rigging for Articulated Characters \(2020\)](https://zhan-xu.github.io/rig-net/) \([Reddit](https://www.reddit.com/r/MachineLearning/comments/ggakn3/r_rignet_neural_rigging_for_articulated_characters/)\)
* [Convolutional neural networks for artistic style transfer \(2017\)](https://harishnarayanan.org/writing/artistic-style-transfer/)
* [Certifiable Robustness to adversarial Attacks; What is the Point? \| Nick Frosst \(2020\)](https://www.youtube.com/watch?v=OfSxYqU-6s0)
* [LAG: Latent Adversarial Generator](https://github.com/google-research/lag)
* [Towards improved generalization in few-shot classification \(2019\)](https://tmramalho.github.io/science/2019/12/07/towards-improved-generalization-in-few-shot-classification/)
* [Convolutional Neural Networks in One Dimension](https://end-to-end-machine-learning.teachable.com/p/321-convolutional-neural-networks)
* [Neural Network Pruning \(2020\)](https://nathanhubens.github.io/posts/deep%20learning/2020/05/22/pruning.html)
* [Hyperbolic RNN in PyTorch](https://github.com/ferrine/hyrnn)
* [deeplearn-rs](https://github.com/tedsta/deeplearn-rs) - Deep learning in Rust.
* [Neural networks trained to communicate with each other without any training data](https://twitter.com/noahtren/status/1269035375051386880)
* [Classical Piano Composer](https://github.com/Skuldur/Classical-Piano-Composer) - Allows you to train a neural network to generate midi music files that make use of a single instrument.
* [Weight Standardization](https://github.com/joe-siyuan-qiao/WeightStandardization) - Normalization method to accelerate micro-batch training.
* [Teaching Machines to Draw \(2017\)](https://blog.otoro.net/2017/05/19/teaching-machines-to-draw/) \([In action](https://otoro.net/sketch-rnn/)\)
* [Benchmarking Neural Network Robustness to Common Corruptions and Perturbations](https://github.com/hendrycks/robustness)
* [pix2code](https://github.com/tonybeltramelli/pix2code) - Generating Code from a Graphical User Interface Screenshot.
* [Gated Linear Networks \(2019\)](https://arxiv.org/abs/1910.01526) \([HN](https://news.ycombinator.com/item?id=23528247)\)
* [Curve Detectors \(2020\)](https://distill.pub/2020/circuits/curve-detectors/)
* [Fourier Features Let Networks Learn High Frequency Functions in Low Dimensional Domains](https://github.com/tancik/fourier-feature-networks)
* [Neural Networks and Deep Learning](https://www.notion.so/Neural-Networks-and-Deep-Learning-f7ff3bae25de4f0085fd52fc8e810827) - What they are and how they work.
* [Teaching physics to neural networks removes 'chaos blindness' \(2020\)](https://phys.org/news/2020-06-physics-neural-networks-chaos.html) \([HN](https://news.ycombinator.com/item?id=23597426)\)
* [Understanding Convolutional Neural Networks](https://poloclub.github.io/cnn-explainer/) \([Code](https://github.com/poloclub/cnn-explainer)\) \([HN](https://news.ycombinator.com/item?id=23710799)\)
* [Business Card Neural Network \(2020\)](https://imois.in/posts/card-network/)
* [Functional Neural Networks \(2020\)](https://b-thi.github.io/Posts/FNNs.html)
* [Attention Is All You Need \(2017\)](https://www.youtube.com/watch?v=iDulhoQ2pro)
