# SAR-ATR-methods
This repository contains the supplementary file for article "Review of Synthetic Aperture Radar Automatic Target Recognition: A Dual Perspective on Classical and Deep Learning Techniques"

    ├── LICENSE                 
    ├── README.md
    └── SAR_ATR_methods_Table.csv       # paper review database

## Taxonomy of the Detection Methods:

### 1. Traditional Methods
#### A.	Template-Based Methods
#### B.	Model-Based Methods
#### C.	CFAR-Based Methods
- One-parameter CFAR
- Two-parameter CFAR
- Clutter Modeling and Applications
#### D.	Machine Learning Methods

### 2. Modern Deep Learning Methods
#### A.	Architecture-Based Classification
- Non-CNN Deep Models
- CNN-Based Methods
    - Standard CNNs (Borrowed from Computer Vision)
    - Shallow and deep CNNs
    - Two-Stage and One-Stage Detectors
    - Attention-based CNNs
    - Capsule Networks
- Hybrid Architectures
#### B.	Learning Paradigm Classification
- Supervised Learning
- Semi-supervised Learning
- Unsupervised Learning
- Few-shot Learning
- Transfer Learning
- Adversarial Attack
- Data Augmentation Strategies
    - Classical data augmentation
    - Simulation-based generation
    - GAN-based new samples
- Scattering-Based Feature Enhancement
    - Attributed Scattering Center Based
    - Scattering topology
- Multi-modal Data Processing
    - Polarimetric SAR
    - SAR-optical fusion
    - Complex data
    - Multi-resolution SAR
#### C.	Operational and Task-Specific Methods
- Real-time Detection Systems
- Robust Recognition Systems
- Small-Target Detection
- Multitask

## DATASETS IN SAR OBJECT RECOGNITION

| Dataset                      	| Year 	| Sensor/Source                                                                                	| # Img   	| Img size               	| Res [m]                    	| Band                   	| Pol                	| Target                             	|
|------------------------------	|------	|----------------------------------------------------------------------------------------------	|---------	|------------------------	|----------------------------	|------------------------	|--------------------	|------------------------------------	|
| MSTAR [1]                    	| 1995 	| Aerial X-band radar                                                                          	| 14,577  	| 128×128                	| 0.3                        	| X-band                 	| Single             	| Military vehicles                  	|
| Sandia MiniSAR [2]           	| 2006 	| MiniSAR                                                                                      	| 3,927   	| 224×224                	| 0.1                        	| Ku-band                	| Single, Dual       	| Terrestrial targets in urban areas 	|
| SARSim [3]                   	| 2016 	| simulated data                                                                               	| 21,168  	| 139×139                	| 0.1 to 0.3                 	| X-band                 	| Single             	| Military vehicles                  	|
| OpenSARShip-1.0 [4]          	| 2017 	| Sentinel-1                                                                                   	| 11,346  	| Various                	| 2.7×22 to 3.5×22 and 20×22 	| C-band                 	| Single, Dual       	| Ships (AIS types)                  	|
| OpenSARShip-2.0 [5]          	| 2017 	| Sentinel-1                                                                                   	| 34,528  	| Various                	| 2.7×22 to 3.5×22 and 20×22 	| C-band                 	| Single, Dual       	| Ships (AIS types)                  	|
| SSDD [6]                     	| 2017 	| RADARSAT-2, TerraSAR-X, Sentinel-1                                                           	| 1,16    	| Various 214 to 668     	| 1 to 15                    	| C-band X-band          	| Singl, Dual, Quad  	| Ships                              	|
| SAMPLE [7]                   	| 2019 	| MSTAR + simulated data                                                                       	| 2,732   	| 128×128                	| 0.3                        	| X-band                 	| Single             	| Military vehicles                  	|
| SAR-Ship-Dataset [8]         	| 2019 	| Gaofen-3, Sentinel-1                                                                         	| 43,819  	| 256×256                	| 1.7×4.3 to 25              	| C-band                 	| Single, Dual       	| Ships                              	|
| AIR-SARShip-1.0 [9]          	| 2019 	| Gaofen-3                                                                                     	| 31      	| 3000×3000 to 4140×4140 	| 1 to 3                     	| C-band                 	| Single             	| Ships                              	|
| AIR-SARShip-2.0 [10]         	| 2020 	| Gaofen-3                                                                                     	| 300     	| ~1000×1000             	| 1 to 3                     	| C-band                 	| Single             	| Ships                              	|
| HRSID [11]                   	| 2020 	| Sentinel-1, TerraSAR-X, TanDEM-X                                                             	| 5,604   	| 800×800                	| 0.5 to 3                   	| C-band X-band          	| Dual, Quad         	| Ships                              	|
| LS-SSDD-v1.0 [12]            	| 2020 	| Sentinel-1                                                                                   	| 9       	| 800×800                	| 5x20                       	| C-band                 	| Single, Dual       	| Small ships                        	|
| FUSAR-Ship Dataset v1.0 [13] 	| 2020 	| Gaofen-3                                                                                     	| 16,144  	| 512×512                	| 1.12 × 1.73                	| C-band                 	| Single, Dual       	| Ships (AIS messages)               	|
| DSSDD [14]                   	| 2021 	| TerraSAR-X, Sentinel-1, Gaofen-3                                                             	| 1,236   	| 256×256                	| Not specified              	| C-band X-band          	| Single, Dual       	| Ships                              	|
| SRSDD-v1.0 [15]              	| 2021 	| Gaofen-3                                                                                     	| 666     	| 1024×1024              	| 1                          	| C-band                 	| Single             	| Ships                              	|
| xView3-SAR [16]              	| 2022 	| Sentinel-1                                                                                   	| 991     	| ~29,400× 24,400        	| ~20                        	| C-band                 	| Single, Dual       	| Ships, offshore structures         	|
| SADD [17]                    	| 2022 	| TerraSAR-X                                                                                   	| 2,966   	| 224×224                	| 0.5 to 3                   	| X-band                 	| Single             	| Aircraft                           	|
| MSAR [18]                    	| 2022 	| Multiple                                                                                     	| 28,499  	| 256×256 to 2048×2048   	| 1                          	| C-band                 	| Quad               	| Terrestrial and maritime targets   	|
| SAR-AIRcraft [19]            	| 2023 	| Gaofen-3                                                                                     	| 4,368   	| 800×800 to 1500×1500   	| 1                          	| C-band                 	| Single             	| Aircraft                           	|
| SIVED [20]                   	| 2023 	| simulated data                                                                               	| 1,044   	| 512×512                	| 0.1 to 0.3                 	| Ku-band Ka-band X-band 	| Single             	| Vehicles                           	|
| MRSSD [21]                   	| 2023 	| Capella, ICEYE, TerraSAR-X, Paz, Alos PALSAR, Sentinel-1                                     	| 11,59   	| 512×512                	| 0.5 to 100                 	| L-band  C-band X-band  	| Single, Dual, Quad 	| Ships                              	|
| SARDet-100K [22]             	| 2024 	| Gaofen-3, Sentinel-1, TanDEM-X, RADARSAT-2,  Alos-PALSAR, Capella, ICEYE, Kompsat-5, RISAT-1 	| 116,598 	| 512×512                	| 0.5m to 3m                 	| L-band C-band X-band   	| Single, Dual       	| Ships, vehicles, others            	|

## References

- [1]	E. R. Keydel, S. W. Lee, and J. T. Moore, ‘MSTAR extended operating conditions: a tutorial’, presented at the Aerospace/Defense Sensing and Controls, E. G. Zelnio and R. J. Douglass, Eds., Orlando, FL, Jun. 1996, pp. 228–242. doi: 10.1117/12.242059.
- [2]	‘SAR Data’, Pathfinder Radar ISR & SAR Systems. Accessed: Jan. 12, 2025. [Online]. Available: https://www.sandia.gov/radar/pathfinder-radar-isr-and-synthetic-aperture-radar-sar-systems/complex-data/
- [3]	‘Synthetic SAR Image Generation using Sensor, Terrain and Target Models’. Accessed: Jan. 12, 2025. [Online]. Available: https://ieeexplore-1ieee-1org-100001bck0bcc.han.wat.edu.pl/document/7559326
- [4]	‘OpenSARShip: A Dataset Dedicated to Sentinel-1 Ship Interpretation’. Accessed: Jan. 12, 2025. [Online]. Available: https://ieeexplore-1ieee-1org-100001bck0bdf.han.wat.edu.pl/document/8067489
- [5]	‘OpenSARShip 2.0: A large-volume dataset for deeper interpretation of ship targets in Sentinel-1 imagery’. Accessed: Jan. 12, 2025. [Online]. Available: https://ieeexplore-1ieee-1org-100001bck0bdf.han.wat.edu.pl/document/8124929
- [6]	T. Zhang et al., ‘SAR Ship Detection Dataset (SSDD): Official Release and Comprehensive Data Analysis’, Remote Sensing, vol. 13, no. 18, p. 3690, Sep. 2021, doi: 10.3390/rs13183690.
- [7]	B. Lewis, T. Scarnati, E. Sudkamp, J. Nehrbass, S. Rosencrantz, and E. Zelnio, ‘A SAR dataset for ATR development: the Synthetic and Measured Paired Labeled Experiment (SAMPLE)’, in Algorithms for Synthetic Aperture Radar Imagery XXVI, SPIE, May 2019, pp. 39–54. doi: 10.1117/12.2523460.
- [8]	‘A SAR Dataset of Ship Detection for Deep Learning under Complex Backgrounds’. Accessed: Jan. 12, 2025. [Online]. Available: https://www.mdpi.com/2072-4292/11/7/765
- [9]	S. Xian et al., ‘AIR-SARShip-1.0: High-resolution SAR Ship Detection Dataset’, 2020. Accessed: Dec. 23, 2024. [Online]. Available: https://www.semanticscholar.org/paper/AIR-SARShip-1.0%3A-High-resolution-SAR-Ship-Detection-Xian-Wang/bdf2e09c65e857fd608df15ef5c317a9267489b3
- [10]	‘雷达学报’. Accessed: Jan. 12, 2025. [Online]. Available: https://radars.ac.cn/web/data/getData?newsColumnId=74fe223a-0b01-4830-8d99-1ba276e67ad8&pageType=en
- [11]	S. Wei, X. Zeng, Q. Qu, M. Wang, H. Su, and J. Shi, ‘HRSID: A High-Resolution SAR Images Dataset for Ship Detection and Instance Segmentation’, IEEE Access, vol. 8, pp. 120234–120254, 2020, doi: 10.1109/ACCESS.2020.3005861.
- [12]	T. Zhang et al., ‘LS-SSDD-v1.0: A Deep Learning Dataset Dedicated to Small Ship Detection from Large-Scale Sentinel-1 SAR Images’, Remote Sensing, vol. 12, no. 18, p. 2997, Sep. 2020, doi: 10.3390/rs12182997.
- [13]	X. Hou, W. Ao, Q. Song, J. Lai, H. Wang, and F. Xu, ‘FUSAR-Ship: building a high-resolution SAR-AIS matchup dataset of Gaofen-3 for ship detection and recognition’, Sci. China Inf. Sci., vol. 63, no. 4, p. 140303, Mar. 2020, doi: 10.1007/s11432-019-2772-5.
- [14]	Y. Hu, Y. Li, and Z. Pan, ‘A Dual-Polarimetric SAR Ship Detection Dataset and a Memory-Augmented Autoencoder-Based Detection Method’, Sensors (Basel), vol. 21, no. 24, p. 8478, Dec. 2021, doi: 10.3390/s21248478.
- [15]	S. Lei, D. Lu, X. Qiu, and C. Ding, ‘SRSDD-v1.0: A High-Resolution SAR Rotation Ship Detection Dataset’, Remote Sensing, vol. 13, no. 24, p. 5104, Dec. 2021, doi: 10.3390/rs13245104.
- [16]	F. Paolo et al., ‘xView3-SAR: Detecting Dark Fishing Activity Using Synthetic Aperture Radar Imagery’, Nov. 05, 2022, arXiv: arXiv:2206.00897. doi: 10.48550/arXiv.2206.00897.
- [17]	P. Zhang et al., ‘SEFEPNet: Scale Expansion and Feature Enhancement Pyramid Network for SAR Aircraft Detection With Small Sample Dataset’, IEEE J. Sel. Top. Appl. Earth Observations Remote Sensing, vol. 15, pp. 3365–3375, 2022, doi: 10.1109/JSTARS.2022.3169339.
- [18]	‘雷达学报’. Accessed: Jan. 12, 2025. [Online]. Available: https://radars.ac.cn/web/data/getData?dataType=MSAR
- [19]	Y. KANG, Y. KANG, X. ZENG, Y. WANG, T. ZHANG, and X. SUN, ‘SAR-AIRcraft-1.0: High-resolution SAR Aircraft Detection and Recognition Dataset’, Journal of Radars, vol. 12(4), doi: 10.12000/JR23043.
- [20]	‘SIVED: A SAR Image Dataset for Vehicle Detection Based on Rotatable Bounding Box’. Accessed: Jan. 12, 2025. [Online]. Available: https://www.mdpi.com/2072-4292/15/11/2825
- [21]	M. F. Humayun, F. A. Bhatti, and K. Khurshid, ‘iVision MRSSD: A comprehensive multi-resolution SAR ship detection dataset for state of the art satellite based maritime surveillance applications’, Data in Brief, vol. 50, p. 109505, Oct. 2023, doi: 10.1016/j.dib.2023.109505.
- [22]	Y. Li et al., ‘SARDet-100K: Towards Open-Source Benchmark and ToolKit for Large-Scale SAR Object Detection’, Sep. 30, 2024, arXiv: arXiv:2403.06534. doi: 10.48550/arXiv.2403.06534.

