# Optimized instance segmentation by super-resolution and maximal clique generation

Code Developed for paper Optimized instance segmentation by super-resolution and maximal clique generation

[https://content.iospress.com/articles/integrated-computer-aided-engineering/ica200621](https://content.iospress.com/articles/integrated-computer-aided-engineering/ica230700)

In this repository, a new proposal has been developed. Our proposal is based on detecting several initial detections to generate a number of sub-images using super-resolution (SR) techniques, increasing the number of pixels of the elements contained in it, and re-infer using the same pre-trained CNN model. A reduced set of windows is calculated in the super-resolved image. This analysis is done by finding maximal cliques in the graph. Experiments show an improvement of up to 8.1% for the YOLACT++ model used in the Jena sequence of the CityScapes dataset.

A demo is provided to run our proposal on the following jupyter notebook:

* [https://github.com/IvanGarcia7/OSCOD/blob/main/DEMO.ipynb](https://github.com/IvanGarcia7/Optimized_instance_segmentation_by_super_resolution_and_maximal_clique_generation/blob/main/Main.ipynb)

Within the jupyter notebook, all the necessary steps are established to initialize the work environment, download the pre-trained super-resolution and object detection models and execute the proposal. 

# Workflow of the proposed technique:

![WORKFLOW](https://github.com/IvanGarcia7/Optimized_instance_segmentation_by_super_resolution_and_maximal_clique_generation/blob/main/IMAGES/ICAE2.svg?raw=true)

# Execution Test:

## Input Image:

After downloading and loading the necessary models, we want to improve the detections on a given image as input, e.g. the Figure below:

![INPUT IMAGE](https://github.com/IvanGarcia7/Optimized_instance_segmentation_by_super_resolution_and_maximal_clique_generation/blob/main/IMAGES/darmstadt_000084_000019_leftImg8bit_RAW.png?raw=true)

After performing the successive detections, an output image will be generated. 

## Output:

![OUTPUT IMAGE](https://github.com/IvanGarcia7/Optimized_instance_segmentation_by_super_resolution_and_maximal_clique_generation/blob/main/IMAGES/darmstadt_000084_000019_leftImg8bit_MASK0.png?raw=true)



