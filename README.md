# CSE597
How to run the code: 
* Install all the required packages through the README2.md (requirement.txt does not contain all the required package, need to see the error to do some installs)
* Download ViT-L-14.tar from README2.md, put it at the root directory of the repo
* Create a folder named checkpoints, download mplug_large.pth from README2.md and move the .pth file to that folder
* Dowload the data indices from https://drive.google.com/file/d/1fVwdDvXNbH8uuq_pHD_o5HI7yqeuz0yS/view and put untar it and put the folder to the root of the repo
* Download the ms coco dataset (test2015, train2014, val2014). Create a folder called ln_data at the root of the repo. The COCO dataset should be placed in the directory level: ln_data->other->images->mscoco->images->(test2015, train2014, val2014)
* In grounding_mplug.py, at line 366, set evaluate to false to do the training and validation. Setting evaluate to true will do the evaluation on test set.
* run python grounding_mplug.py
