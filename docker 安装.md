

   10  wget -O /etc/yum.repos.d/docker-ce.repo https://download.docker.com/linux/centos/docker-ce.repo
   11  curl -o /etc/yum.repos.d/docker-ce.repo https://download.docker.com/linux/centos/docker-ce.repo
   12  ll /etc/yum.repos.d/docker-ce.repo 
   13  sudo sed -i 's+download.docker.com+mirrors.cloud.tencent.com/docker-ce+' /etc/yum.repos.d/docker-ce.repo

 yum makecache fast
 yum install docker-ce

 systemctl start docker.service

```

https://newsn.net/say/docker-install-centos-yum-2.html
https://www.cnblogs.com/zsql/p/11078304.html
https://blog.csdn.net/qq_42329675/article/details/102667315
https://www.cnblogs.com/520playboy/p/7910357.html
https://www.cnblogs.com/zzdylan/p/9930144.html
https://www.csdcb.cn/article/category/docker.html
```

```bash
yum list docker-ce --showduplicates | sort -r
```







 docker run --rm --privileged -v /var/run/docker.sock:/var/run/docker.sock -v /var/lib/rancher:/var/lib/rancher rancher/agent:v1.2.6 http://192.168.1.250:9090/v1/scripts/DE8176A746E03536AE56:1546214400000:N43qfw4dnD1FclFJD9PPbRIamJc


 docker run --rm --privileged -v /var/run/docker.sock:/var/run/docker.sock -v /var/lib/rancher:/var/lib/rancher rancher/agent:v1.2.6 http://192.168.1.250:9090/v1/scripts/DE8176A746E03536AE56:1546214400000:N43qfw4dnD1FclFJD9PPbRIamJc




https://www.cnblogs.com/mybxy/p/10576399.html
https://www.cnblogs.com/whgfu/articles/9466859.html
https://www.jianshu.com/p/405fe33b9032

   64  cat <<EOF /etc/yum.repos.d/kubernetes.repo
   65  [kubernetes]
   66  name=Kubernetes
   67  baseurl=https://mirrors.aliyun.com/kubernetes/yum/repos/kubernetes-el7-x86_64/
   68  enabled=1
   69  gpgcheck=1
   70  repo_gpgcheck=1
   71  gpgkey=https://mirrors.aliyun.com/kubernetes/yum/doc/yum-key.gpg https://mirrors.aliyun.com/kubernetes/yum/doc/rpm-package-key.gpg
   72  EOF



   73  setenforce 0

   74  yum install -y kubelet kubeadm kubectl
   75  history
   76  yum install -y kubelet kubeadm kubectl
   77  sed -i 's+download.docker.com+mirrors.cloud.tencent.com/docker-ce+' /etc/yum.repos.d/docker-ce.repo
   78  less /etc/yum.repos.d/docker-ce.repo 

swapoff -a

docker pull mirrorgooglecontainers/pause:3.1

docker pull registry.aliyuncs.com/google_containers/kube-apiserver:v1.17.3 



   84  sed -i 's/.*swap.*/#&/' /etc/fstab

   86  wget https://dl.k8s.io/v1.16.2/kubernetes-server-linux-amd64.tar.gz
   88  wget https://dl.k8s.io/v1.16.2/kubernetes-server-linux-amd64.tar.gz


yum install ntpdate -y
ntpdate ntp1.aliyun.com


timedatectl set-timezone Asia/Shanghai
 timedatectl status|grep 'Time zone'
 yum -y install rdate
rdate -s time-b.nist.gov

 systemctl start docker
 systemctl enable docker

less /etc/docker/daemon.json 

{
"registry-mirrors": ["https://docker.mirrors.ustc.edu.cn"],
"insecure-registries": ["192.168.1.244:5000"]
}









 docker run -d --name click --ulimit nofile=262144:262144 yandex/clickhouse-server 





# [docker 安装clickhouse server]

https://www.cnblogs.com/ronnieyuan/p/12580729.html

https://blog.csdn.net/lcl_xiaowugui/article/details/104724726/

https://www.jianshu.com/p/362252f2284b

https://www.cnblogs.com/tochw/p/14407790.html











openeuler

https://repo.openeuler.org/openEuler-20.03-LTS/ISO/x86_64/

https://blog.csdn.net/frdevolcqzyxynjds/article/details/105648163





https://my.oschina.net/mengyoufengyu/blog/3166273

https://www.cnblogs.com/soldier-cnblogs/p/13069175.html

源

https://mirrors.huaweicloud.com/home

https://support.huaweicloud.com/instg-kunpengcpfs/kunpengdocker_03_0004.html









centos8 ip

https://www.cnblogs.com/hunttown/p/14761630.html

https://www.cnblogs.com/liuhedong/p/10695969.html





docker arm64

https://download.docker.com/linux/centos/8/aarch64/stable/Packages/



k8s

https://www.bboy.app/2021/02/23/%E5%8D%87%E7%BA%A7%E5%AE%B6%E4%B8%AD%E7%9A%84k8s%E9%9B%86%E7%BE%A4/





loki日志

https://www.cnblogs.com/sanduzxcvbnm/p/14234480.html

http://t.zoukankan.com/fengjian2016-p-13356125.html

https://javazhiyin.blog.csdn.net/article/details/106846335









mycat

https://www.bilibili.com/video/av90941982/

http://www.zuidaima.com/blog/4063043883584512.htm

https://www.cnblogs.com/longsanshi/p/8440463.html

https://zhuanlan.zhihu.com/p/54386055

https://blog.csdn.net/weixin_40838333/article/details/100187320   重点