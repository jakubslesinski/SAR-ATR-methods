# SAR-ATR-methods
This repository contains the supplementary file for article "Review of Synthetic Aperture Radar Automatic Target Recognition: A Dual Perspective on Classical and Deep Learning Techniques"


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
