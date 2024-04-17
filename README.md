# MarinaPipe Dataset

Please, download the dataset in the [LINK](https://zenodo.org/records/10951363).

MarinaPipe is an underwater pipeline RGB images dataset recorded in a marina near the north of Portugal by our partner OceanScan-MST using a lightweight autonomous underwater vehicle (LAUV). It contains videos, image frames, and annotation for pipeline segmentation.

This dataset is released with the paper "Bridging the Sim-to-Real GAP for Underwater Image Segmentation" by Luiza Ribeiro Marnet, Stella Grasshof, Yury Brodskiy, and Andrzej Wasowski.<br>

When using MarinaPipe, please reference the paper "Bridging the Sim-to-Real GAP for Underwater Image Segmentation" and acknowledge OceanScan-MST for collecting the data using the lightweight autonomous underwater vehicle (LAUV).

# Description

Seven original videos are available in the repository.<br>

From each of the seven original videos, we extracted five frames per second. Ten percent of these frames were randomly selected from labeling. <br>
The selected images with the respective labels are available for downloading.<br>
Two types of annotation were used: fine and coarse.  The images below exemplify the differences between both. Notice that in the fine annotation the label tries follow the contours of the visible pipeline.<br>

|RGB image    |Coarse annotation| Fine annotation | 
|---------|---------------|-------------------|
|<img align="left" height="100" alt="frame0-01-25 00" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/39a34b5f-8a65-41a7-af78-41a46a916d06">|<img align="left" height="100" alt="frame0-01-25 00_label" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/e155d889-7927-4a8e-a5ef-cef7988a626f">|<img align="left" height="100" alt="frame0-01-25 00_label" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/f5e45a39-2b74-4301-8817-cbdade6468a8">| 

The table below summarizes the datasets. <br>
In the column "annotation type", "both" refers to fine and coarse annotation. <br>


|Video    |Selected frames| Frames with pipes | Annotation Type | Occlusions |
|---------|---------------|-------------------|-----------------|------------|
|1        | 236           | 43                | Both            | Yes        |
|2        | 237           | 70                | Both            | No         |
|3        | 260           | 2                 | Both            | No         |
|4        | 268           | 11                | Both            | Yes        |
|5        | 266           | 45                | Coarse          | Yes        |
|6        | 270           | 11                | Coarse          | Yes        |
|7        | 186           | 17                | Both            | Yes        |

In the table above, "occlusions" refer to marine sediments partially covering some pipelines.<br>

The images below show the differences between a pipeline with and without occlusions. Notice that this dataset does not consider fish on top of the pipeline as occlusion.

|Occlusion    |No occlusion | 
|---------|---------------|
|<img align="left" height="100" alt="frame0-00-25 60" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/194809ef-98e4-4006-bbf2-a142cae855c8">|<img align="left" height="100" alt="frame0-00-53 80" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/7df79aab-f761-4583-9348-3e6b30f9a4f4">| 
|<img align="left" height="100" alt="frame0-02-38 20" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/f221b49b-066b-42fe-b84f-ebe0f3c3b594">|<img align="left" height="100" alt="frame0-01-01 40" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/6698023a-c1d7-43b7-8341-6d19275fdc4c">| 


## Dataset Structure

Upon downloading the dataset, the following folders will be encountered:<br>
* video_1
* video_2
* video_3
* video_4
* video_5
* video_6
* video_7

Inside each of these folders are the folders:
* original_selected_images: image frames selected for being labeled;
* resized_selected_images: the same frames, but cropped;
* fine_annotation: the labels for the fine annotation;
* coarse_annotation: the labels for the coarse annotation.

Notice that the folders video_5 and video_6 do not contain the folder fine_annotation since the frames from these videos were only labeled for coarse annotation, as mentioned in the table above.

The images below show the difference between cropped images and their respective original images. We decided to crop the images like that to mimic the pipeline crossing the image, as would be the case for most of the images in pipeline tracking tasks.<br>


|Original    |Cropped | 
|---------|---------------|
|<img align="left" height="100" alt="frame0-04-35 80" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/f0a60164-e256-43b6-a97f-6900459504f7">|<img align="left" height="100" alt="frame0-04-35 80" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/a4b2ae97-703e-4a11-a2b9-974b90fd0aea">|
|<img align="left" height="100" alt="frame0-08-12 40" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/8505edb9-0b1f-4c4b-a052-abbf7b9b711b">|<img align="left" height="100" alt="frame0-08-12 40" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/d5eb73a5-c852-4416-8ed7-b7f5450c3f30">|


## Acknowledgements

<a href="remaro logo">
    <img align="left" height="60" alt="remaro logo" src="https://github.com/remaro-network/Uncertainty-Driven-Active-Learning-for-Underwater/assets/58445878/31ab8e37-cc9e-4592-8f43-aebf9251cac6">
</a>
This work is part of the Reliable AI for Marine Robotics (REMARO) Project. <br> For more info, please visit: <a href="https://remaro.eu/">https://remaro.eu/</a>. <br><br>
<br style="clear: both;">

<a href="eiva_logo">
    <img align="left" height="70" alt="EIVA__1_-removebg-preview" src="https://github.com/remaro-network/Uncertainty-Driven-Active-Learning-for-Underwater/assets/58445878/f995bd10-ba93-4d3d-8abb-39b8b2c6c11a">
</a>
This research was developed in collaboration with EIVA a/s. <br>Please, visit <a href="https://www.eiva.com/">EIVA's webpage</a>. <br><br>
<br style="clear: both;">

<a href="eu_flag">
    <img align="left" height="60" alt="OceanScan logo" src="https://github.com/remaro-network/MarinaPipe-dataset/assets/58445878/690de90c-3024-463c-a8c9-81173dd4126a">
</a>
We thank OceanScan - Marine Systems & Technology Lda for recording the real pipeline dataset. The dataset was recorded using a lightweight autonomous underwater vehicle (LAUV) <br>Please, visit <a href="https://www.oceanscan-mst.com/">OceanScan's webpage</a>. <br><br>
<br style="clear: both;">

<a href="eu_flag">
    <img align="left" height="60" alt="EU logo" src="https://github.com/remaro-network/Uncertainty-Driven-Active-Learning-for-Underwater/assets/58445878/7577c757-8b02-487a-9742-eea398a9100d">
</a>
Partially supported by the European Union’s Horizon 2020 research and innovation programme under the Marie Skłodowska Curie grant agreement No 956200, REMARO. <br><br>
