---
title: MISP 2.4.137 released (New exclusion module for the correlation engine, many improvements and security vulnerabilities resolved)
date: 2021-01-20
layout: post
banner: /img/blog/galaxy2.0/1.jpeg
---

# MISP 2.4.137 released

We have released 2.4.137, a security and bug fix release including a collection of fixes and improvements collected over the past month.

Building tools for the security community sure has its perks - over the past week we have received two independent security test results of two separate organisations, revealing several vulnerabilities. The update to this version is therefore highly recommended.

A little note on vulnerability - we [always welcome organisations helping us secure MISP](/security/) and our tooling in general and would hereby like to thank everyone taking part in the process!

# Several vulnerabilities resolved

- [CVE-2021-25324] Stored XSS via the galaxy cluster view - Discovered by Daniel Kubica of ESET, spol. s r.o.
- [CVE-2021-25325] Stored XSS via the galaxy element index - Discovered by Daniel Kubica of ESET, spol. s r.o.
- [CVE-2021-25323] Weak default password change request policy not requiring the entry of the current password - Discovered by Daniel Kubica of ESET, spol. s r.o.
- [CVE-2021-3184] Reflected XSS via the set homepage button - Reported by an anonymous party

# A long list of quality of life improvements

- The synchronisation now compresses the data exchanged, improving the transfer rates during the exchange
- Additional metrics and comparison tools for the sync connections
- Better management of API key usage along with logging
- A new tool that allows the exclusion of certain values from the correlation engine (useful to avoid having regularly observed values recurring in a large number of events generating too much noise)

Along with many other fixes. A special thank you to @JakubOnderka for providing a steady stream of QoL improvements, making MISP more pleasant to use by the day!

# Acknowledgement

We would like to thank all the [contributors](/contributors), reporters and users who have helped us in the past months to improve MISP and information sharing at large. This release includes multiple updates in [misp-objects](/objects.html), [misp-taxonomies](/taxonomies.html) and [misp-galaxy](/galaxy.html)
.

As always, a detailed and [complete changelog is available](/Changelog.txt) with all the fixes, changes and improvements.

