# Encoder-Decoder-based Video Captioning

This repository provides an ***Encoder-Decoder Sequence-to-Sequence*** model to generate captions for input videos. Moreover, ***pre-Trained VGG16 model*** is being used to extract features for every frame of the video.

The ability to be applied for numerous applications mark ***Video Captioning***'s importance. For example, it can be applied to help search videos across web pages in an efficient manner and it can also cluster the videos having a large degree of similarity in terms of their respective generated captions.

## Requirements
- `Tensorflow`
- `Keras`
- `OpenCV`
- `NumPy`
- `FuncTools`

## Usage
### Data
- The ***MSVD*** dataset developed by Microsoft can be downloaded from [***here***](https://www.dropbox.com/sh/whatkfg5mr4dr63/AACKCO3LwSsHK4_GOmHn4oyYa?dl=0).
- This data set contains 1450 short YouTube clips that have been manually labeled for training and 100 videos for testing.
- Each video has been assigned a unique ID and each ID has about 15–20 captions.
### Training and Testing
- To extract features for frames of every single input videos using pre-Trained VGG16 model, run `Extract_Features_Using_VGG.py`.
- To train the developed model, run `training_model.py`.
- To use the trained ***Video Captioning*** model for inference, run `predict_model.py`.
- To use the trained model for ***real-time Video-Caption generation***, run `Video_Captioning.py`.

## Results
Following are a few results of the developed ***Video Captioning*** approach on test videos:-
| Test Video        | Generated Caption           |
| ------------------- |:----------------------------:|
| ![alt text](https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/0lh_UWF9ZP4_62_69.gif) | a woman is mixing some food |
| <img src="https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/7NNg0_n-bS8_21_30.gif" width="320"> | a man is performing on a stage |
| ![alt text](https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/ezgif-4-989de822710c.gif) | a man is mixing ingredients in a bowl |
| <img src="https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/Je3V7U5Ctj4_569_576.gif" width="320"> | a man is spreading a tortilla |
| <img src="https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/qeKX-N1nKiM_0_5.gif" width="320"> | a woman is seasoning some food |
| ![alt text](https://github.com/fork123aniket/Encoder-Decoder-based-Video-Captioning/blob/main/input_videos/TZ860P4iTaM_15_28.gif) | a cat is playing the piano |

