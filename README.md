# "Automated recognition of optical image based potato leaf blight diseases using deep learning"

**Kulendu Kashyap Chakraborty**, Rashmi Mukherjee, Chandan Chakroborty, Kangkana Bora. \
[https://doi.org/10.1016/j.pmpp.2021.101781](https://www.sciencedirect.com/science/article/abs/pii/S088557652100182X?via%3Dihub), In [Physiological and Molecular Plant Pathology (2021): 101781](https://www.sciencedirect.com/journal/physiological-and-molecular-plant-pathology).

<!-- <p align='center'>
 <img src='https://github.com/kulendu/NITTTR-project/blob/master/images/NITTTR_Kolkata_New_Logo.jpg' width=170px style='border-radius:100%;'>
</p> -->

## 1. Introduction
During some months of the year the potato plants suffer from some leaf diseases, known as *Blights*. These are formed and can be classified as two-staged disease:
- **Early blight** : Early blight of potato is caused by the *fungal pathogen Alternaria solani*. The disease affects leaves, stems and tubers and can reduce yield, tuber size, storability of tubers, quality of fresh-market and processing tubers and marketability of the crop.
In most production areas, early blight occurs annually to some degree. The severity of early blight is dependent upon the frequency of *foliar wetness from rain, dew, or irrigation*; the nutritional status of the foliage; and cultivar susceptibility.
- **Late blight** : Late blight is caused by the fungus like *oomycete pathogen Phytophthora infestans*. This potentially devastating disease can infect potato foliage and tubers at any stage of crop development. The primary host is potato, but P. infestans also can infect other solanaceous plants, including tomatoes, petunias and hairy nightshade, that can act as source of inoculum to potato.

## 2. Comparison of Normal leaf VS Early blight VS Late blight
| Normal leaf |  Leaf with Early blight | Leaf with Late blight |
:-------------------------:|:-------------------------:|:-------------------------:
![](images/normal.JPG)  |  ![](images/early-blight.JPG) | ![](images/late-blight.JPG)

### 2.1. Potato Cropping Period and Late Blight favourable Period
![](images/period.png)

### 2.2. Disease cycle 
- The fungus over-summers as mycelium in the infected seed potato kept in cold stores.
- These tubers when planted in the next crop season (main crop and subsequent ones) serve as the source of primary inoculum.
- When the plants emerge from such tubers, the fungus invades a few of the growing sprouts and sporulates (produce sporangia) under humid conditions. Further spread of the disease takes place by these sporangia through air or rain splashes.
- Initiation of the disease generally takes about 3-7 days before clearly visible symptoms develop. The fungus produces white sporulation on the underside of the leaves which is clearly visible in the early morning hours.
- These sporangia further infect new leaves and stems of the nearby plants and this cycle continues after every 4-10 days depending upon the prevailing temperature and humidity levels.
- If the temperature is lower than 100 C, disease development slows down and takes more time up to 12 days while at temperature of 16-180 C, it takes only 4-5 days to complete one cycle.
- Sporangia washed by rain or carried by irrigation water cause infection on tubers in the soil.
- Partially exposed tubers can easily become infected.
- These infected tubers serve as the primary source of inoculum for the next year's crop.

![](https://www.pau.edu/potato/images/lb66.jpg)



## 3. Abstract
The Potato crop (Solanum tuberosum L.) is one of the most important vegetable food crop grown globally. The
yield of potato crop is greatly hampered both in quality and quantity by fungal blight diseases which pose a
major threat to the global food security. Late blight caused by Phytophthora infestans and early blight caused by
Alternaria solani are the most devastating foliage diseases for potato crops. In reality, the farmers presume such
disorders by visualizing mainly the color change in the potato leaves that is usually risky due to subjectivity and
huge time consumption. Under such situations, there is an urgent need to design computational models that
would automatically detect these diseases rapidly and quantitatively even at its early phase. This paper explores
recent deep learning models for automated recognition of late and early blight diseases based on the optical
images of potato leaves. Initially, four deep learning models viz., VGG16, VGG19, MobileNet and ResNet50 have
been trained with PlantVillage Dataset. It is observed that VGG16 provides the highest accuracy of 92.69% in
comparison with other models. Now, to further enhance the performance of VGG16, fine-tuning of the model has
been done based on the concept of parameter tweaking. The proposed methodology finally achieved 97.89%
accuracy for classification between late and early blight syndromes as compared to healthy potato leaf. This
study showed the detailed architecture of the fine-tuned VGG16 model with validation accuracy and losses. Our
proposed methodology has also been compared with the existing techniques.

## 4. Project overview
To demostrate the working for the proposed project, the figure (below) has all the proposed steps:
![](https://github.com/kulendu/NITTTR-project/blob/master/images/Fig1.png)

## 5. Model Comparision and Evaluation

*include about whast have been done weith the models and model's choosed?*

### 5.1. Model evaluation
| Model | Accuracy (in %) |
:-------------------------:|:-------------------------:|
 VGG16   | 92.06 |
 **VGG16 (fine-tuned**) | **97.89** |
 VGG19 | 80.39 |
 ResNet50 | 73.75 |
 MobileNet | 78.84 |
 
 ***Bold** indicates the model with best performance*
 
 ### 5.2. VGG 16 fined-tuned architecture
 <img src='https://github.com/kulendu/NITTTR-project/blob/master/images/2.png' width=40%>

*Fine-tuned architecture for VGG 16.*
 
### 5.3. Results
<img src='https://github.com/kulendu/NITTTR-project/blob/master/images/a.png' width=60%>

*The above graphs depicts the accuracy and loss for the fine-tuned VGG 16 model.*
<hr>

## 6. Setup
```sh
> git clone git@github.com:kulendu/Automated-recognition-of-optical-image-based-potato-leaf-blight-diseases-using-Deep-Learning.git
```
```sh
> cd Automated-recognition-of-optical-image-based-potato-leaf-blight-diseases-using-Deep-Learning/
```
```sh
> pip install -r req.txt
```

