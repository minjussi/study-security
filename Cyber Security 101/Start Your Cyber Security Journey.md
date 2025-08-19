# Offensive Security

🔒 해커보다 똑똑해지려면 해커처럼 생각하기

## First Hack

- 해킹 시도의 첫 걸음: 숨겨진 특징들 찾기 (ex. url)
- dirb 명령어 사용: dirb는 브루트 포스 기법을 활용해 숨겨진 페이지 url을 찾는 도구

  <pre>dirb http://fakebank.thm</pre>

---

# Defensive Security

🔒 IT 인프라를 준비하고 사전에 공격을 방어 (blue team으로 알려져 있음)
🔒 주요 업무는 공격을 예방하고, 발생한 공격을 탐지하고 적절한 대응을 하는 것임

## SOC (Security Operations Centre)

- 악의적인 사이버 보안 이벤트를 감지하기 위해 네트워크와 시스템을 모니터링
- Security Information and Event Management (SIEM) 도구를 활용해 보안과 관련된 정보 수집
- 수상한 활동이 감지되는 IP 주소를 찾아 block

---

# Search Skills

🔒 수많은 정보 중 의미 있는 정보를 찾을 수 있어야 함

## Search Engines

ex. Google, Bing, DuckDuckGo

- "exact phrase": 쌍따옴표 ("")를 붙여서 검색하면 해당 단어나 구문이 정확하게 들어간 페이지를 검색함
- site: 도메인 이름을 정확하게 명시하여 검색을 특정함
- -: 마이너스 기호 (-)를 붙여서 검색하면 해당 단어나 구문이 있는 페이지를 제외하고 결과를 반환함
- filetype: 웹 페이지 대신 지정한 파일 형식의 결과를 반환함

## Specialized Search Engines

1. Shodan: 인터넷에 연결된 디바이스를 찾을 수 있는 서치 엔진

- 특정 버전의 서버, 네트워킹 장비, 산업용 제어 시스템 및 IoT 장치를 검색할 수 있음
- ex. apache 2.4.1을 검색하면, 헤더에 "apache 2.4.1"이 포함된 서버 목록이 반환됨
- Search Query Examples(https://www.shodan.io/search/examples), Shodan trends(https://www.shodan.io/search/examples) 참고

2. Censys: 인터넷에 연결된 인터넷 연결 호스트, 웹사이트, 인증서 및 기타 인터넷 자산에 중점

- 사용 중인 도메인 열거, 열린 포트 및 서비스 감사, 네트워크 내 악성 자산 발견 등에 활용

3. VirusTotal: 바이러스 스캐닝 서비스

- 파일을 업로드하거나 url을 입력해서 한 번에 여러 바이러스 백신과 웹사이트 엔진으로 검사 가능
- 파일 해시를 입력해 이전에 업로드된 파일 결과 확인 가능

4. Have I Been Pwned(HIBP): 유출된 데이터에 존재하는 이메일 주소인지 알려주는 서비스

- 이메일 주소가 나타났다는 것은 개인정보와 패스워드가 유출되었다는 의미
- 대부분의 비밀번호는 암호화된 형태로 저장되기 때문에 간단한 비밀번호는 유추하기 쉬움

## Vulnerabilities and Exploits

**CVE**

- Common Vulnerabilities and Exposures: 표준화된 취약점 식별자로 모든 사람이 동일하게 취약점을 식별할 수 있게 함
- More information: https://www.cve.org/ , https://nvd.nist.gov/

**Exploit Database**

- 허가가 있을 때만 익스플로잇을 시도해야 함
- 다양한 익스플로잇 코드 확인 가능: https://www.exploit-db.com/
- PoC(Proof of Concept) 및 익스플로잇 코드 확인: Github

## Technical Documentation

**Linux Manual Pages**

- 모든 명령어에는 man 페이지 존재
- ex. ip 명령어를 확인하고 싶으면 man ip 입력 -> ip 명령어에 대한 정보 출력 (q로 나가기 가능)
- AttackBox: 브라우저에서 접근할 수 있는 linux 시스템
