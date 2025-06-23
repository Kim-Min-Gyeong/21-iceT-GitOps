# 🚀 KoCo GitOps Deployment Repository

이 레포는 [ArgoCD](https://argo-cd.readthedocs.io/)를 통해 Kubernetes 클러스터에 배포되는 모든 애플리케이션 및 인프라 구성 요소를 **GitOps 방식**으로 관리합니다.

## 📂 레포 구조

```bash
21-iceT-GitOps/
├── apps/                        # ArgoCD Application CR들 (app-of-apps 방식이면 여기에 한꺼번에 정의)
│   ├── app-spring.yaml
│   ├── app-fastapi.yaml
│   └── app-argocd.yaml
├── spring/                      # Spring 서비스 배포 정의
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
├── fastapi/                     # FastAPI 서비스 배포 정의
│   └── helm-values.yaml
├── argocd/                      # ArgoCD 자체 배포 관련 리소스 (Ingress 등)
│   ├── alb-ingress.yaml
│   └── server-patch.yaml
└── base/                        # 공통 리소스 (ConfigMap, Secret 등)
