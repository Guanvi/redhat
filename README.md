# redhat
- 隐藏下边任务栏

    `mv /usr/share/gnome-shell/extensions/window-list@gnome-shell-extensions.gcampax.github.com \
    /usr/share/gnome-shell/extensions/window-list@gnome-shell-extensions.gcampax.github.com.back`
    
    
    
- 下载必备包
    `scp -r redhat@47.106.129.114:~/redhat ./`

- 安装git2.9.5所需包
    ```
    yum install curl-devel expat-devel gettext-devel openssl-devel zlib-devel
    yum install gcc perl-ExtUtils-MakeMaker
    ```
    
    
- 交换左Control和Caps Lock键
    `setxkbmap -option ctrl:swapcaps`
    
- 将caps lock键改为ctrl键
    `setxkbmap -option ctrl:nocaps`
    
    
- 安装rust及bat
    
    ```
    curl https://sh.rustup.rs -sSf | sh
    source $HOME/.cargo/env
    cargo install bat
    ```

- vultr使用BBR加速上网

     ```
     wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh
     chmod 700 bbr.sh
     ./bbr.sh
     重启服务器，输入 lsmod | grep bbr 如果看到 tcp_bbr 就说明 BBR 已经启动了。
     ```


