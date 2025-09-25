1. **WAS : Apache Tomcat**

2. **CVE**

1) [CVE-2025-24813](https://nvd.nist.gov/vuln/detail/CVE-2025-24813) — **Default Servlet 쓰기 허용 + ‘file.Name’ 경로 동등성 → RCE/정보노출**. ([NVD][1])
2) [CVE-2024-56337](https://nvd.nist.gov/vuln/detail/CVE-2024-56337) — **CVE‑2024‑50379 불완전 패치 → RCE(대소문자 구분 없는 FS + Default Servlet write)**. ([NVD][2])
3) [CVE-2024-50379](https://nvd.nist.gov/vuln/detail/CVE-2024-50379) — **JSP 컴파일 TOCTOU 레이스 → RCE(Default Servlet write, case‑insensitive FS)**. ([NVD][3])
4) [CVE-2024-52317](https://nvd.nist.gov/vuln/detail/CVE-2024-52317) — **HTTP/2 요청·응답 혼선(Request/Response mix‑up) → 세션 간 데이터 섞임**. ([NVD][4])
5) [CVE-2024-38286](https://nvd.nist.gov/vuln/detail/CVE-2024-38286) — **TLS 핸드셰이크 남용 → OutOfMemoryError 유발 DoS**. ([NVD][5])
6) [CVE-2024-23672](https://tomcat.apache.org/security-11.html) / [CVE-2024-24549](https://tomcat.apache.org/security-11.html) — **WebSocket 유지·HTTP/2 헤더 처리 결함 → DoS**. ([Apache Tomcat][6])
7) [CVE-2020-1938](https://nvd.nist.gov/vuln/detail/CVE-2020-1938) — **AJP 요청 주입/파일 읽기(‘Ghostcat’) → 조건부 RCE**. ([NVD][7])
8) [CVE-2020-9484](https://nvd.nist.gov/vuln/detail/CVE-2020-9484) — **세션 지속성(FileStore) 디시리얼라이제이션 → RCE(특정 구성)**. ([NVD][8])
9) [CVE-2021-25329](https://nvd.nist.gov/vuln/detail/CVE-2021-25329) — **CVE‑2020‑9484 불완전 수정 → 세션 지속성 경로 RCE(엣지 케이스)**. ([NVD][9])
10) [CVE-2022-23181](https://nvd.nist.gov/vuln/detail/CVE-2022-23181) — **FileStore 사용 시 TOCTOU → 로컬 권한 상승(LPE)**. ([NVD][10])
11) [CVE-2019-0232](https://nvd.nist.gov/vuln/detail/CVE-2019-0232) — **Windows + enableCmdLineArguments=true인 CGI 서블릿 → RCE**. ([NVD][11])
12) [CVE-2019-0199](https://nvd.nist.gov/vuln/detail/CVE-2019-0199) — **HTTP/2 SETTINGS 남용·쓰레드 고갈 → DoS**. ([NVD][12])
13) [CVE-2020-11996](https://nvd.nist.gov/vuln/detail/CVE-2020-11996) — **특수 HTTP/2 시퀀스 → 고CPU/응답불가 DoS**. ([NVD][13])
14) [CVE-2021-43980](https://nvd.nist.gov/vuln/detail/CVE-2021-43980) — **블로킹 I/O 단순화로 동시성 버그 → 응답 혼선(정보노출)**. ([NVD][14])
15) [CVE-2018-11784](https://www.rapid7.com/db/vulnerabilities/apache-tomcat-cve-2018-11784/) — **Default Servlet 디렉터리 리다이렉트 → 오픈 리다이렉트**. ([Rapid7][15])
16) [CVE-2018-1336](https://nvd.nist.gov/vuln/detail/CVE-2018-1336) — **UTF‑8 디코더 오버플로 → 무한루프 DoS**. ([NVD][16])
17) [CVE-2018-8037](https://nvd.nist.gov/vuln/detail/CVE-2018-8037) — **async 처리 레이스 → 타 사용자 응답 노출**. ([NVD][17])
18) [CVE-2016-5388](https://nvd.nist.gov/vuln/detail/CVE-2016-5388) — **CGI(httpoxy) 환경변수 오염 → 프록시 강제/정보노출**. ([NVD][18])
19) [CVE-2016-0763](https://nvd.nist.gov/vuln/detail/CVE-2016-0763) — **ResourceLinkFactory 권한 체크 누락 → SecurityManager 우회**. ([NVD][19])

> **참고(공식 목록):** Tomcat의 공식 보안 페이지(버전별)에서 전수 목록과 영향 버전을 확인할 수 있습니다 — [Tomcat 11](https://tomcat.apache.org/security-11.html) / [Tomcat 10](https://tomcat.apache.org/security-10.html) / [Tomcat 9](https://tomcat.apache.org/security-9.html) / [Tomcat 8](https://tomcat.apache.org/security-8.html). ([Apache Tomcat][6])

[1]: https://nvd.nist.gov/vuln/detail/CVE-2025-24813?utm_source=chatgpt.com "CVE-2025-24813 Detail - NVD"
[2]: https://nvd.nist.gov/vuln/detail/CVE-2024-56337?utm_source=chatgpt.com "CVE-2024-56337 Detail - NVD"
[3]: https://nvd.nist.gov/vuln/detail/cve-2024-50379?utm_source=chatgpt.com "CVE-2024-50379 Detail - NVD"
[4]: https://nvd.nist.gov/vuln/detail/CVE-2024-52317?utm_source=chatgpt.com "CVE-2024-52317 Detail - NVD"
[5]: https://nvd.nist.gov/vuln/detail/cve-2024-38286?utm_source=chatgpt.com "CVE-2024-38286 Detail - NVD"
[6]: https://tomcat.apache.org/security-11.html?utm_source=chatgpt.com "Apache Tomcat 11 vulnerabilities"
[7]: https://nvd.nist.gov/vuln/detail/cve-2020-1938?utm_source=chatgpt.com "CVE-2020-1938 Detail - NVD"
[8]: https://nvd.nist.gov/vuln/detail/cve-2020-9484?utm_source=chatgpt.com "CVE-2020-9484 Detail - NVD"
[9]: https://nvd.nist.gov/vuln/detail/cve-2021-25329?utm_source=chatgpt.com "CVE-2021-25329 Detail - NVD"
[10]: https://nvd.nist.gov/vuln/detail/cve-2022-23181?utm_source=chatgpt.com "CVE-2022-23181 Detail - NVD"
[11]: https://nvd.nist.gov/vuln/detail/cve-2019-0232?utm_source=chatgpt.com "CVE-2019-0232 Detail - NVD"
[12]: https://nvd.nist.gov/vuln/detail/cve-2019-0199?utm_source=chatgpt.com "CVE-2019-0199 Detail - NVD"
[13]: https://nvd.nist.gov/vuln/detail/cve-2020-11996?utm_source=chatgpt.com "CVE-2020-11996 Detail - NVD"
[14]: https://nvd.nist.gov/vuln/detail/cve-2021-43980?utm_source=chatgpt.com "CVE-2021-43980 Detail - NVD"
[15]: https://www.rapid7.com/db/vulnerabilities/apache-tomcat-cve-2018-11784/?utm_source=chatgpt.com "Apache Tomcat - Open Redirect (CVE-2018-11784)"
[16]: https://nvd.nist.gov/vuln/detail/cve-2018-1336?utm_source=chatgpt.com "cve-2018-1336 - NVD"
[17]: https://nvd.nist.gov/vuln/detail/cve-2018-8037?utm_source=chatgpt.com "cve-2018-8037 - NVD"
[18]: https://nvd.nist.gov/vuln/detail/cve-2016-5388?utm_source=chatgpt.com "CVE-2016-5388 Detail - NVD"
[19]: https://nvd.nist.gov/vuln/detail/cve-2016-0763?utm_source=chatgpt.com "CVE-2016-0763 Detail - NVD"
