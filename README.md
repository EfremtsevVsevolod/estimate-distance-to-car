# Digital breakthrough 2022. Ulyanovsk region championship
The championship task is to develop an algorithm that allows you to determine the distance to the vehicle in front in real-time, using a dataset of car photos from different distances. Subsequently, this algorithm can be used in navigation systems to warn of a dangerous approach and monitor distance compliance.

**Place according to the championship results: `2 out of 383` 🏆🏆🏆**

## Data
* Training data set: https://lodmedia.hb.bizmrg.com/case_files/791333/train_dataset_train.zip
* Test data set: https://lodmedia.hb.bizmrg.com/case_files/791333/test_dataset_test .zip

## Brief description of the solution:
1. At the first step, car license plates were detected on the image using the state-of-the-art model YOLOv7, determining their sizes and coordinates.
2. At the second step, the found numbers were filtered and the number related to the car in question was determined.
3. Next, the metainformation of the photo in question was added for the correct operation of the algorithm on devices with different cameras.
4. Using a linear regression model, the distance to the car of interest was calculated.

## Technical features:
* Python, PyTorch, YOLOv7, Linear Regression
* Computer vision, Distance estimation, Object detection, ANPR recognition, Exif data
