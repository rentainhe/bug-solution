## 挖矿debug

#### 1. Change to Root

```bash
$ sudo su root
```

- ctrl + d，切换回个人账号

(可选)

```bash
$ netstat -napt
```

监听网络端口，查看进程号，如果没发现，去proc目录

```bash
$ cd /proc
```

查看当前目录的python进程

```bash
$ find . -name python
```

kill对应进程号

#### 2. Optional

查看是哪个账号登录挖矿系统

```bash
$ systemctl status 进程号
```

```bash
$ cd /home/user/miniconda3/envs
$ cd /home/use/miniconda3/bin
$ ll -rt # 查看是否有root权限创建的文件，有的话删除
```

查看定时任务

```bash
$ crontab -l
```

删除定时任务

```bash
$ crontab -r
```



