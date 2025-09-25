1. **WAS : JBoss / WildFly**

2. **CVE**

1) [CVE-2017-12149](https://nvd.nist.gov/vuln/detail/CVE-2017-12149) — HTTP Invoker **디시리얼라이제이션 RCE**. ([NVD][1])
2) [CVE-2015-7501](https://access.redhat.com/security/cve/cve-2015-7501) — Apache Commons‑Collections **디시리얼라이제이션 RCE**(JBoss 미들웨어 전반 영향). ([Red Hat Customer Portal][2])
3) [CVE-2017-7504](https://nvd.nist.gov/vuln/detail/cve-2017-7504) — JBossMQ JMS over HTTP **디시리얼라이제이션 RCE**(JBoss 4.x). ([NVD][3])
4) [CVE-2010-0738](https://nvd.nist.gov/vuln/detail/cve-2010-0738) — **JMX Console** 메서드 처리 결함(권한우회). ([NVD][4])
5) [CVE-2012-0874](https://nvd.nist.gov/vuln/detail/CVE-2012-0874) — **EJBInvoker/JMXInvoker** 기본 무인증 → RCE 가능. ([NVD][5])
6) [CVE-2016-7065](https://nvd.nist.gov/vuln/detail/CVE-2016-7065) — JMX 서블릿 **직렬화 오브젝트** 처리로 DoS/코드실행 가능(인증 필요). ([NVD][6])
7) [CVE-2016-7066](https://nvd.nist.gov/vuln/detail/CVE-2016-7066) — `/tmp/auth` 권한 문제로 **CLI 임의 실행(로컬 EoP)**. ([NVD][7])
8) [CVE-2016-4978](https://access.redhat.com/security/cve/cve-2016-4978) — **JMS ObjectMessage** 디시리얼라이제이션 RCE. ([Red Hat Customer Portal][8])
9) [CVE-2016-4993](https://nvd.nist.gov/vuln/detail/cve-2016-4993) — Undertow **CRLF 헤더 주입 / 응답 분할**. ([NVD][9])
10) [CVE-2018-1067](https://nvd.nist.gov/vuln/detail/cve-2018-1067) — Undertow **헤더 주입(불완전 패치로 재발)**. ([NVD][10])
11) [CVE-2014-7816](https://nvd.nist.gov/vuln/detail/CVE-2014-7816) — Undertow **경로 조작(Windows 경로 트래버설)**. ([NVD][11])
12) [CVE-2018-1048](https://nvd.nist.gov/vuln/detail/cve-2018-1048) — Undertow AJP **인코딩된 슬래시 허용 → 경로 트래버설/정보노출**. ([NVD][12])
13) [CVE-2018-1047](https://nvd.nist.gov/vuln/detail/cve-2018-1047) — Undertow `getResource` **경로 트래버설(정보노출)**. ([NVD][13])
14) [CVE-2019-14843](https://nvd.nist.gov/vuln/detail/cve-2019-14843) — WildFly Security Manager **권한검사 오류(인증 우회/권한상승 경로)**. ([NVD][14])
15) [CVE-2017-12165](https://nvd.nist.gov/vuln/detail/cve-2017-12165) — Undertow **HTTP 요청 스머글링(공백 처리)**. ([NVD][15])
16) [CVE-2017-12196](https://nvd.nist.gov/vuln/detail/cve-2017-12196) — Undertow **Digest 인증 URI 불일치 → 권한 우회(MITM)**. ([NVD][16])
17) [CVE-2016-5406](https://nvd.nist.gov/vuln/detail/cve-2016-5406) — EAP 도메인 컨트롤러 **RBAC 전파 실패 → 권한상승**. ([NVD][17])
18) [CVE-2016-6311](https://nvd.nist.gov/vuln/detail/CVE-2016-6311) — EAP 7 **리다이렉트 시 내부 IP 노출(Host 미지정)**. ([NVD][18])


[1]: https://nvd.nist.gov/vuln/detail/CVE-2017-12149?utm_source=chatgpt.com "CVE-2017-12149 Detail - NVD"
[2]: https://access.redhat.com/security/cve/cve-2015-7501?utm_source=chatgpt.com "CVE-2015-7501"
[3]: https://nvd.nist.gov/vuln/detail/cve-2017-7504?utm_source=chatgpt.com "CVE-2017-7504 Detail - NVD"
[4]: https://nvd.nist.gov/vuln/detail/cve-2010-0738?utm_source=chatgpt.com "cve-2010-0738 - NVD"
[5]: https://nvd.nist.gov/vuln/detail/CVE-2012-0874/change-record?changeRecordedOn=11%2F06%2F2023T21%3A10%3A05.097-0500&utm_source=chatgpt.com "CVE-2012-0874 - NVD"
[6]: https://nvd.nist.gov/vuln/detail/CVE-2016-7065?utm_source=chatgpt.com "CVE-2016-7065 - NVD"
[7]: https://nvd.nist.gov/vuln/detail/CVE-2016-7066?utm_source=chatgpt.com "CVE-2016-7066 Detail - NVD"
[8]: https://access.redhat.com/security/cve/cve-2016-4978?utm_source=chatgpt.com "CVE-2016-4978"
[9]: https://nvd.nist.gov/vuln/detail/cve-2016-4993?utm_source=chatgpt.com "CVE-2016-4993 Detail - NVD"
[10]: https://nvd.nist.gov/vuln/detail/cve-2018-1067?utm_source=chatgpt.com "CVE-2018-1067 Detail - NVD"
[11]: https://nvd.nist.gov/vuln/detail/CVE-2014-7816?utm_source=chatgpt.com "CVE-2014-7816 - NVD"
[12]: https://nvd.nist.gov/vuln/detail/cve-2018-1048?utm_source=chatgpt.com "CVE-2018-1048 Detail - NVD"
[13]: https://nvd.nist.gov/vuln/detail/cve-2018-1047?utm_source=chatgpt.com "CVE-2018-1047 Detail - NVD"
[14]: https://nvd.nist.gov/vuln/detail/cve-2019-14843?utm_source=chatgpt.com "CVE-2019-14843 Detail - NVD"
[15]: https://nvd.nist.gov/vuln/detail/cve-2017-12165?utm_source=chatgpt.com "cve-2017-12165 - NVD"
[16]: https://nvd.nist.gov/vuln/detail/cve-2017-12196?utm_source=chatgpt.com "CVE-2017-12196 Detail - NVD"
[17]: https://nvd.nist.gov/vuln/detail/cve-2016-5406?utm_source=chatgpt.com "CVE-2016-5406 Detail - NVD"
[18]: https://nvd.nist.gov/vuln/detail/CVE-2016-6311?utm_source=chatgpt.com "CVE-2016-6311 Detail - NVD"
