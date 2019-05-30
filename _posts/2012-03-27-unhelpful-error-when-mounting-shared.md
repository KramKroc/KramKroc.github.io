---
title: Unhelpful error when mounting a shared folder in Oracle VM
published: true
categories:
  - Blog
tags:
- virtualbox
---

Today I devoted much too much time to trying to figure out why I couldn't mount a shared directory on my Oracle VM. The error being returned from the mount command was:

```terminal
/sbin/mount.vboxsf: mounting failed with the error: Protocol error
```

It turned out that the reason this was occurring was because I had used the wrong name for the shared folder, I used a lower case name of the shared folder directory instead of the mixed case one. So the successful command ended up looking like the following:

```terminal
mount -t vboxsf Documents /home/user/documents
```

FYI: my host system is Ubuntu 11.10 and the guest OS was Centos