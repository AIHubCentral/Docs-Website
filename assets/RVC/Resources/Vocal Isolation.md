---
icon: chevron-right
order: 5000
---

``Last update: Feb 29, 2024``  

***
###### ‎
:::content-center
## Introduction :icon-book:
:::     
- A vocal isolation app is a software designed to extract a person's vocals from an audio file, usually through the use of AI models.

- They can remove undesired noises, like background noise, reverb, echo, music, etc.    

- The goal is to get an audio sample with clean vocals, which is what RVC needs to give the most accurate & quality results.

- For RVC users, the best app is Ultimate Vocal Remover 5 (or **UVR**). It can be used either <u>[locally](https://docs.ai-hub.wtf/extra/glossary/#local-running)</u> or through the <u>[cloud](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#cloud-uvr-)</u>.

- If you want to remove noise manually to avoid ai artifacts you can use RX 11, which is mentioned in this guide. 
***
<img src="../uvrmvsep-img/3.jpg" alt="image" width="" height="auto">‎       

###### ‎ 
:::content-center
## Local UVR
!!!warning 
*You'll require great specs & GPU to run it effectively. Otherwise, use either the <u>[google colab version](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#cloud-uvr)</u> or the hugging face space.*
!!!
:::
‎ 
:   ‎ 

### Installation :icon-download:
*** 
1. Go to their <u>[official website</u>](https://ultimatevocalremover.com/) & press `Download UVR`. And if you want to use BS Roformer you are going to need to install [this](https://github.com/TRvlvr/model_repo/releases/download/uvr_update_patches/UVR_Patch_4_14_24_18_7_BETA_full_Roformer.exe).

    <img src="../uvrmvsep-img/1.jpg" alt="image" width="" height="auto">   

***
###### ‎ 
2. It will redirect you their GitHub page. Click the download link for your **operating system**.   
UVR is available both on **Windows & Mac**.
***
###### ‎ 
3. Once the installer finishes downloading, execute it & follow the instructions.     
Make sure to tick `🗹 Create a desktop shortcut` for an easier access to UVR.

    <img src="../uvrmvsep-img/2.jpg" alt="image" width="500" height="auto"> 
***
###### ‎       
###### ‎     
### How to Use :icon-checklist:  
***  

==- *Extracting Vocals From Songs 🎶*
###### ‎  
#### 1. Input audio.        
###### ‎  
- Click `Select input` to select your audio/s. Or just drag the files to it.  
‎   
- In `Select output` you can define the folder for the results.      

    <img src="../uvrmvsep-img/4.jpg" alt="image" width="300" height="auto">         ‎    

!!!success 
For better results, have the audio in a <u>[lossless format](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats)</u> (**WAV** or **FLAC**), & not MP3.
!!!
***
‎ 
#### 2. Select FLAC & GPU Conversion.
###### ‎  
a. At the right you can select the output format.       
We recommend picking `FLAC`. Learn why <u>[here](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats)</u>.   
‎  
b. If your GPU is **compatible with <u>[CUDA](https://docs.ai-hub.wtf/extra/glossary/#cuda)</u>**, toggle `GPU Conversion` on for a faster process.    

    <img src="../uvrmvsep-img/16.png" alt="image" width="350" height="auto">‎      

###### ‎       
>This step is not mandatory, but recommended for better results.
***
‎
#### 3. Extract vocals. 
###### ‎  
a. In **CHOOSE PROCESS METHOD** select `MDX-Net`, and select either the `BS Roformer-Viper-X 1296` or `MDX23C` model.   

    <img src="../uvrmvsep-img/5.jpg" alt="image" width="250" height="auto">‎      
###### ‎  
###### ‎    
b. Now click the long `Start Processing` button.    
###### ‎  
!!!success 
<u>**TIP:**</u> To **test** models/options more efficiently, tick `Sample Mode` to only process 30 seconds of your sample.
!!!   
***
‎
#### 4. Clean vocals. 
###### ‎    
- Usually songs include reverb & backing vocals. These **negatively** impact the results in RVC. 

- So if the output has any undesired noises, follow the procedure on **Cleaning Vocals**.       
‎  
===

==- *Cleaning Vocals 🗣️*

###### ‎    
#### 1. Input audio.
###### ‎      
- Click `Select input` to input the vocals. Or just drag the files to it.  
‎   
- In `Select output` you can define the folder for the results.    

    <img src="../uvrmvsep-img/4.jpg" alt="image" width="300" height="auto">         ‎    

!!!success 
For better results, have the audio in a [lossless format](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats)</u> (**WAV** or **FLAC**), & not MP3.
!!!
***
‎   
#### 2. Select FLAC & GPU Conversion.
###### ‎      
a. At the right you can select the output format.       
We recommend picking `FLAC`. Learn why <u>[here](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats)</u>.     
‎   
b. If your GPU is **compatible with <u>[CUDA](https://docs.ai-hub.wtf/extra/glossary/#cuda)</u>**, toggle `GPU Conversion` on for a faster process.    
    ‎       
        <img src="../uvrmvsep-img/16.png" alt="image" width="350" height="auto">‎      
###### ‎       
>This step is not mandatory, but recommended for better results.
***
‎   
#### 3. Select model.  
###### ‎      
a. In **Process Method** select `VR`.     
‎   
b. Set **Window Size** to ``320``. (optional)        
Lower Window Size yield a higher output **quality**, but will take **longer** to process.   
‎   
b. Check the <u>[model list](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#best-models)</u>. In **Select VR Model** pick the one according to what you need to remove.         
‎       
If you need to remove multiple noises, follow this pipeline for the best results:   
``Remove instrumental -> Remove reverb -> Extract main vocals -> Remove noise``  
###### ‎  
!!!success 
<u>**TIP:**</u> To **test** models/options more efficiently, tick `Sample Mode` to only process 30 seconds of your sample.
!!!  
***
‎  
#### 4. Process.
###### ‎      
Click the `Start processing` button at the bottom. And that will be all. 

***
###### ‎  
:::content-center
[!button variant="danger" size="m" corners="pill" icon="heart-fill" iconAlign="right" text="Support UVR"](https://www.buymeacoffee.com/uvr5)
:::     
‎  
===

!!!success
*If an issue arises, read the **Troubleshooting** chapter.*
!!!
***
###### ‎   
###### ‎       
### Troubleshooting :icon-tools:

***

==- *A model isn't there.*
###### ‎ 
- Click the wrench (🔧) on the left & go to `Download Center`
- Select the category of the model (MDX-NET or VR)
- Unfold its dropdown & select the model that you need
- Then click the download button (📥). The model will download, which will take a few minutes
===

==- *UVR extracted too little/too much.*
###### ‎
- Modify the `Aggression Setting` value on the right. 
- This determines the **depth** of the extraction. Only the **VR** method has it.
- A higher value will deepen the extraction, and a lower one will soften it.
- Each audio is different, so you'll have to test the ideal value.
===

==- *I can't remove some of the backing vocals.*
###### ‎
- Run the audio through BVE. Modify the <u>[Aggression Setting](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#uvr-extracted-too-little-too-much)</u> if necessary.
===

==- *I couldn't find my answer.*
###### ‎   
- Report your issue <u>[here](https://docs.ai-hub.wtf/rvc/#contributions)</u>.
===

***
###### ‎ 
###### ‎ 
:::content-center
## X-Minus Pro
‎ 
:   ‎ 
:::

### How to Use :icon-checklist:

***

!!!warning
Most of the extraction model are behind a pay wall.
!!!

==- *Extrating Vocals From Songs* 🎶
###### 
#### 1. Choose a Separator
######
a. First go to <u>[X-minus's website](https://x-minus.pro)</u> and click the "Vocal Remover" at the top right. 

<img src="../x-minus-img/1.png" alt="image" width="600" height="auto"> 

b. Then select "Music and vocals" and choose "Bs Roformer"
  
<img src="../x-minus-img/2.png" alt="image" width="600" height="auto">

***
#### 2. Upload Your Audio File

c. Then click "select a file" and choose a audio file, or you can drag and drop a file. And when it's done it will look like this: 

<img src="../x-minus-img/3.png" alt="image" width="600" height="auto">

d. You can now click "Vocals" to download the vocals and "Other" to download the instrumentals.

===

==- *Cleaning Vocals* 🗣️
######
#### 1. Choose a De-Noiser
######
a.  In "De-Noise" select "Mel-Roformer De-Noise". You can also check the [model list](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#best-models) to see what is the best model for your needs.

<img src="../x-minus-img/4.png" alt="image" width="600" height="auto">

***
#### 2. Upload Your Audio File

c. Then click "select a file" and choose a audio file, or you can drag and drop a file. And when it's done it will look like this: 

<img src="../x-minus-img/3.png" alt="image" width="600" height="auto">

d. You can now click "Vocals" to download the vocals and "Other" to download the instrumentals.

===



###### ‎ 
:::content-center
## Cloud UVR
‎ 
:   ‎ 
:::

### How to Use :icon-checklist:

***
==- *Extracting Vocals From Songs* 🎶
###### ‎       
#### 1. Set up Colab
###### ‎ 
a. First access the Colab space <u>[here](https://colab.research.google.com/github/Eddycrack864/Music-Source-Separation-Universal-Colab/blob/main/Music_Source_Separation_Universal_Colab.ipynb)</u>. This Colab only uses **WAV** audios. If yours isn't, convert it to WAV or use <u>[MVSEP](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#mvsep)</u>.     
‎       
b. Then **Log in** to your Google account.      
‎   
c. Execute the **Setup** cell by pressing the play button :icon-play:. Grant all the permissions.   
‎   
    <img src="../uvrmvsep-img/3-setup.png" alt="image" width="350" height="auto">‎   
‎   
- It'll finish once the logs say "Ready!".     
‎   
    <img src="../uvrmvsep-img/3-check.png" alt="image" width="200" height="auto">

***

‎  
#### 2. Set up folders
###### ‎ 
- In Google Drive, make two folders, named **Separar** & **Vocales**.       
‎       
    <img src="../uvrmvsep-img/3-folders.png" alt="image" width="370" height="auto">     
‎     
‎     
- Name them as you want, as long as the input/output folders match the paths.      
‎       
    <img src="../uvrmvsep-img/3-paths.png" alt="image" width="400" height="auto">
***
‎  
#### 3. Separate
###### ‎   
a. Select the ``MDX23C 8KFFT InstVoc HQ 2`` model & run the **Separation** cell.     
‎   
    <img src="../uvrmvsep-img/3-model.png" alt="image" width="320" height="auto">‎   
‎       
‎   
b. Download the result located in the output folder.
***
‎
#### 4. Clean vocals
###### ‎    
- Usually songs include reverb & backing vocals. These **negatively** impact the results in RVC.    
‎   
- So if the output has any undesired noises, follow the procedure on **Cleaning Vocals**.     
‎  
===

==- *Cleaning Vocals* 🗣️ 
#####  ‎  ‎ 
#### 1. Set up Colab
###### ‎
a. Access the Colab space <u>[here](https://colab.research.google.com/github/Eddycrack864/Ultimate-Vocal-Remover-5.6-for-Google-Colab/blob/main/Ultimate_Vocal_Remover_5_6_for_Google_Colab.ipynb)</u> & **Log in** to your Google account. Credits to <u>[Eddy](https://github.com/Eddycrack864)</u> for the Colab.         
‎   
b. Execute the **Install** cell. This will take around 5 - 10 minutes.     
‎   
<img src="../uvrmvsep-img/3-install.png" alt="image" width="270" height="auto">‎  
‎    
- It'll finish once the logs say "Installation Completed".      
‎    
<img src="../uvrmvsep-img/3-installdone.png" alt="image" width="270" height="auto">‎    

***
‎ 
#### 2. Run UI
###### ‎ 
a. Then below run the **WebUI** cell. This will take around 3 minutes.      
***For advanced users***, tick `VIP_MODELS` if you wish to use them.        
‎    
<img src="../uvrmvsep-img/3-webui.png" alt="image" width="310" height="auto">‎    
‎      
‎    
b. Open the **public URL**. That **Gradio** link contains the UVR app.      
‎       
    <img src="../uvrmvsep-img/20.png" alt="image" width="425" height="auto">‎  
###### ‎  
!!!warning 
Don't close **Colab** until you're done using it, and don't press buttons continuously too **quickly**, as it may cause errors.         
!!!
***
‎    
#### 3. Select vocals & options
###### ‎  
a. Tap the **Input Audio** box & select your audio, or simply drag & drop.     
‎        
    <img src="../uvrmvsep-img/21.png" alt="image" width="425" height="auto">‎           
‎       
‎       
b. Once it's done uploading, in **CHOOSE PROCESS METHOD**, select ``VR Arc``.       
‎   
<img src="../uvrmvsep-img/22.png" alt="image" width="600" height="auto">‎       
‎       
‎       
c. On the left, tick `GPU Conversion` & set **WINDOW SIZE** to `320`.       
Lower Window Size yield a higher output **quality**, but will take **longer** to process.       
‎    
<img src="../uvrmvsep-img/3-options.png" alt="image" width="300" height="auto">‎ 
*** 
‎ 
#### 4. Select model
###### ‎  
d. Check the <u>[model list](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#best-models)</u> & in **CHOOSE VR MODEL** pick the one according to what you need to remove.    
‎       
If you need to remove multiple noises, follow this pipeline for the best results:   
``Remove instrumental -> Remove reverb -> Extract main vocals -> Remove noise``  
***
‎  
#### 5. Start Processing
###### ‎  
a. Click **Start Processing** below. Wait a moment for the audio to process.       
‎       
b. Playable audios will then appear in the output boxes below. To download the output, click the three dots on the right and `Download`.            
     
- If you're extracting lead vocals, remember to download the backing ones if you wish to keep them.    

!!!success 
**TIP:** To **test** models/options more efficiently, tick **Sample Mode** to only process 30 seconds of your sample.
!!!  

===

!!!success
*If an issue arises, read the **Troubleshooting** chapter.*
!!!
***

###### ‎  
###### ‎  

### Troubleshooting :icon-tools:
***
==- *UVR extracted too little/too much.*
###### ‎
- Modify the `Aggression Setting` value on the right. 
- This determines the depth of the extraction. Only the VR method has it.
- A higher value will deepen the extraction, and a lower one will soften it.
- Each audio is different, so you'll have to test the ideal value.
===

==- *I can't remove some of the backing vocals.*
- Run the audio through MDX23C or DeNoise. Modify the Aggression Setting if necessary.
===

==- *I get a red error message.*
- This is normal. Try repeating your action.
- If it persists, reload the Gradio page.
===

==- *Cannot connect to GPU backend.*
###### ‎   
- You have exhausted the <u>[GPU runtime](https://docs.ai-hub.wtf/rvc/extra/glossary/#google-colab)</u> of Colab.
===

==- *I couldn't find my answer.*
###### ‎   
- Report your issue <u>[here](https://docs.ai-hub.wtf/rvc/#contributions)</u>.
===

***

######
:::content-center
## UVR Zero GPU 
:::
***
###### ‎  
######

## How to use :icon-checklist:

***

==- Extract vocals
###### ‎

Access the space <u>[here](https://huggingface.co/spaces/TheStinger/UVR5_UI)</u>, you don't need an account to use this.           
    
#### 2. Select vocals & options
###### ‎  
a. Tap the **Input Audio** box & select your audio, or simply drag & drop.     
‎        
<img src="../hugging-img/1.png" alt="image" width="1000" height="auto">‎           
‎       
‎       
b. Once it's done uploading, in **CHOOSE PROCESS METHOD**, select ``BS/Mel Roformer``. Under that you can change **Segment Size** and **Overlap**, the defaults are fine.   
‎   
<img src="../hugging-img/2.png" alt="image" width="1000" height="auto">‎              

‎ 
#### 3. Select model
###### ‎  
d. Check the <u>[model list](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#best-models)</u> & in **CHOOSE MODEL** pick the one according to what you need to remove.    
‎       
If you need to remove multiple noises, follow this pipeline for the best results:   
``Remove instrumental -> Remove reverb -> Extract main vocals -> Remove noise``  
‎  
#### 4. Start Processing
###### ‎  
a. Click **Spererate!** below. Wait a moment for the audio to process.       
‎       
b. Playable audios will then appear in the output boxes below. To download the output, click the little download icon in the top right.            
     
- If you're extracting lead vocals, remember to download the backing ones if you wish to keep them.     
===

!!!success
*If an issue arises, read the **Troubleshooting** chapter.*
!!!
***

###### ‎  
###### ‎  

### Troubleshooting :icon-tools:
***
==- *UVR extracted too little/too much.*
###### ‎
- Modify the `Aggression Setting` value on the right. 
- This determines the depth of the extraction. Only the VR method has it.
- A higher value will deepen the extraction, and a lower one will soften it.
- Each audio is different, so you'll have to test the ideal value.
===

==- *I can't remove some of the backing vocals.*
- Run the audio through BVE. Modify the Aggression Setting if necessary.
===

==- *I couldn't find my answer.*
###### ‎   
- Report your issue <u>[here](https://docs.ai-hub.wtf/rvc/#contributions)</u>.
===

==- Errors
#### GPU task aborted:
ZeroGPU HuggingFace Spaces have a max inference time duration, it’s the time it takes to do an Inference (use the model, not the time of your audio file itself), on default it’s around 1 minute which is what Ilaria RVC uses. You need to retry with a shorter audio, you could also split your audio.
***
#### You have exceeded your GPU quota ( NUMBER s left vs. 60s requested). Sign-up on Hugging Face to get more quotas or retry in Hour:Minutes:Seconds
ZeroGPU HuggingFace Spaces have a quota per account, if you aren’t signed in you will get less quota so it’s better to login for more quota. You could get the ‘Sign-up’ part even if you are logged in. The ZeroGPU Quota can’t be seen but it isn’t unlimited. You can either:
- Login so you get more quota
- Wait
- Pay to be an HuggingFace PRO Member to get X5 times more quota

===

***

###### ‎
###### ‎ 
:::content-center
## RX 11
:::
‎ 
:   ‎ 

### Installation :icon-download:
*** 
1. Go to their <u>[official website</u>](https://www.izotope.com/en/shop/rx-11-advanced/?srsltid=AfmBOor--irjtR7Bsl08_bPj-7UMUGd49tYy9C_U2iXOAupjQ74Mat_s) & buy it or sail the seven seas and find a treasure box which contains RX 11. 
***
###### ‎ 
### Usage 
2. To use RX 11 it is **STONGLY** recommended that you read this <u>[guide](https://rentry.co/RVC-dataset-RX11)</u> on RX 11.
***

###### ‎  
:::content-center     
## MVSEP
:::
‎      
:   ‎

###### ‎ 
### Important Notes ‎ :icon-alert:
***
- MVSEP is a website for isolating vocals, that works similarly as UVR.

- The <u>[UVR Colab](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#cloud-uvr)</u> is much faster & convenient for this task. Use MVSEP if you run out of GPU runtime or feel lazy to convert your audio to WAV.

- For free users, you can't convert audios in batches or longer than 10 minutes. If that's your case, trim it into different pieces.
***
###### ‎ 
###### ‎  
### How to Use ‎ :icon-checklist:
***
==- *Extracting Vocals From Songs* 🎶
###### ‎     
#### 1. Log in.  
###### ‎
a. First, make an account <u>[here</u>](https://mvsep.com/register).        
‎       
b. Once logged in, go to the <u>[main page</u>](https://mvsep.com).     

!!!
Logging in is not mandatory, but recommended for **shorter waiting lists**.
!!!
***
‎
#### 2. Select audio.   
###### ‎
a. Click `Browse File` & select your audio, or simply drag & drop. The audio will begin to upload.  

    
    <img src="../uvrmvsep-img/9.png" alt="image" width="330" height="auto">‎   
    
***
‎
#### 3. Extract vocals.
###### ‎
a. In **Separation type** select `BS Roformer`     
‎     
b. In **Output encoding** select `FLAC`.          
We recommend selecting FLAC from now on. Learn more <u>[here</u>](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats).        
‎     
c. Once the audio is done uploading, click `Separate`       

    <img src="../uvrmvsep-img/11.png" alt="image" width="400" height="auto">‎   

!!! Leave "Model Type" untouched.
!!!
***
‎
#### 4. Download output.      
###### ‎
- When it's done converting it will redirect you to a page where you can listen the results.      
     
a. Tap the three buttons of the **Vocals** audio and then `Download`.    
‎     
b. Same thing for the **Instrumental**, if you wish to keep it.      

    <img src="../uvrmvsep-img/12.png" alt="image" width="400" height="auto">‎   
***

‎
#### 4. Clean vocals
###### ‎    
- Usually songs include reverb & backing vocals. These **negatively** impact the results in RVC.    
‎   
- So if the output has any undesired noises, follow the procedure on **Cleaning Vocals**.     
‎  
===

==- Cleaning Vocals 🗣️   
###### ‎     
#### 1. Log in.  
###### ‎
a. First, make an account <u>[here</u>](https://mvsep.com/register).      
‎     
b. Once logged in, go to the <u>[main page</u>](https://mvsep.com).     

!!!
Logging in is not mandatory, but recommended for **shorter waiting lists**.
!!!
***
‎
#### 2. Select audio & output format.    
###### ‎
a. Click `Browse File` & select your audio, or simply drag & drop. The audio will begin to upload.      
‎     
    <img src="../uvrmvsep-img/9.png" alt="image" width="330" height="auto">‎        
‎       
‎     
b. In **Output encoding** select `FLAC`.      
We recommend selecting FLAC from now on. Learn more <u>[here</u>](https://docs.ai-hub.wtf/extra/glossary/#lossless-formats).        

    <img src="../uvrmvsep-img/10.png" alt="image" width="420" height="auto">‎    
***
‎
#### 3. Select model.  
###### ‎
a. In **Separation Type**, select `DeNoise by aufr33`.      
‎     
b. Check the <u>[model list](https://docs.ai-hub.wtf/rvc/resources/vocal-isolation/#best-models)</u>. Pick the one according to what you need to remove.         
‎       
If you need to remove multiple noises, follow this pipeline for the best results:       
``Remove instrumental -> Remove reverb -> Extract main vocals -> Remove noise`` 
*** 
‎
#### 4. Download output.       
###### ‎
a. Click `Separate` & when it's done converting it will redirect you to a page, where you can listen the results.    
‎     
b. Tap the three dots of the audio you need and then `Download`.    
If you wish to keep the backing vocals stem, remember to download it too.      
      
    <img src="..\uvrmvsep-img\12.png" alt="image" width="400" height="auto">‎   
***
:::content-center
[!button variant="danger" corners="pill" icon="heart-fill" iconAlign="right" text="Support MVSEP"](https://mvsep.com/billing)
:::

===

!!!success
*If an issue arises, read the ***Troubleshooting*** chapter.*
!!!

***
###### ‎ 
###### ‎ 
### Troubleshooting ‎ :icon-tools:
***
==- *MVSEP extracted too much/too little.*
###### ‎ 
- Using the **Separation Type** of `DeNoise by aufr33`, you can modify the `Aggressiveness`. 
This determines the depth of the extraction.
- A higher value will deepen the extraction, and a lower one will soften it.
- Each audio is different, so you'll have to test the ideal value.
===

==- *I can't remove some of the backing vocals.*
###### ‎ 
- Try running the audio through MelBand Karaoke or BVE. Modify the Aggression Setting if necessary.
===

==- *I couldn't find my answer.*
###### ‎   
- Report your issue <u>[here](https://docs.ai-hub.wtf/rvc/#contributions)</u>.
===
***       
###### ‎ 
###### ‎ 
:::content-center
## Best Models
#### `Their most convenient models, oriented to RVC.`    
###### ‎ 
:::

+++ UVR
Extraction | Process Method | Model
:---: | :---: | :---:
Vocals/Instrumental | MDX-Net | BS Roformer-Viper-X 1296 / 1297
Reverb | VR | UVR-DeEcho-DeReverb
Main Vocals | VR | UVR-BVE-4B_SN-44100-1
Noise | VR | UVR-DeNoise 

+++ MVSEP
Extraction | Separation Type | Model
:---: | :---: | :---:
Vocals/Instrumental | BS Roformer | ver 2024.08
Reverb | Reverb Removal | Reverb removal by anvuew (BS Roformer)
Main Vocals | MelBand Karaoke | Extract from vocals
Noise | DeNoise by aufr33  | Aggresive 

+++ X-Minus
Extraction | Model
:---: | :---: 
Music and Vocals | BS Roformer
De-Reverb | MDX23C (De-Reverb)
Extract Backing Vocals | UVR BVE 2 
De-Noise | Mel Roformer De-Noise 

+++
***
###### ‎
:::content-center
#### `You have reached the end.`

[!badge variant="info" size="xl" corners="pill" icon="paper-airplane" iconAlign="right" text="Report Issues"](https://docs.ai-hub.wtf/rvc/contributions/)
:::
