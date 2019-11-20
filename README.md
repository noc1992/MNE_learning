# MNE 패키지에 대해 혼자 공부해보는 공간 입니다.

### tutorial을 보며 혼자 공부해 본 공간입니다.

### 1112 - 튜토리얼 시작 : 
    - 샘플 데이터 설치 
    - raw데이터 시각화 
    - 역이미징 사용 
    - 역 모델링(역해법 계산)

### 1113 - 전처리 파트 1 : 
    - 아티팩트 처리 
    - 불량 채널 보간 
    - 불량 데이터 스팬 거부 
    - 데이터 정제 및 리샘플링

### 1114 - 전처리 파트 2 : 
    - ICA 아티팩트 복구

### 1115 - 전처리 파트 3 : 
    - ICA 응용 버전들 - fastICA / picard / infomax

### 1116 - 전처리 파트 4 : 
    - SSP와 아티팩트 복구 
    - EEG 기준 설정 
    - SSS와 멕스웰 필터링 / 
### 1119 주파수 및 시간 주파수 센서 분석
    - mne.time_frequency : tfr_morlet, psd_multitaper, psd_welch
    
### 1120 MNE 패키지의 전반적 기초
    - 데이터 로드 :  mne.datasets.sample.data_path() 
    - reject
    - vis_epochs.average(), aud_epochs.average()
    - 역 모델링 
        1) mne.minimum_norm.read_inverse_operator, mne.minimum_norm.apply_inverse
        2) stc.plot
