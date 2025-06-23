# 🚀 KoCo GitOps Deployment Repository

이 레포는 [ArgoCD](https://argo-cd.readthedocs.io/)를 통해 Kubernetes 클러스터에 배포되는 모든 애플리케이션 및 인프라 구성 요소를 **GitOps 방식**으로 관리합니다.

## 📂 레포 구조

```bash
21-iceT-GitOps/
├── alb/
│   ├── argocd-ingress.yaml
│   ├── spring-ingress.yaml
│   └── fastapi-ingress.yaml
├── argocd/
│   └── deployment.yaml
├── spring/
│   └── deployment.yaml
├── apps/
│   └── app-alb.yaml

