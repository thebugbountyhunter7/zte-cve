# zte-cve

The vulnerability is a Server Info Exposure in ZTE devices. This vulnerability is triggered when an attacker modifies the headers in any of the formats listed above and locates to the "/server-status" endpoint. The headers in question include: Forwarded, X-Client-IP, X-Forwarded-By, X-Forwarded-For, X-Forwarded-For-IP, X-Forwarded-Host, X-Host, X-Originating-IP, X-Remote-Addr, X-Remote-IP, and X-True-IP.

When these headers are modified to have a value of "127.0.0.1", the server information becomes accessible and can be leaked. This includes sensitive information such as system details, resource utilization, and active connections. This information can be used by an attacker for malicious purposes, such as planning a more targeted attack on the system.

The impact of this vulnerability is significant as it can lead to exposure of sensitive information about the system and aid attackers in executing further attacks. It is crucial to address this vulnerability as soon as possible to protect the device and the information it holds.
