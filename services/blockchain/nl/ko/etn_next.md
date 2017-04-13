---

copyright:
  years: 2016, 2017
lastupdated: "2016-10-07"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}


# 추가 테스트
{: #etn_next}


체인코드 함수, 원장, 장기 실행, 동시성 및 복합 트랜잭션을 테스트하기 위해 (별도로 기술하지 않는 한) 고급 보안 비즈니스 네트워크 환경에서 다음 테스트가 실행되었습니다. 유효성 검증기 및 멤버십 서비스 노드가 LinuxONE OS의 보안 서비스 컨테이너 내에서 VM 게스트로서 실행되었습니다. 아래에서 사용된 값은 고객 입력을 기반으로 선택되었으며, 이를 최대값으로 생각해서는 안 됩니다. (참고: 이러한 테스트 중 일부는 [Node.js SDK](etn_txn.html) 및 [합의 및 가용성 테스트](etn_pbft.html) 섹션에서 반복됩니다.) 

{:shortdesc}

1. 체인코드 함수 - 체인코드 인터페이스는 REST API 및 CLI를 사용하여 `Deploy`, `Invoke` 및  `Query` 트랜잭션이 제대로 작동함을 보증하도록 실행되었습니다. Hyperledger 프로토콜 스펙에서 설명한 대로, REST API 및 CLI는 둘 다 블록, 블록체인, 체인코드, 네트워크, 등록자 및 트랜잭션을 포함하여 모든 엔드포인트 기능을 테스트하기 위해 활용되었습니다. 
2. 원장 - 서로 다른 드라이브 환경을 기반으로, 원장에서 1K 페이로드의 20,000개 레코드 작성. 테스트에는 직렬화된 방식으로 20,000개의 레코드를 작성하는 하나의 클라이언트가 포함되어 있습니다.
3. 장기 실행 - 이 테스트는 example02 데모 체인코드를 사용하여 72시간 동안 다중 노드 간에 호출, 체인 높이 및 조회를 전송하여 수행되었습니다. 
4. Node.js SDK - 개선된 Node.js SDK는 사용자를 등록 및 등록접수하고 개발 모드의 피어(피어 시작: `peer node start –peer -chaincodedev`) 및 네트워크 모드(피어 시작: `peer node start`) 모두에서 배치, 호출 및 조회를 수행하는 데 사용되었습니다.
5. 기본 동시성 - 이 테스트는 1KB 페이로드로 10분 동안 4개 피어 각각에 동시 호출을 전송하고 체인 높이를 측정하며 원장 상태를 조회하여 수행되었습니다. 
6. 복합 트랜잭션 - 이 테스트는 10분 동안 10k - 500K 범위의 다양한 페이로드 크기의 조회 및 호출을 혼합하여 피어에 무작위로 제출하여 수행되었습니다. 네트워크 피어 전체에서 공유 원장이 동기화되도록 전체 상태의 조회 및 체인 높이가 측정되었습니다.