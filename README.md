# 🚀 KoCo GitOps Deployment Repository

이 레포는 [ArgoCD](https://argo-cd.readthedocs.io/)를 통해 Kubernetes 클러스터에 배포되는 모든 애플리케이션 및 인프라 구성 요소를 **GitOps 방식**으로 관리합니다.

## 📂 레포 구조

```bash
21-iceT-GitOps/
├── spring/                      # Spring 서비스 배포 정의
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
├── fastapi/                     # FastAPI 서비스 배포 정의
│   └── helm-values.yaml
├── argocd/                      # ArgoCD 자체 배포 관련 리소스
│   └── argocd-ingress.yaml
└── base/    

