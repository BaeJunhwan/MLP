# MLP-based MNIST Digit Classification

PyTorch를 활용하여 MNIST 손글씨 숫자 분류 모델을 구현하고, 모델 구조 변경에 따른 성능 변화를 비교한 프로젝트입니다.
기본 MLP 모델에서 시작해 hidden layer 크기, Dropout, Batch Normalization 등을 적용한 ModifiedMLP 모델을 구성하고 test accuracy 변화를 확인했습니다.

## Features

* MNIST 데이터셋을 활용한 손글씨 숫자 분류 모델 구현
* Flatten, Linear Layer, ReLU를 활용한 MLP 신경망 구성
* CrossEntropyLoss와 Adam optimizer를 사용한 모델 학습
* Dropout과 Batch Normalization을 적용한 모델 성능 비교
* 모델 구조 변경에 따른 test accuracy 변화 확인

## Model Comparison

| Model       | Structure                                                                                                    | Test Accuracy |
| ----------- | ------------------------------------------------------------------------------------------------------------ | ------------- |
| SimpleMLP   | Linear(784→20) → ReLU → Linear(20→10)                                                                        | 95.6%         |
| TwoLayerMLP | Linear(784→50) → ReLU → Dropout → Linear(50→50) → ReLU → Dropout → Linear(50→10)                             | 97.0%         |
| ModifiedMLP | Linear(784→256) → BatchNorm → ReLU → Dropout → Linear(256→128) → BatchNorm → ReLU → Dropout → Linear(128→10) | 98.4%         |

## Tech Stack

* Python
* PyTorch
* Jupyter Notebook

## What I Learned

* 이미지 데이터를 Flatten하여 MLP 모델의 입력으로 사용하는 과정을 이해했습니다.
* CrossEntropyLoss와 optimizer를 활용해 loss 계산, backpropagation, 파라미터 갱신이 이루어지는 흐름을 학습했습니다.
* hidden layer 크기, Dropout, Batch Normalization 적용 여부가 모델 성능에 영향을 줄 수 있음을 확인했습니다.
* 모델 구조를 수정하고 test accuracy를 비교하며 성능 개선 과정을 경험했습니다.
