---
permalink: /centos
layout: post
title: CentOS
category: os
command: lsb_release --release
link: https://wiki.centos.org/About/Product
activeSupportColumn: true
releaseDateColumn: true
sortReleasesBy: 'release'
releases:
  - releaseCycle: "CentOS 6"
    release: 2011-07-10
    support: 2017-05-10
    eol: 2020-11-30
    latest: "6.10"
    link: https://wiki.centos.org/Manuals/ReleaseNotes/CentOS6.10
  - releaseCycle: "CentOS Linux 7"
    release: 2014-07-07
    support: 2020-08-06
    eol: 2024-06-30
    latest: "7 (2009)"
    link: https://wiki.centos.org/Manuals/ReleaseNotes/CentOS7.2009
  - releaseCycle: "CentOS Linux 8"
    release: 2019-09-24
    support: 2021-12-31
    eol: 2021-12-31
    latest: "8 (2111)"
    link:  https://wiki.centos.org/Manuals/ReleaseNotes/CentOS8.2111
  - releaseCycle: "CentOS Stream 8"
    release: 2019-09-24
    support: 2024-05-31
    eol: 2024-05-31
    latest: "8"
    link: https://wiki.centos.org/Manuals/ReleaseNotes/CentOSStream
    
  - releaseCycle: "CentOS Stream 9"
    release: 2021-09-15
    support: true
    eol: false
    latest: "9"
    link: https://wiki.centos.org/Manuals/ReleaseNotes/CentOSStream

---

> [CentOS](https://centos.org/) is a Linux distribution that provides a free, enterprise-class, community-supported computing platform functionally compatible with Red Hat Enterprise Linux.

The CentOS distribution comes in two variants: CentOS Linux and CentOS Stream.  CentOS Linux is rebuilt from Red Hat Enterprise Linux source code and referred to as the downstream variant.  CentOS Stream is the upstream variant, and contains content that is planned for the next minor release of Red Hat Enterprise Linux.

CentOS Linux currently has 2 major released branches that are active: CentOS Linux 7 and CentOS Linux 8. **The CentOS Project provides updates or other changes ONLY for the latest version of each major branch**. Thus, if the latest minor version of CentOS Linux 7 is version 7.9 then the CentOS Project only provides updated software for this minor version in the 7 branch. If you are using an older minor version than the latest in a given branch, then you are missing security and bugfix updates.

Since minor versions of CentOS are point in time releases of a major branch, starting with CentOS Linux 7, CentOS Linux uses a date code as the minor version. As an example, `CentOS Linux 7 (1406)` means June 2014 and `CentOS Linux 7 (1503)` means March 2015. For releases before CentOS 7 - minor versions are incremental (6.0, 6.1, 6.2, etc.).

CentOS Stream only has major versions, no minor versions.

The project has [announced](https://blog.centos.org/2020/12/future-is-centos-stream/) that work on CentOS Linux 8 will cease at the end of 2021.
