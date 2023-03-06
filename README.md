# <p align=center>Bento800🍱</p>

![Figure from paper](Overview.png)

## 🎑 News
* [23/03/06] **Bento800🍱_Text📝** is released.
* [22/10/22] [**Paper**](https://dl.acm.org/doi/10.1145/3552485.3554935) and **Bento800🍱 (Version1.0)** are released.
* [22/09/13] Add Bento800 creation process.
* [22/08/04] This repo is created.

## 🍀 Overview

**Bento800** is the **first manually annotated** synthetic box lunch presentation dataset for novel **aesthetic box lunch presentation design**.

**Bento800** is composited from **34** single food images in **6** categories: 

<p align=center> Rice🍚(10) ; Fried Chicken🍗(5) ; Salt-grilled Salmon🐟(5) ; Tamagoyaki🧈(6) ; Croquette🍪(5) ; Fried Shrimp🍤(3) </p>

with **3** different types of food presentations: 

(1) Place fried chicken on rice; 

(2) Place salt-grilled salmon and tamagoyaki on rice; 

(3) Place croquette and fried shrimp on rice, the fried shrimp is on the croquette.

## 🌱 Dataset Creation Process
### Bento800🍱_Text📝
* Image Details

| Content | Tools | Details|
|  :----: | :----: | :----------|
| Resize | - | Paste images in Bento800 onto a transparent image.|

* Text Description Details

| Content | Tools | Details|
|  :----: | :----: | :----------|
| Text Paraphrasing | [ChatGPT](https://chat.openai.com/auth/login) | Rephrase the above sentences with the template “**Rephrase: [Input] with 25 examples**” and “**Rephrase: [Input]**"+"**Please try again**"&times;24.|

### Bento800🍱
* Image Details

| Content | Tools | Details|
|  :----: | :----: | :----------|
| Image Collection | [Google Image](https://www.google.com/imghp) | These high-resolution images contain **at least one complete food item**.|
| Remove Background | [removebg](https://www.remove.bg/) | Remove the background and unnecessary parts.|
| Image Compositing | - | Manually composite + random data augmentation.|

* Annotation Details

| Content | Tools | Details|
|  :----: | :----: | :----------|
| Modal Segmentation | [Dataloop](https://dataloop.ai/) | Manually marked visible parts and occluded parts.|
| Food Item Labels & Bounding Box & Ordering List | [VGG Image Annotator (VIA)](https://www.robots.ox.ac.uk/~vgg/software/via/via_demo.html) | Manually annotated several food item attributes.|




## 🎁 Download

| Content | Size | Files | Format | Details |
| :---- |  :----:  |  :----: | :----: | :----------|
| **Bento800🍱_Text📝** [[Google Drive](https://drive.google.com/drive/folders/1_VvAbIzeuVew4fa98CcE11mB9SoAI3q-?usp=sharing)] [[Tencent Cloud](https://share.weiyun.com/dqrudYM8)]| - | 1600 | | Main Folder|
| &boxvr;&nbsp; [Image](https://drive.google.com/drive/folders/1hNPdDelpsuLvx-Ts5dGWjPBKidgRvjNj?usp=sharing) | 216MB | 800 | PNG | Food images from Bento800 of size 600&times;600
| &boxvr;&nbsp; [Text](https://drive.google.com/drive/folders/1I7xcVwWHvc0T8yPw-_2XKlnZRm3tMnW-?usp=sharing) | 793 KB | 800 | TXT | 9 descriptions for each image in Bento800

| Content | Size | Files | Format | Details |
| :---- |  :----:  |  :----: | :----: | :----------|
| **Bento800🍱v1.0** [[Google Drive](https://drive.google.com/drive/folders/11BoD8z5TmhwSfdo9juiGbYsJnGQwrRx0?usp=sharing)] | - | 872 | | Main Folder|
| &boxvr;&nbsp; [S1_collection](https://drive.google.com/drive/folders/1kc7d1BHvLqx2C0zuI6ryrBjePdPtDwm5?usp=sharing) | 3.26 MB | 34 | JPG | 34 food images in 6 categories |
| &boxvr;&nbsp; [S2_removebg](https://drive.google.com/drive/folders/1YW1qGMHdwLeU_HjBREm4VMmVYVaF-8gA?usp=sharing) | 2.81 MB | 34 | PNG | Remove Background |
| &boxvr;&nbsp; [S3_train](https://drive.google.com/drive/folders/1FQ7VbOMQfi-0xFb2wjgsI8PV4VS8C8Jy?usp=sharing) | 410 MB | 766 | PNG | Training images |
| &boxvr;&nbsp; [S3_val](https://drive.google.com/drive/folders/1qda3UC653ACx7mY3DR45LG-HYu2pBl-N?usp=sharing) | 18.8 MB| 34 | PNG | Testing images |
| &boxvr;&nbsp; [S4_segmentation](https://drive.google.com/drive/folders/1k-d7ABYK1FTDLiTUA3XQLa-HqKV64hH6?usp=sharing) | 8.72 MB | 2 | JSON | Semantic Segmentation |
| &boxvr;&nbsp; [S5_annotation](https://drive.google.com/drive/folders/1FtWZWGi533BqWXhojrGfbbBPmdgw63Vh?usp=sharing) | 403 KB | 2 | CSV | Simple text descriptions + Ordering id + Bounding Box + Food item labels|

## 📚 Feedback

Please fill out the [Bento800 Dataset Feedback Form](https://forms.gle/jqS1PEKwmrCpqZL76).

I  would greatly value your thoughts, suggestions, concerns or problems.

## ⭐ Citation

#### <p align=center>“We eat🍴 first with our eyes👀~ ”</p>

If you find this dataset helpful for your research, please cite it as below:

```bibtex

@inproceedings{zhou2022able,
  title={ABLE: Aesthetic Box Lunch Editing},
  author={Zhou, Yutong and Shimada, Nobutaka},
  booktitle={Proceedings of the 1st International Workshop on Multimedia for Cooking, Eating, and related APPlications},
  pages={53--56},
  year={2022}
}

```
