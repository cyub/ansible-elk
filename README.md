## ansible role for elk stack

ansible是python语言开发的配置管理工具。这里是使用ansible自动部署elk脚本。

### 安装ansible

使用python包管理工具pip安装ansible

```
sudo pip install ansible
```

### 配置Inventory文件

将服务器your_host_for_elk添加到inventory中

```
# 文件位置：/etc/ansible/hosts
[elk]
your_host_for_elk ansible_ssh_user=root ansible_python_interpreter=/usr/bin/python3
```
### 执行playbook

```
ansible-playbook  site.yml
```

### 日志收集分析系统架构图

![elk](https://www.plantuml.com/plantuml/png/0/ZLAnQiCm4Dtr5OVt3B7t4kYNABOS2yjMaUIfP6jBA1GwX9f0SUbGo9GCXNJma9-fxUGlgZYsOyUXH8FGlQTxT--aaLHOg2XWIFeqlCC21n3maDkUu0419IA2N0qICFBuAzl6sUmfJrwBxxH8F_9aaoSF1jmZn8YhG74GTE8fSAWWjg8yH0ZqgWNUNxBdpson71vIe5es5WuOkzLs7w-E9Omkvr96nWGhmB8v3yihqyloPbz-Fr_irkkhvSt_vAs-VFQu-KtVhfQtQlaBastAr5LA5K4SAilmbl780SByyoOOd-Ytb5uN9GnBHMr9iB3FA9-ESOYhLgO8sueBAERBVFQ3KFiz1eERqzpRasmH9chFe4LOgCdLwD57azH3h0OfTnqrjkg3nhgcEf5cArz79wTuH497__C_)