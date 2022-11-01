# Cyber Threat Information Sharing 
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
> Feature Data Set is extracted from incidents that are becoming issues. This can be used for AI learning, rule making, and threat hunting.
1. Ukraine cyber war
```sh
Since the outbreak of the Ukrainian War (February 2022) to the present (October 2022), more than 1,000 cyberattacks have occurred.
KrCERT has determined that the weapon (malware) used here is likely to be reused. 
In order to minimize damage from the distribution of malicious code variants, 
it is continuously collecting and extracting feature data set, 
and there are a total of 12 types of malicious code families that are collected and managed in this way.
```

2. Proecessing...



## 
KrCERT : https://boho.or.kr/krcert/intro.do
