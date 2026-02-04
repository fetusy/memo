---
title: Notepad++ 해킹
date: 2026-02-03T10:30:00+09:00
draft: false
---
프로그램 내의 코드 오류로 인한 버그가 아닌, 업데이트 서버 자체가 해킹당해 가짜 업데이트를 유포한 공급망 공격(Supply Chain Attack) 입니다.

2026년 2월 2일, Notepad++ 개발자는 [공식 사이트](https://notepad-plus-plus.org/news/hijacked-incident-info-update/) 를 통해 2025년 6월부터 업데이트 배포 서버가 해커에게 장악되어 있었다고 밝혔습니다.

카스퍼키는 이번 공격에서 총 3가지의 서로 다른 감염 체인이 발견되었다고 발견했습니다.

**체인 #1 (2025년 7~8월):** 정상적인 Notepad++ 업데이트 프로세스(GUP.exe)를 이용해 악성 update.exe를 실행했습니다. 이 과정에서 2010년대 초반의 아주 오래된 소프트웨어 취약점을 악용해 보안 솔루션을 우회하는 치밀함을 보였습니다.

**체인 #2 (2025년 9월):** 시스템 정보를 수집하는 스크립트를 실행한 뒤, 'Cobalt Strike'라는 도구를 심어 PC를 원격 제어하려 했습니다.

**체인 #3 (2025년 10월):** 'Chrysalis'라는 백도어를 심는 방식으로, 주로 중국어권 해킹 그룹이 사용하는 수법과 유사한 패턴이 관찰되었습니다.


이번 공격은 무차별 공격이 아니라 특정 대상을 노린 것으로 보입니다. 카스퍼스키가 확인한 피해 사례는 다음과 같습니다.

- 필리핀 정부 기관 및 엘살바도르 금융 기관
- 베트남의 IT 서비스 제공업체
베트남, 엘살바도르, 호주 등의 개인 사용자들

 

참고문헌: 
[Kaspersky Securelist: The Notepad++ supply chain attack breakdown](https://securelist.com/notepad-supply-chain-attack/118708/)
