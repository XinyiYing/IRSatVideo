
# *<center>IRSatVideo Dataset: A Semi-simulated Dataset for Infrared Small Target Detection in Satellite Videos</center>*

***IRSatVideo is a large-scale dataset for multi-frame infrared small target (MIRST) detection in LEO and GEO satellite videos. 
IRSatVideo is a semi-simulated dataset with a real satellite background image and synthesized satellite motion, target appearance, trajectory and intensity. 
IRSatVideo-LEO is developed by landset 7-8, and consists of 200 image sequences, 91021 frames. 
IRSatVideo-GEO is developed by GaoFen 4, and consists of 200 image sequences, 94136 frames. 
Note that, we provide instance-level segmentation annotations to offer an infrared satellite videos benchmark for MIRST detection and tracking. [[Paper]](https://arxiv.org/abs/2409.12448)***<br>

### Downloads

To access IRSatVideo dataset, please fill the following form: 
[[Microsoft Forms]](https://forms.cloud.microsoft/r/eYC3mNz5s3).

### Implementation

<center><img src="./pics/simulation.png" width="1000"/></center>
Fig. 1 Implementation details of the IRSatVideo dataset. <br><br>

Table 1 Details of parameters for data generation.
<center><img src="./pics/parameters.png" width="900"/></center>

### Data Format
```
  IRSatVideo-LEO
    └── images
        ├── AfricaWest-1_38
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── EastAfrica-0
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── ...
    └── masks
        ├── AfricaWest-1_38
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── EastAfrica-0
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── ...		
    └── video_idx
        ├── train_IRSatVideo-LEO.txt
        ├── test_IRSatVideo-LEO.txt
        ├── test_IRSatVideo-LEO-easy.txt
        ├── test_IRSatVideo-LEO-middle.txt
        ├── test_IRSatVideo-LEO-hard.txt
    └── img_idx
        ├── AfricaWest-1_38.txt
        ├── EastAfrica-0.txt
        ├── ...
    └── voc
        ├── AfricaWest-1_38
            ├── 0000.xml
            ├── 0001.xml
            ├── ...
```
```
  IRSatVideo-GEO
    └── images
        ├── GF4_IRS_E67.9_N18.0_20210625_L1A0000392439
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── GF4_IRS_E70.6_N47.5_20210911_L1A0000418901
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── ...
    └── masks
        ├── GF4_IRS_E67.9_N18.0_20210625_L1A0000392439
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── GF4_IRS_E70.6_N47.5_20210911_L1A0000418901
            ├── 0000.png
            ├── 0001.png
            ├── ...
        ├── ...		
    └── video_idx
        ├── train_IRSatVideo-GEO.txt
        ├── test_IRSatVideo-GEO.txt
        ├── test_IRSatVideo-GEO-SCR1.txt
        ├── test_IRSatVideo-GEO-SCR2.txt
        ├── test_IRSatVideo-GEO-SCR3.txt
    └── img_idx
        ├── GF4_IRS_E67.9_N18.0_20210625_L1A0000392439.txt
        ├── GF4_IRS_E70.6_N47.5_20210911_L1A0000418901.txt
        ├── ...
    └── voc
        ├── GF4_IRS_E67.9_N18.0_20210625_L1A0000392439
            ├── 0000.xml
            ├── 0001.xml
            ├── ...
```

### Contact
Please contact us at ***yingxinyi18@nudt.edu.cn*** for any questions.

### Citiation
```
@article{RFR,
  author = {Xinyi Ying, Li Liu, Zaipin Lin, Yangsi Shi, Yingqian Wang, Ruojing Li, Xu Cao, Boyang Li, Shilin Zhou},
  title = {Infrared Small Target Detection in Satellite Videos: A New Dataset and A Novel Recurrent Feature Refinement Framework},
  journal = {IEEE Transactions on Geoscience and Remote Sensing},
  year = {2025},
}
```
