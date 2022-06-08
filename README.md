# MFPointNet_feature_dataset
To address the lack of sufficient dataset for using neural networks to recognize the machining features, we established a novel machining feature dataset called MFDataset. The MFDataset contains 33 subcategories features, with approximately 2000 features per category. The detailed category of dataset is shown in Fig.1 below.

![image](https://github.com/leiruoshan/MFPointNet_feature_dataset/blob/main/Fig1.svg)

The MFDataset includes in detail:

Slots: T-through slot, V-through slot, Rounded groove, Swallowtail groove, A-keyway, B-keyway, C-keyway, Half-moon keyway, Straight groove, Ring-shaped groove (10 types)

Holes: Round through hole, Round blind hole, Cylindrical countersunk hole, Tapered countersunk hole, Round stepped hole, A-center hole (6 types)

Steps: Rectangular through step, General step, Shaft step (3 types)

Threads: Internal screw thread, External screw thread (2 types)

Transitions: Rounding, Chamfer, Round (3 types)

Protrudes: Convex hull, Boss (2 types)

Bases: Plane, External cylindrical surface (2 types)

Others: Opened pocket, Closed pocket, Triangular rib reinforcement, General removal of volume, Spherical crown (5 types)

The 33 subategories features are shown in Fig.2 below.

![image](https://github.com/leiruoshan/MFPointNet_feature_dataset/blob/main/Fig2.svg)

These feature models are ".STL" data format. To train the neural network, we need to transform these models into the data format suitable for inputting the CNNs. In our proposed method, we convert them into the ".binvox" data format (voxel) and ".txt" data format (point cloud format, after point downsampling) separately.

(1) Binvox feature datasets:

Fig.3 below depicts some voxelized models of machining feature.

![image](https://github.com/leiruoshan/MFPointNet_feature_dataset/blob/main/Fig3.svg)

(2) Point cloud feature datasets:

After the extraction of feature surface point sets and the Poisson distribution sampling in turn, we contruct the point cloud datasets as some models are shown in Fig.4 below. The Fig.4 shows the 1024 points and 512 points of each feature model respectively.

![image](https://github.com/leiruoshan/MFPointNet_feature_dataset/blob/main/Fig4.svg)

The detailed list of machining features and their parameters (parameters range) are provided in the included with this repository.
