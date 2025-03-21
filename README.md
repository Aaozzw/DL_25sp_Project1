# DL_25sp_Project1
CS6953/ECE7123 Deep Learning Project1

Group members: Zhuoao Wang, Tianyu Luo, Yuqi Wang

### Project Introduction

Opetimizing ResNet18 for CIFAR-10 Classification.

### Directory Structure
```
│  Parameter.xlsx                   # Parameter log
│  RN18_V6_1.ipynb                  # Main file
│  
├─data      # overwrite after Run 'RN18_V6_1.ipynb'
│  │  cifar-10-python.tar.gz
│  │  
│  └─cifar-10-batches-py
│          
├─input     #Create the floder and place it in the path
│      cifar_test_nolabel.pkl       # Test set
│      
└─output    # overwrite after Run 'RN18_V6_1.ipynb'
        Acc.png                     # Accuracy plot
        smaller_resnet_final.pth    # Trained model
        submission.csv              # Result file
        Train loss.png              # Loss plot
```

### Usage Instructions

After cloning to the local Machine, you can directly run the 'RN18_V6_1.ipynb'.
**pls create the 'input' folder and ensure that the 'cifar_test_nolavel.pkl' are inside it.**
The results will be automatically saved on the './output' folder.

If you do not to train the model and only analyze the test set.
pls, simply comment out code in the main function:
```python
    #train_model(model, trainloader, testloader, config, device)
```
