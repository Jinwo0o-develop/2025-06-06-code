# 2025-06-06-code
class User:

    def __init__(self, name, email, password):
        self.name = name
        self.email = email
        self.password = password
        
    def say_hello(self):
        print(f"안녕하세요! 저는 {self.name}입니다!")
    
    def login(self, email, password):
        if self.email == email and self.password == password:
            print("로그인 성공, 환영합니다")
            self.say_hello()
        else:
            print("로그인 실패, 없는 아이디이거나 잘못된 비밀번호입니다.")

    def __str__(self):
        return f"사용자: {self.name}, 이메일: {self.email}"

#인스턴스 생성
user1 = User("강영훈","younghoon@codeit.xyz","12345")
user2 = User("이윤수","yoonsoo@codeit.xyz","abcde")

#로그인 시도
user1.login("younghoon@codeit.xyz","12345")

#로그인 시도 실패
user2.login("23","23")

print(str(user1))

# 설명
코드잇에서 클래스와 인스턴스를 설명해주었고, 아직은 따라하기밖에 못했다.
함수를 통한 일반화와 매직메소드(스폐셜메소드)라는걸 배웠고, 덕분에 인스턴스를 좀 이해했다.
프로그래머들이 코드를 줄이기 위해 일반화를 잘 해야한다는 것과 코드스타일이 얼마나 중요한지 많이 느낀 하루였다.
