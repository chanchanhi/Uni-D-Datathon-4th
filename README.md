# UNI-D 4th Baseline
## Image Denoising Task Using Restormer

## Training
### classification.ipynb에 있는 코드를 기준으로 실행하면된다. 이때 3번의 training 과정이 있으며 점차 learning rate를 줄여가며 정확도를 높힌다. 이때 여전히 분류하지 못하는 모델을 확인하고 추후에 그 모델의 경우 분류할 이유가 없기에 image restoration 하는 모델에서 같은 모델이 처리하도록 한다.
## Inference
### 먼저 test.ipynb 에서 실행하면 test이미지에 대한 path와 label을 Map 형식으로 받아서 json파일로 저장 가능하고 이파일을 minjun branch에서 test할때 사용한다.

## 모델 환경 RTX 3090 24GB

### 코드에서 사용한 models.resnet18(pretrained=True)은 PyTorch의 torchvision 라이브러리에서 제공하는 ResNet-18 모델의 사전 학습된(pretrained) 버전을 로드하는 것입니다. 이 사전 학습된 모델은 ImageNet 데이터셋에서 미리 학습된 가중치를 사용하고 있습니다.
