```π‘ FastCampus κ°μ μκ° λ° μ λ¦¬```

### Firebase Cloud Messaging
μμΈν μ€λͺμ κ³΅μλ¬Έμλ₯Ό μ°Έμ‘°νμ [π](https://firebase.google.com/docs/cloud-messaging)

+ μν€νμ² κ°μ
  1. Message building and targeting
  2. FCM backend
  3. Platform-level message transport
  4. SDK on device
 
+ μ ν
  1. μλ¦Ό λ©μμ§ : FCM SDKμμ μλμΌλ‘ μ²λ¦¬['BE BETTER' μ±μμ ν΄λ΄]  
  (κ΅¬νμ μ½μ§λ§, μ¬λ¬κ°μ§ μΌμ΄μ€μμ λμνκΈ° μ΄λ ΅λ€, forgroundμμ λμνμ§ μλλ€λκ° νλ..)  
  2. λ°μ΄ν° λ©μμ§ : ν΄λΌμ΄μΈνΈ μ±μμ μ²λ¦¬  
  (κ΅¬νμ κΉλ€λ‘­μ§λ§, μ¬λ¬κ°μ§ μΌμ΄μ€μμ λμνκΈ° μ½λ€)
  
π‘ Notification Channel μμ±νκΈ°  
π‘ RemoteViews - Custom Notification  
π‘ FLAG(μμ λ° λ°±μ€ν)  
π‘ PandingIntent : intentμ κΆνμ λΆμ¬νλ€? μ΄λ°λλ? μ¬κΈ°μ  λΈν°νΌμΌμ΄μμ΄ μΈννΈκΆνμ κ°κ²λ¨  
π‘ λ³Έ νλ‘μ νΈμμλ [μ΄κ³³μμ]( https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages/send?apix_params=%7B%22parent%22%3A%22projects%2Fdofcm-6b3db%22%2C%22resource%22%3A%7B%22message%22%3A%7B%22token%22%3A%22cpA0utRXQdCWUS2GPJBhSb%3AAPA91bEg_CDdozxwvvF95yobkhLCvklF4qOK1zDgnKZTR1q1KQUVrvPDYIzJLXuG3Qf3hq0XbiXkV_L1i4C7ytB6TQKfetFSGVjCL5_uOFegJ-te2n9s9p5K8NjL_Ol6oZ8qd1HYGKAf%22%2C%22data%22%3A%7B%22type%22%3A%22CUSTOM%22%2C%22title%22%3A%22Test%20title%22%2C%22message%22%3A%22Test%20message%22%7D%7D%7D%7D)
μ κ³΅νλ APIλ₯Ό ν΅ν΄ FCMμ λ³΄λλ€.  

#### μμ±ν μ λ³΄  
+ Request Parameters : ```projects/dofcm-?????```  
+ Request Body :  
  ```
  {
    "message": {
      "token": "ν ν°κ°",
      "data": {
       "type": "CUSTOM",
       "title": "Test title",
       "message": "Test message"
      }
    }
  }
  ```
  
<img src="https://user-images.githubusercontent.com/63087903/119834149-a8723f00-bf3a-11eb-8f4b-1733c8c8a0a1.jpg" width="200" height="430">
