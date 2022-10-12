# Cyber Threat Information Sharing 
> KrCERT는 AI 및 데이터 연관 분석을 위해 FENS 시스템을 개발하여 내부적으로 활용하고 있으며, 해당 시스템을 통해 추출된 최근 침해사고 위협정보 & 특징정보 데이터셋을 외부에 공유하고 기업 및 연구기관에서 적극 활용하여 AI 모델 개발, 위협 헌팅 등 보안 성능의 향상을 기대한다.
> KrCERT has developed and internally used the FENS system for AI and data correlation analysis. It is expected that the security performance such as AI model development and threat hunting will be improved by sharing the recent intrusion threat information & feature dataset extracted through the system and actively utilizing it in companies and research institutes.

## FENS(Feature Engineering Normalization System)
### 0. Introduction
> The FENS system is a system designed to create/analyze/manage data sets by analyzing intrusion information in real time to respond quickly to intrusion incidents, identify threats, and preemptively respond.

### 1. Main Functions

 1.1. Automatic analysis: When intrusion incident information such as malicious code is registered in FENS, dynamic analysis is requested from the sandbox, and static analysis information and metadata are analyzed through static analysis libraries such as IDA Python.

 1.2. Extraction and analysis of feature information: From the analyzed information, it goes through the normalization process (Filtering, Cleansing, Converting) for AI learning and threat identification, then extracts features from the raw data, processes them in a format suitable for analysis, and saves them as a json file.
      
 1.3. Visualization analysis: Visualization analysis was applied for efficient association analysis. By normalizing each characteristic information, information is generated based on node/edge and stored in the graph DB, and the stored characteristic information is visualized according to the normalized data standard.
 <img width="1912" alt="스크린샷 2022-09-15 오후 2 37 59" src="https://user-images.githubusercontent.com/13616727/190322993-8d11a259-bc82-440d-9d06-1022376a604d.png">

 
### 2. Architecture

<img width="1008" alt="스크린샷 2022-09-15 오후 2 32 13" src="https://user-images.githubusercontent.com/13616727/190322290-4234b79e-0db1-4756-8f2e-3a776b80e338.png">




## Feature Data Sheet
> Companies and institutions are applying and researching various techniques such as AI to efficiently analyze and respond to a rapidly increasing amount of malicious code. For such a study, it is necessary to accurately identify the characteristics of an intrusion accident, and it is most important to determine which features to select and use to improve accuracy and efficiency. KrCERT analyzes various incidents and malicious codes, selects and categorizes high-importance features among numerous features of malicious codes, and utilizes them for analysis and response.

1. Malware Feature : <a href = "Feature Sheet/Malware Feature Data Sheet.pdf">Feature Sheet/Malware Feature Data Sheet.pdf</a>
2. APK Feature : <a href = "Feature Sheet/Android Feature Data Sheet.pdf">Feature Sheet/Android Feature Data Sheet.pdf</a>

## Data Set
> 이슈에 대해 침해사고 유형별 특징정보를 추출하고 있으며, 이를 통해 AI 학습, 룰 제작, 위협 헌팅 등에 활용 할 수 있다.
1. Ukraine cyber war
```sh
우크라이나 전쟁 발발(2022년 2월) 이후 현재(2022년 9월)까지 1000여건 이상의 사이버 공격이 발생하고 있다. 
KrCERT는 여기에서 사용된 무기(악성코드)가 재사용될 가능성이 높다고 판단됐고 변종 악성코드 유포로부터 피해를 최소화히기 위해
이를 지속적으로 수집하고 특징정보를 추출하고 있으며, 이렇게 수집되고 관리되고 있는 악성코드 패밀리는 총 12종이다. 
```

2. Proecessing...



## 
KrCERT : https://boho.or.kr/krcert/intro.do
