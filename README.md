# Metal Artifact Reduction for CT images

[Hong Wang](https://hongwang01.github.io/)

*Senior Researcher, [Jarvis Lab@Tencent](https://jarvislab.tencent.com/), Shenzhen, China*

----------
| Method | Domain | Original Link |
|---|---|---|
| InDuDoNet (MICCAI2021) | Dual-Domain | [https://github.com/hongwang01/InDuDoNet](https://github.com/hongwang01/InDuDoNet)|
| InDuDoNet+ (MedIA2023) | Dual-Domain | [https://github.com/hongwang01/InDuDoNet_plus](https://github.com/hongwang01/InDuDoNet_plus)|
| DICDNet (TMI2021)| Image-Domain | [https://github.com/hongwang01/DICDNet](https://github.com/hongwang01/DICDNet)|
| ACDNet (IJCAI2022) | Image-Domain | [https://github.com/hongwang01/ACDNet](https://github.com/hongwang01/ACDNet)|
| OSCNet (MICCAI2022) | Image-Domain | [https://github.com/hongwang01/OSCNet](https://github.com/hongwang01/OSCNet)|


Network architectures
----------
* [InDuDoNet](https://github.com/hongwang01/InDuDoNet)

<div  align="center"><img src="https://github.com/hongwang01/InDuDoNet/blob/main/figs/net.png" height="60%" width="70%" alt=""/></div>


* [InDuDoNet+](https://github.com/hongwang01/InDuDoNet_plus)

<div  align="center"><img src="https://github.com/hongwang01/InDuDoNet_plus/blob/main/figs/priornet.jpg" height="60%" width="70%" alt=""/></div>


* [DICDNet](https://github.com/hongwang01/DICDNet)

<div  align="center"><img src="https://github.com/hongwang01/DICDNet/blob/main/figs/DICDNet.jpg" height="60%" width="70%" alt=""/></div>


* [ACDNet](https://github.com/hongwang01/ACDNet)

<div  align="center"><img src="https://github.com/hongwang01/ACDNet/blob/main/figs/model.jpg" height="60%" width="70%" alt=""/></div>


* [OSCNet](https://github.com/hongwang01/OSCNet)

<div  align="center"><img src="https://github.com/hongwang01/OSCNet/blob/main/Figures/intro.jpg" height="60%" width="70%" alt=""/></div>


## Synthesized DeepLesion

- Clean CT Images: Download 1200 CT images from the [DeepLesion dataset](https://nihcc.app.box.com/v/DeepLesion)
- Simulation Protocol: Refer to [1][2] with the imaging parameters in [bulid_geometory.py](https://github.com/hongwang01/InDuDoNet/blob/main/deeplesion/build_gemotry.py)
- Simulation Tool: Python. 
- Training Data: Pairing 1000 clean images with 90 metals collected from [1]. Following [2], in each training iteration, we randomly chose one CT image with synthesized metal artifacts from the pool of 90 different metal mask pairs
- Testing Data: Pairing another 200 clean CT images with another 10 metals collected from [1] with sizes [2061, 890, 881, 451, 254, 124, 118, 112, 53, 35]
- Download Link: [NetDisk](https://pan.baidu.com/s/1Tu-vTrx7OYCr7eoRDoAgDw?pwd=dicd ) with pwd: dicd
- Please refer to [InDuDoNet](https://github.com/hongwang01/InDuDoNet/blob/main/deeplesion/Dataset.py) and [DICDNet](https://github.com/hongwang01/DICDNet/blob/main/dataset.py) for the data pre-processing
- *If this dataset is helpful for your research, please cite our work.*


## Citation

```
@inproceedings{wang2021indudonet,
  title={InDuDoNet: An Interpretable Dual Domain Network for CT Metal Artifact Reduction},
  author={Wang, Hong and Li, Yuexiang and Zhang, Haimiao and Chen, Jiawei and Ma, Kai and Meng, Deyu and Zheng, Yefeng},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={107--118},
  year={2021},
  organization={Springer}
}
```

```
@article{wang2023indudonet+,
  title={InDuDoNet+: A deep unfolding dual domain network for metal artifact reduction in CT images},
  author={Wang, Hong and Li, Yuexiang and Zhang, Haimiao and Meng, Deyu and Zheng, Yefeng},
  journal={Medical Image Analysis},
  volume={85},
  pages={102729},
  year={2023}
}
```

```
@article{wang2021dicdnet,
  title={DICDNet: Deep Interpretable Convolutional Dictionary Network for Metal Artifact Reduction in CT Images},
  author={Wang, Hong and Li, Yuexiang and He, Nanjun and Ma, Kai and Meng, Deyu and Zheng, Yefeng},
  journal={IEEE Transactions on Medical Imaging},
  volume={41},
  number={4},
  pages={869--880},
  year={2021},
  publisher={IEEE}
}
```

```
@inproceedings{wang2022ada,
  title={Adaptive Convolutional Dictionary Network for CT Metal Artifact Reduction},
  author={Wang, Hong and Li, Yuexiang and Meng, Deyu and Zheng, Yefeng},
  booktitle={The 31st International Joint Conference on Artificial Intelligence},
  year={2022},
  organization={IEEE}
}
```

```
@inproceedings{wang2022orientation,
  title={Orientation-Shared Convolution Representation for CT Metal Artifact Learning},
  author={Wang, Hong and Xie, Qi and Li, Yuexiang and Huang, Yawen and Meng, Deyu and Zheng, Yefeng},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={665--675},
  year={2022},
  organization={Springer}
}
```

## Acknowledgement
The authors would like to thank [Dr. Lequan Yu](https://yulequan.github.io/) for providing the related reference code. If necessary, please contact the author about the original synthesis code.

## References

[1] Y.   Zhang   and   H.   Yu,   “Convolutional   neural   network   based   metalartifact  reduction  in  X-ray  computed  tomography,”IEEE  Transactionson Medical Imaging, vol. 37, no. 6, pp. 1370–1381, 2018.

[2] Yu, L., Zhang, Z., Li, X., Xing, L.: Deep sinogram completion with image prior for metal artifact reduction in CT images. IEEE Transactions on Medical Imaging40(1), 228–238 (2020).

## Contact
If you have any question, please feel free to concat Hong Wang (Email: hongwang9209@hotmail.com)
