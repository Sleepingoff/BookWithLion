---
created: 2023-10-07T09:26
updated: 2023-10-07T18:27
---
# AI)DDoS 공격 대해서 설명해주세요.

황병헌

#트래픽 #보안 공격

## 답변 드리겠습니다!

<aside>
📌 DDoS(Distributed Denial of Service) 공격은 여러 컴퓨터가 동시에 한 서버나 네트워크에 대량의 트래픽을 보내서 그 서비스를 이용할 수 없게 만드는 공격 방법입니다. 이는 정상적인 사용자들이 해당 서비스를 이용하는 것을 방해하거나 불가능하게 만듭니다.

DDoS 공격은 다양한 형태로 발생할 수 있습니다:

Volume-based attacks: 가장 일반적인 DDoS 공격 형태로, 대량의 트래픽을 목표 시스템에 전송하여 네트워크 대역폭을 포화 상태로 만듭니다. UDP flood, ICMP flood 등이 여기에 속합니다.Protocol attacks: 목표 시스템의 자원(예: 연결 테이블)을 소진시켜 시스템 장애를 유발합니다. SYN flood, Ping of Death 등이 여기에 속합니다.Application layer attacks: HTTP GET/POST floods와 같은 애플리케이션 계층에서 작동하는 공격으로, 특정 웹 애플리케이션 자원을 타깃으로 합니다.

DDoS 공격은 보안 인증서를 갖춘 HTTPS 사이트에서도 발생할 수 있으며, 많은 경우 봇넷(botnet)과 같은 감염된 컴퓨터 네트워크를 활용하여 실행됩니다.

DDoS 공격 방어는 복잡한 문제로, 다양한 전략과 기술들이 필요합니다:

대역폭 확장: 가장 직접적인 방법인데, 간단하게 말해서 네트워크의 용량을 늘려서 더 많은 트래픽을 처리할 수 있도록 하는 것입니다.공격 패턴 인식 및 차단: IDS(Intrusion Detection System)나 IPS(Intrusion Prevention System)와 같은 시스템들은 비정상적인 트래픽 패턴(예: DDoS 공격)을 감지하고 차단하는 역할을 합니다.CDN(Content Delivery Network) 사용: CDN은 전세계에 분산된 서버 네트워크로, 웹 트래픽을 분산시키고 공격 트래픽을 필터링하는 역할을 할 수 있습니다.애플리케이션 레벨 보호: 웹 애플리케이션 방화벽(WAF)과 같은 도구를 사용하여 애플리케이션 계층에서의 공격을 막을 수 있습니다.

DDoS 공격 방어는 상황에 따라 다양한 전략과 기술들의 조합이 필요하며, 이는 지속적인 모니터링과 유지 관리가 요구됩니다.

</aside>

## 이런 질문도 나올 수 있어요!

### DDoS 공격을 막기 위한 방법에 대해서 설명해주세요.

DDoS 공격을 막기 위한 방법에는 여러 가지가 있습니다. 다음은 그 중 일부입니다:

대역폭 확장: 가장 간단한 방법 중 하나는 네트워크의 대역폭을 늘려서 더 많은 트래픽을 처리할 수 있게 하는 것입니다. 이 방법은 단순하지만, 대량의 DDoS 공격에 대해서는 비용 효율적이지 않을 수 있습니다.공격 패턴 인식 및 차단: IDS(Intrusion Detection System)나 IPS(Intrusion Prevention System)와 같은 시스템들이 비정상적인 트래픽 패턴(예: DDoS 공격)을 감지하고 차단하는 역할을 합니다.CDN(Content Delivery Network) 사용: CDN은 전세계에 분산된 서버 네트워크로, 웹 트래픽을 분산시키고 공격 트래픽을 필터링하는 역할도 할 수 있습니다.애플리케이션 레벨 보호: 웹 애플리케이션 방화벽(WAF)과 같은 도구를 사용하여 애플리케이션 계층에서의 공격을 막습니다.DDoS 보호 서비스 이용: Cloudflare, AWS Shield 등과 같은 서비스들이 DDoS 공격으로부터 웹사이트를 보호해주는 서비스를 제공합니다.시스템 및 네트워크 모니터링: 정상적인 상황에서의 시스템 및 네트워크 작동 패턴에 대한 이해와 지속적인 모니터링으로 이상 징후를 조기에 감지하고 대응할 수 있습니다.긴급 응답 계획 마련: DDoS 공격 발생 시 즉각적으로 대응하기 위해 사전에 긴급 응답 계획을 마련하고 준비해두는 것도 중요합니다.

## 만반의 준비! 이것도 알아둘까요?

### **제목 heading3**

내용

---

⚠️여기에 각주내용 및 출처, 그림 제목 등에 대해서 달아주세요!!!

표: 노션에서 제공해주는 기본 표 사용. 데이터베이스X

그림: 피그잼으로 도식화하여 사용 ~ 임시로 레퍼런스 사용 가능

코드: 노션에서 제공해주는 코드 블럭 사용 

단축키: ```(백틱 3개)

`백틱`: 메서드 및 코드 블럭에서 사용한 내용을 본문에서 언급할 때 

단축키: 해당 내용을 드래그하여 ctrl+E

인용: 노션에서 제공해주는 기본 스타일 사용

출처가 필요한 내용: *기울게* → 추후 일괄 수정 예정*

⚠️ 질문에 대한 답변 완료 및 저작권, 맞춤법 등의 추가 검사까지 완료

→페이지 아이콘 바꾸기 ✅ 해당 아이콘으로 페이지 아이콘을 바꿔주세요!