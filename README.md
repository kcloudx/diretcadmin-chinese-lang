# diretcadmin-chinese-lang

## install
```bash

#### Install Git 
yum install -y git

#### clean old lang files 
rm -rf /usr/local/directadmin/data/skins/evolution/lang/zh_Han*
rm -rf /usr/local/directadmin/data/skins/evolution/lang/login-zh_Han*


#### Clone lang package 
cd /opt
[ -d "/opt/kcloudxda" ] && rm -rf /opt/kcloudxda
git clone https://github.com/kcloudx/diretcadmin-chinese-lang kcloudxda


##### Evolution 
\cp -Rp /opt/kcloudxda/evolution/lang/zh_Han* /usr/local/directadmin/data/skins/evolution/lang/
\cp -Rp /opt/kcloudxda/evolution/lang/login-zh_Han* /usr/local/directadmin/data/skins/evolution/lang/

#### Modify permission 
chown diradmin:diradmin -R /usr/local/directadmin/data/skins/evolution/

```
