<p align="center" dir="auto">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" rel="nofollow">
    <img src="https://camo.githubusercontent.com/29fa0dade8ce1281054a2a4844513e68f8868f15057452c709392fe49b01d398/68747470733a2f2f692e696d6775722e636f6d2f576d4d6e5352742e706e67" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology" data-canonical-src="https://i.imgur.com/WmMnSRt.png" style="max-width: 100%;">
  </a>
</p>
<h1 align="center" tabindex="-1" dir="auto"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><b>CS331.N21.KHCL - THỊ GIÁC MÁY TÍNH NÂNG CAO - ADVANCED COMPUTER VISION </b></h1>

# Information:
- Course: Advanced Computer Vision.
- Course ID: CS331.N21.KHCL
- Lecturer: PhD Mai Tien Dung
- Term: Second term (2022-2023)

# Contact:
<table>
  <thead>
    <tr>
      <th align = "center"> STT </th>
      <th> Name </th>
      <th> Email </th>
      <th> Github </th>
      <th> Linkedin </th>
      <th> Facebook </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align = "center">1</td>
      <td>Pham Huu Hung</td>
      <td>
        <a href = "mailto:20521371@gm.uit.edu.vn">20521371@gm.uit.edu.vn</a>
      </td>
      <td>
        <a href = "https://github.com/HungPham2002">HungPham2002</a>
      </td>
      <td>
        <a href = "https://www.linkedin.com/in/h%C3%B9ng-ph%E1%BA%A1m-h%E1%BB%AFu-488996277/">Hùng Phạm Hữu</a>
      </td>
      <td>
        <a href = "https://www.facebook.com/Hungzt103/" rel = "nofollow">Phạm Hữu Hùng</a>
      </td>
    </tr>
    <tr>
      <td align = "center">2</td>
      <td>Le Van Duy</td>
      <td>
        <a href = "mailto:20521233@gm.uit.edu.vn">20521233@gm.uit.edu.vn</a>
      </td>
      <td>
        <a href = "https://github.com/leduy-it">leduy-it</a>
      </td>
      <td>
        <a href = "https://www.linkedin.com/in/leduy-it/">Le Van Duy</a>
      </td>
      <td>
        <a href = "https://www.facebook.com/DuyEkko" rel = "nofollow">Lê Văn Duy</a>
      </td>
    </tr>
  </tbody>
</table>

# Introduction:
- the importance of handwritten address recognition in natural language processing and character recognition. Automating the recognition and extraction of information from images containing handwritten addresses can be valuable in various real-life applications, such as data entry automation, customer information management, and enhancing user experience in mobile applications.
- For countries like Vietnam, where handwritten addresses come in diverse forms and features, building an effective handwritten address recognition model is a significant challenge. The CRNN (Convolutional Recurrent Neural Network) method, which combines convolutional and language networks, has proven effective in this regard. The convolutional network helps the model learn and extract low-level features from images, while the language network aids in processing sequential information and contextualizing character strings. However, to ensure flexibility and the ability to recognize diverse Vietnamese handwritten addresses, the CRNN method needs to be combined with other techniques.
- One advanced technique applied is using the CTC Loss (Connectionist Temporal Classification Loss), which trains the model by matching the predicted output character sequences with target character sequences without requiring exact alignment. This allows the model to recognize long text passages, where determining character boundaries becomes challenging.
- The research proposes a model for recognizing Vietnamese handwritten addresses using the CRNN method with CTC Loss. The model is trained on a large dataset containing images of Vietnamese handwritten addresses to ensure diversity and high accuracy. The performance of the model is evaluated on a test dataset and compared with previous methods to assess its accuracy and effectiveness.
# Description Problem:
![description problem](https://camo.githubusercontent.com/a36e6118ddc69a0b965c506246cf08c1b2db66a64aa8d3c4f6c94377f80df377/68747470733a2f2f692e696d6775722e636f6d2f76776c737835322e706e67)
Given an image of a Vietnamese handwritten line, we need to use an OCR model to transcribe the image into text like above.
# Dataset:
The dataset, which have 1838 traning images and 538 testing images. Theirs labels in json file, is provided by Cinnamon AI.

Here are 10 samples of the dataset:
![sample](https://camo.githubusercontent.com/42caf01b97c950f82d8a2880c192433426e7aecb48ffecaca1b9dbfa7dac04d3/68747470733a2f2f692e696d6775722e636f6d2f66545865746b302e6a7067)
Here is the structure of the json file containing the labels:
![label](https://camo.githubusercontent.com/66f97a1a493e3c63c5a37158f77e5d35aaa1c3ce435c4ed0bebeda89951a21e0/68747470733a2f2f692e696d6775722e636f6d2f554b7a414e53492e706e67)
Dataset which we merged based on the Cinnamon's dataset: https://drive.google.com/drive/folders/1M4N7bGyAls6X64RTDal6JrO3j136lx-T?usp=drive_link

More detail about dataset, the private test can be downloaded at the google drive link: https://drive.google.com/drive/folders/1Qa2YA6w6V5MaNV-qxqhsHHoYFRK5JB39
# Approaching:
Idea: we want to detect text from a text image:
- ![idea](https://drive.google.com/uc?export=view&id=1rO7XMFKJyg-81cw_wWoVguwH8w44jGzx)
- However, character segmentation is not practical because:
![charactersegmentation](https://drive.google.com/uc?export=view&id=1-k6bKUUQfTvb8SV6rcCfaims_dl4OPBh)
- Too time comsuming
- Too expensive
- Impossible in most cases
This project will use state of the art CRNN model which is a combination of CNN, RNN and CTC loss for image-based sequence recognition tasks, specially OCR (Optical Character Recognition) task which is perfect for handwritten text.
![crnn](https://drive.google.com/uc?export=view&id=1gvoDFLSQL9H6tZy_rNxgN27eLdzPnAkL)
This model is much more superior than traditional way which does not involve any bounding box detection for each character (character segmentation).

In this model, the image will be dissected by a fixed number of timesteps in the RNN layers so as long as each character is seperated by two or three parts to be processed and decoded later then the spacing between each character is irrelevant like so:
![dissect](https://drive.google.com/uc?export=view&id=1CEoqdg8s_rUX_Z_OHccuavESKkpp0ARs)
# The Proposed Neural Architecture:
The neural network architecture CRNN consists of 3 components, including convolutional layers, recurrent layers, and a transcription layer, from bottom to top.
- ![architecture](https://drive.google.com/uc?export=view&id=1eKZ8A4TtEQlewstK2qKO8l-ZN4PkdvkW)

At the bottom layer of CRNN, the convolutional layers automatically extract a feature sequence from each input image. Above the convolutional layers is a recurrent network built to make predictions for each frame of the feature sequence (the output of convolutional layers).

The Transcription layer at the topmost level of CRNN is used to translate each prediction frame made by the recurrent layers into a label sequence. Although CRNN is built from various network architectures (e.g., CNN and RNN), it can be trained with a loss function.
## Feature sequence extraction with CNN layers:
![CNN](https://drive.google.com/uc?export=view&id=1o1abPGFZ9NqsxFoMhp4p5kYgf9NtwP3O)
- In the CRNN (Convolutional Recurrent Neural Network) model, the components of the convolutional layers are constructed by adopting convolutional and max-pooling layers from a standard CNN model, thereby eliminating fully connected layers. These components are employed to extract a sequential feature representation from an input image. Prior to feeding the images into the network, all images are required to be resized to a uniform height. Subsequently, a sequence of feature vectors is extracted from the feature maps generated by the convolutional layers' components, serving as the input for the recurrent layers.

- More specifically, each feature vector of a feature sequence is generated by traversing the feature maps from left to right along the columns. In other words, from the feature maps, a sequence of feature vectors is created. By reshaping the matrix into a vector, each vector is formed by concatenating the columns at position i across all feature maps.
- Each vector in the sequence of feature vectors is extracted from feature maps corresponding to a receptive field. These feature vectors can be considered as representations of the image for that specific region. Consequently, the model can utilize these features to identify objects and information within the image.
- ![receptivefield](https://drive.google.com/uc?export=view&id=18sqOno0xb8iIwBMBIccEmTr3Nfe42rJs)
## Sequence labeling with RNN layer:
For sentence and text understanding, considering the context from both left to right and right to left can provide valuable information. To utilize information from both directions, we combine two LSTM networks: one processes the input sequence in the forward direction, and the other processes it in the backward direction, forming a bidirectional LSTM network. In this project, we stack multiple layers of bidirectional LSTM, creating a deep bidirectional LSTM network to leverage information from both directions effectively.
- ![DeepBidirectionalLSTM](https://drive.google.com/uc?export=view&id=1y7hWGZKDcHgEQyOQeOtt_3cxizd-eVM1)
## Transcription layer:
- The objective is to convert the per-frame predictions of the RNN into a predicted label sequence.
- let's assume:

+ The input X (which is the output of the RNN) has a length of 10 time steps.
+ The label of X is "chào" (meaning "hello" in English).
+ The output Y has a length of 4, Y = [c, h, à, o].
Instead of directly predicting "chào" as a whole, the RNN will predict its variations, such as "cchhhààooo, cccchàààoo, ..." and so on.

From these alignments, by removing duplicate characters, we can obtain the desired result "chào" as the final predicted label sequence.
- ![ideaRNNprocession](https://drive.google.com/uc?export=view&id=1KXE_flXITS8-5D0dkNJpfkphVxm7pTxR)
- The mentioned approach has two issues:
  + It forces the RNN's output to correspond to exactly one character, which doesn't account for frames without any characters (e.g., background frames).
  + The output can be incorrect, for example, "heeeeellloo" being predicted as "helo" instead of "hello."
To address these issues, the Connectionist Temporal Classification (CTC) method is used. CTC loss introduces a special blank token, represented as "-", to create alignments. When encoding text, we add multiple arbitrary blank characters between any two characters and also between consecutive similar characters. For example, "hello" will have alignments like "heeeel–llo", "-hell-l–oo", and so on, always with at least one "-" between two "l" characters.

CTC is suitable for two tasks:

+ Training: It computes the loss to train the network.
+ Prediction (inference): It decodes this matrix to obtain the output text. This is done by calculating 
<blockquote style="text-align: center;">
  Y* = argmax p(Y|X)
</blockquote>
, where Y* is the predicted label sequence given the input X.

### Probability of label sequence:
- The given notation:
  + Input X: The per-frame predictions X = x1, x2, ..., xT (where T is the length of the sequence).
  + Output Y: The label sequence.
  + A: A single alignment.
  + A(X,Y): The set of all alignments A for the output sequence Y.
  + at: a single character at each time step of Alignment A.
- ![Probability](https://drive.google.com/uc?export=view&id=1ZXgFGIBx1NJpnkXdaHkhC3Wdyd3erxoq)
- ![VisualizeProbability](https://drive.google.com/uc?export=view&id=1z5nhqa8RZ1bC4eJDOpCz-sRwWyDRO_RB)

Once we have the Loss function, we proceed to compute the gradients as usual. Parameters will be adjusted to minimize the negative log likelihood function.

In the training process. During training, we provide a sample data (an image) and its corresponding Ground Truth text (actual label sequence). The CTC Loss function estimates the loss by computing the probability of the Ground Truth Text based on the output of the BLSTM network. It attempts to find the most probable path corresponding to the Ground Truth Text.

To measure the distance between the actual label sequence and the predicted label sequence from the model, the objective of the training process is to minimize the loss. In other words, the goal is to make the predicted label sequence from the model as close as possible to the actual label sequence.

The Decoding process is quite simple and involves two steps:
+ Finding the alignment that passes through the characters with the highest probabilities in each time step.
Removing consecutive identical characters and then removing blank characters.
+ In summary, during training, the CTC Loss function helps find the best alignment between the predicted and actual label sequences, and during decoding, the process involves removing duplicates and blank characters from the predicted label sequence.

<p>
  To gain a better understanding of CTC, readers can refer to
  <a href="https://distill.pub/2017/ctc/">here.</a>
</p> 

# The Network Architecture to solve the problem:
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>__________________________________________________________________________________________________
Layer (type)                    Output Shape         Param #     Connected to                     
==================================================================================================
input_1 (InputLayer)            [(None, 118, 2167, 1 0                                            
__________________________________________________________________________________________________
conv2d (Conv2D)                 (None, 118, 2167, 64 640         input_1[0][0]                    
__________________________________________________________________________________________________
max_pooling2d (MaxPooling2D)    (None, 39, 722, 64)  0           conv2d[0][0]                     
__________________________________________________________________________________________________
activation (Activation)         (None, 39, 722, 64)  0           max_pooling2d[0][0]              
__________________________________________________________________________________________________
conv2d_1 (Conv2D)               (None, 39, 722, 128) 73856       activation[0][0]                 
__________________________________________________________________________________________________
max_pooling2d_1 (MaxPooling2D)  (None, 13, 240, 128) 0           conv2d_1[0][0]                   
__________________________________________________________________________________________________
activation_1 (Activation)       (None, 13, 240, 128) 0           max_pooling2d_1[0][0]            
__________________________________________________________________________________________________
conv2d_2 (Conv2D)               (None, 13, 240, 256) 295168      activation_1[0][0]               
__________________________________________________________________________________________________
batch_normalization (BatchNorma (None, 13, 240, 256) 1024        conv2d_2[0][0]                   
__________________________________________________________________________________________________
activation_2 (Activation)       (None, 13, 240, 256) 0           batch_normalization[0][0]        
__________________________________________________________________________________________________
conv2d_3 (Conv2D)               (None, 13, 240, 256) 590080      activation_2[0][0]               
__________________________________________________________________________________________________
batch_normalization_1 (BatchNor (None, 13, 240, 256) 1024        conv2d_3[0][0]                   
__________________________________________________________________________________________________
add (Add)                       (None, 13, 240, 256) 0           batch_normalization_1[0][0]      
                                                                 activation_2[0][0]               
__________________________________________________________________________________________________
activation_3 (Activation)       (None, 13, 240, 256) 0           add[0][0]                        
__________________________________________________________________________________________________
conv2d_4 (Conv2D)               (None, 13, 240, 512) 1180160     activation_3[0][0]               
__________________________________________________________________________________________________
batch_normalization_2 (BatchNor (None, 13, 240, 512) 2048        conv2d_4[0][0]                   
__________________________________________________________________________________________________
activation_4 (Activation)       (None, 13, 240, 512) 0           batch_normalization_2[0][0]      
__________________________________________________________________________________________________
conv2d_5 (Conv2D)               (None, 13, 240, 512) 2359808     activation_4[0][0]               
__________________________________________________________________________________________________
batch_normalization_3 (BatchNor (None, 13, 240, 512) 2048        conv2d_5[0][0]                   
__________________________________________________________________________________________________
add_1 (Add)                     (None, 13, 240, 512) 0           batch_normalization_3[0][0]      
                                                                 activation_4[0][0]               
__________________________________________________________________________________________________
activation_5 (Activation)       (None, 13, 240, 512) 0           add_1[0][0]                      
__________________________________________________________________________________________________
conv2d_6 (Conv2D)               (None, 13, 240, 1024 4719616     activation_5[0][0]               
__________________________________________________________________________________________________
batch_normalization_4 (BatchNor (None, 13, 240, 1024 4096        conv2d_6[0][0]                   
__________________________________________________________________________________________________
max_pooling2d_2 (MaxPooling2D)  (None, 4, 240, 1024) 0           batch_normalization_4[0][0]      
__________________________________________________________________________________________________
activation_6 (Activation)       (None, 4, 240, 1024) 0           max_pooling2d_2[0][0]            
__________________________________________________________________________________________________
max_pooling2d_3 (MaxPooling2D)  (None, 1, 240, 1024) 0           activation_6[0][0]               
__________________________________________________________________________________________________
lambda (Lambda)                 (None, 240, 1024)    0           max_pooling2d_3[0][0]            
__________________________________________________________________________________________________
bidirectional (Bidirectional)   (None, 240, 1024)    6295552     lambda[0][0]                     
__________________________________________________________________________________________________
bidirectional_1 (Bidirectional) (None, 240, 1024)    6295552     bidirectional[0][0]              
__________________________________________________________________________________________________
dense (Dense)                   (None, 240, 141)     144525      bidirectional_1[0][0]            
__________________________________________________________________________________________________
the_labels (InputLayer)         [(None, 240)]        0                                            
__________________________________________________________________________________________________
input_length (InputLayer)       [(None, 1)]          0                                            
__________________________________________________________________________________________________
label_length (InputLayer)       [(None, 1)]          0                                            
__________________________________________________________________________________________________
ctc (Lambda)                    (None, 1)            0           dense[0][0]                      
                                                                 the_labels[0][0]                 
                                                                 input_length[0][0]               
                                                                 label_length[0][0]               
==================================================================================================
Total params: 21,965,197
Trainable params: 21,960,077
Non-trainable params: 5,120
__________________________________________________________________________________________________
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="__________________________________________________________________________________________________
Layer (type)                    Output Shape         Param #     Connected to                     
==================================================================================================
input_1 (InputLayer)            [(None, 118, 2167, 1 0                                            
__________________________________________________________________________________________________
conv2d (Conv2D)                 (None, 118, 2167, 64 640         input_1[0][0]                    
__________________________________________________________________________________________________
max_pooling2d (MaxPooling2D)    (None, 39, 722, 64)  0           conv2d[0][0]                     
__________________________________________________________________________________________________
activation (Activation)         (None, 39, 722, 64)  0           max_pooling2d[0][0]              
__________________________________________________________________________________________________
conv2d_1 (Conv2D)               (None, 39, 722, 128) 73856       activation[0][0]                 
__________________________________________________________________________________________________
max_pooling2d_1 (MaxPooling2D)  (None, 13, 240, 128) 0           conv2d_1[0][0]                   
__________________________________________________________________________________________________
activation_1 (Activation)       (None, 13, 240, 128) 0           max_pooling2d_1[0][0]            
__________________________________________________________________________________________________
conv2d_2 (Conv2D)               (None, 13, 240, 256) 295168      activation_1[0][0]               
__________________________________________________________________________________________________
batch_normalization (BatchNorma (None, 13, 240, 256) 1024        conv2d_2[0][0]                   
__________________________________________________________________________________________________
activation_2 (Activation)       (None, 13, 240, 256) 0           batch_normalization[0][0]        
__________________________________________________________________________________________________
conv2d_3 (Conv2D)               (None, 13, 240, 256) 590080      activation_2[0][0]               
__________________________________________________________________________________________________
batch_normalization_1 (BatchNor (None, 13, 240, 256) 1024        conv2d_3[0][0]                   
__________________________________________________________________________________________________
add (Add)                       (None, 13, 240, 256) 0           batch_normalization_1[0][0]      
                                                                 activation_2[0][0]               
__________________________________________________________________________________________________
activation_3 (Activation)       (None, 13, 240, 256) 0           add[0][0]                        
__________________________________________________________________________________________________
conv2d_4 (Conv2D)               (None, 13, 240, 512) 1180160     activation_3[0][0]               
__________________________________________________________________________________________________
batch_normalization_2 (BatchNor (None, 13, 240, 512) 2048        conv2d_4[0][0]                   
__________________________________________________________________________________________________
activation_4 (Activation)       (None, 13, 240, 512) 0           batch_normalization_2[0][0]      
__________________________________________________________________________________________________
conv2d_5 (Conv2D)               (None, 13, 240, 512) 2359808     activation_4[0][0]               
__________________________________________________________________________________________________
batch_normalization_3 (BatchNor (None, 13, 240, 512) 2048        conv2d_5[0][0]                   
__________________________________________________________________________________________________
add_1 (Add)                     (None, 13, 240, 512) 0           batch_normalization_3[0][0]      
                                                                 activation_4[0][0]               
__________________________________________________________________________________________________
activation_5 (Activation)       (None, 13, 240, 512) 0           add_1[0][0]                      
__________________________________________________________________________________________________
conv2d_6 (Conv2D)               (None, 13, 240, 1024 4719616     activation_5[0][0]               
__________________________________________________________________________________________________
batch_normalization_4 (BatchNor (None, 13, 240, 1024 4096        conv2d_6[0][0]                   
__________________________________________________________________________________________________
max_pooling2d_2 (MaxPooling2D)  (None, 4, 240, 1024) 0           batch_normalization_4[0][0]      
__________________________________________________________________________________________________
activation_6 (Activation)       (None, 4, 240, 1024) 0           max_pooling2d_2[0][0]            
__________________________________________________________________________________________________
max_pooling2d_3 (MaxPooling2D)  (None, 1, 240, 1024) 0           activation_6[0][0]               
__________________________________________________________________________________________________
lambda (Lambda)                 (None, 240, 1024)    0           max_pooling2d_3[0][0]            
__________________________________________________________________________________________________
bidirectional (Bidirectional)   (None, 240, 1024)    6295552     lambda[0][0]                     
__________________________________________________________________________________________________
bidirectional_1 (Bidirectional) (None, 240, 1024)    6295552     bidirectional[0][0]              
__________________________________________________________________________________________________
dense (Dense)                   (None, 240, 141)     144525      bidirectional_1[0][0]            
__________________________________________________________________________________________________
the_labels (InputLayer)         [(None, 240)]        0                                            
__________________________________________________________________________________________________
input_length (InputLayer)       [(None, 1)]          0                                            
__________________________________________________________________________________________________
label_length (InputLayer)       [(None, 1)]          0                                            
__________________________________________________________________________________________________
ctc (Lambda)                    (None, 1)            0           dense[0][0]                      
                                                                 the_labels[0][0]                 
                                                                 input_length[0][0]               
                                                                 label_length[0][0]               
==================================================================================================
Total params: 21,965,197
Trainable params: 21,960,077
Non-trainable params: 5,120
__________________________________________________________________________________________________" tabindex="0" role="button" style="display: inherit;">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>

More information regarding the implementation can be found in the jupyter notebook in the github.

The number of callbacks I used are very helpful which are ModelCheckpoint, EarlyStopping and ReduceLROnPlateau which allows my model to keep on improving after 2 hours of training.

# Evaluation Metrics:
Evaluation is based on character error rate (CER)

- CER is calculated based on Edit distance (or Levenshtein distance)
Given a predicted string A, and the ground truth string B, CER is specified by:

![CER](https://drive.google.com/uc?export=view&id=1O1bhhZQplshvNRV2BkeWPd_XTU1xNrwn)

- Word Error Rate:

![WER](https://drive.google.com/uc?export=view&id=1-w5-zS_OXG3R5MnX_1pZeSUB7J4PNBp_)

- Sequece Error Rate:

![SER](https://drive.google.com/uc?export=view&id=1UQfNG2FqT-RxaqPXlcaCDPhuoWh22u2j)

# Results:
Here are the important three evaluation metris for a test set (the host's private test):

  + CER (Character Error Rate): 0.08803356531644808

  + WER (Word Error Rate): 0.2735233391975599

  + SER (Sequence Error Rate): 0.9253187613843351

We got a pretty good results with CER at 8% and WER at 27%!

There are plenty of examples where the model predicts every single character perfectly like this!

![test](https://drive.google.com/uc?export=view&id=1I0aKAAbBgE8MokfvFfDZ8cpPrgioZ902)

# References:
[1] https://github.com/TomHuynhSG/Vietnamese-Handwriting-Recognition-OCR

[2] https://viblo.asia/p/tim-hieu-bai-toan-ocr-voi-crnn-va-ctc-loss-ocr-from-scratch-with-pytorch-p1-OeVKBA905kW

[3] https://viblo.asia/p/nhan-dien-text-trong-hinh-anh-voi-crnnctc-Eb85o9rBZ2G

[4] <a href="https://arxiv.org/pdf/1507.05717.pdf"> An End-to-End Trainable Neural Network for Image-based Sequence Recognition and
Its Application to Scene Text Recognition</a>

[5] https://distill.pub/2017/ctc/

[6] https://stanford.edu/~shervine/l/vi/teaching/cs-230/cheatsheet-recurrent-neural-networks
