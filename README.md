## OpenSSL Versioning ##

OpenSSL is often utilized by Internet servers and Hypertext Transfer Protocol Secure (HTTPS) websites, wherein the identify of the involved website/web service is validated, and the information flowing between the website/web service and user is encrypted. 

*Source: https://https.cio.gov*

The Common Vulnerabilities and Exposures (CVE) system lists publicly known Information Security (InfoSec) issues. CVE-2020-1971 (https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-1971) was a High Severity issue reported as an OpenSSL advisory (https://www.openssl.org/news/secadv/20201208.txt) on 8 December 2020. In brief, a vulnerability issue affected OpenSSL v1.0.2, which is out of support and no longer receiving public updates. OpenSSL v1.1.1i and beyond, theoretically, is no longer vulnerable to the referenced issue. 

*Source: https://www.openssl.org/news/vulnerabilities-1.0.2.html*


## Bundled OpenSSL versions ## 

Various Github commentators/contributors have noted, such as on 10 August 2015, that various bundled OpenSSL versions may be out of date.

*Source: https://github.com/docker/compose/issues/1834*

Yet, various offerings (e.g., various Docker Compose offerings) may still continue to incorporate outdated OpenSSL versions.

*Example #1*<br/>
$ docker-compose version<br/>
docker-compose version 1.23.2, build 1110ad0<br/>
docker-py version: 3.7.3<br/>
CPython version: 2.7.16<br/>
OpenSSL version: OpenSSL 1.1.1c  28 May 2019<br/>

*Source: https://dockerlabs.collabnix.com/intermediate/workshop/DockerCompose/version_Command.html*

*Example #2*<br/>
$ docker-compose version<br/>
docker-compose version 1.26.2, build eefe0d31<br/>
docker-py version: 4.2.2<br/>
CPython version: 3.7.7<br/>
OpenSSL version: OpenSSL 1.1.0l  10 Sep 2019<br/>

*Source: https://github.com/docker/compose/issues/7686*

*Example #2*<br/>
$ docker-compose version<br/>
docker-compose version 1.26.0-rc3, build 46118bc5 (rc refers to Release Candidate, which is software that is nearing final release quality assurance/quality control)<br/>
docker-py version: 4.2.0<br/>
CPython version: 3.7.6<br/>
OpenSSL version: OpenSSL 1.1.1d  10 Sep 2019<br/>

*Source: https://github.com/docker/compose/issues/7348*

By out of date, please recall that OpenSSL v1.1.1i and beyond is, theoretically, no longer vulnerable to the issue identified in CVE-2020-1971. Along this vein, the Cybersecurity & Infrastructure Security Agency (CISA) notes that, "OpenSSL has released a security update to address a vulnerability affecting all versions of 1.0.2 and 1.1.1 released before version 1.1.1i. An attacker could exploit this vulnerability to cause a denial-of-service condition."

*Source: https://us-cert.cisa.gov/ncas/current-activity/2020/12/08/openssl-releases-security-update*

Apart from CVE-2020-1971, additional OpenSSL CVEs are available here: https://www.openssl.org/news/vulnerabilities.html.

Also, other CVEs are available at the National Vulnerability Database (NVD) (https://nvd.nist.gov) and U.S. Computer Emergency Response Team (CERT)-CISA (https://us-cert.cisa.gov) portals.

## Docker Compose versions ## 

As discussed, OpenSSL versions affected by CVE-2020-1971, among others, had been bundled with Docker Compose. Some of the more recent Docker Compose versions are listed here: https://docs.docker.com/compose/release-notes/<br/>

For convenience, please refer to Table 1 below.

### Table 1: Docker Compose Release Versions ###

|Version Number|Release Date |
|--------------|-------------|
|1.28.2        | (2021-01-26)|
|1.28.0        | (2021-01-20)|
|1.27.4        | (2020-09-24)|
|1.27.3        | (2020-09-16)|
|1.27.2        | (2020-09-10)|
|1.27.1        | (2020-09-10)|
|1.27.0        | (2020-09-07)|
|1.26.2        | (2020-07-02)|

It should be noted that Docker Compose v1.28.0 might still be deploying with OpenSSL v1.1.1h (i.e., vulnerable to CVE-2020-1971). OpenSSL v1.1.1i and above have the security update for CVE-2020-1971. The OpenSSL version should be confirmed when utilizing the bundled versions of Docker Compose v1.28.0 and prior. 

This bundling issue has persisted for quite some time (e.g., https://github.com/docker/compose/issues/1601).



