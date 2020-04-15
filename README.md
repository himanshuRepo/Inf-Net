# Inf-Net
code for "Inf-Net: Automatic COVID-19 Lung Infection Segmentation from CT Scans" submit to TMI20.
![alt text](./Inf-Net.png)<br>
Figure 1. The architecture of our proposed Inf-Net model, which consists of three reverse attention (RA) modules connected to the paralleled partial decoder (PPD).

# Semi-Inf-Net
![alt text](./Semi-InfNet.png)<br>
Figure 2. Overview of the proposed Semi-supervised Inf-Net framework.

# Task Description
![alt text](./COVID'19-Infection.png)<br>
Figure 3. Example of COVID-19 infected regions in CT axial slice, where the red and green masks denote the ground-glass opacity (GGO) and consolidation,
respectively. The images are collected from [1].
[1] COVID-19 CT segmentation dataset, link: https://medicalsegmentation.com/covid19/, accessed: 2020-04-11.
# Pre-trained Model
coming soon

# Evaluation Tool
Google Drive: https://drive.google.com/open?id=1BGUUmrRPOWPxdxnawFnG9TVZd8rwLqCF <br>
or <br>
Other link: 

# COVID-SemiSeg Dataset
We also build a semi-supervised COVID-19 infection segmentation (COVID-SemiSeg) dataset, with 100 labeled CT scans from the COVID-19 CT Segmentation dataset [1] and 1600 unlabeled images from the COVID-19 CT Collection dataset [2]. <br>
[1]“COVID-19 CT segmentation dataset,” https://medicalsegmentation.com/covid19/, accessed: 2020-04-11. <br>
[2]J. P. Cohen, P. Morrison, and L. Dao, “COVID-19 image data collection,” arXiv, 2020.<br>
Our COVID-SemiSeg Dataset can be downloaded at google drive: <br>
https://drive.google.com/open?id=1bbKAqUuk7Y1q3xsDSwP07oOXN_GL3SQM <br>
## Training set
1. Lung infection which consists of 50 labels by doctors (Doctor-label) and 1600 pesudo labels generated (Pesudo-label) by our Semi-Inf-Net model.<br>
Download: http://dpfan.net/wp-content/uploads/LungInfection-Train.zip <br>
2. Multi-Class lung infection which also composed of 50 multi-class labels (GT) by doctors and 50 lung infection labels (Prior) generated by our Semi-Inf-Net model.<br>
Download: http://dpfan.net/wp-content/uploads/MultiClassInfection-Train.zip <br>
## Testing set
1. The Lung infection segmentation set contains 48 images associate with 48 GT.<br>
Download: http://dpfan.net/wp-content/uploads/LungInfection-Test.zip <br>
2. The Multi-Class lung infection segmentation set has 48 images and 48 GT.<br>
Download: http://dpfan.net/wp-content/uploads/MultiClassInfection-Test.zip <br>

# Results
To compare the infection regions segmentation performance, we consider the two state-of-the-art models U-Net and U-Net++. We also show the multi-class infection labeling results in Fig. 5. As can be observed, our model, Semi-Inf-Net & FCN8s, consistently performs the best among all methods. It is worth noting that both GGO and consolidation infections are accurately segmented by Semi-Inf-Net & FCN8s, which further demonstrates the advantage of our model. In contrast, the baseline methods, DeepLabV3+ with different strides and FCNs, all obtain unsatisfactory results, where neither GGO and consolidation infections can be accurately segmented. <br>
Overall results: http://dpfan.net/wp-content/uploads/COVID-SemiSeg-Results.zip <br>
## Download link: <br>
Lung infection segmentation results: http://dpfan.net/wp-content/uploads/Lung-infection-segmentation.zip <br>
Multi-class lung infection segmentation: http://dpfan.net/wp-content/uploads/Multi-class-lung-infection-segmentation.zip
## Visualization Results: <br>
![alt text](./InfectionSeg.png)<br>
Figure 4. Visual comparison of lung infection segmentation results.
![alt text](./MultiClassInfectionSeg.png)<br>
Figure 5. Visual comparison of multi-class lung infection segmentation results, where the red and green labels indicate the GGO and consolidation, respectively.

# Paper list (update continue)
https://github.com/HzFu/COVID19_imaging_AI_paper_list

# Manuscript
http://dpfan.net/wp-content/uploads/2020TMISubmissionInfNet.pdf

# Citation
Please cite our paper if you find the work useful: 

	@article{fan2020InfNet,
  	title={Inf-Net: Automatic COVID-19 Lung Infection Segmentation from CT Scans},
  	author={Fan, Deng-Ping and Zhou, Tao and Ji, Ge-Peng and Zhou, Yi and Chen, Geng and Fu, Huazhu and Shen, Jianbing and Shao, Ling},
  	Journal = {arXiv},
  	year={2020}
	}
  
