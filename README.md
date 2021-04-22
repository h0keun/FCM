### Firebase Cloud Messaging
자세한 설명은 공식문서를 참조하자 [📌](https://firebase.google.com/docs/cloud-messaging)

+ 아키텍처 개요
  1. Message building and targeting
  2. FCM backend
  3. Platform-level message transport
  4. SDK on device
 
+ 유형
  1. 알림 메시지 : FCM SDK에서 자동으로 처리['BE BETTER' 앱에서 해봄]  
  (구현은 쉽지만, 여러가지 케이스에서 대응하기 어렵다, forground에서 동작하지 않는다던가 하는..)  
  2. 데이터 메시지 : 클라이언트 앱에서 처리  
  (구현은 까다롭지만, 여러가지 케이스에서 대응하기 쉽다)
  
### Firebase 프로젝트
