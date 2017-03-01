# Spatio-Temporal Road Detection from Aerial Imagery using CNNs

This repository gathers a semi-automatic tool for labelling videos, as well as a labelled database of videos of roads from the point of view of a small commercial drone. The work done is detailed in the article _Spatio-Temporal Road Detection from Aerial Imagery using CNNs_, presented at the VISAPP 2017, the International Conference on Computer Vision Theory and Applications.

The author of this project is [Belén Luque] (https://www.linkedin.com/in/belén-luque-lópez-ab5046bb/), under the supervision of [Javier Ruiz Hidalgo] (https://imatge.upc.edu/web/people/javier-ruiz-hidalgo) and [Josep Ramon Morros] (https://imatge.upc.edu/web/people/josep-ramon-morros).

## Abstract of the article

The main goal of this paper is to detect roads from aerial imagery recorded by drones. To achieve this, we propose a modification of SegNet, a deep fully convolutional neural network for image segmentation. In order to train this neural network, we have put together a database containing videos of roads from the point of view of a small commercial drone. Additionally, we have developed an image annotation tool based on the watershed technique, in order to perform a semi-automatic labeling of the videos in this database. The experimental results using our modified version of SegNet show a big improvement on the performance of the neural network when using aerial imagery, obtaining over 90% accuracy.

## Publication

_To be updated when the link is published_

## Labelling tool

The technical details on how the tool works are detailed in the article mentioned above. To use the labelling tool, follow the instructions in videoLabeler.py and run the script. Note that the numpy and OpenCV libraries are required.

## Database

The labelled database consists on 3.313 images, gathered from snippets of different Youtube videos. These images have been labelled using the developed semi-automatic tool. The results have been supervised and corrected when needed by the author.

As the videos are not from the author, only the labels are provided. In the labels, (0,0,0) correspond to the class sky, (4,4,4) to road and (6,6,6) to _other_.

The videos used are the following:
* [Video 1] (https://www.youtube.com/watch?v=7ZKsSl5Bxzk)
* [Video 2] (https://www.youtube.com/watch?v=uEkl2M3u4QY)
* [Video 3] (https://www.youtube.com/watch?v=Itas_NSL7k8)
* [Video 4] (https://www.youtube.com/watch?v=5hT6MoJmxNI)
* [Video 5] (https://www.youtube.com/watch?v=KNALyO9zaaA)
* [Video 6] (https://www.youtube.com/watch?v=X2-qVT90lbE)
* [Video 7] (https://www.youtube.com/watch?v=bHV8gidxP-M)
* [Video 8] (https://www.youtube.com/watch?v=oQkOoqHm7O8)
* [Video 9] (https://www.youtube.com/watch?v=75pjRpMBV7A)

A script _will be soon_ provided to obtain the correspondent frames of each video, so the names and ordering of the frames match the labels.

The frames used for each video are:

| Video | Frames from the video | 
| :---: | :---: | :---: |
| Video 1 | [1878-1908] / [2505-2555] / [2918-2948] / [4768-4798] / [7118-7158] / [8509-8528] | 
| Video 2 | [841-916] / [3040-3136] / [2847-2940] / [357-436] / [541-638] / [640-749] / [943-1001] / [1057-1232] / [1916-2033] / [3644-3744] / [3814-3874] / [3904-4032] / [4536-4556] / [4616-4656] / [5083-5113] / [5183-5213] / [5304-5334] | 
| Video 3 | [227-257] | 
| Video 4 | [2110-2150] / [2404-2444] | 
| Video 5 | [2785-2839] / [3337-3450] / [3588-3722] / [4894-5030] | 
| Video 6 | [4299-4329] / [4673-4703] / [4956-4986] / [5026-5036] / [6711-6741] | 
| Video 7 | [1705-1735] / [1821-1836] / [2914-2944] / [3404-3444] | 
| Video 8 | [2681-2721] / [2751-2781] | 
| Video 9 | [2-402] / [809-989] / [1026-1280] / [1673-1769] | 

The order in which the frames are provided follows the order of the labels' names.
