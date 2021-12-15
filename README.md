# diretcadmin-chinese-lang

## 安装方式
```bash

#### Install Git / 安装 GIT
yum install -y git

#### clean old lang files / 删除旧的文件
rm -rf /usr/local/directadmin/data/skins/enhanced/lang/cn
rm -rf /usr/local/directadmin/data/skins/evolution/lang/zh_Han*
rm -rf /usr/local/directadmin/data/skins/evolution/lang/login-zh_Han*
rm -rf /usr/local/directadmin/data/skins/evolution/lang/zh_Han*


#### Clone lang package / 克隆我们的语言包
cd /opt
[ -d "/opt/kcloudxda" ] && rm -rf /opt/kcloudxda
git clone https://github.com/kcloudx/diretcadmin-chinese-lang kcloudxda


##### Evolution / 风格中文语言包
cp -Rp /opt/kcloudxda/evolution/lang/zh_Hans.* /usr/local/directadmin/data/skins/evolution/lang/
cp -Rp /opt/kcloudxda/evolution/lang/login-zh_Hans.* /usr/local/directadmin/data/skins/evolution/lang/
cp -Rp /opt/kcloudxda/evolution/lang/zh_Hans /usr/local/directadmin/data/skins/evolution/lang/

cp -Rp /opt/kcloudxda/evolution/lang/zh_Hant.* /usr/local/directadmin/data/skins/evolution/lang/
cp -Rp /opt/kcloudxda/evolution/lang/login-zh_Hant.* /usr/local/directadmin/data/skins/evolution/lang/
cp -Rp /opt/kcloudxda/evolution/lang/zh_Hant /usr/local/directadmin/data/skins/evolution/lang/
#### Modify permission / 修改文件权限
chown diradmin:diradmin -R /usr/local/directadmin/data/skins/evolution/

```
