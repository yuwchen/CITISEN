# CITISEN
<a href="https://www.youtube.com/watch?v=CPofug0IW5I&feature=youtu.be" target="_blank"><img src="https://i.imgur.com/z90yoJp.png" 
alt="CITISEN video"  width=80% height=80% border="10" text-align: center /></a>


## Introduction
In this work, we present a deep learning-based speech signal-processing mobile application known as CITISEN. The CITISEN can perform three functions: speech enhancement (SE), model adaptation (MA), and background noise conversion (BNC), which allow CITISEN to be used as a platform for utilizing and evaluating SE models and flexibly extend the models to address various noise environments and users. For SE, CITISEN downloads pretrained SE models on the cloud server and then uses these models to effectively reduce noise components from instant or saved recordings provided by users. When it encounters noisy speech signals with unknown speakers or noise types, the MA function allows CITISEN to improve the SE performance effectively. A few audio files of unseen speakers or noise types are recorded and uploaded to the cloud server and then used to adapt the pretrained SE model. Finally, for the BNC, CITISEN removes the original background noise using an SE model, and then mixes the processed speech signal with new background noise. The novel BNC function can evaluate SE performance under specific conditions, cover people’s tracks, and provide entertainment.


## User interface and usage

### Four main pages in CITISEN
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_main.png" 
alt="main"  width=40% height=40% />

The CITISEN application has four pages, "Speech Enhancement", "Background Noise Conversion", "Model Adaptation", and "Recording". The page name and the navigator buttons of each page are listed on the top-left and bottom in the application, respectively.


### Speech Enhancement page
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_SE.png" 
alt="main"  width=40% height=40% />

The “gender” button on the upper-right corner is used to specify the user’s gender. By pressing the “model switch” button, an SE model list will pop up, and users can change the SE model. After pressing the “preview” button, users will hear their original instant recording, and after pressing the “activate” button, users will hear their enhanced instant recording.

### Background Noise Conversion page


<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_BNC.png" 
alt="main"  width=40% height=40% />

By pressing the “sound switch” button, a background noise list will pop up. After pressing the “record noise” button, users can record and save a new noise signal. After pressing the “activate” button, users will hear the enhanced instant recording with the specified background noise. Note that the “gender” button and the “model switch” button have the same function as those in the “speech enhancement” page.

### Uploading page

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_uploading.png" 
alt="main"  width=40% height=40% />

The “uploading” page is used for uploading the data for the Model Adaptation function. As CITISEN provides both unknown noise adaptation and new speaker adaptation, there are two file upload buttons: “record speech” and “record noise.” To start the recording, users can simply press one button. After finishing the recording by pressing the button again, CITISEN will pop up a submission window. Users can then name the audio file and upload the recorded audio to the server. 

### Recording page

A. Recording page of CITISEN (Part I). A new audio file can be recorded after pressing the “record new” button. The file can then be named and saved in a pop-up submission window.

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_recording_a.png" 
alt="main"  width=40% height=40% />

B. Recording page of CITISEN (Part II). By pressing the “choose file” button, users can choose an audio file on a pop-up window.

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_recording_b.png" 
alt="main"  width=40% height=40% />

C. Recording page of CITISEN (Part III). Users can choose an SE model type and an SE model by using the “gender” and “model switch” button. In addition, users can evaluate the SE results visually and aurally.

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/app_recording_c.png" 
alt="main"  width=40% height=40% />


The “recording” page supports classic recording and SE model evaluation. Specifically, on the “recording” page, users can save, playback, and run SE on a saved speech signal. First, users can record new audio by pressing the “record new” button, and CITISEN will redirect to a processing page. After finishing the recording by pressing the “stop” button, users can name and save the record. The workflow is shown in Fig. A. Then, users can choose an audio file, a model mode, and an SE model with the “choose file,” “gender,” and “model switch” buttons, respectively. Finally, by pressing the “run” button, an enhanced speech signal is generated. Because CITISEN demonstrates both the noisy spectrogram and enhanced spectrogram, users can visually evaluate the SE results. In addition, users can aurally evaluate the results by pressing the “play” and “stop” buttons to listen to the original and the enhanced speech signals. An illustration showing more details about the “recording” page is shown in Fig. B and Fig. C. 


## Download

* Download apk for Android.

|| Google drive | Dropbox | 
|:------:|:------:|:------:| 
|URL| [links](https://drive.google.com/file/d/1FyfM3gcELodCzqN3zodJXp4hRjGQS4oF/view)|[links](https://www.dropbox.com/s/ljydb8afzpczaw2/denoiser_pytorch_211122.apk)|
|QR code |<img src="https://github.com/yuwchen/CITISEN/blob/master/images/CITISEN_qrcode_google.png" alt="main"  width=100% height=100% />|<img src="https://github.com/yuwchen/CITISEN/blob/master/images/CITISEN_qrcode.png" alt="main"  width=100% height=100% />|
  
* [Download] CITISEN for iOS.

## Paper 
* See [Paper](https://arxiv.org/pdf/2008.09264.pdf) for more detail. 

## Results and demo
* You can listen to some samples on the [Demo webpage](https://bio-asp-lab.github.io/CITISEN_demo/).

## Citations
@misc{alex2020citisen,  
  title={CITISEN: A Deep Learning-Based Speech Signal-Processing Mobile Application},  
  author={Alexander Chao-Fu Kang and Kuo-Hsuan Hung and Yu-Wen Chen and You-Jin Li and Ya-Hsin Lai and Kai-Chun Liu and Sze-Wei Fu and Syu-Siang Wang and Yu Tsao},   
  year={2020},  
  eprint={2008.09264},  
  archivePrefix={arXiv},  
  primaryClass={eess.AS}  
    }


## License
* The CITISEN work is released under MIT License. See LICENSE for more details.

## Acknowledgments
* [Bio-ASP Lab](https://bio-asplab.citi.sinica.edu.tw), CITI, Academia Sinica, Taipei, Taiwan

