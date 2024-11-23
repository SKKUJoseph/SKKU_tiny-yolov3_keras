# keras-yolo3와 Roboflow

[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)

이 저장소는 Keras를 활용한 YOLOv3 (TensorFlow 백엔드)의 구현체로, [allanzelener/YAD2K](https://github.com/allanzelener/YAD2K)를 참고하여 작성되었습니다.

## 학습 목표
* Roboflow에서 커스텀 이미지 감지 데이터를 불러오는 방법
* Keras에서 YOLOv3 모델을 설정하는 방법
* YOLOv3 모델을 학습시키는 방법
* 학습된 모델을 이용하여 추론(Inference)하는 방법
* 추후 사용을 위해 Keras 모델 가중치를 저장하는 방법

## 리소스

* [이 블로그 포스트](https://blog.roboflow.ai/training-a-yolov3-object-detection-model-with-a-custom-dataset/)는 튜토리얼에 대한 상세한 내용을 제공합니다.
* 이 노트북에서 튜토리얼을 실행할 수 있는 코드를 확인할 수 있습니다: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ByRi9d6_Yzu0nrEKArmLMLuMaZjYfygO#scrollTo=WgHANbxqWJPa)
* 읽기 전용으로는 Tutorial.ipynb 파일에 저장된 코드를 확인할 수 있습니다.

## Roboflow를 이용한 데이터 관리

[Roboflow](https://roboflow.ai)는 컴퓨터 비전용 데이터셋을 관리, 전처리, 증강, 버전 관리하는 작업을 간단하게 만들어줍니다.  
개발자는 Roboflow를 활용해 코드 작성량을 50% 줄이고, 어노테이션 품질을 자동으로 확인하며, 학습 시간을 단축하고, 모델 재현성을 높일 수 있습니다.

![alt text](https://i.imgur.com/WHFqYSJ.png)

## 모델 가중치 다운로드

이 저장소를 사용하는 데 도움이 되도록 사전 학습된 모델 가중치를 제공합니다. 아래 링크에서 가중치를 다운로드할 수 있습니다:

**[YOLOv3 모델 가중치 다운로드](https://drive.google.com/uc?id=YOUR_SHARED_FILE_ID)**

### Google Drive를 통한 파일 공유 방법

1. Google Drive에 모델 가중치 파일(e.g., `yolov3_weights.h5`)을 업로드합니다.
2. 업로드한 파일을 우클릭한 뒤 **"공유"**를 선택합니다.
3. 공유 설정에서 **"링크 복사"**를 클릭합니다.
4. 링크 액세스 권한을 **"링크가 있는 사용자가 보기 가능"**으로 설정합니다.
5. 링크에서 파일 ID를 복사합니다. 예를 들어, 링크가 아래와 같다면:
https://drive.google.com/file/d/1A2B3C4D5E6F7G8H9I/view?usp=sharing

파일 ID는 `1A2B3C4D5E6F7G8H9I`입니다.
6. 위 다운로드 링크의 `YOUR_SHARED_FILE_ID` 부분을 이 파일 ID로 교체합니다.

이제 사용자는 제공된 링크를 클릭하여 사전 학습된 가중치를 바로 다운로드할 수 있습니다.
