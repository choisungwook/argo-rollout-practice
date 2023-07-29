# 개요
* kind 쿠버네티스 클러스터 생성
* 쿠버네티스 버전 1.27

# 전제조건
docker 설치

# 생성 방법
```bash
kind create cluster --config cluster.yml
```

# 삭제 방법
```bash
kind delete cluster --name argo-practice
```
