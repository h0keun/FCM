```💡 FastCampus 강의 수강 및 정리```

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
  
💡 Notification Channel 생성하기  
💡 RemoteViews - Custom Notification  
💡 FLAG(작업 및 백스텍)  
💡 PandingIntent : intent의 권한을 부여한다? 이런느낌? 여기선 노티피케이션이 인텐트권한을 갖게됨  
💡 본 프로젝트에서는 [이곳에서]( https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages/send?apix_params=%7B%22parent%22%3A%22projects%2Fdofcm-6b3db%22%2C%22resource%22%3A%7B%22message%22%3A%7B%22token%22%3A%22cpA0utRXQdCWUS2GPJBhSb%3AAPA91bEg_CDdozxwvvF95yobkhLCvklF4qOK1zDgnKZTR1q1KQUVrvPDYIzJLXuG3Qf3hq0XbiXkV_L1i4C7ytB6TQKfetFSGVjCL5_uOFegJ-te2n9s9p5K8NjL_Ol6oZ8qd1HYGKAf%22%2C%22data%22%3A%7B%22type%22%3A%22CUSTOM%22%2C%22title%22%3A%22Test%20title%22%2C%22message%22%3A%22Test%20message%22%7D%7D%7D%7D)
제공하는 API를 통해 FCM을 보냈다.  

#### 작성한 정보  
+ Request Parameters : ```projects/dofcm-6b3db```  
+ Request Body :  
  ```
  {
    "message": {
      "token": "토큰값",
      "data": {
       "type": "CUSTOM",
       "title": "Test title",
       "message": "Test message"
      }
    }
  }
  ```
  
<img src="https://user-images.githubusercontent.com/63087903/119834149-a8723f00-bf3a-11eb-8f4b-1733c8c8a0a1.jpg" width="200" height="430">
