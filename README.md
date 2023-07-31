# 동방 과제록-이세카이로부터 탈출
종스크롤 탄막 게임

## 🖥️ 프로젝트 소개
- 튕겨내기 공격(패링)을 추가한 동방프로젝트와 같은 종스크롤 탄막 게임
- 기존 탄막게임처럼 일반공격이 있지만 마나를 소모
- 패링으로 적의 공격을 튕겨내서 반사가능, 성공하면 마나회복
- 패링으로 반사한 공격을 다시 패링할 경우 반사공격의 공격력과 속도가 상승

## 🕰️ 제작기간
- 23.5.2~23.5.28 (약 1개월)

## 🧑‍🤝‍🧑 멤버구성
- 팀장 : 구본관 - 전반적인 기능, 직업 / 보스전 구현
- 팀원 : 강윤원 - 디자인
- 팀원 : 오상훈 - 점수 시스템, 난이도 구현
- 팀원 : 정재민 - 스토리 , 대화문 구현

## ⚙️ 개발엔진
- JAVASCRIPT, HTML

## 📌 주요 기능
### 메인 화면
- 게임시작 / 게임방법 / 게임종료
  
### 플레이어
- 이동 / 기본공격 / 패링

### 난이도 선택
해당 난이도를 클리어하면 다음 난이도로 이어서 진행, 하드모드 클리어 시 엔딩 진행
- EASY : 모든 적 체력 표시, 웨이브마다 체력 회복, 적과 보스 패턴 약화
- NOMAL : 모든 적의 탄막 속도 증가, 일반공격 시 마나 소모량 증가
- HARD : 모든 적의 탄막 속도 증가, 일반공격 시 마나 소모량 증가, 적과 보스 패턴 강화, 보스 발악패턴 추가
  
### 직업 선택
- 전사(요우무) : 기본 체력 증가, 이동속도 증가
- 마법사(마리사) : 패링 범위, 패링 공격력 증가
- 궁수(에이린) : 일반공격력 증가, 마나 소모량 감소, 마나 회복량 증가

### 웨이브 구성
웨이브는 3개로 구성
- 몬스터1(레이무) : 플레이어를 향해서 반사가능 탄막과 반사불가 탄막 번갈아가며 발사
- 몬스터2(레이센) : 랜덤각도와 랜덤속도로 조금의 반사가능 탄막과 다량의 반사불가 탄막 발사
- 벽돌 : 일반공격으로는 파괴불가능하고 패링공격으로만 파괴가능, 체력에 따라서 빨강 / 파랑 / 초록 벽돌로 구분

### 보스(유카리)
웨이브 클리어 시 대화문과 함께 등장
- 쉴드 : 패링공격으로만 파괴 가능한 쉴드로 방어, 파괴 시 일정시간 후 재생
- 기본패턴 : 15도씩 360도로 반사가능 탄막과 반사불가 탄막 번갈아가며 발사
- 유도공격 : 거대한 탄막불가 탄막 플레이어에게 일정각도로 흩뿌려서 발사

### 보스 발악패턴
하드 난이도에서만 사용
- 보스를 공격할 수 없지만 보스의 체력은 지속적으로 감소(타임어택)
- 화면 밖에서 가운데로 탄막 발사
- 화면 가운데(보스)에서 나선형으로 거대한 탄막 발사


### 엔딩
보스의 발악패턴에서 생존유무에 따라서 엔딩 결정
- 생존 엔딩 : 해피엔딩
- 사망 엔딩 : 배드엔딩
