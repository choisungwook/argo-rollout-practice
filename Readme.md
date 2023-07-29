# 개요
* argo rollout 연습

# 쿠버네티스 설치
* kind cluster 사용
* [kind cluster 설치 문서](./kind-cluster/)

# argo rollout 설치
## rollout controller 설치
* argo rollout에서 공식으로 제공하는 quick start 설치
* 참고자료: https://argoproj.github.io/argo-rollouts/#why-argo-rollouts

```bash
kubectl create namespace argo-rollouts
kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/install.yaml
```

## argo CLI 플러그인 설치
* argo CLI는 kubectl argo 플러그인
* 설치방법은 [공식 문서](https://argoproj.github.io/argo-rollouts/installation/#manual) 참고

## 대시보드 설치
* github release에서 dashboard-install.yaml을 다운로드하고 kubectl apply
* 실습을 편하기 위해 nodeport설정함
```bash
curl -LO https://github.com/argoproj/argo-rollouts/releases/download/v1.5.1/dashboard-install.yaml
kubectl apply -n argo-rollouts -f dashboard-install.yaml
```
