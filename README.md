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
    cargo install bat
    source $HOME/.cargo/env
    cargo install bat
    ```



