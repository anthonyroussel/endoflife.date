---
title: OpenSSL
layout: post
category: framework
iconSlug: openssl
permalink: /openssl
releasePolicyLink: https://www.openssl.org/policies/releasestrat.html
changelogTemplate: |
  https://www.openssl.org/news/changelog.html#openssl-{{"__RELEASE_CYCLE__" | replace:'.',''}}
eolColumn: Supported
activeSupportColumn: false
command: openssl version
releaseDateColumn: true
sortReleasesBy: releaseCycle
releases:
  - releaseCycle: "3.0"
    eol: 2026-09-07
    release: 2021-09-07
    latest: "3.0.3"
    lts: true
  - releaseCycle: "1.1.1"
    eol: 2023-09-11
    release: 2018-09-11
    latest: "1.1.1o"
    lts: true
  - releaseCycle: "1.1.0"
    eol: 2019-09-11
    release: 2016-08-26
    latest: "1.1.0l"
  - releaseCycle: "1.0.2"
    eol: 2019-12-31
    release: 2015-01-22
    latest: "1.0.2u"
    lts: true


---

> [OpenSSL](https://www.openssl.org/) is a software library for applications that secure communications over computer networks against eavesdropping or need to identify the party at the other end. It is widely used by Internet servers, including the majority of HTTPS websites. 

It is supported for [UNIX-like platforms](https://github.com/openssl/openssl/blob/master/NOTES-UNIX.md), [Android](https://github.com/openssl/openssl/blob/master/NOTES-ANDROID.md), [Windows](https://github.com/openssl/openssl/blob/master/NOTES-WINDOWS.md), [DOS platform with DJGPP](https://github.com/openssl/openssl/blob/master/NOTES-DJGPP.md), [OpenVMS](https://github.com/openssl/openssl/blob/master/NOTES-VMS.md), [Perl](https://github.com/openssl/openssl/blob/master/NOTES-PERL.md) and [Valgrind](https://github.com/openssl/openssl/blob/master/NOTES-PERL.md).

LTS releases will be supported for at least five years and they will specify one at least every four years. Non-LTS releases will be supported for at least two years.

As of release 3.0.0, the OpenSSL versioning scheme is changing to a more contemporary format: MAJOR.MINOR.PATCH

With this format, API/ABI compatibility will be guaranteed for the same MAJOR version number. Previously they guaranteed API/ABI compatibility across the same MAJOR.MINOR combination.

- MAJOR: API/ABI incompatible changes will increase this number
- MINOR: API/ABI compatible feature releases will change this
- PATCH: Bug fix releases will increment this number. We also allow backporting of accessor functions in these releases.