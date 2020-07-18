# Edge_computing

Nvidia Jetson nano


# Model Links
## For N stress detection
Download link for pretrained model
[link](https://drive.google.com/drive/folders/1pVvE13rbemEhJkpmHpb0Y5s4UAAWjaDd?usp=sharing).


## For Leaf Rust (*Puccinia triticina*)
Different models for leaf rust identification
[link](https://drive.google.com/drive/folders/16cp_STmyDPZApVKWuAFTSKa9bHb8TVj7?usp=sharing )


# Using the model on the device
Example for making inference on the image when datasetdirectory has subdirectory healthy_diseases, with test directory  in it containing images to be tested whether it is diseased or not.
```bash
cd jetson-inference/python/training/classification
DATASET=~/datasets/healthy_diseased
imagenet-console.py --model=resnet50/resnet50.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/12_diseased.jpg
```

 *Note:  you can aso import onxx model in your pc as it is general format for saving model across devices* _emphasize_
