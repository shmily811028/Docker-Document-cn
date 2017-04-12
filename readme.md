#docker 命令注释

###Options:

	--api-cors-header=                   在远程API设置CORS的标题
	-b, --bridge=                        将容器桥接
	--bip=                               制定桥接IP
	-D, --debug=false                    启用调试模式
	-d, --daemon=false                   启用守护进程模式
	--default-gateway=                   容器默认网关IPv4地址
	--default-gateway-v6=                容器默认网关IPv6地址
	--default-ulimit=[]                  设置默认的容器ulimit
	--dns=[]                             使用DNS服务器
	--dns-search=[]                      DNS搜索域使用
	-e, --exec-driver=native             使用的驱动程序
	--exec-opt=[]                        设置驱动程序选项
	--exec-root=/var/run/docker          Root of the Docker execdriver
	--fixed-cidr=                        固定IP的IPv4子网
	--fixed-cidr-v6=                     固定IP的IPv6子网
	-G, --group=docker                   UNIX套接字组
	-g, --graph=/var/lib/docker          Root of the Docker runtime
	-H, --host=[]                        守护程序套接字(s)连接到
	-h, --help=false                     打印使用情况
	--icc=true                           启用容器间通信
	--insecure-registry=[]               启用不安全的注册表通信
	--ip=0.0.0.0                         绑定容器端口时的默认IP
	--ip-forward=true                    使用 net.ipv4.ip_forward
	--ip-masq=true                       启用IP伪装
	--iptables=true                      使iptables规则添加
	--ipv6=false                         使IPv6网络
	-l, --log-level=info                 设置日志级别
	--label=[]                           设置 key=value标签的守护进程
	--log-driver=json-file               容器日志的默认驱动程序
	--log-opt=map[]                      设置日志驱动选项
	--mtu=0                              设置容器网络MTU
	-p, --pidfile=/var/run/docker.pid    用于守护进程PID文件的路径
	--registry-mirror=[]                 首选Docker注册表镜像
	-s, --storage-driver=                存储驱动程序使用
	--selinux-enabled=false              启用SELinux支持
	--storage-opt=[]                     设置存储驱动选项
	--tls=false                          使用 TLS; implied by --tlsverify
	--tlscacert=~/.docker/ca.pem         只信任CA证书
	--tlscert=~/.docker/cert.pem         TLS证书文件
	--tlskey=~/.docker/key.pem           TLS密钥文件
	--tlsverify=false                    使用TLS并验证远程
	--userland-proxy=true                使用用户代理为环回流量
	-v, --version=false                  打印版本信息并退出				

###Commands:
	attach    连接到正在运行的容器
	build     从Dockerfile制作镜像
	commit    将一个容器的变化创建为新的镜像
	cp        将文件/文件夹从容器的文件系统复制到主路径
	create    创建新容器
	diff      检查容器文件系统的更改
	events    从服务器获取实时事件
	exec      在运行容器中运行命令
	export    将容器内容保存为tar压缩包
	history   显示一个镜像的历史
	images    镜像列表
	import    从一个压缩包创建一个新的镜像
	info      显示整个系统的信息
	inspect   返回一个容器或镜像的底层信息
	kill      停止正在运行的容器
	load      从一个压缩包加载一个镜像
	login     在docker服务器中登录
	logout    在docker服务器中登出
	logs      取出容器的日志
	pause     暂停容器内的所有进程
	port      查看NAT-ed 至 PRIVATE_PORT的公开端口
	ps        容器列表
	pull      从docker服务器中pull下来一个镜像或者容器
	push      将一个镜像或者容器push到docker服务器
	rename    重命名现有容器
	restart   重新启动正在运行的容器
	rm        删除一个或多个容器
	rmi       删除一个或多个镜像
	run       运行一个命令在一个新的容器
	save      保存镜像到TAR压缩包
	search    搜索Docker Hub中的镜像
	start     启动一个停止的容器
	stats     显示一连串的容器的资源使用情况统计数据
	stop      停止正在运行的容器
	tag       将图像标记到存储库中
	top       查找容器的运行进程
	unpause   恢复暂停的容器
	version   显示docker的版本信息
	wait      阻塞,直到一个容器停止,然后打印它的退出代码

##### Run 'docker COMMAND --help' for more information on a command.


###run以下命令

	-a, --attach=[]             附着在STDIN、STDOUT和STDERR
	--add-host=[]               添加一个自定义host-to-IP映射 (host:ip)
	--blkio-weight=0            阻塞IO ( 相对权重), 10至1000之间
	-c, --cpu-shares=0          CPU 分配(相对权重 )
	--cap-add=[]                添加Linux功能
	--cap-drop=[]               删除 Linux 功能
	--cgroup-parent=            可选的 cgroup 容器
	--cidfile=                  将容器ID写入文件
	--cpu-period=0              限制 CPU CFS (完全公平调度器) 周期
	--cpu-quota=0               限制 CPU CFS 配额
	--cpuset-cpus=              使用CPU数量? (0-3, 0,1)
	--cpuset-mems=              允许使用内存量? (0-3, 0,1)
	-d, --detach=false          在后台运行容器并打印容器ID
	--device=[]                 在容器中添加有一个主机
	--dns=[]                    设置自定义DNS服务器
	--dns-search=[]             设置自定义DNS搜索域
	-e, --env=[]                设置环境变量
	--entrypoint=               重写默认镜像入口
	--env-file=[]               读入一个文件的环境变量
	--expose=[]                 暴露一个端口或一系列端口
	-h, --hostname=             容器主机名
	--help=false                打印用法?
	-i, --interactive=false     保持输入打开即使不连接
	--ipc=                      IPC 命名空间的使用
	-l, --label=[]              在容器上设置元数据
	--label-file=[]             读入一行分隔文件的标签?
	--link=[]                   添加链接到另一个容器
	--log-driver=               容器驱动日志
	--log-opt=[]                日志驱动器选项
	--lxc-conf=[]               添加自定义LXC选项
	-m, --memory=               内存限制
	--mac-address=              容器Mac地址 (e.g. 92:d0:c6:0a:29:33)
	--memory-swap=              总内存 (memory + swap), '-1' 禁用掉?
	--name=                     给容器分配名称
	--net=bridge                设置容器的网络模式
	--oom-kill-disable=false    禁用OOM Killer
	-P, --publish-all=false     将所有暴露端口发布到随机端口
	-p, --publish=[]            向主机发布容器的端口
	--pid=                      命名空间使用的PID
	--privileged=false          给这个容器扩展权限
	--read-only=false           将容器的根文件系统挂载为只读
	--restart=no                当容器退出时重新应用策略
	--rm=false                  退出时自动删除容器
	--security-opt=[]           安全选项
	--sig-proxy=true            代理接收到进程的信号
	-t, --tty=false             分配一个伪tty
	-u, --user=                 命名空间或 UID (format: <name|uid>[:<group|gid>])
	--ulimit=[]                 Ulimit 选项
	--uts=                      命名空间使用的UTS
	-v, --volume=[]             绑定挂载卷
	--volumes-from=[]           从指定容器装入卷(s)
	-w, --workdir=              容器内的工作目录














