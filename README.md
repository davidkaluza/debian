# Debian Linux Toys

change font size in tty

    dpkg-reconfigure console-setup

rsync

    apt-get install rsync

create /etc/rsyncd.conf

    echo -e "motd file = /etc/rsyncd.motd
    log file = /var/log/rsyncd.log
    pid file = /var/run/rsyncd.pid
    lock file = /var/run/rsync.lock
    
    [my_path]
       path = /opt/rsync
       comment = My Rsync Server
       read only = no
       list = yes
       secrets file = /etc/rsyncd.secret
       " > rsyncd.conf
