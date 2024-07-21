# 개요
api 서버는 불과 일주일 전에 만들었던 스프링부트 게시판 CRUD 서버를 활용하기로 한다.  
가장 기본적인 수준으로 구현되었기에 한편으로 지나치지 않다.  
목표를 인프라 구성으로 두었기 때문에 깊게 들어가지 않도록 한다.  
기본적인 구현 내용은 다음 참고  
https://zerotay-blog.vercel.app/2.project/AWS%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/%EB%B0%B1%EC%97%94%EB%93%9C%20-%20%EA%B2%8C%EC%8B%9C%ED%8C%90%20CRUD/
# 환경 변수 설정
해당 내용에서 추가적으로 세팅이 필요한 요소는 [[쿠버네티스]]에서 제어 가능한 설정 파일을 두는 것이다.
![Pasted image 20240720142414](https://github.com/user-attachments/assets/afb050e0-855f-48fc-a2ba-af21311be28f)  
application.yml 파일에서 로컬 환경 변수를 활용하도록 했다.
이것은 나중에 [[ConfigMap]]으로 값이 들어가도록 할 것이다.

# 참고
- 파드에서 사용하기 위한 외부 환경 변수 주입 방법
	- https://youngseo-computerblog.tistory.com/80
