# 소득구간별 출산율 분석
<br>

## 🗓️기간
2024.10.28 ~ 2024.11.23
<br>

## 데이터 수집
Kosis.kr 사이트에서 소득구간별 출산자녀 현황 csv 다운로드

## 데이터 전처리
![데이터전처리1](https://github.com/user-attachments/assets/cede4d6d-f3c9-4348-be1e-3da75d261947)<br>  
![데이터전처리2](https://github.com/user-attachments/assets/2c97bf6e-2bac-4ce2-921a-c30b4929f23e)<br>
- 0, 1번째 행 삭제 후 기존에 남아있는 2번째 행 열 이름 재설정<br>
- 소득구간 만원 단위 제거, 데이터 타입 확인 후 숫자형 데이터로 변환<br>

## 데이터 변환
![데이터변환](https://github.com/user-attachments/assets/d031f2ed-440f-48bd-99ac-23d53146451c)<br>
- 소득 구간, 자녀 수, 평균 출생아 수 등의 데이터를 to_numpy()를 이용해 NumPy 배열로 전환

## 시각화
1. 막대 그래프 <br>
![막대 그래프](https://github.com/user-attachments/assets/851f2d9a-18f7-409b-9390-9494fc41981e)<br>
2. 누적 막대 그래프 <br>
![누적막대그래프](https://github.com/user-attachments/assets/c7ea5c9a-b2bb-4a66-93fb-9dfaba8d3287)<br>
3. 선 그래프 <br>
![선 그래프](https://github.com/user-attachments/assets/986d7499-34d6-47c3-bf46-9f949501e29d)<br>
4. 산점도 <br>
![산점도](https://github.com/user-attachments/assets/bc60033f-b325-4c0d-a7a6-8789a52db66f)

## 결론
소득 구간이 낮은 가정일수록 출산율이 높을 것이라는 가설을 세웠습니다. 공영 방송에서 소개된 가정들을 살펴보면 소득이 낮은 가정일수록 자녀 수가 많고, 반대로 소득이 높은 가정일수록 자녀 수가 적다는 경향이 보였습니다. 데이터 분석 결과 소득구간이 1,000만원 미만인 가정의 경우 평균 출생아수는 1.08로 가장 높았고 소득구간이 1,000만원 이상인 가정의 경우 평균 출생아수는 0.64로 2번 째로 낮게 나왔습니다. 이로써 소득구간이 낮은 가정일수록 평균 출생아수는 높은 것으로 결론이 났습니다.


