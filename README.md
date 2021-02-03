# winstrom-reports

Jasper Reports sources for Abra FlexiBee 

https://www.flexibee.eu/podpora/dokumentace/napoveda/uzivatelske_reporty/

QuickStart
----------

1. Install https://community.jaspersoft.com/project/jaspersoft-studio/releases
1. Install FlexiBee client with JasperReport project support https://github.com/Vitexus/flexibee-client-deb
1. Install FlexiBee Tools with Jasper Compiler & Uploader https://github.com/VitexSoftware/AbraFlexi-Report-Tools
1. Clone this repo: https://github.com/Vitexus/winstrom-reports
1. Open repo as project in jasperstudio & edit & save
1. upload your report to FlexiBee server using  **upreport** command


Classpath
---------

Anytime you can run **updatejasperclasspath** tool to update .classpath files to use current FlexiBee jars.
(It search all .classpath files in home directory that contain /usr/share/flexibee/lib/winstrom-*)

```terminal
vitex@exiv:~$ /usr/share/flexibee/bin/updatejasperclasspath
Updating jasper studio classpaths to use FlexiBee 2020.2.1.2
updating /home/vitex/Projects/VitexSoftware/FlexiBee/winstrom-reports/.classpath
updating /home/vitex/Projects/VitexSoftware/FlexiBee/CustomReports/CustomFlexiBeeReports/.classpath
updating /home/vitex/Projects/VitexSoftware/FlexiBee/CustomReports/MyReports/.classpath
updating /home/vitex/Projects/aacuk/MyReports/.classpath
```


Copy & Paste
------------

Installation commands on Debian

```shell
sudo apt install lsb-release wget
echo "deb http://repo.vitexsoftware.cz $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/vitexsoftware.list
echo "deb http://repo.vitexsoftware.cz 3thparty main" | sudo tee -a /etc/apt/sources.list.d/vitexsoftware.list
sudo wget -O /etc/apt/trusted.gpg.d/vitexsoftware.gpg http://repo.vitexsoftware.cz/keyring.gpg
sudo apt update
sudo apt install git flexibee-tools flexibee-client jaspersoftstudio
```
And finally clone the source files
```
git clone https://github.com/Vitexus/winstrom-reports
/usr/share/flexibee/bin/updatejasperclasspath
```

All tested on Debian 10 Buster

See Also: https://github.com/VitexSoftware/flexibee-dark-gui (Dark skin for FlexiBee Desktop client)
