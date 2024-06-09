# Realtime_people_counting_crosswalk

  mobilenet_ssd 모델 + 객체 트래킹을 활용한 인구 카운팅 코드를 통한 횡단보도에서의 유동인구 카운트

  ## 목차
   
   1. 개요
   2. 프로젝트 팀 구성 및 역할
   3. 프로젝트 절차 및 방법
   4. 구현 결과
   5. 결론

## 1. 개요

* 문제 발생: 집 앞 사거리 신호체계가 바뀐 뒤, 신호가 꼬여서 오히려 교통체증 발생  
* 문제 확인: 도시 계획에 있어 횡단보도 시간을 유동인구 수에 따라 할당  
* 문제 해결 : 수업에서 학습한 내용을 바탕으로 횡단보도의 유동인구를 파악하는 프로젝트 진행
  
    
## 2. 프로젝트 팀 구성 및 역할

<img src = "https://github.com/subin111/Realtime_people_counting_crosswalk/assets/143717650/b45ddc38-fc2d-4c89-bf66-7101d22a4af8" width = "650" height = "350"/>



  
## 3. 프로젝트 절차 및 방법

* 개발 세부 계획
  
<img src = "https://github.com/subin111/Realtime_people_counting_crosswalk/assets/143717650/c3a296b2-ed57-4c7d-8083-c3868b8f956e" width = "650" height = "350"/>


* 작성 일지
  
  <img src = "https://github.com/subin111/Realtime_people_counting_crosswalk/assets/143717650/681ac8a0-ce68-4c43-96b0-f1f9639f1985" width = "650" height = "400"/>



## 4. 구현 결과

* 시연 영상
  




  
## 5. 결론

   * 결론
     - opencv 활용
     - MMdetection의 기본 Architecture 이해
     - Faster-RCNN Model을 활용한 Object detection 수행
     - Tracking  Centeroid Algorithm을 통합한 유동인구 카운트 Algorithm 최종 구현
        
   * 한계점
     - 많은 사람들이 지나가면서 겹치게 되는 경우 다시 ID가 새로 배정되어 총 유동인구 수가 부정확해지거나 ID가 서로 바뀌는 ID switch현상 발생
     - 많은 사람들이 한 번에 겹쳐있는 경우 개별적으로 객체 인식이 어려움

   * 해결 방법
     - 객체가 서로 겹칠 때 객체의 이동 방향을 판단하는 코드를 이용
     - 여러 사람들이 겹쳐있는 이미지를 추가적으로 모델에 학습

     
