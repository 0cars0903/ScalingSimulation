# ScalingSimulation
---------------------
## 과제 정의
* 압연 공정 Scale 발생 영향인자 분석 및 불량률 예측과 개선방안 도출
### 압연공정
* 금속 소성 가공 방법의 하나로 Roll을 이용하여 두께를 줄이고 일정하게 만드는 과정
1. 온도에 따른 분류 
    - 열간압연  
    - 냉간압연  
    
2. 형상에 따른 분류
    - 평판 압연
    - 형상 압연
    - 링 압연
    - 나사 단조
    
### Scale
* 물에 각종 광물질, 가스, 이온이 존재하는 데 공정 중의 온도상승으로 화학적 결합(염)이 생성되어 침전되는 현상
* 표면이나 배관등에 부착되어 Scale이 형성된다.
* 압연과정에서 강판의 표면에 스케일 층이 형상된다.  
* 마찰계수가 달라져서 강판을 휘어지게 하며, 설비와의 마찰이 증가해 고장의 원인이 된다. 
![image](https://user-images.githubusercontent.com/111993984/222941625-beecf4ec-b2f7-49bd-ade2-75f31b5abeda.png)  

### 분석 배경
* 00 공장의 고객사에서 최근 들어 압연공정에서 Scale 불량이 급증  
* 데이터 수집 후 다양한 분석을 통해 불량 발생의 근본 원인 규명
* 결과를 해석하고 개선 기회를 도출(다양한 분류모델을 활용한 Scale 발생 영향인자 도출 및 핵심 인자를 통한 최적조건 도출로 개선안 제시)
-----------
## 데이터 분석
### 데이터 정제(이상치 처리)
![image](https://user-images.githubusercontent.com/111993984/222941748-5864c0fe-9c7e-4b29-8a34-2a2a723b0b51.png)  
![image](https://user-images.githubusercontent.com/111993984/222941770-e44e96dc-2ebb-4dac-a300-dc333c758091.png)  

### 그래프 분석
![image](https://user-images.githubusercontent.com/111993984/222941844-c6c38f6b-fae9-49ef-b659-d2ebf50d186a.png)  

### 가설검정(t-test)
![image](https://user-images.githubusercontent.com/111993984/222941870-4984e7b9-217e-4e65-8d86-9ebc9ca8b240.png)  
![image](https://user-images.githubusercontent.com/111993984/222941880-51150575-78f3-4335-8aa5-4b3b83f851f8.png)  

### 가설검정(ANOVA)
![image](https://user-images.githubusercontent.com/111993984/222941898-03e69cca-8fcc-4144-88cc-bb3cfacf4a9a.png)

### 모델링 분석
![image](https://user-images.githubusercontent.com/111993984/222941903-fede4aa6-cb36-4748-93ac-7feb0ef0dfd0.png)

### 개선방안
![image](https://user-images.githubusercontent.com/111993984/222941922-f22e27ab-4113-460d-8b3b-aae3a510021d.png)

### 개선방안(교육 종료 후 추가 분석한 결과) : 시뮬레이션을 통한 최적 조건의 효과성 입증 및 관리 조건 도출
* 핵심인자로 선정된 가열대 온도, 균열대 온도, 가열로 온도, 압연온도, HSB 등을 이용하여 시뮬레이션 진행  
![image](https://user-images.githubusercontent.com/111993984/222941971-d56311b9-fb5b-4fa7-b4ef-ce96faacfa6b.png)  

* 균열도 최적조건, HSB 처리를 실시할 경우, 불량률이 32%에서 21%까지 감소한다.
* 압연온도의 최적조건만 달성하더라도 불량률이 0%가 되는 것을 확인하였다.
* 압연 공정 시 온도의 중요성을 확인할 수 있었다.  
* 가열로 공정에서는 온도가 매우 높아서 화학적 결합 반응이 일어나더라도, 가역 반응으로 인하여 Scale 발생 확률이 낮으나,  
* 압연 공정의 온도는 비교적 낮은 온도에서 진행되어 화학적 결합 반응이 발생할 수 있다. 
* 액상페야라이트(Fe2SiO4)의 녹는점 이하에서 공정이 진행되는 압연 공정이 불량 발생이 낮출 수 있는 핵심 공정이다.
