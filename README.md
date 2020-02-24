# Multi-Object-Tracking-Paper-List
Some new works could be found in the MOT16、MOT17 ranking list, but it seems that no work opening their source code in recent months, so I did not update the source code list. Sometimes, I think that the MOT benchmark may lead the researchers to a wrong direction. The MOT17 benchmark provides three kinds of detection results: DPM, Faster RCNN and SDP, if you analyse the results based on different detections, you would find that most trackers has similar performance on Faster RCNN and SDP detections. The trackers ranking well mostly rely on the good performance on DPM detections and they have similar performance with DeepSort when adopting Faster RCNN and SDP detections. So if you want to improve your MOTA score, focus on DPM result.<br>  
Multi-object tracking is a deeply explored but not successfully solved computer vision task. This filed needs more open sources and more standard evaluation metrics. Opening source code is not the characteristic for this field（maybe the large number of parameters waited to be tuned)......  This is a paper list for multi-object-tracking.
## Datasets
### Surveillance Scenarios
[PETS2009](http://www.cvg.reading.ac.uk/PETS2009/a.html) : An old dataset.<br>
[MOT dataset](https://motchallenge.net/) : A dataset for multi-person detection and tracking, mostly used.<br>
[UA-DETRAC](http://detrac-db.rit.albany.edu/) : A dataset for multi-car detection and tracking. <br>
[AVSS2018 Challenge](https://iwt4s2018.wordpress.com/challenge/) : AVSS2018 Challenge based on UA-DETRAC is opened!<br>
[DukeMTMC](http://vision.cs.duke.edu/DukeMTMC/) : A dataset for multi-camera multi-person tracking. <br>
[PoseTrack](https://posetrack.net/): A dataset for multi-person pose tracking. <br>
[NVIDIA AI CITY Challenge](https://www.aicitychallenge.org/): Challenges including "Traffic Flow Analysis", "Anomaly Detection" and "Multi-sensor Vehicle Detection and Reidentification", you may find some insteresting codes on their [Github repos](https://github.com/NVIDIAAICITYCHALLENGE)<br>
[Vis Drone](http://www.aiskyeye.com/views/index): Tracking videos captured by drone-mounted cameras.<br>
[JTA Dataset](http://imagelab.ing.unimore.it/imagelab/page.asp?IdPage=25): A huge dataset for pedestrian pose estimation and tracking in urban scenarios created by exploiting the highly photorealistic video game Grand Theft Auto V developed by Rockstar North.<br>
[Path Track](http://people.ee.ethz.ch/~daid/pathtrack/) A new dataset with many scenes.<br>
[MOTS](https://www.vision.rwth-aachen.de/page/mots) MOTS: Multi-Object Tracking and Segmentation. In CVPR 2019<br>
### Driving Scenarios
[KITTI-Tracking](http://www.cvlibs.net/datasets/kitti/eval_tracking.php) : Multi-person or multi-car tracking dataset.<br>
[MOTS](https://www.vision.rwth-aachen.de/page/mots) Multi-Object Tracking and Segmentation. In CVPR 2019<br>
[Apollo-Tracking](http://apolloscape.auto/tracking.html) 3D Lidar multi-object tracking.<br> 
[Baidu Trajectory](http://apolloscape.auto/trajectory.html) Interesting dataset for trajectory prediction for Autonomous drive, wait to be opened.<br>

## Overview
P Emami,PM Pardalos,L Elefteriadou,S Ranka "Machine Learning Methods for Solving Assignment Problems in Multi-Target Tracking" [[paper]](http://xueshu.baidu.com/s?wd=paperuri%3A%28dcfbdc0f8f79fe44d9166fd2481e37aa%29&filter=sc_long_sign&tn=SE_xueshusource_2kduw22v&sc_vurl=http%3A%2F%2Farxiv.org%2Fpdf%2F1802.06897&ie=utf-8&sc_us=15766836095004964816)<br>
Wenhan Luo, Junliang Xing, Anton Milan, Xiaoqin Zhang, Wei Liu, Xiaowei Zhao and Tae-Kyun Kim, "Multiple Object Tracking: A Literature Review" [[paper]](http://pdfs.semanticscholar.org/3dff/acda086689c1bcb01a8dad4557a4e92b8205.pdf)<br>
A 101 slide [[paper]](http://vision.stanford.edu/teaching/cs231b_spring1415/slides/greedy_fahim_albert.pdf)<br>
## Evaluation Metric
**CLEAR MOT** : Bernardin, K. & Stiefelhagen, R. "Evaluating Multiple Object Tracking Performance: The CLEAR MOT Metric" [[paper]](https://cvhci.anthropomatik.kit.edu/images/stories/msmmi/papers/eurasip2008.pdf)<br>
**IDF1** : Ristani, E., Solera, F., Zou, R., Cucchiara, R. & Tomasi, C. "Performance Measures and a Data Set for Multi-Target, Multi-Camera Tracking" [[paper]](https://users.cs.duke.edu/~ristani/bmtt2016/ristani2016MTMC.pdf)<br>
**Evaluation Code**: [[Python]](https://github.com/cheind/py-motmetrics)<br> 
## Researcher
**Computer Vision Group at RWTH Aachen University** [[webpage and source code]](https://www.vision.rwth-aachen.de/publications/0000/)<br>
**Anton Milan** [[webpage and his source code]](http://www.milanton.de/)<br>
**Laura Leal-Taixé** [[webpage and her source code]](https://lealtaixe.github.io/publications/)<br>
**Dynamic Vision and Learning Group** [[webpage and their source code]](https://dvl.in.tum.de/research/mot/)<br>
**Longyin Wen** [[webpage and his source code]](http://www.cbsr.ia.ac.cn/users/lywen/)<br>
**UCF** [[webpage]](http://crcv.ucf.edu/projects/tracking)<br>
Some source codes in above webpage are not listed in below Open Source.Such as:<br>
"segTrack"<br>
"Exploiting Hierarchical Dense Structures on Hypergraphs for Multi-Object Tracking"<br>
"Learning an image-based motion context for multiple people tracking"<br> 
## Open Source
### Online
**Towards-Realtime-MOT** Zhongdao Wang, Liang Zheng, Yixuan Liu, Shengjin Wang. Towards Real-Time Multi-Object Tracking. [[paper]](https://arxiv.org/pdf/1909.12605v1.pdf) [[code]](https://github.com/Zhongdao/Towards-Realtime-MOT)<br>
**Track-no-bnw** Bergmann P, Meinhardt T, Lealtaixe L, et al. Tracking without bells and whistles[J]. (ICCV2020). [[paper]](https://arxiv.org/pdf/1903.05625.pdf)[[code]](https://github.com/phil-bergmann/tracking_wo_bnw)<br>
**DeepMot** Yihong Xu Yutong Ban Xavier Alameda-Pineda Radu Horaud, "DeepMOT:A Differentiable Framework for Training Multiple Object Trackers" [[paper]](https://arxiv.org/pdf/1906.06618.pdf)[[code]](https://gitlab.inria.fr/yixu/deepmot)<br>
**TrackR-CNN,MOTS** Paul Voigtlaender and Michael Krause, "MOTS: Multi-Object Tracking and Segmentation" In CVPR2019 [[paper]](https://www.vision.rwth-aachen.de/media/papers/mots-multi-object-tracking-and-segmentation/MOTS.pdf)[[code]](https://github.com/VisualComputingInstitute/TrackR-CNN/tree/master)<br>
**Tracktor** Philipp Bergmann, Tim Meinhardt, Laura Leal-Taixe "Tracking without bells and whistles" In Arxiv [[paper]](https://arxiv.org/pdf/1903.05625.pdf)[[code]](https://github.com/phil-bergmann/tracking_wo_bnw)<br>
**DMAN** Zhu, Ji and Yang, Hua and Liu, Nian and Kim, Minyoung and Zhang, Wenjun and Yang, Ming-Hsuan "Online Multi-Object Tracking with Dual Matching Attention Networks" [[paper]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Ji_Zhu_Online_Multi-Object_Tracking_ECCV_2018_paper.pdf) [[code]](https://github.com/jizhu1023/DMAN_MOT) In ECCV2018<br>
**LSST** Weitao Feng, Zhihao Hu, Wei Wu, Junjie Yan, Wanli Ouyang "Multi-Object Tracking with Multiple Cues and Switcher-Aware Classification" [[paper]](https://arxiv.org/abs/1901.06129) SOA tracker on MOT ranking list. No code now.<br>
**SST** Sun. S., Akhtar, N., Song, H., Mian A., & Shah M. (2018). Deep Affinity Network for Multiple Object Tracking[[paper]](https://arxiv.org/abs/1810.11780)[[code]](https://github.com/shijieS/SST): Interesting work and expect the author to update their DPM tracking results on MOT17 benchmark.<br>
**MOTDT** Long Chen, Haizhou Ai "Real-time Multiple People Tracking with Deeply Learned Candidate Selection and Person Re-identification" in ICME 2018 [[code]](https://github.com/longcw/MOTDT)[[paper]](https://www.researchgate.net/publication/326224594_Real-time_Multiple_People_Tracking_with_Deeply_Learned_Candidate_Selection_and_Person_Re-identification)!<br>
**TMPORT** : E. Ristani and C. Tomasi. Tracking Multiple People Online and in Real Time. in ACCV 2014 [[paper]](https://users.cs.duke.edu/~tomasi/papers/ristani/ristaniAccv14.pdf) [[code]](http://vision.cs.duke.edu/DukeMTMC/)<br>
**MOT-RNN** : Anton Milan, Seyed Hamid Rezatofighi, Anthony Dick, Konrad Schindler, Ian Reid "Online Multi-target Tracking using Recurrent Neural Networks"[[paper]](http://www.milanton.de/files/aaai2017/aaai2017-anton-rnntracking.pdf) [[code]](https://bitbucket.org/amilan/rnntracking) In AAAI 2017.<br>
**DeepSort** : Wojke, Nicolai and Bewley, Alex and Paulus, Dietrich "Simple Online and Realtime Tracking with a Deep Association Metric" [[paper]](https://arxiv.org/abs/1703.07402) [[code]](https://github.com/nwojke/deep_sort) In ICIP 2017<br>
**Sort** : Bewley, Alex and Ge, Zongyuan and Ott, Lionel and Ramos, Fabio and Upcroft, Ben "Simple Online and Realtime Tracking"[[paper]](https://arxiv.org/abs/1602.00763) [[code]](https://github.com/abewley/sort) In ICIP 2016.<br>
**MDP** : Yu Xiang, Alexandre Alahi, and Silvio Savarese "Learning to Track: Online Multi-Object Tracking by Decision Making
" [[paper]](http://openaccess.thecvf.com/content_iccv_2015/papers/Xiang_Learning_to_Track_ICCV_2015_paper.pdf) [[code]](http://cvgl.stanford.edu/projects/MDP_tracking/) In International Conference on Computer Vision (ICCV), 2015 <br>
**CMOT** : S. H. Bae and K. Yoon. "Robust online multi-object tracking based on tracklet confidence and online discriminative appearance learning" [[paper]](https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Bae_Robust_Online_Multi-Object_2014_CVPR_paper.pdf) [[code]](https://cvl.gist.ac.kr/project/cmot.html) In CVPR 2014<br> 
**RCMSS** : Mohamed A. Naiel1, M. Omair Ahmad, M.N.S. Swamy, Jongwoo Lim, and Ming-Hsuan Yang "Online Multi-Object Tracking Via 
Robust Collaborative Model and Sample Selection"[[paper]](https://users.encs.concordia.ca/~rcmss/include/Papers/CVIU2016.pdf) [[code]](https://users.encs.concordia.ca/~rcmss/) Computer Vision and Image Understanding 2016 <br>
**MHT-DAM** : Chanho Kim, Fuxin Li, Arridhana Ciptadi, James M. Rehg "Multiple Hypothesis Tracking Revisited"[[paper]](https://www.cc.gatech.edu/~ckim314/papers/MHTR_ICCV2015.pdf) [[code]](http://rehg.org/mht/) In ICCV 2015<br>
**OMPTTH** : Jianming Zhang, Liliana Lo Presti and Stan Sclaroff, "Online Multi-Person Tracking by Tracker Hierarchy," [[paper]]() [[code]](http://cs-people.bu.edu/jmzhang/tracker_hierarchy/Tracker_Hierarchy.htm) Proc. Int. Conf. on Advanced Video and Signal Based Surveillance (AVSS), 2012.<br>
**SMOT** : C. Dicle, O. Camps, M. Sznaier. "The Way They Move: Tracking Targets with Similar Appearance" [[paper]](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Dicle_The_Way_They_2013_ICCV_paper.pdf) [[code]](https://bitbucket.org/cdicle/smot) In ICCV, 2013.<br>
### Batch
**muSSP** Wang C, Wang Y, Wang Y, et al. muSSP: Efficient Min-cost Flow Algorithm for Multi-object Tracking[C]. neural information processing systems, 2019: 423-432. [[paper]](http://papers.nips.cc/paper/8334-mussp-efficient-min-cost-flow-algorithm-for-multi-object-tracking)[[code]](https://github.com/yu-lab-vt/muSSP)<br>
**TNT** Gaoang Wang, Yizhou Wang, Haotian Zhang, Renshu Gu, Jenq-Neng Hwang "Exploit the Connectivity: Multi-Object Tracking with TrackletNet" [[paper]](https://arxiv.org/pdf/1811.07258.pdf) [[code]](https://github.com/GaoangW/TNT)<br>
**NT** Longyin Wen*, Dawei Du*, Shengkun Li, Xiao Bian, Siwei Lyu Learning Non-Uniform Hypergraph for Multi-Object Tracking, In AAAI 2019 [[paper]](http://www.cs.albany.edu/~lsw/papers/aaai19a.pdf)[[code]](https://github.com/longyin880815) Waited!<br>
**headTracking**: Shun Zhang, Jinjun Wang, Zelun Wang, Yihong Gong,Yuehu Liu: "Multi-Target Tracking by Learning Local-to-Global Trajectory Models" in PR 2015 [[paper]](https://www.researchgate.net/publication/265295656_Multi-Target_Tracking_by_Learning_Local-to-Global_Trajectory_Models) [[code]](https://github.com/gengshan-y/headTracking) seems like a repo.<br>
**IOU** : E. Bochinski, V. Eiselein, T. Sikora. "High-Speed Tracking-by-Detection Without Using Image Information" [[paper]](http://elvera.nue.tu-berlin.de/files/1517Bochinski2017.pdf) [[code]](https://github.com/bochinski/iou-tracker/) In International Workshop on Traffic and Street Surveillance for Safety and Security at IEEE AVSS 2017, 2017. <br>
**NMGC-MOT** Andrii Maksai, Xinchao Wang, Franc¸ois Fleuret, and Pascal Fua "Non-Markovian Globally Consistent Multi-Object Tracking
" [[paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Maksai_Non-Markovian_Globally_Consistent_ICCV_2017_paper.pdf)[[code]](https://github.com/maksay/ptrack_cpp) In ICCV 2017<br>
**D2T** Christoph Feichtenhofer, Axel Pinz, Andrew Zisserman, "Detect to Track and Track to Detect" [[paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Feichtenhofer_Detect_to_Track_ICCV_2017_paper.pdf) [[code]](https://github.com/feichtenhofer/Detect-Track) In ICCV 2017<br>
**H2T** : Longyin Wen, Wenbo Li, Junjie Yan, Zhen Lei, Dong Yi, Stan Z. Li. "Multiple Target Tracking Based on Undirected Hierarchical Relation Hypergraph," [[paper]](http://www.cbsr.ia.ac.cn/users/lywen/papers/CVPR2014_HyperGraphMultiTargetsTracker.pdf) [[code]](http://www.cbsr.ia.ac.cn/users/lywen/) IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2014.<br>
**LDCT** : F. Solera, S. Calderara, R. Cucchiara "Learning to Divide and Conquer for Online Multi-Target Tracking" [[paper]](http://ieeexplore.ieee.org/document/7410854/) [[code page 1]](https://github.com/francescosolera/LDCT) [[code page 2]](http://imagelab.ing.unimore.it/imagelab/researchActivity.asp?idActivity=09) In Proceedings of International Converence on Computer Vision (ICCV), Santiago Cile, Dec 12-18, 2015<br>
**CEM** : Anton Milan, Stefan Roth, Konrad Schindler "Continuous Energy Minimization for Multi-Target Tracking" [[paper]](http://www.milanton.de/files/pami2014/pami2014-anton.pdf) [[code]](http://www.milanton.de/contracking/) in pami 2014<br>
**OPCNF** : Chari, Visesh and Lacoste-Julien, Simon and Laptev, Ivan and Sivic, Josef "On Pairwise Costs for Network Flow Multi-Object Tracking" [[paper]](https://arxiv.org/abs/1408.3304) [[code]](http://www.di.ens.fr/willow/research/flowtrack/) In CVPR 2015<br>
**KSP** : J. Berclaz, F. Fleuret, E. Türetken and P. Fua "Multiple Object Tracking using K-Shortest Paths Optimization" [[paper]](https://cvlab.epfl.ch/files/content/sites/cvlab2/files/publications/publications/2011/BerclazFTF11.pdf) [[code]](https://cvlab.epfl.ch/software/ksp)  IEEE Transactions on Pattern Analysis and Machine Intelligence, 2011.<br>
**GMCP** : Amir Roshan Zamir, Afshin Dehghan, and Mubarak Shah "GMCP-Tracker: Global Multi-object Tracking Using Generalized Minimum Clique Graphs" [[paper]](http://crcv.ucf.edu/papers/eccv2012/GMCP-Tracker_ECCV12.pdf) [[code]](http://crcv.ucf.edu/projects/GMCP-Tracker/) European Conference on Computer Vision (ECCV), 2012.<br>
### Driving Scenarios
**MOTBeyondPixels** Sarthak Sharma*, Junaid Ahmed Ansari*, J. Krishna Murthy, and K. Madhava Krishna Beyond Pixels: Leveraging Geometry and Shape Cues for Online Multi-Object Tracking In ICRA 2018 [[paper]](https://arxiv.org/abs/1802.09298)[[code]](https://github.com/JunaidCS032/MOTBeyondPixels)<br>
**CIWT** Aljoˇsa Oˇsep, Alexander Hermans Combined Image and World-Space Tracking in Traffic Scenes In ICRA 2017 [[paper]](https://www.vision.rwth-aachen.de/media/papers/paper_final_compressed.pdf) [[code]](https://github.com/aljosaosep/ciwt)<br>
### MCMT
**DeepCC** Ristani and C. Tomasi "Features for Multi-Target Multi-Camera Tracking and Re-Identification" In CVPR 2018 [[paper]](https://arxiv.org/pdf/1803.10859.pdf) [[code]](https://github.com/ergysr/DeepCC)<br>
**towards-reid-tracking** Lucas Beyer∗  Stefan Breuers∗ "Towards a Principled Integration of Multi-Camera Re-Identification andTracking through Optimal Bayes Filters"[[paper]](https://arxiv.org/pdf/1705.04608.pdf)[[code]](https://github.com/VisualComputingInstitute/towards-reid-tracking)<br>
### RGBD Tracking
**DetTA** Stefan Breuers, Lucas Beyer "Detection-Tracking for Efficient Person Analysis: The DetTA Pipeline" [[paper]](https://arxiv.org/abs/1804.10134)[[code]](https://github.com/sbreuers/detta)<br>

## Private Detection
**POI** : F. Yu, W. Li, Q. Li, Y. Liu, X. Shi, J. Yan. "POI: Multiple Object Tracking with High Performance Detection and Appearance Feature" [[paper]](https://arxiv.org/pdf/1610.06136.pdf) [[detection]](https://drive.google.com/open?id=0B5ACiy41McAHMjczS2p0dFg3emM) In BMTT, SenseTime Group Limited, 2016<br>
## New papers
### CVPR
#### 2017
Eldar Insafutdinov, Mykhaylo Andriluka, Leonid Pishchulin, Siyu Tang, Evgeny Levinkov, Bjoern Andres, Bernt Schiele "Art Track: Articulated Multi-Person Tracking in the Wild" [[paper]](https://arxiv.org/abs/1612.01465)<br>
Manmohan Chandraker, Paul Vernaza, Wongun Choi, Samuel Schulter "Deep Network Flow for Multi-Object Tracking" [[paper]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Schulter_Deep_Network_Flow_CVPR_2017_paper.pdf)<br>
Jeany Son, Mooyeol Baek, Minsu Cho, and Bohyung Han, "Multi-Object Tracking with Quadruplet Convolutional Neural Networks" [[paper]](http://openaccess.thecvf.com/content_cvpr_2017/papers/Son_Multi-Object_Tracking_With_CVPR_2017_paper.pdf)<br>
#### 2018
Girdhar R, Gkioxari G, Torresani L, et al. Detect-and-Track: Efficient Pose Estimation in Videos[C].(CVPR2018)[[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Girdhar_Detect-and-Track_Efficient_Pose_CVPR_2018_paper.pdf)[[code]](https://rohitgirdhar.github.io/DetectAndTrack/)  
Rolling Shutter and Radial Distortion Are Features for High Frame Rate Multi-Camera Tracking[[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bapat_Rolling_Shutter_and_CVPR_2018_paper.pdf)   
Features for Multi-Target Multi-Camera Tracking and Re-Identification [[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Ristani_Features_for_Multi-Target_CVPR_2018_paper.pdf)  
#### 2019
Self-Supervised Adaptation of High-Fidelity Face Models for Monocular Performance Tracking [[paper]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Raaj_Efficient_Online_Multi-Person_2D_Pose_Tracking_With_Recurrent_Spatio-Temporal_Affinity_CVPR_2019_paper.pdf)  
Eliminating Exposure Bias and Metric Mismatch in Multiple Object Tracking [[paper]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Maksai_Eliminating_Exposure_Bias_and_Metric_Mismatch_in_Multiple_Object_Tracking_CVPR_2019_paper.pdf)
### ICCV
A. Sadeghian, A. Alahi, S. Savarese, Tracking The Untrackable: Learning To Track Multiple Cues with Long-Term Dependencies [[paper]](https://arxiv.org/abs/1701.01909)<br>
Andrii Maksai, Xinchao Wang, Franc¸ois Fleuret, and Pascal Fua "Non-Markovian Globally Consistent Multi-Object Tracking
" [[paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Maksai_Non-Markovian_Globally_Consistent_ICCV_2017_paper.pdf)[[code]](https://github.com/maksay/ptrack_cpp)<br>
Christoph Feichtenhofer, Axel Pinz, Andrew Zisserman, "Detect to Track and Track to Detect" [[paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Feichtenhofer_Detect_to_Track_ICCV_2017_paper.pdf) [[code]](https://github.com/feichtenhofer/Detect-Track)<br>
Qi Chu, Wanli Ouyang,  Xiaogang Wang, Bin Liu, Nenghai Yu "Online Multi-Object Tracking Using CNN-Based Single Object Tracker With Spatial-Temporal Attention Mechanism" [[paper]](http://openaccess.thecvf.com/content_ICCV_2017/papers/Chu_Online_Multi-Object_Tracking_ICCV_2017_paper.pdf)<br>
**Track-no-bnw** Bergmann P, Meinhardt T, Lealtaixe L, et al. Tracking without bells and whistles[J]. (ICCV2020). [[paper]](https://arxiv.org/pdf/1903.05625.pdf)[[code]](https://github.com/phil-bergmann/tracking_wo_bnw)

### ECCV2018
Ren, Liangliang and Lu, Jiwen and Wang, Zifeng and Tian, Qi and Zhou, Jie "Collaborative Deep Reinforcement Learning for Multi-Object Tracking" [[paper]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Liangliang_Ren_Collaborative_Deep_Reinforcement_ECCV_2018_paper.pdf)<br>
Kim, Chanho and Li, Fuxin and Rehg, James M "Multi-object Tracking with Neural Gating Using Bilinear LSTM" [[paper]](http://openaccess.thecvf.com/content_ECCV_2018/papers/Chanho_Kim_Multi-object_Tracking_with_ECCV_2018_paper.pdf)<br>

### New paper
M Fabbri, F Lanzi, S Calderara, A Palazzi "Learning to Detect and Track Visible and Occluded Body Joints in a Virtual World" [[paper]](https://www.researchgate.net/publication/323957071_Learning_to_Detect_and_Track_Visible_and_Occluded_Body_Joints_in_a_Virtual_World) [[code]] Waited!<br>
Cong Ma, Changshui Yang, Fan Yang, Yueqing Zhuang, Ziwei Zhang, Huizhu Jia, Xiaodong Xie "Trajectory Factory: Tracklet Cleaving and Re-connection by Deep Siamese Bi-GRU for Multiple Object Tracking" In ICME 2018 [[paper]](https://arxiv.org/abs/1804.04555)<br>
Kuan Fang, Yu Xiang, Xiaocheng Li and Silvio Savarese "Recurrent Autoregressive Networks for Online Multi-Object Tracking" In IEEE Winter Conference on Applications of Computer Vision (WACV), 2018. [[webpage]](http://yuxng.github.io/)<br>
Tharindu Fernando, Simon Denman, Sridha Sridharan, Clinton Fookes "Tracking by Prediction: A Deep Generative Model for Mutli-Person localisation and Tracking" In WACV 2018 [[paper]](https://arxiv.org/pdf/1803.03347.pdf)<br>

### Multi-person Face Tracking
Shun Zhang, Yihong Gong, Jia-Bin Huang, Jongwoo Lim, Jinjun Wang, Narendra Ahuja and Ming-Hsuan Yang "Tracking Persons-of-Interest via Adaptive Discriminative Features" In ECCV 2016 [[paper]](https://link.springer.com/content/pdf/10.1007%2F978-3-319-46454-1_26.pdf) [[code]](https://github.com/shunzhang876/AdaptiveFeatureLearning)<br>
Chung-Ching Lin, Ying Hung"A Prior-Less Method for Multi-Face Tracking in Unconstrained Videos" In CVPR 2018 [[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Lin_A_Prior-Less_Method_CVPR_2018_paper.pdf)<br>

### Multi-person Pose Tracking
Yuliang Xiu, Jiefeng Li, Haoyu Wang, Yinghong Fang, Cewu Lu "Pose Flow: Efficient Online Pose Tracking" [[paper]](https://arxiv.org/abs/1802.00977) Idea is interesting but the true source code is not opened.<br>
Bin Xiao, Haiping Wu, and Yichen Wei "Simple Baselines for Human Pose Estimation and Tracking" [[paper]](https://arxiv.org/pdf/1804.06208.pdf)[[code]](https://github.com/Microsoft/human-pose-estimation.pytorch)  
Girdhar R, Gkioxari G, Torresani L, et al. Detect-and-Track: Efficient Pose Estimation in Videos[C].(CVPR2018)[[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Girdhar_Detect-and-Track_Efficient_Pose_CVPR_2018_paper.pdf)[[code]](https://rohitgirdhar.github.io/DetectAndTrack/)
Multi-Person Articulated Tracking With Spatial and Temporal Embeddings [[paper]](http://openaccess.thecvf.com/content_CVPR_2019/papers/Jin_Multi-Person_Articulated_Tracking_With_Spatial_and_Temporal_Embeddings_CVPR_2019_paper.pdf)  
### Multi-camera Tracking
Rolling Shutter and Radial Distortion Are Features for High Frame Rate Multi-Camera Tracking[[paper]](http://openaccess.thecvf.com/content_cvpr_2018/papers/Bapat_Rolling_Shutter_and_CVPR_2018_paper.pdf)
CityFlow: A City-Scale Benchmark for Multi-Target Multi-Camera Vehicle Tracking and Re-Identification[[paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Tang_CityFlow_A_City-Scale_Benchmark_for_Multi-Target_Multi-Camera_Vehicle_Tracking_and_CVPR_2019_paper.pdf)]
