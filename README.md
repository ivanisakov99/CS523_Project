# RED_CNN
This work is directly adapted from the implementation of [Low-Dose CT with a Residual Encoder-Decoder Convolutional Neural Network (RED-CNN)](https://arxiv.org/ftp/arxiv/papers/1702/1702.00288.pdf), which is located in this repo:
https://github.com/SSinyu/RED-CNN

Team members:
* Ivan Isakov, isakovi@bu.edu
* Nicholas Hildenbrand, nhilden@bu.edu

Slides:
* [Presentation](https://docs.google.com/presentation/d/19Hggoo2K1bJLmPTwurCvEA5fHauHIlUo/edit#slide=id.gd23168b479_0_29)

## <ins>Running the script</ins>
1. The reproduction of this project must be in done using a GPU in the SCC. 
2. Navigate to the SCC in the browser and select desktop from the interactive apps drop down.
3. Fill in the following:
    List of modules to load (space separated): python3/3.8.6 pytorch/1.7.0
    Working Directory: /projectnb/cs523/Niko_Ivan
    Initial command to run: xfce4-terminal
    Number of hours: 5
    Number of cores: 1
    Number of gpus: 1
    GPU compute capability: 6.0
    Project: cs523
4. run `module load python3/3.8.6`
5. run `module load pytorch`
6. run `python prep.py` to convert 'dicom file' to 'numpy array'
7. run `python main.py --load_mode=0` to train. If the available memory(RAM) is more than 10GB, it is faster to run `--load_mode=1`.
8. run `python main.py --mode='test' --test_iters=12000` to test.

## <ins>Example Results</ins>
![result_0](https://user-images.githubusercontent.com/60196280/123520314-1fa40b80-d67e-11eb-9955-cd5701abae89.png)
![result_2](https://user-images.githubusercontent.com/60196280/123520338-3ba7ad00-d67e-11eb-98c1-70d6848c121b.png)

## <ins>References</ins>
* Low-Dose CT with a Residual Encoder-Decoder Convolutional Neural Network (RED-CNN), Chen et al. (https://arxiv.org/ftp/arxiv/papers/1702/1702.00288.pdf)
* RED_CNN implementation (https://github.com/SSinyu/RED-CNN)
* Image Dataset (https://wiki.cancerimagingarchive.net/pages/viewpage.action?pageId=52758026)
* Grand Challenge (https://www.aapm.org/GrandChallenge/LowDoseCT/#patientData)
