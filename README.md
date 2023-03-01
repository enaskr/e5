# 새 버전이 개발 중입니다 ...... 완료되면 이 리포지토리는 더 이상 유지 관리되지 않습니다.
# E5 구독 자동 갱신 절차
이 항목은 이 사이트의 소스 코드(백엔드)입니다. https://e5.qyi.io/
(FrontEnd) https://github.com/luoye663/e5-html
#### 튜토리얼
https://qyi.io/archives/687.html

#### 프로그램램:
- [ ] 기본 데이터를 위한 경량 h2 스토리지
- [x] 로그는 TDengine/influxdb를 사용하여 저장됩니다.
- [ ] MySQL 종속성 제거
- 
### 2021-08-19
1、시작 취소 redis 지우기  
2、통화 로그를 인풋에 넣어 MySQL 압력 줄이기
### 2021-07-28
rabbitMQ 종속성 제거, 스레드 풀을 사용하여 구현 간소화(실행 시간 세분화 감소)

### 2020-12-20
프런트엔드 프레임워크가 여러 애플리케이션과 계정당 최대 5개의 애플리케이션을 지원하는 Angular로 변경되었습니다.
## 설명
이 프로젝트는 저의 초보자 연습용 작업으로, 코드가 매우 복잡하며 2020년 3월부터 지금까지 진행 중입니다.  
직접 구축하려면 직접 조사해야 하고 기술 지원이 제공되지 않으며 (게으른) 구성 파일을 수정하는 것을 잊지 마십시오. 
src/main/resources/application-online.properties 
```
user.admin.githubId  - 본인의 github id  
데이터베이스 구성  
redis구성  
Rabbit구성  
github.client_id  
github.client_secret  
(이 2가지 모두 https://github.com/settings/developers 앱을 요청하기만 하면 됩니다.)
```
## 주의사항


## 사용된 기술 프레임워크
### spring boot  

### Redis
라이브러리 1개가 기본값이며, 구성 파일 자체에서 변경할 수 있습니다. 

### Mysql
자체 가져오기 sql  
명확한 로그 기능이 작성되지 않았으며 나중에 추가되었습니다.  
로그가 몽고DB에 저장되어야 하는 것이 당연한 것 아닌가요?
### Mybatis Plus

### Spring Security
사용 권한은 몇 가지에 불과하므로 mysql에 기록되지 않습니다.
### log4j2
로깅 프레임워크

## Thanks

> [IntelliJ IDEA](https://www.jetbrains.com/zh-cn/idea/buy/#personal?billing=yearly) 는 모든 면에서 개발자의 생산성을 극대화하는 JVM 플랫폼 언어용 IDE입니다.

Special Thanks [JetBrains](https://www.jetbrains.com/?from=) 오픈 소스 프로젝트는 무료 [IntelliJ IDEA](https://www.jetbrains.com/idea/?from=) 다음과 같은 IDE의 라이선스  
[<img src=".github/jetbrains-variant-3.png" width="200"/>](https://www.jetbrains.com/)
