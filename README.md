# Visual Question Answering Using CLIP + LSTM

 <div align="center">
    <a href="https://colab.research.google.com/github/reshalfahsi/vqa-clip-lstm/blob/master/Visual_Question_Answering_Using_CLIP_LSTM.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"></a>
    <br />
 </div>


<div align="center">
    <img src="https://github.com/reshalfahsi/vqa-clip-lstm/blob/master/assets/architecture.png" alt="architecture" >
    </img>
    CLIP + LSTM architecture.
    <br />
</div>


The visual question-answering problem can be described as "asking our computer to reply to the assigned questions about a particular image." In this project, a CLIP + LSTM architecture comes to lend a helping hand, trying to solve the problem. The image and text encoders of CLIP cultivate the given image and question, respectively. The concatenated image-text representation from CLIP is then applied to the vectorized answer text via the Hadamard product before feeding it to LSTM. By a fashion of autoregressive, the answer to the question is finally served to us. Here, the VizWiz-VQA dataset is utilized to train, validate, and test the model. The training set of the dataset is used in the training and validation phases. It is divided by a ratio of 99:1. The validation set of the dataset is employed for testing. The SQuAD and BLEU metrics are utilized to gauge the performance of the model quantitatively. In inference time, the test set of VizWiz-VQA is leveraged.


## Experiment

Give yourself a delightful excursion by passing through the line of codes regarding the experiment provided in this [notebook](https://github.com/reshalfahsi/vqa-clip-lstm/blob/master/Visual_Question_Answering_Using_CLIP_LSTM.ipynb).


## Result

## Quantitative Result

Here are the evaluation metric results of the model.

SQuAD Metric                   | Score
------------------------------ | -------------
BLEU 1-gram                    | 44.67%
Exact Match                    | 44.32%
F1-score                       | 44.63%


## Loss Curve

<p align="center"> <img src="https://github.com/reshalfahsi/vqa-clip-lstm/blob/master/assets/loss_curve.png" alt="loss_curve" > <br /> Loss curves of the CLIP + LSTM model on the train and validation sets. </p>


## Qualitative Result

The following image exhibits the collated results of the VQA model.

<p align="center"><img src="https://github.com/reshalfahsi/vqa-clip-lstm/blob/master/assets/qualitative.png" alt="qualitative"><br/> A collection of qualitative results containing question-answer-image triads.</p>


## Credit

- [An Image Is Worth 16x16 Words: Transformers for Image Recognition at Scale](https://arxiv.org/pdf/2010.11929.pdf)
- [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/pdf/2103.00020.pdf)
- [Less Is More: Linear Layers on CLIP Features as Powerful VizWiz Model](https://arxiv.org/pdf/2206.05281.pdf)
- [Long Short-Term Memory](https://www.bioinf.jku.at/publications/older/2604.pdf)
- [SQuAD: 100,000+ Questions for Machine Comprehension of Text](https://arxiv.org/pdf/1606.05250.pdf)
- [A Call for Clarity in Reporting BLEU Scores](https://arxiv.org/pdf/1804.08771)
- [CLIP](https://github.com/openai/CLIP)
- [yousefkotp's Visual Question Answering](https://github.com/yousefkotp/Visual-Question-Answering)
- [aladdinpersson's Image Captioning](https://github.com/aladdinpersson/Machine-Learning-Collection/tree/master/ML/Pytorch/more_advanced/image_captioning)
- [VizWiz-VQA](https://vizwiz.org/tasks-and-datasets/vqa/)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
