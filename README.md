## nginx-proxy
Compiling nginx for reverse proxy
## note: on RHEL9 (centos9, Rocky 9)
Cần cài epel & remi repository để  cài được  GeoIP GeoIP-devel
### First, upgrade the system OS - need root permission.
`sudo dnf upgrade --refresh`
### activated the Code Ready Builder (CRB)
`sudo dnf config-manager --set-enabled crb`
### Import Epel & remi repository - these repo support GeoIP GeoIP-devel which removed from base repository by default on RHEL 9
`sudo dnf install \`
    `https://dl.fedoraproject.org/pub/epel/epel-release-latest-9.noarch.rpm \`
    `https://dl.fedoraproject.org/pub/epel/epel-next-release-latest-9.noarch.rpm`
`sudo dnf install dnf-utils http://rpms.remirepo.net/enterprise/remi-release-9.rpm -y`

