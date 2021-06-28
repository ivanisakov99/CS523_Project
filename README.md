# RED_CNN
This work is directly adapted from the implementation of [Low-Dose CT with a Residual Encoder-Decoder Convolutional Neural Network (RED-CNN)](https://arxiv.org/ftp/arxiv/papers/1702/1702.00288.pdf), which is located in this repo:
https://github.com/SSinyu/RED-CNN

Team members:
* Ivan Isakov, isakovi@bu.edu
* Nicholas Hildenbrand, nhilden@bu.edu

Slides:
* [Presentation](https://docs.google.com/presentation/d/19Hggoo2K1bJLmPTwurCvEA5fHauHIlUo/edit#slide=id.gd23168b479_0_29)

## <ins>Running the script</ins>
1. run `python prep.py` to convert 'dicom file' to 'numpy array'
2. run `python main.py --load_mode=0` to train. If the available memory(RAM) is more than 10GB, it is faster to run `--load_mode=1`.
3. run `python main.py --mode='test' --test_iters=10000` to test.

## <ins>Example Results</ins>
![result_0](https://user-images.githubusercontent.com/60196280/123520314-1fa40b80-d67e-11eb-9955-cd5701abae89.png)
![result_2](https://user-images.githubusercontent.com/60196280/123520338-3ba7ad00-d67e-11eb-98c1-70d6848c121b.png)

## <ins>References</ins>
* Low-Dose CT with a Residual Encoder-Decoder Convolutional Neural Network (RED-CNN), Chen et al. (https://arxiv.org/ftp/arxiv/papers/1702/1702.00288.pdf)
* RED_CNN implementation (https://github.com/SSinyu/RED-CNN)
* Image Dataset (https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=52758026)
* Grand Challenge (https://www.aapm.org/GrandChallenge/LowDoseCT/#patientData)
