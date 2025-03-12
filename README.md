# 참조 사이트

https://adjh54.tistory.com/577

- 어드민 추가 ???
- 로그인 하고 타임아웃 설정하여 로그아웃 처리
- 테마 아이콘 제거

brew install redis
redis-cli --version

# foreground 상태에서 redis 실행

$ redis-server

# background 상태에서 redis를 실행합니다.

$ brew services start redis

# background 상태에서 실행되는

$ brew services info redis

# homebrew background에서 실행중인 서비스 조회

$ brew services list

redis-cli 실행 후 확인
LRANGE tokenBlackList 0 -1

# 확인 사항

- 스프링 테스트 로직 확인 ...
- token 타임 아웃 확인
- radis 디스크 저장 장소 및 지우는 시간 확인
- access token 타임아웃 시 refress 토컨 가지고 로그인 시 재 할당 확인

# 로그인 token 테스트

- acc 받고 타임아웃 후 --> ref 채크 (성공 시 : acc, ref 생성, 실패 시 : 재로그인 요청 )
- acc 받고 또 로그인 후 acc 받음 : 앞 acc 는 유효 ???

- radis 삭제 ( 로그아웃 안하는 경우가 거이다임 ㅎㅎㅎ)
  : 그러나 삭제 루틴은 확인
