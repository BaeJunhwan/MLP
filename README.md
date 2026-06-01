# MLP MNIST Classification

PyTorch를 활용하여 MLP 기반 MNIST 손글씨 숫자 분류 모델을 학습한 프로젝트입니다.
28×28 크기의 손글씨 숫자 이미지를 입력으로 사용하고, Linear layer와 ReLU를 포함한 MLP 구조를 구성하여 0부터 9까지의 숫자를 분류하는 과정을 다루었습니다.

## Project Structure

* `mlp.ipynb`: MNIST 데이터 로드, MLP 모델 정의, 학습 및 평가 과정이 포함된 Jupyter Notebook

## Features

* MNIST 데이터셋을 활용한 손글씨 숫자 분류
* 28×28 이미지 데이터를 Flatten하여 MLP 입력으로 변환
* Linear layer와 ReLU를 활용한 신경망 구조 구성
* CrossEntropyLoss를 사용한 loss 계산
* Optimizer를 활용한 모델 파라미터 업데이트
* Test dataset을 활용한 모델 정확도 평가
* Hidden layer 크기, activation function, dropout 적용 여부에 따른 성능 변화 확인

## Development Environment

* Language: Python
* Framework: PyTorch
* Environment: Jupyter Notebook

## What I Learned

이 프로젝트를 통해 머신러닝 모델 학습의 기본 흐름을 경험했습니다.
데이터를 불러오고 전처리한 뒤, MLP 모델을 정의하고 loss를 계산하며 optimizer를 통해 모델의 파라미터가 갱신되는 과정을 확인했습니다.

또한 hidden layer 크기와 dropout 적용 여부에 따라 모델의 성능이 달라질 수 있다는 점을 확인하면서, 모델 구조와 학습 설정이 결과에 영향을 준다는 것을 배웠습니다.
이를 통해 데이터 전처리, 모델 설계, 학습, 평가로 이어지는 딥러닝 모델 구현 과정을 이해할 수 있었습니다.

## How to Run

1. Jupyter Notebook 환경에서 `mlp.ipynb` 파일을 엽니다.
2. 필요한 라이브러리를 설치합니다.

```bash
pip install torch torchvision
```

3. Notebook의 셀을 순서대로 실행하여 모델을 학습하고 평가합니다.

## Future Improvements

* CNN 모델과 MLP 모델의 성능 비교
* Learning rate, hidden layer 크기 등 하이퍼파라미터 실험 추가
* 학습 loss와 accuracy 변화를 시각화
* 모델 구조별 결과 비교 정리
