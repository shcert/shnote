# SIEM(Security Information Event Management) 빅데이터 기반 보안 정보 이벤트 관련 시스템

기업 전산시스템에서 발생되는 모든 이벤트를 수집하여 빅테이터 분석 수준으로 통합 분석하는 시스템이다.  
인프라 전체에서 발생하는 로그를 수집, 저장 및 분석합니다.   
로그를 시각화, 필터를 효과적으로 수행하게 도와주고 실시간으로 관제역할을 해준다.  

# 특징 

* 빅데이터 기반 보안솔루션으로 기업에 발생하는 다양한 데이터들을 분석하여 위협 요소를 파악할수 있게 해줌
* 실시간 위험을 탐지 및 대응을 위해 이벤트 로그 데이터를 실시간으로 수집하고 분석하는 기능을 하며, <br>침해 공격 로그에 대한 포렌식과 컴플라이언스 또는 법적 조사를 위해 해당 데이터의 신속한 검색 및 리포팅 기능도 제공
* 데이터를 정규화 하여 데이터를 표준화 하고 분석함

* 대포적인 장비
    * ELK Stack <- 유로지만 제한이 splunk보다 덜함(정확하게는 플러그인과 엔지니어 도움)
    * splunk <- 유로에 제한이 많음 하지만 사용자 친화적이고 회사에서 보증하는 서비스이기에 많은 기업들이 splunk를 많이 사용한다.