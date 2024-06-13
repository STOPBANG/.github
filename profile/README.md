## STOPBANG 멈춰방

✨ 나에게 꼭 맞는 공인중개사, 멈춰방에서 찾을 수 있습니다!

💁‍♀️ 멈춰방은 부동산 거래를 하는 입주예정자, 공인중개사가 이용하는 서비스입니다.

💁‍♀️ 식당을 가기 전에 후기를 찾아보고 가듯, 중요한 선택 중 하나인 부동산 거래를 하기 전에 멈춰방에서 거래 후기와 별점을 확인할 수 있습니다.

<br>

### 💻 실행 매뉴얼
---

1️⃣ Git Clone하기

```bash
git clone https://github.com/STOPBANG/stop_bang_msa.git
```


2️⃣ stop_bang_msa 폴더로 이동하기

```bash
cd stop_bang_msa/
```


3️⃣ 쿠버네티스 환경 구축 및 클러스터 연결


적정 노드 스펙: 노드 3개, 메모리 3GB, 부팅디스크 30

```bash
gcloud container clusters get-credentials {클러스터이름} --zone {리전} --project {프로젝트ID}
```


4️⃣ 현재 사용하는 프로젝트로 환경 변경

```bash
gcloud config set project {프로젝트ID}
```


5️⃣ Service(LoadBalancer) IP 고정

```bash
gcloud compute addresses create {IP이름} --region asia-northeast3 
gcloud compute addresses describe {IP이름} --region asia-northeast3
```


6️⃣ 카카오 API에 IP 주소를 등록하기 위해 팀장/팀원에게 연락하기

전시현 (20201009@sungshin.ac.kr), 황지수 (20201019@sungshin.ac.kr)


7️⃣ 클러스터에 오브젝트 생성하는 파일에 실행권한 주기 (필요 시)

```bash
chmod 0744 k8s-script.sh
```


8️⃣ 클러스터에 오브젝트 생성하는 파일 실행하기

```bash
./k8s-script.sh
```


9️⃣ kubectl get svc에서 LoadBalancer type으로 생성한 service의 외부 IP:3000으로 접근


[💻 실행 매뉴얼 보러가기](https://www.canva.com/design/DAGHU2_ZUCI/W4dQDDwqfeQCjq-vMbtLEQ/view?utm_content=DAGHU2_ZUCI&utm_campaign=designshare&utm_medium=link&utm_source=editor)



### 📖 최종 발표자료
---
[발표자료 보러가기](https://www.miricanvas.com/v/13bar62)

### 🎞 데모영상
---
[데모영상 보러가기](https://www.youtube.com/watch?v=tZHxczvC-NY)
