# Spring Boot 매니페스트

이 디렉토리에는 GHCR에서 가져온 Spring Boot 애플리케이션의 Kubernetes 매니페스트가 포함되어 있습니다.

## 📦 이미지 정보
- **이미지**: `ghcr.io/social-archive/springboot-developer:latest`
- **포트**: 8080 (컨테이너) → 8082 (NodePort 30082)
- **접근**: http://localhost:8082

## 📁 파일 구성
- `springboot-deployment.yaml`: Spring Boot 애플리케이션 배포 설정
- `springboot-service.yaml`: NodePort 서비스 설정 (포트 30082)

## 🚀 ArgoCD 배포
ArgoCD UI에서 새로운 Application을 생성할 때:
- **Repository**: https://github.com/social-archive/argo_test.git
- **Path**: `spring-manifests`
- **Namespace**: `springboot-app` (또는 원하는 네임스페이스)
