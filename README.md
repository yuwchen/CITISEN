# CITISEN
<a href="https://www.youtube.com/watch?v=BUfY64TCXi4&feature=youtu.be" target="_blank"><img src="https://i.imgur.com/z90yoJp.png" 
alt="CITISEN video"  width=80% height=80% border="10" text-align: center /></a>


## Introduction
In this work, we present a deep-learning-based speech signal processing mobile application, termed CITISEN, which supports three functions: speech enhancement (SE), acoustic scene conversion (ASC), and model adaptation (MA). For the SE function, CITISEN could effectively reduce noise components from speech signals and accordingly enhance their clarity and intelligibility. For the ASC function, CITISEN converts the current background sound to that sounds like a different background. Finally, the MA function in CITISEN can effectively adapt SE models with few audio files when encountering unknown speaker or unseen noise types; the adapted SE model is used to carry out enhancement on the upcoming noisy utterances. Experimental results have confirmed the effectiveness of these three functions in terms of objective evaluation and subjective listening tests. The promising results reveal that the developed CITISEN mobile application can be potentially used as a front-end processor for various speech-related services, such as voice communication, assertive hearing devices, and virtual reality headsets.

## User interface and usage

### Four main pages in CITISEN
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/main.png" 
alt="main"  width=60% height=60% />

The CITISEN application has four pages, "Speech Enhancement", "Acoustic Scene Conversion", "Model Adaptation", and "Recording". The page name and the navigator buttons of each page are listed on the top-left and bottom in the application, respectively.

### Speech Enhancement page
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/SE.png" 
alt="main"  width=60% height=60% />

For the "Speech Enhancement" page, a user first specify his/her gender identity. Then, by pressing the "SE Model Switch" button, the user can select one suitable SE models from a listed of saved models. CITISEN provides several default SE models trained using our own collected speech data sets. Users can also run MA to prepare adapted SE models and save them as new SE models. Then, by pressing the SE button, the noisy speech is then transformed to clean one online.

### Acoustic Scene Conversion page
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/ASC.png" 
alt="main"  width=60% height=60% />

In the "Acoustic Scene Conversion" page, CITISEN mixes acoustic scene on enhanced speech to generate new speech signals with converted acoustic scene. The "Acoustic Scene Conversion" page has a "Record Noise" button, by which users can record and save noise signals for ASC. Meanwhile, the page has a volume bar by which allows users to adjust the volume of background noise and accordingly specify the SNR level of converted speech. To change the acoustic scenes, users first press “SE Model Switch” button to select an SE model. Then, by pressing “Background Noise Switch” button, as shown in the left side, and an acoustic scene selection window will pop up and list all acoustic scene options, as shown in the right side. Users can select the target scene for ASC, and the speech with converted scene will be generated accordingly.

### Model Adaptation page
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/MA.png" 
alt="main"  width=60% height=60% />

There are two file upload buttons: "Record Noise" and "Record Speech", as shown in the left side. By pressing one of these two buttons, users can record pure noise or speaker speech signals and upload the recorded audio to our server. To start recording, users could simply press on one of the buttons, as shown in left side. Once finishing recording, by pressing the button again, CITISEN will pop up a submitting window, as shown in right side. The submitting window will ask the user to name the audio file, and the audio will be sent to the server. After receiving the audio file, the server will estimate an adapted SE model by fine-tuning the original SE model using the recorded audio data. The name of the audio file will also be used to name the adapted SE model, which is later sent from the server to mobile device and appears in the "Speech Enhancement" and "Acoustic Scene Conversion" pages. Accordingly, users can run SE and ASC functions using the adapted SE model.

### Recording page

A. recording or loading saved audio files

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/Rec.png" 
alt="main"  width=60% height=60% />

B. selecting a model to perform SE

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/Recording3.png" 
alt="main"  width=60% height=60% />

C. demonstrating the processed speech by spectrogram plots

<img src="https://github.com/yuwchen/CITISEN/blob/master/images/Recording2.png" 
alt="main"  width=60% height=60% />


The "Recording" page is for users to record speech and noise of the current environment and also save the enhanced or converted audio files. For the "Speech Enhancement" and "Acoustic Scene Conversion" pages, users can immediately listen to enhanced or converted speech online. On the other hand, the "Recording" page allows users to save and playback later on the processed audio files. Users first record (upper path in Fig. A) or load an existing (bottom path in Fig. A) audio file and then press on the "SE Model Switch" button. Then, an SE model selection window will pop up, as shown on the right of Fig. B. By selecting a suitable SE model and then pressing on run button (as shown on left side of Fig. B), enhanced speech will be generated. CITISEN has the function to demonstrate two spectrogram plots: noisy and enhanced speech spectrogram plots (as shown on right side of Fig. C), so that users can visually check the SE results. In addition to these two plots, users can press "Play" and "Stop" buttons, on top of spectrogram plots, to play and listen the original and processed audio files.
 
 

## Download
* [Download](https://drive.google.com/file/d/1OabFInICw8_PVq5x5TWpaiW1dOuwiaaH/view) CITISEN apk for Android.
<img src="https://github.com/yuwchen/CITISEN/blob/master/images/CITISEN_qrcode.jpg" alt="main"  width=25% height=25% />

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
