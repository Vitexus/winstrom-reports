# winstrom-reports

Jasper Reports sources for Abra FlexiBee

QuickStart
----------

1. Clone this repo: https://github.com/Vitexus/winstrom-reports
1. Install https://community.jaspersoft.com/project/jaspersoft-studio/releases
1. Install FlexiBee client with JasperReport project support
1. Install Jasper compiler with FlexiBee support https://github.com/VitexSoftware/jaspercompiler

```shell
git clone https://github.com/Vitexus/winstrom-reports
sudo apt install lsb-release wget
echo "deb http://repo.vitexsoftware.cz $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/vitexsoftware.list
sudo wget -O /etc/apt/trusted.gpg.d/vitexsoftware.gpg http://repo.vitexsoftware.cz/keyring.gpg
sudo apt update
sudo apt install jaspercompiler flexibee-client
```

All tested on Debian 10 Buster

See Also: https://github.com/VitexSoftware/flexibee-dark-gui (Dark skin for FlexiBee Desktop client)
