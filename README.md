# MarinaPipe Dataset
Underwater pipeline RGB images dataset recorded in the botom flor of a recorded in a marina close to the north of Portugal, by our partner OceanScan-MST using a lightweight autonomous underwater vehicle (LAUV). It contains videos, image frames and annotation for pipelinesegmentation.

This dataset is released together with the paper "Bridging the Sim-to-Real GAP for Underwater Image Segmentation", by Luiza Ribeiro Marnet, Stella Grasshof, Yury Brodskiy, and Andrzej Wasowski.

The seven original videos are available in the repository.

From each video, 5 frames per second were extracted. From these frames, 10% were randomely selected from labeling. 
The selected images with the respective labels are available for downloading.
Two types of annotation were used, fine and coarse.  The images below exemplify the the differences between both.

The table bellow sumarizes the datasets.
In annotation type, both referes to both fine and coarse annoation. 

|Video    |Selected frames| Frames with pipes | Annotation Type | Occlusions |
|---------|---------------|-------------------|-----------------|------------|
|1        | 236           | 43                | Both            | Yes        |
|2        | 237           | 70                | Both            | No         |
|3        | 260           | 2                 | Both            | No         |
|4        | 268           | 11                | Both            | Yes        |
|5        | 266           | 45                | Coarse          | Yes        |
|6        | 270           | 11                | Coarse          | Yes        |
|7        | 186           | 17                | Both            | Yes        |

In the table above, occlusions refers to the fact that some pipelines are partially covered by marine sedments.
The images bellow show the differences between a pipeline with occlusions (left) and a pipeline with no occlusions (right).

## Dataset Structure

When downloading the dataset, inside the root you will find the folders:

The images below show the difference between a cropped image and its respective original image.

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
We thank OceanScan - Marine Systems & Technology Lda for recording the real pipeline dataset. <br>Please, visit <a href="https://www.oceanscan-mst.com/">OceanScan's webpage</a>. <br><br>
<br style="clear: both;">

<a href="eu_flag">
    <img align="left" height="60" alt="EU logo" src="https://github.com/remaro-network/Uncertainty-Driven-Active-Learning-for-Underwater/assets/58445878/7577c757-8b02-487a-9742-eea398a9100d">
</a>
Partially supported by the European Union’s Horizon 2020 research and innovation programme under the Marie Skłodowska Curie grant agreement No 956200, REMARO. <br><br>
