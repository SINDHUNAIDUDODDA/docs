---
title: Security
weight: 7505
---

<table width="100%">
<tr style="vertical-align: top;">
<td width="30%" style="border: none;">
<h4>Security policy</h4>
<p style="padding: 8px">Rancher Labs supports responsible disclosure, and endeavours to resolve all issues in a reasonable time frame. </p>
</td>
<td width="30%" style="border: none;">
<h4>Reporting process</h4>
<p style="padding: 8px">Please submit possible security issues by emailing <a href="mailto:security@rancher.com">security@rancher.com</a></p>
</td>
<td width="30%" style="border: none;">
<h4>Announcments</h4>
<p style="padding: 8px">Subscribe to the <a href="https://forums.rancher.com/c/announcements">Rancher announcements forum</a> for release updates.</p>
</td>
</tr>
</table>

### Rancher Vulnerabilities

| ID | Description | Date | Resolution |
|----|-------------|------|------------|
| [CVE-2018-20321](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2018-20321) |  Any project member with access to the `default` namespace can mount the `netes-default` service account in a pod and then use that pod to execute administrative privileged commands against the Kubernetes cluster.  | 29 Jan 2019 | [Rancher v2.1.6](https://github.com/rancher/rancher/releases/tag/v2.1.6) and [Rancher v2.0.11](https://github.com/rancher/rancher/releases/tag/v2.0.11) - Rolling back from these versions or greater have specific [instructions]({{< baseurl >}}/rancher/v2.x/en/upgrades/rollbacks/).  |
| [CVE-2019-6287](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-6287) | Project members continue to get access to namespaces from projects that they were removed from if they were added to more than one project. | 29 Jan 2019  |  [Rancher v2.1.6](https://github.com/rancher/rancher/releases/tag/v2.1.6) and [Rancher v2.0.11](https://github.com/rancher/rancher/releases/tag/v2.0.11)  |
| [CVE-2019-11202](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-11202) | The default admin, that is shipped with Rancher, will be re-created upon restart of Rancher despite being explicitly deleted. | 16 Apr 2019  |  [Rancher v2.2.2](https://github.com/rancher/rancher/releases/tag/v2.2.2), [Rancher v2.1.9](https://github.com/rancher/rancher/releases/tag/v2.1.9) and [Rancher v2.0.14](https://github.com/rancher/rancher/releases/tag/v2.0.14)  |
| [CVE-2019-12274](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-12274) | Nodes using the built-in node drivers using a file path option allows the machine to read arbitrary files including sensitive ones from inside the Rancher server container. | 5 Jun 2019  |  [Rancher v2.2.4](https://github.com/rancher/rancher/releases/tag/v2.2.4), [Rancher v2.1.10](https://github.com/rancher/rancher/releases/tag/v2.1.10) and [Rancher v2.0.15](https://github.com/rancher/rancher/releases/tag/v2.0.15)  |
| [CVE-2019-12303](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-12303) |  Project owners can inject extra fluentd logging configurations that makes it possible to read files or execute arbitrary commands inside the fluentd container. Reported by Tyler Welton from Untamed Theory. | 5 Jun 2019  |  [Rancher v2.2.4](https://github.com/rancher/rancher/releases/tag/v2.2.4), [Rancher v2.1.10](https://github.com/rancher/rancher/releases/tag/v2.1.10) and [Rancher v2.0.15](https://github.com/rancher/rancher/releases/tag/v2.0.15)   |
