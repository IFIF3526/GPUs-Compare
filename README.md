![header](https://capsule-render.vercel.app/api?type=waving&color=6FC7E1&height=250&section=header&text=GPU/CPU%20Compare&fontColor=003153&fontSize=58&animation=fadeIn&fontAlignY=38&desc=Compare%20to%20Steam%20Games%20Recommended%20Requirements!&descAlignY=55&descAlign=57)

# GPUs Compare App

http://ec2-3-34-135-181.ap-northeast-2.compute.amazonaws.com:8501

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
[![Streamlit Badge](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=Streamlit&logoColor=white)](https://streamlit.io/)

## 기능
---

- NVIDIA 와 AMD의 그래픽카드의 성능을 비교하여 볼수있다.
- benchmark점수를 비교하여 더 좋은 그래픽카드는 무엇인지 알아볼수 있다.
- WordCloud를 이용하여 데이터의 빈도를 눈으로 확인할수 있다.
- 탐색적 데이터 분석 (Exploratory Data Analysis)
  - 전체 데이터
  - 통계치
  - 연도별로 출시한 그래픽카드를 보며 확인할수 있다.

---


## 과정

- FLASK와 Streamlit을 이용하여 웹 개발 환경을 구축하고 개발하였습니다.
- AWS - EC2로 서버를 구축하여 배포하고 관리합니다.
- Google Colab을 이용하여 데이터 가공을 하였습니다.

---

## 컬럼명 설명
1. manufacturer : 제조사
2. productName : 제품 이름 (그래픽카드)
3. releaseYear : 출시년도
4. memSize : 그래픽카드에 탑재되어있는 VRAM의 용량 이 메모리가 크면 클수록 렌더링에 필요한 텍스처를 많이 저장할수 있지만, 그래픽카드의 근본적인 연산성능과는 관련이 없는 스펙입니다.
5. memBusWidth : 메모리 버스 또는 메모리 인터페이스 라고도 합니다. 그래픽카드 메모리와 GPU간의 통로를 뜻하며, 이 수치가 높을수록 한번에 지나다닐수 있는 폭이 넓어지게 됩니다. 쉽게 표현하여 차선이라고도 합니다. 384 memBusWidth의 경우엔 384 차선이겠네요.
6. gpuClock : 그래픽카드 칩셋의 동작 클럭입니다. 일반적으로 gpuClock가 높다면 그래픽카드의 처리속도가 빨라집니다.
7. memClock : 유효 메모리 클럭입니다 메모리 버스를 차선에 비유하였다면 memClock은 차의 속도로 비유합니다.
8. bus : 버스 인터페이스 (Bus Interface)
컴퓨터를 열어보면 CPU,하드디스크,RAM등 이 있다. 서로 독립적으로 동작하는 것이 아니라 서로 데이터를 주고 받는다. 이런 데이터를 주고 받기위한게 I/O 버스(BUS) 이다. 지하철이나 비행기도 이용방법을 알아야 탑승이 가능 한것 처럼 I/O버스의 통신방식을 이해하지 못하면 데이터를 보낼수도 받을수도 없다. CPU 내에는 I/O 버스의 통신방식을 이해하고 있는 것이 바로 버스 인터페이스 이다. 버스 인터페이스 장치는 버스가 어떻게 데이터를 전송하는지 그에 대한 프로토콜 혹은 통신방식을 알고 있다.
출처: https://cinrueom.tistory.com/39 [내 의지로 여기서 끝을 보겠노라.:티스토리]
9. memType : 그래픽카드에 탑재된 메모리의 종류입니다. 
10. G3Dmark : 1초당 그려지는 프레임(Frame Per Second)즉 FPS의 숫자를 기준으로 점수를 매긴다. 높을수록 성능이 뛰어나다는 것이다.


### DATA BY
1. https://www.kaggle.com/datasets/alanjo/graphics-card-full-specs
2. https://www.kaggle.com/datasets/alanjo/gpu-benchmarks

![Footer](https://capsule-render.vercel.app/api?type=waving&color=6FC7E1&height=100&section=footer)
