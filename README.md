# LVMS (Leave Management System)

연차 관리 시스템 - 직원들의 연차를 효율적으로 관리하기 위한 웹 애플리케이션

## 🚀 주요 기능

- 연차 신청 및 승인 프로세스
- 잔여 연차 현황 관리
- 부서별 연차 사용 현황 대시보드
- 연차 사용 내역 레포트 생성
- 사용자 권한 관리 (관리자, 부서장, 일반 직원)

## 🛠 기술 스택

### Backend
- Spring Boot 3.2.0
- JPA & MyBatis
- Spring Security
- PostgreSQL

### Frontend
- Thymeleaf
- Bootstrap 5
- jQuery

## 📋 시스템 요구사항

- JDK 17 이상
- PostgreSQL 15 이상
- Gradle 8.x

## 🔧 개발환경 설정

1. JDK 설치
```bash
# JDK 버전 확인
java -version
```

2. PostgreSQL 데이터베이스 생성
```sql
CREATE DATABASE lvms;
```

3. 프로젝트 클론
```bash
git clone https://github.com/[your-username]/lvms.git
cd lvms
```

4. 애플리케이션 설정
- `src/main/resources/application.yml` 파일 생성
```yaml
spring:
  datasource:
    url: jdbc:postgresql://localhost:5432/lvms
    username: your_username
    password: your_password
```

5. 애플리케이션 실행
```bash
./gradlew bootRun
```

## 📦 프로젝트 구조

```
lvms/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/lvms/
│   │   │       ├── config/     # 설정 파일
│   │   │       ├── controller/ # 컨트롤러
│   │   │       ├── domain/     # 엔티티
│   │   │       ├── dto/        # DTO
│   │   │       ├── repository/ # JPA 리포지토리
│   │   │       ├── mapper/     # MyBatis 매퍼
│   │   │       └── service/    # 서비스
│   │   └── resources/
│   │       ├── mapper/         # MyBatis XML
│   │       ├── static/         # 정적 파일
│   │       └── templates/      # Thymeleaf 템플릿
│   └── test/                   # 테스트 코드
```

## 🔨 빌드 및 테스트

```bash
# 테스트 실행
./gradlew test

# 빌드
./gradlew build

# jar 파일 생성
./gradlew bootJar
```

## 📝 API 문서

- Swagger UI: `http://localhost:8080/swagger-ui.html`

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 라이센스

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## 👥 연락처

프로젝트 관리자 - [@hichang4u](https://github.com/hichang4u)

프로젝트 링크: [https://github.com/hichang4u/lvms](https://github.com/hichang4u/lvms)
