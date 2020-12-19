# OCTFeatureMapVisualization
Feature map visualization and filter visualization in a deep neural network.


**What Is Optical Coherence Tomography?**

Optical coherence tomography (OCT) is a non-invasive imaging test. OCT uses light waves to take cross-section pictures of your retina.

With OCT, your ophthalmologist can see each of the retina’s distinctive layers. This allows your ophthalmologist to map and measure their thickness. These measurements help with diagnosis. They also provide treatment guidance for glaucoma and diseases of the retina. These retinal diseases include age-related macular degeneration (AMD) and diabetic eye disease.

OCT is useful in diagnosing many eye conditions, including:

1. macular hole
2. macular pucker
3. macular edema
4. age-related macular degeneration
5. glaucoma
6. central serous retinopathy
7. diabetic retinopathy
8. vitreous traction

**ABOUT OUR DATA SET (Dataset is in Kaggle https://www.kaggle.com/paultimothymooney/kermany2018 )**

1. The dataset is organized into 3 folders (train, test, val). It contains subfolders for each image        category (NORMAL,CNV,DME,DRUSEN). There are 84,495 X-Ray images (JPEG) and 4 categories                  (NORMAL,CNV,DME,DRUSEN).

2. Images are labeled as (disease)-(randomized patient ID)-(image number by this patient) and split into    4 directories: CNV, DME, DRUSEN, and NORMAL.

**WHAT ALL TO EXPECT FROM THIS KERNEL**

1. Feature map visualization and filter visualization.

2. Modular code so that functions in this kernel can be used easily by everyone,all you need to do is define the model and pass it through function call to convert_data function as demonstrated in last line by convert_data(model).

3. You can easily increase accuracy by adjusting hyper-parameters, for demonstration purposes,due to memory constraints and since I just wanted to show feature map visualization and filter visualization while maintaining modularity of code.

4. Scalable approach thus you can easily put in any adaptive learning model or a bigger CNN too and pass the model to convert_data function. It will detect all convolutional layers and plot 32 feature maps of each convolutional layer in model.

**HOW WILL VISUALIZATION OF FEATURES AND FILTERS HELP**

1. What I find best part about feature visualization is that it kind of tells us how our eye detects feature. If suppose we have an object we analyze many features of that object like its shape,colour,size etc, when we see an object say in a photograph our eye tries to find patterns in the photograph that is peculiar to something it has seen before.These patterns thus play a vital role in discerning the object we detect.What more images in these dataset is of an eye itself (talk about inception :P).

2. Large Convolutional Network models have recently demonstrated impressive classification performance on the ImageNet benchmark. However there is no clear understanding of why they perform so well, or how they might be improved. Thus visualization can help to gain an insight to what our model has learnt.

3. The patterns so detected can be study to adjust hyperparameters and filters in a way to get more accuracy.
