# [FMNIST Colab notebook](https://github.com/stevedepp/FMNIST/blob/master/FMNIST_Depp.ipynb)

A demo of a Colab [notebook's](https://github.com/stevedepp/FMNIST/blob/master/FMNIST_Depp.ipynb) speed and ease of use in building the basics of computer vision classification: 
- [x] retrieving dependencies.  
- [x] retrieving data from Google Drive and loading into Colab environment.  
- [x] exploring data and transforming where necessary.   
- [x] segmenting the data into representative train, validation and test sets. 
- [x] reshaping the sets per model needs.  
- [x] model hyperparameters. 
- [x] running and evaluating DNN and CNN models.  
- [x] employing deconvolutions to review layer activations for tunning model dimensions. 

The colab notebook from this demo video is included in this repo's code library [here](https://github.com/stevedepp/FMNIST/blob/master/FMNIST_Depp.ipynb).

Transcript & slides are below. Please click this demo video to hear it with sound.

![demo](https://user-images.githubusercontent.com/38410965/111723158-7c9b5480-8839-11eb-834a-4c7a0849980c.mp4)











**Steve Depp**   
**462-55**   

**Goals**  
- [x] Colab  
- [x] GPU  
- [ ] Publish Jupyterbook on GitHub (tomorrow)  


**Colab**  
Dislikes  
- A bit laggy   
Likes
- Autocomplete
- Hierarchical section headings
- Github / Drive
- GPU access
   


GPU 

|                 | CPU         | GPU        |
| :---            | :---        | :---       | 
| Fully connected | 17 seconds  | 14 seconds |
| Convolutional   | 377 seconds | 23 seconds |
    

**Steps**  
  
Colab hooks up:  
- [x] Kaggle
- [x] Google drive

Easy to load / explore data:  
- [x] nulls & nans
- [x] greys
- [x] correlations

Performance  
- [x] structure
- [x] accuracy

Under the hood
- [x] activations
- [x] filters
- [x] class activation heatmaps



**Steps**    

Hooked up & Loaded up:  
- [x] Kaggle
- [x] Google docs

<img width="732" alt="Access Google drive Kaggle" src="https://user-images.githubusercontent.com/38410965/112354314-f18be580-8ca2-11eb-9385-e6b6f6420514.png">

<img width="766" alt="Load dataset" src="https://user-images.githubusercontent.com/38410965/112354284-e9cc4100-8ca2-11eb-818e-6c42deffba1b.png">

**Steps**

Looked at the data

- [x] nulls & nans … none

<img width="489" alt="(9, 'Ankle-boot') (4, 'Coat) (9, 'Ankle-boot') (4, 'Coat')" src="https://user-images.githubusercontent.com/38410965/112354225-d9b46180-8ca2-11eb-904a-5faf0273b7e4.png">

- [x] greys
  - light sneakers = 42.79 
  - dark coats = 98.04

<img width="292" alt="Figure Mean pixel values by item" src="https://user-images.githubusercontent.com/38410965/112354179-ce613600-8ca2-11eb-95f7-54e87b7202f5.png">

- [x] correlations
  - boots vs dresses (27%) and t-shirts (25%)
  - dresses vs sandals (17%) and sneakers (20%)
  - train = test

<img width="820" alt="Table Mean correlations amongst images of items in train set" src="https://user-images.githubusercontent.com/38410965/112354148-c73a2800-8ca2-11eb-94d2-3eb0163f983e.png">

<img width="803" alt="Table Mean correlations diff fro" src="https://user-images.githubusercontent.com/38410965/112354104-bee1ed00-8ca2-11eb-98d4-09a902c33ea4.png">

Performance

- [x] Structure 
- [x] Accuracy 

<img width="920" alt="Fully connected" src="https://user-images.githubusercontent.com/38410965/112354048-b25d9480-8ca2-11eb-8e8b-e783b219d705.png">

<img width="945" alt="Confused" src="https://user-images.githubusercontent.com/38410965/112353975-a4a80f00-8ca2-11eb-9a60-303c07ff6628.png">

**Steps**
 
Under the hood
- [x] activations
- [x] filters
- [x] class activation heatmaps

Shirt = 6

![Pasted Graphic 18](https://user-images.githubusercontent.com/38410965/112353921-98bc4d00-8ca2-11eb-8b75-b670e84de64b.png)

Convolutional 2 activation

![Pasted Graphic 25](https://user-images.githubusercontent.com/38410965/112353877-8e01b800-8ca2-11eb-8f8c-1eb77599e2a3.png)

Convolutional 1

<img width="934" alt="Pasted Graphic 19" src="https://user-images.githubusercontent.com/38410965/112353756-70cce980-8ca2-11eb-9794-9c9967afc70c.png">

Convolutional 2

<img width="926" alt="Pasted Graphic 20" src="https://user-images.githubusercontent.com/38410965/112353687-5eeb4680-8ca2-11eb-9292-b65e9367a531.png">

T-shirt = 0

![10](https://user-images.githubusercontent.com/38410965/112353668-572ba200-8ca2-11eb-94a2-1c637460d680.png)

Convolutional 2 activation

![Pasted Graphic 24](https://user-images.githubusercontent.com/38410965/112353626-4b3fe000-8ca2-11eb-90a0-428dab740b62.png)

Convolutional 1

![Pasted Graphic 22](https://user-images.githubusercontent.com/38410965/112353509-2c414e00-8ca2-11eb-9152-3cfc6156cfce.png)

Convolutional 2

![Pasted Graphic 23](https://user-images.githubusercontent.com/38410965/112353459-2186b900-8ca2-11eb-9d72-3661a274b0fc.png)


<img width="762" alt="T-shirt = 0" src="https://user-images.githubusercontent.com/38410965/112353378-12077000-8ca2-11eb-92cb-cafa7265d76e.png">

<img width="934" alt="d Convolutional layer filters" src="https://user-images.githubusercontent.com/38410965/112353296-fdc37300-8ca1-11eb-8db7-f2b42d417c82.png">

**Conclusion**  

Colab is a worth using
- [x] Access to teams
- [x] Access to GPUs

CNN > FC  
- Both generalized
- CNN still climbing at 92%
- Worth it even on a CPU

Under the hood  
- Not much confusion except shirts (6)
- Can remove some filters
