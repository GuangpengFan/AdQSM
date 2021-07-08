# AdQSM
AdQSM is a new tree quantitative structure model (QSM) that can reconstruct the 3D branch geometry of individual tree from Terrestrial Laser Scanner (TLS) point clouds. Many attributes of the trunk or branch can also be quantitatively calculated (as shown in the "Introduction.pdf"). For example, tree volume (trunk and branch), DBH and tree height parameters can be extracted directly. It allows point clouds collected by different sensors to serve as input point clouds. In addition to TLS, UAV-based Laser Scanner, Mobile Laser Scanner, SLAM and even Photogrammetry are also included under the premise of appropriate point cloud density.
At present, AdQSM is attracting more and more attention. Due to the need to further test and improve AdQSM, we provided AdQSM (Test Version) to worldwide as an open tool with an end-user interface. In order to facilitate the use of AdQSM, we released the software (test version) that runs on Windows and provided part of the tree parameter quantitative calculation function. Now, you can download, install, and quickly display your modeling results for free.

…		…	

1. The current test version of the software can support the tree point cloud in (.xyz) format
 
2. There are two important parameters (Height_Segmentation(HS) and Clound Parameter (CP)) in the process of modeling. HS represents the height of each segment of the point cloud, and CP represents the extraction rate of the point cloud. The default values are 0.50 and 0.003, respectively. According to the existing experimental results, we recommend that people set the value of CP as 0.003 (the default value) when rebuilding the point cloud of a single tree. 
We recommend setting different values of HS for multiple reconstruction (e.g. 0.5, 0.6, 0.7, 0.8, 0.9, 1.0) and calculating the average value of each parameter as the final tree reconstruction result.
According to our test results, we do not recommend to change the value of “Cloud Parameter” frequently (except in case of non modeling, large deviation, etc.)
 

 

3. After setting the parameter values of HS and CP, click "Reconstruct" and the modeling result data will be saved in "treesparams.csv", "treesparams.txt" and "branchinfo.txt" under the installation path.
 

The following paper implements AdQSM. If you use AdQSM or any part of it, we would appreciate your acknowledgement and citation of our paper.

```bibtex
@article{fan2020adqsm,
  title={AdQSM: A New Method for Estimating Above-Ground Biomass from TLS Point Clouds},
  author={Fan, Guangpeng and Nan, Liangliang and Dong, Yanqi and Su, Xiaohui and Chen, Feixiang},
  journal={Remote Sensing},
  volume={12},
  number={18},
  pages={3089},
  year={2020},
  publisher={Multidisciplinary Digital Publishing Institute}
}
```

At present, only 29 destructive sampled trees have tested the accuracy of adqsm in calculating branch volume and trunk volume. Therefore, in the current open source version, we can not guarantee that AdQSM has enough accuracy and stability.

*The right of interpretation of AdQSM belongs to its author and R&D team. To further improve AdQSM, we welcome any invitation for collaboration and test feedback from those who need AdQSM research.
