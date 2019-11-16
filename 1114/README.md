# 1.ICA와 아티팩트 복구
  1-1 ICA란
    소스신호가 알 수 없는 비율로 함께 혼합된 일련의 기록에서 독립적인 소스 신호를 추정하는 기술 예) 블라인드 소스 분리(파티장에서 말소리분리)
   
  1-2 파이썬에서 ICA
   fastica, picard, infomax 등을 활용
   
  1-3 드리프트를 제거하기 위한 필터링 필요
   저주파수 드리프트를 제거해야 함. 
   
  1-4 ICA솔루션 피팅 및 시각화
   ica.exclued 사용 수동으로 구성요서 지정 가능.  mne.preprocessing.ICA.save(), mne.preprocessing.read_ica().
   apply() 방법을 활용해 제거된 아티팩트로 센서신호 재구성 가능
   
  1-5 EOG 채널을 사용하여 ICA구성요소 선택
   EOG, ECG센서를 패턴으로 사용하여 IC를 검사, EOG/ECG 패턴과 일치하는 IC를 자동 제외
    find_bads_eog()로 일치하는 IC를 자동으로 찾은 다음  plot_scores()으로 확인 
    
  1-6 시뮬레이션 된 채널을 사용하여 ICA구성 요소 선택
   EOG 채널이 없는 경우 EOG의 프록시를 사용할 수 있는  find_bads_eog()의 ch_name라는 매개변수가 있음.
   ECG의 경우  find_bads_ecg()사용 가능 (옵션 사용 가능, 'ctps'(교차 평가 단계 통계 3 ) 및 'correlation'(데이터와 ECG 채널 간의 피어슨 상관 관계).)
   
  1-7 템플릿 일치를 사용하여 ICA구성 요소 선택
   mne.preprocessing.corrmap() 사용 
