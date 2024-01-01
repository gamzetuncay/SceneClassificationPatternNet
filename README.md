# SceneClassificationPatternNet

**Scene Classification of PatternNet Dataset Using Transfer Learning** 

A variety of applications depend on the scene classification of high-resolution satellite images. Due to high spatial resolution remote sensing images can be easily acquired, several types of scene classification techniques were developed in recent years. Transfer learning, particularly leveraging convolutional neural networks (CNNs), has proven to be effective in image classification. It also has found applications in remote sensing. This paper aims to analyze the use of deep convolutional neural networks (CNNs) for scene classification, using two efficient methods for CNN feature extraction. First, pre-trained ResNet18 model is used as general feature extractors. Second, pre-trained ResNet18 model on the scene classification dataset will be fine-tuned. Within the scope of this project, the capabilities of ResNet (Residual Network) are specifically explored on the publicly available PatternNet dataset, which encompasses 38 classes. This investigation aims to contribute insights into the efficacy of deep learning approaches, shedding light on their potential applications and advancements in the field of remote sensing.

Note: Before going to the code it is requested to work on a jupyter notebook with GPU.


1. Download the dataset from [https://sites.google.com/view/zhouwx/dataset](https://sites.google.com/view/zhouwx/dataset)
2. Create a virtual environment and activate environment
```
$ python -m venv myenv 
$ source myenv/bin/activate
```

3. Run below code tp prepare the environment
```
pip install -r requirements.txt
```

File structure should look like this
   ```
    - SceneClassificationPatternNet
      -- data_preprocessing.py
      -- myenv
      -- transfer_learning.ipynb
      -- requirements.txt
      -- PaternNet
        ---images
        ---patternnet_description.pdf
   ```

4. Run below code to prepare dataset
```
python data_preprocessing.py
```
5. Now you can open and run transfer_learning.ipynb
