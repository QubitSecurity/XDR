다음 형식으로 **Nginx** CVE 전수 목록을 정리했습니다. (공식 *nginx security advisories* 기반) ([Nginx][1])

---

1. **Web : Nginx**

2. **CVE**

1) [CVE-2025-23419](https://www.cve.org/CVERecord?id=CVE-2025-23419) — SSL session reuse vulnerability
2) [CVE-2024-7347](https://www.cve.org/CVERecord?id=CVE-2024-7347) — Buffer overread in the ngx\_http\_mp4\_module
3) [CVE-2024-32760](https://www.cve.org/CVERecord?id=CVE-2024-32760) — Buffer overwrite in HTTP/3
4) [CVE-2024-31079](https://www.cve.org/CVERecord?id=CVE-2024-31079) — Stack overflow & use‑after‑free in HTTP/3
5) [CVE-2024-35200](https://www.cve.org/CVERecord?id=CVE-2024-35200) — NULL pointer dereference in HTTP/3
6) [CVE-2024-34161](https://www.cve.org/CVERecord?id=CVE-2024-34161) — Memory disclosure in HTTP/3
7) [CVE-2024-24989](https://www.cve.org/CVERecord?id=CVE-2024-24989) — NULL pointer dereference in HTTP/3
8) [CVE-2024-24990](https://www.cve.org/CVERecord?id=CVE-2024-24990) — Use‑after‑free in HTTP/3
9) [CVE-2022-41741](https://www.cve.org/CVERecord?id=CVE-2022-41741) — Memory corruption in the ngx\_http\_mp4\_module
10) [CVE-2022-41742](https://www.cve.org/CVERecord?id=CVE-2022-41742) — Memory disclosure in the ngx\_http\_mp4\_module
11) [CVE-2021-23017](https://www.cve.org/CVERecord?id=CVE-2021-23017) — 1‑byte memory overwrite in resolver
12) [CVE-2019-9511](https://www.cve.org/CVERecord?id=CVE-2019-9511) — Excessive CPU usage in HTTP/2 (small window updates)
13) [CVE-2019-9513](https://www.cve.org/CVERecord?id=CVE-2019-9513) — Excessive CPU usage in HTTP/2 (priority changes)
14) [CVE-2019-9516](https://www.cve.org/CVERecord?id=CVE-2019-9516) — Excessive memory usage in HTTP/2 (zero‑length headers)
15) [CVE-2018-16843](https://www.cve.org/CVERecord?id=CVE-2018-16843) — Excessive memory usage in HTTP/2
16) [CVE-2018-16844](https://www.cve.org/CVERecord?id=CVE-2018-16844) — Excessive CPU usage in HTTP/2
17) [CVE-2018-16845](https://www.cve.org/CVERecord?id=CVE-2018-16845) — Memory disclosure in the ngx\_http\_mp4\_module
18) [CVE-2017-7529](https://www.cve.org/CVERecord?id=CVE-2017-7529) — Integer overflow in the range filter
19) [CVE-2016-4450](https://www.cve.org/CVERecord?id=CVE-2016-4450) — NULL pointer dereference while writing client request body
20) [CVE-2016-0742](https://www.cve.org/CVERecord?id=CVE-2016-0742) — Invalid pointer dereference in resolver
21) [CVE-2016-0746](https://www.cve.org/CVERecord?id=CVE-2016-0746) — Use‑after‑free during CNAME processing in resolver
22) [CVE-2016-0747](https://www.cve.org/CVERecord?id=CVE-2016-0747) — Insufficient limits of CNAME resolution in resolver
23) [CVE-2014-3616](https://www.cve.org/CVERecord?id=CVE-2014-3616) — SSL session reuse vulnerability
24) [CVE-2014-3556](https://www.cve.org/CVERecord?id=CVE-2014-3556) — STARTTLS command injection
25) [CVE-2014-0133](https://www.cve.org/CVERecord?id=CVE-2014-0133) — SPDY heap buffer overflow
26) [CVE-2014-0088](https://www.cve.org/CVERecord?id=CVE-2014-0088) — SPDY memory corruption
27) [CVE-2013-4547](https://www.cve.org/CVERecord?id=CVE-2013-4547) — Request line parsing vulnerability
28) [CVE-2013-2070](https://www.cve.org/CVERecord?id=CVE-2013-2070) — Memory disclosure with crafted HTTP backend responses
29) [CVE-2013-2028](https://www.cve.org/CVERecord?id=CVE-2013-2028) — Stack‑based buffer overflow with crafted request
30) [CVE-2012-2089](https://www.cve.org/CVERecord?id=CVE-2012-2089) — Buffer overflow in the ngx\_http\_mp4\_module
31) [CVE-2012-1180](https://www.cve.org/CVERecord?id=CVE-2012-1180) — Memory disclosure with crafted backend responses
32) [CVE-2011-4315](https://www.cve.org/CVERecord?id=CVE-2011-4315) — Buffer overflow in resolver
33) [CVE-2011-4963](https://www.cve.org/CVERecord?id=CVE-2011-4963) — Windows directory aliases vulnerabilities
34) [CVE-2010-2266](https://www.cve.org/CVERecord?id=CVE-2010-2266) — Invalid UTF‑8 sequence handling on Windows
35) [CVE-2010-2263](https://www.cve.org/CVERecord?id=CVE-2010-2263) — Windows file default stream vulnerabilities
36) [CVE-2009-4487](https://www.cve.org/CVERecord?id=CVE-2009-4487) — Error log data not sanitized
37) [CVE-2009-3555](https://www.cve.org/CVERecord?id=CVE-2009-3555) — SSL renegotiation protocol vulnerability
38) [CVE-2009-3898](https://www.cve.org/CVERecord?id=CVE-2009-3898) — Directory traversal vulnerability
39) [CVE-2009-2629](https://www.cve.org/CVERecord?id=CVE-2009-2629) — Buffer underflow vulnerability
40) [CVE-2009-3896](https://www.cve.org/CVERecord?id=CVE-2009-3896) — Null pointer dereference vulnerability

> **출처:** 공식 *nginx security advisories* 페이지를 기준으로 정리했습니다. 필요 시 \*\*버전 영향 범위(취약/비취약 버전)\*\*도 각 항목에 덧붙여 드리겠습니다. ([Nginx][1])


[1]: https://nginx.org/en/security_advisories.html "nginx security advisories"
