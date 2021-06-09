# description
## “배경 및 목표”  ##
컴퓨터가 보다 인간과 같이 이미지 속에서 사물을 인식하고 이를 간단한 문장, 캡션으로 표현할 수 있게 하는 머신러닝 연구영역을 통해 Convolution Neural Network와 Recurrent Neural Network과 같은 대표적인 머신러닝 모델의 구조와 원리를 조금 더 명확히 이해보고자 공개된 관련 프로젝트를 진행해 보았습니다. 

## “프로젝트 개요 및 기술내역, 배운 것” ##
 전처리 후 벡터화된 이미지와 문자열들을 '데이터 제너레이터', 새로운 데이터 생성기,를 통해 연결하고 이를 학습하여, 입력받은 이미지와 제일 연관된 단어1, 그리고 이 단어 1과 제일 밀접한 단어2 등등을 도출하여 이미지에 대한 간단한 표현을 구현하는 프로젝트입니다. 가령, 강아지 한 마리가 풀밭에서 뛰어노는 사진이 입력되면 이것이 벡터화되고, 최종적으로 A dog is running at grass와 같은 문장이 도출됩니다.

# requirements
! 버전은 추후 업데이트 예정
numpy
pandas
matplotlib
string
os
PIL
glob
pickle

keras

# Explanation of Data

train_captions.txt
ex) key, desc : 사진명, 캡션
1000268201_693b08cb0e.jpg,A child in a pink dress is climbing up a set of stairs in an entry way .
1000268201_693b08cb0e.jpg,A girl going into a wooden building .
1000268201_693b08cb0e.jpg,A little girl climbing into a wooden playhouse .
1000268201_693b08cb0e.jpg,A little girl climbing the stairs to

Images 폴더
위 키값에 대응하는 .jpg 이미지들

## 학습과정

![캡처](https://user-images.githubusercontent.com/82523058/121379659-34df2180-c97f-11eb-8db5-34921f1e8ad3.PNG)
