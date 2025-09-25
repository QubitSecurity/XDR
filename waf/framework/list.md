1. **Framework / Library : Apache Log4j 2**

2. **CVE**

1) [CVE-2021-44228 (Log4Shell)](https://nvd.nist.gov/vuln/detail/CVE-2021-44228) — JNDI Lookup 악용을 통한 **무인증 RCE**. ([NVD][1])
2) [CVE-2021-45046](https://nvd.nist.gov/vuln/detail/CVE-2021-45046) — 룩업 우회에 의한 추가 RCE/DoS 가능. ([NVD][2])
3) [CVE-2021-45105](https://nvd.nist.gov/vuln/detail/CVE-2021-45105) — **자가참조 룩업**으로 인한 DoS. ([NVD][3])
4) [CVE-2021-44832](https://nvd.nist.gov/vuln/detail/CVE-2021-44832) — **JDBC Appender + JNDI** 구성 변경 시 RCE. ([NVD][4])

* 참고(공식): Log4j 보안 공지(요약/완화). ([logging.apache.org][5])

---

1. **Framework / Library : Spring (Core/Cloud)**

2. **CVE**

1) [CVE-2022-22965 (Spring4Shell)](https://spring.io/security/cve-2022-22965) — 데이터 바인딩 결함으로 **무인증 RCE**(주로 Tomcat WAR 배포 조합). ([Home][6])
2) [CVE-2022-22963 (Spring Cloud Function)](https://spring.io/security/cve-2022-22963) — **SpEL** 기반 라우팅 표현식 처리로 RCE. ([Home][7])
3) [CVE-2022-22947 (Spring Cloud Gateway)](https://spring.io/security/cve-2022-22947) — Actuator 노출 시 **코드 주입 → RCE**. ([Home][8])

* 배경/가이드: Microsoft·CISA 분석(영향/완화). ([Microsoft][9])

---

1. **Framework : Apache Struts 2**

2. **CVE**

1) [CVE-2017-5638](https://nvd.nist.gov/vuln/detail/CVE-2017-5638) — **Content‑Type 헤더** 처리 결함으로 RCE(Jakarta Multipart). ([NVD][10])
2) [CVE-2017-9805](https://nvd.nist.gov/vuln/detail/CVE-2017-9805) — **REST 플러그인(XStream) 디시리얼라이제이션 RCE**. ([NVD][11])
3) [CVE-2018-11776](https://nvd.nist.gov/vuln/detail/CVE-2018-11776) — **네임스페이스 처리** 오류로 RCE. ([NVD][12])

* 참고(공식 공지/요약): Struts 2018 보안 공지(S2‑057 포함). ([Apache Struts][13])

---

1. **Library : Apache Shiro**

2. **CVE**

1) [CVE-2016-4437](https://nvd.nist.gov/vuln/detail/CVE-2016-4437) — `rememberMe` **디시리얼라이제이션 RCE/권한우회**(키 미설정 시). ([NVD][14])
2) [CVE-2020-11989](https://nvd.nist.gov/vuln/detail/CVE-2020-11989) — Spring 동적 컨트롤러 조합 시 **인증 우회**. ([NVD][15])

* 참고(공식 목록): Shiro Security Reports. ([Apache Shiro][16])

---

1. **Library : Alibaba Fastjson**

2. **CVE**

1) [CVE-2022-25845](https://nvd.nist.gov/vuln/detail/CVE-2022-25845) — **autoType 우회 디시리얼라이제이션 → RCE**(1.2.83 미만). ([NVD][17])

---

1. **Library : FasterXML Jackson‑databind**

2. **CVE**

1) [CVE-2017-7525](https://nvd.nist.gov/vuln/detail/CVE-2017-7525) — 폴리모픽 **디시리얼라이제이션 RCE**(ObjectMapper). ([NVD][18])
2) [CVE-2019-12384](https://nvd.nist.gov/vuln/detail/CVE-2019-12384) — `logback-core` 등 **가젯 체인**을 통한 RCE 가능. ([NVD][19])
3) [CVE-2020-8840](https://nvd.nist.gov/vuln/detail/CVE-2020-8840) — **xbean‑reflect/JNDI** 차단 미비로 RCE 가능. ([NVD][20])

---

1. **Library : XStream**

2. **CVE**

1) [CVE-2020-26217](https://nvd.nist.gov/vuln/detail/CVE-2020-26217) — **XML 디시리얼라이제이션 RCE**(블록리스트 의존 시). ([NVD][21])
2) [CVE-2021-29505](https://nvd.nist.gov/vuln/detail/CVE-2021-29505) — 입력 조작으로 **호스트 명령 실행** 가능(화이트리스트 미적용 시). ([NVD][22])

* 참고(공식): XStream 보안 페이지(문서화된 CVE 일람). ([x-stream.github.io][23])

---

1. **Library : SnakeYAML**

2. **CVE**

1) [CVE-2022-1471](https://nvd.nist.gov/vuln/detail/CVE-2022-1471) — `Constructor()` 타입 제한 부재로 **RCE**(2.0 이상으로 변경/`SafeConstructor` 권고). ([NVD][24])
2) [CVE-2022-25857](https://nvd.nist.gov/vuln/detail/CVE-2022-25857) — 중첩 깊이 제한 부재로 **DoS**. ([NVD][25])
3) [CVE-2022-38752](https://nvd.nist.gov/vuln/detail/CVE-2022-38752) — 스택 오버플로우 유발 **DoS**. ([NVD][26])

---

1. **Library : Apache Commons Text**

2. **CVE**

1) [CVE-2022-42889 (Text4Shell)](https://nvd.nist.gov/vuln/detail/CVE-2022-42889) — `StringSubstitutor` 기본 Lookup(`script`,`dns`,`url`)으로 **RCE/원격 접속** 위험(1.10.0에서 기본 비활성). ([NVD][27])

* 참고(공식): Commons Text 보안 리포트. ([commons.apache.org][28])

---

[1]: https://nvd.nist.gov/vuln/detail/cve-2021-44228?utm_source=chatgpt.com "CVE-2021-44228 Detail - NVD"
[2]: https://nvd.nist.gov/vuln/detail/cve-2021-45046?utm_source=chatgpt.com "CVE-2021-45046 Detail - NVD"
[3]: https://nvd.nist.gov/vuln/detail/cve-2021-45105?utm_source=chatgpt.com "CVE-2021-45105 Detail - NVD"
[4]: https://nvd.nist.gov/vuln/detail/cve-2021-44832?utm_source=chatgpt.com "CVE-2021-44832 Detail - NVD"
[5]: https://logging.apache.org/log4j/2.12.x/?utm_source=chatgpt.com "Apache Log4j 2"
[6]: https://spring.io/security/cve-2022-22965?utm_source=chatgpt.com "CVE-2022-22965: Spring Framework RCE via Data Binding on JDK ..."
[7]: https://spring.io/security/cve-2022-22963?utm_source=chatgpt.com "CVE-2022-22963: Remote code execution in Spring Cloud Function ..."
[8]: https://spring.io/security/cve-2022-22947?utm_source=chatgpt.com "CVE-2022-22947: Spring Cloud Gateway Code Injection ..."
[9]: https://www.microsoft.com/en-us/security/blog/2022/04/04/springshell-rce-vulnerability-guidance-for-protecting-against-and-detecting-cve-2022-22965/?utm_source=chatgpt.com "SpringShell RCE vulnerability: Guidance for protecting against and ..."
[10]: https://nvd.nist.gov/vuln/detail/cve-2017-5638?utm_source=chatgpt.com "CVE-2017-5638 Details - NVD"
[11]: https://nvd.nist.gov/vuln/detail/cve-2017-9805?utm_source=chatgpt.com "CVE-2017-9805 Detail - NVD"
[12]: https://nvd.nist.gov/vuln/detail/cve-2018-11776?utm_source=chatgpt.com "CVE-2018-11776 Detail - NVD"
[13]: https://struts.apache.org/announce-2018.html?utm_source=chatgpt.com "Announcements 2018 - Apache Struts"
[14]: https://nvd.nist.gov/vuln/detail/cve-2016-4437?utm_source=chatgpt.com "CVE-2016-4437 Detail - NVD"
[15]: https://nvd.nist.gov/vuln/detail/cve-2020-11989?utm_source=chatgpt.com "CVE-2020-11989 Detail - NVD"
[16]: https://shiro.apache.org/security-reports.html?utm_source=chatgpt.com "Security Reports - Apache Shiro"
[17]: https://nvd.nist.gov/vuln/detail/cve-2022-25845?utm_source=chatgpt.com "CVE-2022-25845 Detail - NVD"
[18]: https://nvd.nist.gov/vuln/detail/cve-2017-7525?utm_source=chatgpt.com "CVE-2017-7525 Detail - NVD"
[19]: https://nvd.nist.gov/vuln/detail/cve-2019-12384?utm_source=chatgpt.com "CVE-2019-12384 Detail - NVD"
[20]: https://nvd.nist.gov/vuln/detail/cve-2020-8840?utm_source=chatgpt.com "CVE-2020-8840 Detail - NVD"
[21]: https://nvd.nist.gov/vuln/detail/cve-2020-26217?utm_source=chatgpt.com "CVE-2020-26217 Detail - NVD"
[22]: https://nvd.nist.gov/vuln/detail/cve-2021-29505?utm_source=chatgpt.com "CVE-2021-29505 Detail - NVD"
[23]: https://x-stream.github.io/security.html?utm_source=chatgpt.com "Security Aspects - XStream"
[24]: https://nvd.nist.gov/vuln/detail/cve-2022-1471?utm_source=chatgpt.com "cve-2022-1471 - NVD"
[25]: https://nvd.nist.gov/vuln/detail/cve-2022-25857?utm_source=chatgpt.com "CVE-2022-25857 Detail - NVD"
[26]: https://nvd.nist.gov/vuln/detail/cve-2022-38752?utm_source=chatgpt.com "CVE-2022-38752 Detail - NVD"
[27]: https://nvd.nist.gov/vuln/detail/cve-2022-42889?utm_source=chatgpt.com "CVE-2022-42889 Detail - NVD"
[28]: https://commons.apache.org/proper/commons-text/security.html?utm_source=chatgpt.com "Apache Commons Text Security Reports"
