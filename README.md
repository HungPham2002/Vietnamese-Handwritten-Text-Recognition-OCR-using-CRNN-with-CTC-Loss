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
# Desciption Problem:
![description problem](https://camo.githubusercontent.com/a36e6118ddc69a0b965c506246cf08c1b2db66a64aa8d3c4f6c94377f80df377/68747470733a2f2f692e696d6775722e636f6d2f76776c737835322e706e67)
Given an image of a Vietnamese handwritten line, we need to use an OCR model to transcribe the image into text like above.
# Dataset:
The dataset, which have 1838 traning images and 538 testing images. Theirs labels in json file, is provided by Cinnamon AI.

Here are 10 samples of the dataset:
![sample](https://camo.githubusercontent.com/42caf01b97c950f82d8a2880c192433426e7aecb48ffecaca1b9dbfa7dac04d3/68747470733a2f2f692e696d6775722e636f6d2f66545865746b302e6a7067)
Here is the structure of the json file containing the labels:
![label](https://camo.githubusercontent.com/66f97a1a493e3c63c5a37158f77e5d35aaa1c3ce435c4ed0bebeda89951a21e0/68747470733a2f2f692e696d6775722e636f6d2f554b7a414e53492e706e67)
More detail about dataset, the zip file can be downloaded at the google drive link: https://drive.google.com/drive/folders/1Qa2YA6w6V5MaNV-qxqhsHHoYFRK5JB39
# Approaching:
Idea: we want to detect text from a text image:
![idea](https://drive.google.com/uc?export=view&id=1rO7XMFKJyg-81cw_wWoVguwH8w44jGzx)
However, character segmentation is not practical because:
![charactersegmentation](https://drive.google.com/uc?export=view&id=1-k6bKUUQfTvb8SV6rcCfaims_dl4OPBh)
- Too time comsuming
- Too expensive
- Impossible in most cases
This project will use state of the art CRNN model which is a combination of CNN, RNN and CTC loss for image-based sequence recognition tasks, specially OCR (Optical Character Recognition) task which is perfect for handwritten text.
![crnn](https://drive.google.com/uc?export=view&id=1gvoDFLSQL9H6tZy_rNxgN27eLdzPnAkL)
This model is much more superior than traditional way which does not involve any bounding box detection for each character (character segmentation).

In this model, the image will be dissected by a fixed number of timesteps in the RNN layers so as long as each character is seperated by two or three parts to be processed and decoded later then the spacing between each character is irrelevant like so:
![dissect](https://drive.google.com/uc?export=view&id=1CEoqdg8s_rUX_Z_OHccuavESKkpp0ARs)
# The Proposed Architecture Architecture:
The neural network architecture CRNN consists of 3 components, including convolutional layers, recurrent layers, and a transcription layer, from bottom to top.
![architecture](https://drive.google.com/uc?export=view&id=1eKZ8A4TtEQlewstK2qKO8l-ZN4PkdvkW)

At the bottom layer of CRNN, the convolutional layers automatically extract a feature sequence from each input image. Above the convolutional layers is a recurrent network built to make predictions for each frame of the feature sequence (the output of convolutional layers).

The Transcription layer at the topmost level of CRNN is used to translate each prediction frame made by the recurrent layers into a label sequence. Although CRNN is built from various network architectures (e.g., CNN and RNN), it can be trained with a loss function.
## Feature sequence extraction with CNN layers:
## Sequence labeling with RNN layer:
## Transcription layer:
