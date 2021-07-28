# Algonauts2021-NMA

## Introduction
A Python notebook that contains pre-built functions to load, manipulate and analyze data from the Algonauts 2021 __Mini-Track__ dataset.

This notebook is built on the contributions of Vincent Chooi, Tilek Chubakov, Quentin Lam, Jingyang Ma, Fabian Cabrera, Abdur-Rahman Olanrewaju and Saloni Dabgar, all of whom were project members of the team named *sleepy koalas*, mentored by Hamed Karimi.
The project team is part of the pod *devoted koalas* in Neuromatch Academy's (NMA) 2021 neuroscience session, led by __*the*__ Aastha Sharma.

The notebook and the project as a whole was the fruitful product of the sweat, tears, late-nights and early-mornings of everyone in *devoted koalas*, all great and interesting people. 

### Overview
The Algonauts 2021 Challenge presents a task to predict fMRI voxel activity of subjects, given video as input. The Challenge has two tracks: Full-Track and Mini-Track. This notebook focuses on the Mini-Track and provides the necessary tools to manipulate it, and will not work for the Full-Track. In the Mini-Track, the train set voxel data is divided into 9 non-overlapping RoIs (Region-of-Interest) in the visual cortex, over 10-subjects; whereas the video samples consist of the corresponding 1000 3-second videos that were shown to the subject *without audio*. In the test set, structured similarly, there are 102 samples. 

#### Our Focus Instead
Instead of working on the Challenge, *sleepy koalas* decided to venture into uncharted territory by utilizing the dataset to find out if visual cortex RoIs are semantically-functionally segregated. To give a brief background, current literature (as of 2021) suggests that RoIs of the visual cortex (e.g. EBA, FFA, STS, PPA, LOC) activate preferentially to specific types of stimuli (e.g. EBA to body parts, FFA to faces and LOC to general objects). Our curiosity lies in the question that asks if they really are so, or if they work in conjunction to process large semantic classes of inputs.

The formal hypothesis is stated as follows: 
>Current literature on the visual processing areas of the brain suggests that these regions are modular, such that they are preferentially activated by specific >semantic categories of visual stimuli. We hypothesize that these discrete regions are not selectively activated, but rather, they process general classes of visual >stimuli in conjunction with each other. Specifically, we test the category of human facial features, and whether only FFA & STS activity is predictive of the such >stimuli (i.e. plays a significant role in decoding neural activity in the visual cortex), but also other regions like V1, V2, V3, V4, EBA, LOC & PPA.

#### What We Did
We framed that question into a neural decoding task, whereby we took the voxel data and tried to predict whether the subjects were looking at a specific class of input. Our focus was mainly on human faces, pertaining to the *FFA & STS* region, where the test variable is the presence of *LOC* voxel data. The basic question was: Using FFA & STS data-trained models as baseline, would adding LOC data to the models increase predictive performance? (Spoiler Alert: We found that it hinted toward that possibility, though results were not significant enough to be conclusive.)

Therefore, the tools provided in the notebook will be helpful towards that end. 

### Use
Please give credit to __*devoted koalas* of NMA 2021 Neuroscience__, if you decide to use the notebook and its tools in any substantial work.

All tools are well documented & should be a plug-and-play for anyone who is sufficiently familiar with Python and its machine learning & data analysis libraries. All you need is the original dataset (Mini-Track), which can be downloaded at http://algonauts.csail.mit.edu/challenge.html, and our annotations, included in the repo. However, you will need to re-order the folder structures for it to work on your machine.

</br>

<p align="center">
  <img width="700" alt="Screen_Shot_2021-07-23_at_4 02 17_AM" src="https://user-images.githubusercontent.com/19466657/127380817-b95a1530-baab-4dd1-b1fb-4e3d11beeb10.png">
  <p align="center">Devoted koalas in their common habitat. From top-left to bottom-right: Jingyang Ma, Vincent Chooi, Tilek Chubakov, Abdur-Rahman Olanrewaju, Quentin Lam, Aastha Sharma, Fabian Cabrera. (Saloni Dabgar not present)</p>
</p>



