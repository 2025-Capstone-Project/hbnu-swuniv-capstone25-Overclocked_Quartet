# Source Code
## 주의사항
 - 다른 Open Source SW를 사용하는 경우 저작권을 명시해야 함
 - 산학연계 캡스톤의 경우 기업의 기밀이 담긴 데이터는 제외할 것.
  - BMC: 서버 내 부품의 온도센서데이터(CPU, GPU)를 조회하는 코드
  - Data-Analysis: AI 이상탐지 모델 학습 데이터셋 분석 코드. 전처리(Blur, ClAHE...), 클러스터링 분석 등 포함.
  - YOLO_TRAIN: AI 이상탐지 모델 학습 코드.
  - FAN_Controller: 쿨링 팬 제어 코드, 서버컴퓨터의 온도 측정 정보에 따라 최적 PWM 계산, 라즈베리파이를 사용해 팬 PWM 제어 기능 포함.
  - SpringBoot_Web_Monitoring: 스프링 부트 기반 웹 모니터링 시스템. BMC온도, AI 이상탐지 정보, 팬 PWM 정보 등 조회 가능.
  - lepton_spi_control, lepton_usb_control: Flir Lepton 3.5 카메라 제어 코드. 각각 SPI와 USB 포트로부터 열화상 데이터를 조회하여 OpenCV 포맷으로 표시
  - purethermal1-uvc-capture: AI 이상탐지 코드. Flir Lepton 3.5로부터 얻은 열화상 데이터를 AI 이상탐지 모델에 통과시킨 후 판별 결과를 InfluxDB에 전송
  - sys-temp-to-influxdb: InfluxDB에 온도데이터 전송을 위한 코드. [Local PC - InfluxDB Server]
 
 <span style="color:red">
 - **기업 기밀 데이터가 Github에 공개되었을 시의 책임은 공개한 학생에게 있음**
 </span>
