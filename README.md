# Thief-or-Person-wearing-Mask-Detection

This is a model where a person wearing mask or a thief can be detected. Just follow the simple steps:

1. Run "python gather_annotations.py --dataset thieves --annotations annot.npy --images images.npy" in cmd. You have to create a box around the face with mask in every picture. It will collect all the data and store in .npy file.

2. Run "python train.py --annoatations annot.npy --images images.npy --detector thieves.svm" in cmd. 

3. Run "python test.py --detector thieves.svm --image 55.jpg --annotate thief" in cmd.

This is created using hog+svm model which gives high accuracy. You can also imeplement it in live streaming too. 
