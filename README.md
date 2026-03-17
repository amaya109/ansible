# Ansible 安装指南

适用于 Ubuntu、CentOS、macOS 的安装说明。

---

## Ubuntu

```bash
# 更新包索引
sudo apt update

# 安装 Ansible
sudo apt install -y ansible

# 安装 sshpass & git
sudo apt install -y sshpass git

# 验证安装
ansible --version
sshpass -V
git --version
```

---

## CentOS

```bash
# 安装 EPEL 源
sudo yum install -y epel-release

# 安装 Ansible
sudo yum install -y ansible

# 安装 sshpass & git
sudo yum install -y sshpass git

# 验证安装
ansible --version
sshpass -V
git --version
```

---

## macOS

```bash
# 安装 Homebrew（若未安装）
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 安装 Ansible
brew install ansible

# 安装 sshpass & git
brew install sshpass git

# 验证安装
ansible --version
sshpass -V
git -v
```

---

# 克隆Ansible git repo

```bash
# 删除/root/.ansible (如果已经存在)
/bin/rm -rf /root/.ansible

# 克隆Ansible git repo
git clone https://github.com/amaya109/ansible.git /root/.ansible

# 设置ansible配置文件变量
echo "export ANSIBLE_CONFIG=~/.ansible/ansible.cfg" >> /etc/profile
source /etc/profile
```
