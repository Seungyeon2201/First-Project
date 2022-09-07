# 개인  프로젝트  Idea Note

작성자 | 장르 
---|---
김승연| TPS |
---------
* 스토리
#### [스토리 참고](https://gall.dcinside.com/board/view/?id=hit&no=14141)
#####  로봇이 살고 있는 행성에 유기체가 쳐들어와 멸망하기 직전까지 가게 된다. 이길 가능성이 없어보였던 로봇들은 각자의 정보들을
##### 하나의 로봇(주인공)에게 전달하고 그 로봇을 어린 유기체에 몰래 심어 놓기 위한 계획을 세우게 된다.
--------
* 개발 계획
  * Player
    * Player 움직임 제어
      
      { Idle, Move, Run, RangedAttack, MeleeAttack, Jump, Hit, Sit, Aiming  }
    * List를 이용한 Inventory 구현
    * Aiming시 1인칭 시점으로 변환하여 정밀 조준이 가능하게 구현
    * 카메라 구현은 숄더뷰로 하고 Free Look Camera의 Collider를 구현하여 캐릭터가 가려지는 현상을 방지
  * NPC 
  
    - 구간별로 NPC를 배치해 각 NPC마다 기록 조각 획득
    - Scriptable Object를 이용하여 NPC에게 퀘스트를 받고 연구실에 잠입하고 유기체에 잠입
    - NPC 위치 별로 Scriptable Object를 이용한 Spawn 지역 저장 
  
  * Enemy(FSM을 이용해서 구현)
    - 원거리 공격 : 맞았을 때나 주변에 소리가 범위 내에 인식되면 소리나는 쪽으로 방향 전환하고 Player 탐지시 Player 좌표를 중심으로 특정 범위에 공격
    - 근거리 공격 : 
  * Item
  
     - NPC 기록(NPC의 숫자만큼 모두 모아야 최종 컨텐츠 진입가능)
     
  
    

