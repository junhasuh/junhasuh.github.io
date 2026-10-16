# 서준하 · IT인프라(DevOps) 신입 포트폴리오

https://junhasuh.github.io/

배포가 실패할 때 어디까지 되돌릴지 먼저 정하고, 일부러 실패시켜 확인한 기록입니다.

- **P1** 소개와 대표 근거 3개, 기술, 자격·학력·병역
- **P2~P4 Hibiscus**: 온프레미스·Cloud Run 배포 단계의 순차 전환, 온프레미스 전환 실패 시험, GCP 실행 환경의 접근 경로와 권한 ([저장소](https://github.com/SoftBank-Hackathon-Hibiscus/hibiscus))
- **P5~P6 영주로그 CI/CD**: Jenkins·Ansible·Kubernetes 파이프라인과 실패 시험 4건 ([저장소](https://github.com/junhasuh/yeongjuLog-BE))
- **P7 기반 역량**: Terraform 실습 저장소([aws-terraform-infra](https://github.com/junhasuh/aws-terraform-infra)), CKA 기출 풀이, 강의 실습

기술 블로그: https://policerjack.tistory.com/

## 구성

정적 HTML 한 장으로 된 GitHub Pages 사이트입니다. 빌드 단계는 없습니다.

```
index.html                              페이지 본문(P1~P7)
assets/og.png                           링크 미리보기 이미지
assets/jenkins-stages.png               영주로그 #23 단계 화면(Quality Gate 실패)
assets/yeongju-b3-stages.png            영주로그 #3 단계 화면(Test 실패 뒤 스킵)
assets/yeongju-b5-stages.png            영주로그 #5 단계 화면(Deploy 단계 없음)
assets/yeongju-b7-rollback-log.png      영주로그 #7 콘솔 로그(헬스체크 20번 실패, 롤백)
assets/yeongju-b15-log-1.png, -2.png    영주로그 #15 콘솔 로그 원본(rollout 시간 초과, undo, FAILURE)
assets/yeongju-b22-stages.png           영주로그 #22 단계 화면(Deploy까지 정상)
assets/yeongju-dockerps-cfe545d.png     영주로그 #5 수정 뒤 앱 서버 docker ps
favicon.svg
.nojekyll                               Jekyll 처리 생략
```

Hibiscus 화면(배포 결과, 장애 주입 시간축, 권한 설정)은 [구축 회고](https://policerjack.tistory.com/5)의 원본 그림으로 연결합니다.
