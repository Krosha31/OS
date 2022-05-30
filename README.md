# 
       
    1. a)lscpu, cat /proc/cpuinfo
       b)
       I) lscpu | grep “Model name”
       II) lscpu |grep -E "Core|Thread"
       III) lscpu |grep -E "CPU max|CPU min"
       IV)lscpu |grep -wE "L1d|L1i|L2|L3"
       V)lscpu |grep "Architecture"
    2. RAM(Random Access Memory) – оперативная память компьютера. Та память, которую использует компьютер по ходу работы. В ней хранятся данные открытых процессов
       Swap – место на жестком диске, которое отводится под те же цели, что и для оперативной памяти. Используется при заполнении оперативной памяти
    3. free
    4. sudo swapoff -a
       sudo dd if=/dev/zero of=/swapfile bs=1G count=10 status=progress
       sudo chmod 600 /swapfile
       sudo mkswap /swapfile
       sudo swapon /swapfile
    5. sudo dmidecode -t memory | grep -E "Manufacturer|Serial Number|Form Factor|Size"
    6. df -h
    7. df -h /home
    8. top
    9. glxinfo -B | grep "Device"
    10. ifconfig -a | grep inet
    11. ifconfig -a | grep ether
    12. ip adress| grep inet / ip address | grep ether
    13. ps -efH \ top
    14. export K=5
    15. export PATH=”/home/krosha:$PATH”
    16. apt-get upgrade
    17. -
    18. alias c=clear / gedit  ~/.bash_aliases
    19. Settings → Preferences → Unnamed → Colors
    20. --
    21. grep – утилита поиска по заданному регулярному выражению
       i) cat /proc/cpuinfo | grep "model name" | sort | uniq
       ii)grep "model" /proc/cpuinfo dop
       iii) grep -E "hey|buddy"  /proc/cpuinfo dop
    22. -i
    23. grep -w "You’ve got the wrong door"  dop
    24. grep -v "the leather club's two blocks down" dop
    25. ls /proc |grep info
    26. cat /proc/cpuinfo | grep -n "model name" | sort | uniq
    27. 
