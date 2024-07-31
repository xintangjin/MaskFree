# Mask_free



##Create Environment:

- Python 3 (Recommend to use [Anaconda](https://www.anaconda.com/download/#linux))

- NVIDIA GPU + [CUDA](https://developer.nvidia.com/cuda-downloads)

- Python packages:

```shell
pip install -r requirements.txt
```

##Prepare Dataset:

Download cave_1024_28 ([One Drive](https://bupteducn-my.sharepoint.com/:f:/g/personal/mengziyi_bupt_edu_cn/EmNAsycFKNNNgHfV9Kib4osB7OD4OSu-Gu6Qnyy5PweG0A?e=5NrM6S)), CAVE_512_28 ([Baidu Disk](https://pan.baidu.com/s/1ue26weBAbn61a7hyT9CDkg), code: `ixoe` | [One Drive](https://mailstsinghuaeducn-my.sharepoint.com/:f:/g/personal/lin-j21_mails_tsinghua_edu_cn/EjhS1U_F7I1PjjjtjKNtUF8BJdsqZ6BSMag_grUfzsTABA?e=sOpwm4)), KAIST_CVPR2021 ([Baidu Disk](https://pan.baidu.com/s/1LfPqGe0R_tuQjCXC_fALZA), code: `5mmn` | [One Drive](https://mailstsinghuaeducn-my.sharepoint.com/:f:/g/personal/lin-j21_mails_tsinghua_edu_cn/EkA4B4GU8AdDu0ZkKXdewPwBd64adYGsMPB8PNCuYnpGlA?e=VFb3xP)), TSA_simu_data ([One Drive](https://1drv.ms/u/s!Au_cHqZBKiu2gYFDwE-7z1fzeWCRDA?e=ofvwrD)), TSA_real_data ([One Drive](https://1drv.ms/u/s!Au_cHqZBKiu2gYFTpCwLdTi_eSw6ww?e=uiEToT)), and then put them into the corresponding folders of `datasets/` and recollect them as the following form:

The RGB data for cave_1024_28_RGB, CAVE_512_28_RGB and KAIST_CVPR2021_RGB are synthesized by this paper, if you use this part of the data please cite our article.  ([Baidu Disk](https://pan.baidu.com/s/1omv6hY4V7H2FtwuPoNh4Eg?pwd=dbw4), code: `dbw4`)
 


```shell
|--Mask-free
    |--simulation
    	|-- test_code
    	|-- train_code
    |--visualization
    |--datasets
        |--cave_1024_28
            |--scene1.mat
            |--scene2.mat
            ：  
            |--scene205.mat
        |--cave_1024_28_RGB
            |--scene1.mat
            |--scene2.mat
            ：  
            |--scene205.mat
        |--CAVE_512_28
            |--scene1.mat
            |--scene2.mat
            ：  
            |--scene30.mat
        |--CAVE_512_28_RGB
            |--scene1.mat
            |--scene2.mat
            ：  
            |--scene30.mat
        |--KAIST_CVPR2021  
            |--1.mat
            |--2.mat
            ： 
            |--30.mat
        |--KAIST_CVPR2021_RGB  
            |--1.mat
            |--2.mat
            ： 
            |--30.mat
        |--TSA_simu_data  
            |--mask.mat   
            |--Truth
                |--scene01.mat
                |--scene02.mat
                ： 
                |--scene10.mat
            |--Truth_RGB
                |--scene01.mat
                |--scene02.mat
                ： 
                |--scene10.mat
        |--TSA_real_data  
            |--mask.mat   
            |--Measurements
                |--scene1.mat
                |--scene2.mat
                ： 
                |--scene5.mat
            |--Measurements_RGB
                |--scene1.mat
                |--scene2.mat
                ： 
                |--scene5.mat
        |--ADAR_1K
            |--split_txt
                |--train_list.txt
                |--valid_list.txt
            |--Train_Spec
                |--ADAR_1k_0001.mat
                |--ADAR_1k_0002.mat
                ： 
                |--ADAR_1k_0900.mat
            |--Train_RGB
                |--ADAR_1k_0001.jpg
                |--ADAR_1k_0002.jpg
                ： 
                |--ADAR_1k_0900.jpg
            |--Valid_Spec
                |--ADAR_1k_0901.mat
                |--ADAR_1k_0002.mat
                ： 
                |--ADAR_1k_0950.mat
            |--Valid_RGB
                |--ADAR_1k_0901.jpg
                |--ADAR_1k_0002.jpg
                ： 
                |--ADAR_1k_0950.jpg
```

Following TSA-Net and DGSMP, we use the CAVE dataset (cave_1024_28) as the simulation training set. Both the CAVE (CAVE_512_28) and KAIST (KAIST_CVPR2021) datasets are used as the real training set. 



Code will coming soon.

## Simulation Experiement:

### Training






### Testing	





