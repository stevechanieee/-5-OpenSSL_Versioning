## OpenSSL Versioning ##

OpenSSL is often utilized by Internet servers and Hypertext Transfer Protocol Secure (HTTPS) websites, wherein the identify of the involved website/web service is validated, and the information flowing between the website/web service and user is encrypted. 

*Source: https://https.cio.gov*

The Common Vulnerabilities and Exposures (CVE) system lists publicly known information security issues. CVE-2020-1971 (https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2020-1971) was a High Severity issue reported as an OpenSSL advisory (https://www.openssl.org/news/secadv/20201208.txt) on 8 December 2020. In essence, an issue affected OpenSSL v1.0.2, which is out of support and no longer receiving public updates. OpenSSL v1.1.1i and beyond is not vulnerable to the issue. 

*Source: https://www.openssl.org/news/vulnerabilities-1.0.2.html*


## Bundled OpenSSL versions ## 

Various Github commentators/contributors have noted, such as on 10 August 2015, that the bundled OpenSSL versions are out of date.

*Source: https://github.com/docker/compose/issues/1834*

Yet, various offerings (e.g., various docker-compose offerings) still incorporate outdated OpenSSL versions.

*Example #1*
$ docker-compose version
docker-compose version 1.23.2, build 1110ad0
docker-py version: 3.7.3
CPython version: 2.7.16
OpenSSL version: OpenSSL 1.1.1c  28 May 2019  

*Source: https://dockerlabs.collabnix.com/intermediate/workshop/DockerCompose/version_Command.html*

*Example #2*
$ docker-compose version
docker-compose version 1.26.2, build eefe0d31
docker-py version: 4.2.2
CPython version: 3.7.7
OpenSSL version: OpenSSL 1.1.0l  10 Sep 2019

*Source: https://github.com/docker/compose/issues/7686*

*Example #2*
$ docker-compose version
docker-compose version 1.26.0-rc3, build 46118bc5 (rc refers to Release Candidate, which is software that is nearing final release quality assurance/quality control)
docker-py version: 4.2.0
CPython version: 3.7.6
OpenSSL version: OpenSSL 1.1.1d  10 Sep 2019

*Source: https://github.com/docker/compose/issues/7348*



https://docs.docker.com/compose/release-notes/
1.28.2 - (2021-01-26)
1.28.0 - (2021-01-20)
1.27.4 - (2020-09-24)
1.27.3 - (2020-09-16)
1.27.2 - (2020-09-10)
1.27.1 - (2020-09-10)
1.27.0 - (2020-09-07)
1.26.2 - (2020-07-02)












docker-compose version 1.23.2
https://github.com/docker/compose/issues/7686


The


https://www.ibm.com/support/knowledgecenter/SSKRA3_1.0.6/va/InstallingSolution/install_docker_components.html

docker-compose version 1.23.2


https://www.openssl.org/news/vulnerabilities.html




