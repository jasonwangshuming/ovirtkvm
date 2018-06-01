# ovirtkvm
redhat ovirt manager install
###############################################################
### ovirtengine install
install the centos7 minon
yum install -y epel-release
yum install http://resources.ovirt.org/pub/yum-repo/ovirt-release42.rpm -y
reboot
yum install yum-plugin-priorities 
设置资源库优先级
vi CentOS-Base.repo
priority=1
yum clean all
yum makcecache

yum install ovirt-engine -y

