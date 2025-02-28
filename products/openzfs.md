---
permalink: /openzfs
alternate_urls:
  - /zfs
layout: post
title: OpenZFS
category: app
command: zpool get version [zpool name]
link: https://github.com/openzfs/zfs/blob/master/RELEASES.md
changelogTemplate: |
  https://github.com/openzfs/zfs/releases/tag/zfs-__LATEST__
releaseDateColumn: true
sortReleasesBy: 'releaseCycle'
iconSlug: "NA"
eolColumn: Critical bug fixes
releases:

    - releaseCycle: "OpenZFS 2.1"
      release: 2021-07-02
      eol: 2023-07-02
      lts: true
      latest: "2.1.2"

    - releaseCycle: "OpenZFS 2.0"
      release: 2020-11-30
      eol: false
      latest: "2.0.7"

    - releaseCycle: "OpenZFS 0.8"
      release: 2019-06-23
      eol: 2020-12-14
      latest: "0.8.6"
---

> [OpenZFS](https://openzfs.github.io/openzfs-docs/) is an open-source storage platform that encompasses the functionality of traditional filesystems and volume manager. It includes protection against data corruption, support for high storage capacities, efficient data compression, snapshots and copy-on-write clones, continuous integrity checking and automatic repair, encryption, remote replication with ZFS send and receive, and RAID-Z. Linux and FreeBSD are officially supported, [with plans to support macOS in the future](https://github.com/openzfs/zfs/pull/12110).  

## Release branches

- **OpenZFS LTS** - A designated MAJOR.MINOR release with periodic PATCH releases that incorporate important changes backported from newer OpenZFS releases. This branch is intended for use by distributions which use an LTS, enterprise, or similarly managed kernel (RHEL, Ubuntu LTS, Debian). Minor changes to support these distribution kernels will be applied as needed. New kernel versions released after the OpenZFS LTS release are not supported unless there is not a newer current release. LTS releases will receive patches for at least 2 years. 

- **OpenZFS current** - Tracks the newest MAJOR.MINOR release. This branch includes support for the latest OpenZFS features and recently releases kernels. When a new MINOR release is tagged the previous MINOR release will no longer be maintained (unless it is an LTS release). New MINOR releases are planned to occur roughly annually.

## Officially supported distributions: 

- [Fedora](https://openzfs.github.io/openzfs-docs/Getting%20Started/Fedora/index.html)
- [RHEL-based distributions](https://openzfs.github.io/openzfs-docs/Getting%20Started/RHEL-based%20distro/index.html)
- [FreeBSD](https://openzfs.github.io/openzfs-docs/Getting%20Started/FreeBSD.html)

These distributions have repositories provided directly by the OpenZFS community, while other distributions likely will work, they are not frequently tested and may exhibit issues, especially Ubuntu due to their HWE kernel pulling in patches from newer kernels and still claiming the kernel is from an older branch. [Ubuntu is not supported by OpenZFS](https://github.com/openzfs/zfs/issues/10333).

[Every Linux release][zol] includes a range of supported kernels. Point releases are tagged as needed in order to support the stable kernel available from kernel.org.

[zol]: https://zfsonlinux.org/ "ZFS On Linux"
