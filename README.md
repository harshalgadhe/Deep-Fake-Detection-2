<h1> Deep-Fake-Detection Upgradation </h1>

<b>DeepFake</b> is a technique that aims to replace the face of a targeted person with the face of someone else in a video. It first appeared in autumn 2017 as a script used to generate face-swapped adult content. We have proposed a model which can be used to detect the forged video and hence can become a great public concern recently. <br>
We have proposed better architechure as compared to <a href='https://github.com/harshalgadhe/DeepFake-Detection'>Meso-4 network for Deep Fake detection </a> and can be said to have rare chances of failing when trained fully (i.e for 100 image sequences)

<br>
We used 3775 for training and 665 for validation. The dataset is overall balanced. We have passed 10 frames while training the model resulting in low accuracy<br>

<h1> Model Upgradation</h1>
<ul>
  <li>Rather than using images to predict we feed video directly to our model</li>
  <li>Used custom architecture rather than using Meso-4 architecture </li>
  <li>We build our own prediction model so that one can do prediction for the video without having to understand the code, you just need to add the path</li>
  <li>Due to resources we weren't able to use fine tuning , if used can make the model attained better accuracy</li>
  <li>Dataset has videos not only from DeepFake dataset but also from Celeb dataset as well as face forensics dataset as compared to the one implemented before which only has videos from DeepFake Dataset and hence can do better in real time than the one above</li>
</ul>

<h1>Setting up the model locally or on Colab</h1>
You can run our model locally as well on colab by uploading the .ipynb file on your colab. For running the model on your computer you will have to download dependencies. For downloading click on <a href='https://github.com/harshalgadhe/DeepFake-Detection/blob/main/requirements.txt'>Requirements File</a>. After downloading you need to run the code by opening the command propmt and pasting the following code:
pip install -r /path to requirements.txt file.

<h1> Datasets and Weights file </h1>
<br>
<a href='https://drive.google.com/drive/folders/1dy7yDga-VZH-FfYt-4FCacBck9IbpY8m?usp=sharing'>Preprocessed Dataset</a><br>
<a href='https://drive.google.com/drive/folders/1-P703ueObw3lkCJDgefCB1kSB7yu5DaI?usp=sharing'>Weights File</a><br>

<h1>Model</h1>
The architecure of the model is as 
<img src='https://github.com/harshalgadhe/Deep-Fake-Detection-2/blob/main/images/WhatsApp%20Image%202021-10-13%20at%2010.36.47%20(1).jpeg'><br>
<h3>The results of the prediction model when tested on unseen data is as follows. As you can see the model was able to predict correctly.</h3><br>
<img src='https://github.com/harshalgadhe/Deep-Fake-Detection-2/blob/main/images/Screenshot%20(25).png'><br> 


