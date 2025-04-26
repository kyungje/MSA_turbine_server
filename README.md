# MSA_turbine_server

**MSA_turbine_server**는 마이크로서비스 아키텍처(Microservices Architecture)에서 Hystrix 스트림 데이터를 집계하기 위한 Turbine 서버입니다. 이 프로젝트는 마이크로서비스 환경에서 대시보드 모니터링을 지원하기 위해 설계되었습니다.

## 주요 기능

- Hystrix 스트림 데이터의 집계
- 마이크로서비스 상태 모니터링
- Spring Cloud Netflix Turbine 기반 구현

## 기술 스택

- **언어**: Java
- **프레임워크**: Spring Boot, Spring Cloud Netflix Turbine
- **빌드 도구**: Maven

## 설치 및 실행

1. 저장소를 클론합니다:
   ```bash
   git clone https://github.com/kyungje/MSA_turbine_server.git
   ```
2. 프로젝트 디렉토리로 이동합니다:
   ```bash
   cd MSA_turbine_server
   ```
3. 필요한 의존성을 설치하고 애플리케이션을 실행합니다:
   ```bash
   ./mvnw spring-boot:run
   ```

## 사용 방법

1. 애플리케이션이 실행되면 기본적으로 [http://localhost:8989](http://localhost:8989)에서 Turbine 서버가 실행됩니다.
2. Hystrix 대시보드에서 Turbine 서버의 스트림 데이터를 사용하려면 다음 URL을 입력합니다:
   ```
   http://localhost:8989/turbine.stream
   ```
3. `application.yml` 또는 `bootstrap.yml` 파일에서 Turbine의 클러스터 설정을 수정하여 환경에 맞는 구성을 설정할 수 있습니다.

## 기여

기여를 환영합니다! 이 프로젝트에 기여하려면 다음 단계를 따라주세요:

1. 이 저장소를 포크합니다.
2. 새로운 브랜치를 생성합니다:
   ```bash
   git checkout -b feature/새로운기능
   ```
3. 변경사항을 커밋합니다:
   ```bash
   git commit -m "추가: 새로운 기능 설명"
   ```
4. 브랜치를 푸시합니다:
   ```bash
   git push origin feature/새로운기능
   ```
5. Pull Request를 생성합니다.

## 라이센스

이 프로젝트는 MIT 라이센스를 따릅니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

## 참고 자료

- [Spring Cloud Netflix Turbine 공식 문서](https://cloud.spring.io/spring-cloud-netflix/)
- [Hystrix 대시보드 사용법](https://github.com/Netflix/Hystrix/wiki/Dashboard)
- [마이크로서비스 아키텍처 개요](https://martinfowler.com/articles/microservices.html)
```
