# Failed-to-download-metadata-for-repo-appstream-

Cara mengatasi error seperti:
- Failed to download metadata for repo 'appstream': Cannot prepare internal mirrorlist: No URLs in mirrorlist
- Failed to download metadata for repo 'appstream'

YANG SAYA LAKUKAN DI CENTOS 8.

<ol>
<li>cd /etc/yum.repos.d/</li>
<li>sudo sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*</li>
<li>sudo sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*</li>
<li>sudo yum update -y</li>

<li>cd /etc/yum.repos.d/</li>
<li>sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*</li>
<li>sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*</li>
  <li>yum -y install java</li>
</ol>
SEMOGA BERHASIL
