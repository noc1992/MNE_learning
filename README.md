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
### 1122 raw data : continuous data
    - 연속형 자료 로드
    - raw 객체 쿼리, raw.info()
    - raw 객체 수정
    - 채널 선택, 삭제 및 재정렬
        1) pick_types() : raw 객체를 eeg 및 eog 채널로만 제한
        2) pick_channels()
        3) drop_channels()
    - 채널 이름과 유형 변경 
        1) rename_channels()
        2) set_channel_types() 
    - 시간 영역에서 선택
    - raw 객체에서 데이터만 추출
        1) 이름으로
        2) 유형별로 
        3) 인덱스로
    - 저장 및 내보내기
