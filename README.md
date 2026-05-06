# Chameleon
TeamODD GameJam Team Project

📌 Overview
- Chameleon은 색의 적응하여 장애물들을 헤쳐나가는 플랫포머 기반 게임입니다.

📌 My Role
- 플레이어 동작 구현(wasd 점프 등)
- AudioManager 작업. 객체지향프로그래밍 첫 도입
- 메인 카메라 움직임 작업
- onTrigger2D를 통해 콜라이더의 접근 유무에 따른 게임 오버 시스템 제작
- 다른 신입 프로그래머 코드 수정 및 멘토

📌 Tech Stack
- AudioSource
- Mathf.Clamp()
- Collider2D
- LayerMask

📌 Key Implementation
- PlayerInputManager 작성
- 리지디바디의 중력 구현 -> rb.gravityScale = -Physics2D.gravity.y;
- Bounds를 통해 플레이어의 발위치를 측정하여 플랫포머 특유의 더블 점프와 발판 버그를 대응 <br />
Bounds bounds = capsuleCollider2D.bounds; <br />
footPosition = new Vector2(bounds.center.x, bounds.min.y); <br />
_isOnGround = Physics2D.OverlapCircle(footPosition, 0.1f, collisionLayer); <br />
  
📌 Trouble Shooting
- 객체지향 프로그래밍 구현 문제
  -> 관련 자료들을 직접 찾아보면서 구현
  -> 멘토의 조언

📌 What I Learned
- 짧은 시간 내에 과제를 완수해야 한다는 점. 때문에 여유를 부릴 수 없다.
- 객체지향프로그래밍에 대해서 그 감을 알아갔다.
- 



Assets에서 HTY를 들어가시면 주요 작업을 확인하실 수 있습니다.
<img width="297" height="127" alt="image" src="https://github.com/user-attachments/assets/ee60bbf3-77c8-4b0e-aef9-f5af6238699e" />
