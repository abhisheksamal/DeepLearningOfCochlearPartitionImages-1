# DeepLearningOfCochlearPartitionImages

Excuse our look at this time as we collaborate on this work in progress! Currently four group members are contributing their own variations of Raft.ipynb files to make parallel progress.

Our goal is to create a network that will use optical flow techniques to estimate the displacement of the entire field of view within sequential images collected during sinusoidal stimulation of the membrane. There are many sequential image pairs across 13 animal experiments. The magnitude of the displacements is often sub-pixelar and below the resolution limits stated by classical optics

1) To install, one only needs the main Raft.ipynb file, as well as the LAZRHelpers.ipynb file.

2) We suggest using Google Colab, and uploading sample images to a folder called "Coch_data". 

3) Once data is ready for import, "run all" (ctrl+F9) the Raft notebook. This will uninstall Colab's default Pytorch torchvision library, and install a more recent version through URL. The more recent version will have exclusive RAFT tools used in this code.

4)  The notebook will crash after install. This is okay - "run all" again, and the if statement will skip the install step.

5)  Main code runs and imports data. The data is pre-processed, pushed through a small, pretrained RAFT model. Output colored images are displayed to try to visualize the optical flow.

![CohcleaDataSample](https://user-images.githubusercontent.com/48164184/162343901-f901e60b-d73a-4a6e-aad0-c17d6236f1c2.PNG)
a) Raw data, cropped to the section we expect the Regions of Interest (ROI) to be.

![OpticalFlowRawOutput](https://user-images.githubusercontent.com/48164184/162343997-16b17e28-d235-4a71-b1b1-a96c3b12312b.PNG)
b) Raw out put of optical flow

6)  There are sections commented out which have potential to save images, and even create GIF files from the saved images.
