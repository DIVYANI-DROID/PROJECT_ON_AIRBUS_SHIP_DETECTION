# PROJECT_ON_AIRBUS_SHIP_DETECTION
Problem to solve:
Airbus wants to locate ships and put a bounding box around them in satellite images. 
Airbus has been doing most of their analytics and machine learning on-prem, in their own data centers, and is interested in learning about the advantages of using AWS Sagemaker for model training and hosting. 
Main techniques used:
  1. RLE- Run Length Encoding Image segmentation
  2. Image augmentation 
  3. Main model: U–net  
  Benefits of re-using the technique or code later:
    1. The U-Net combines the location information from the down sampling path with the contextual information in the upsampling path to finally obtain a general          information combining localization and context, which is necessary to predict a good segmentation map. 
    2. No dense layer, so images of different sizes can be used as input (since the only parameters to learn on convolution layers are the kernel, and the size of          the kernel is independent from input image’ size). 
    3. The use of massive data augmentation is important in domains like biomedical segmentation, since the number of annotated samples is usually limited.
