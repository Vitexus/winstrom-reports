# winstrom-reports

Jasper Reports sources for Abra Flexi 

[https://www.flexibee.eu/podpora/dokumentace/napoveda/uzivatelske_reporty/](https://podpora.flexibee.eu/cs/articles/4553831-uzivatelske-reporty)

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


And finally clone the source files
```
git clone https://github.com/Vitexus/winstrom-reports
/usr/share/flexibee/bin/updatejasperclasspath
```

See Also: https://github.com/VitexSoftware/flexibee-dark-gui (Dark skin for FlexiBee Desktop client)
