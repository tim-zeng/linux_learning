## linux学习文档





### vim实例测试



> 实例一：行号显示(:set nu)



![](\linux学习文件\linux学习image\vim\实例一\行号显示.png)



> 实例二：光标移到到指定位置12列20行(12G20->)，gg到第一行第一列，G到最后一列



![image-20201123112744805](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例二\移动光标2.png)



![image-20201123112744805](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例二\移动光标2.png)



![image-20201123112823910](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例二\移动光标3.png)



> 实例三：复制8-12行到最后一行粘贴（8G ，4yy，G，p）复制到了54-57行



![image-20201123113117759](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例三\复制粘贴.png)



> 实例四：将实例三复制的四行删除两行（54G，2dd）



![image-20201123113414402](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例四\删除.png)



> 实例五：将4行-14行的teat换成TEAT（：4，14s/teat/TEAT/gc）



![image-20201123113726414](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例五\替换.png)



> 实例六：在第一行插入“vim测试完成”（gg，O，插入vim测试完成，Esc）



![image-20201123114152695](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\vim\实例六\插入.png)



### tar测试实例



> 实例一：利用tar打包gzip压缩文件，并显示程式运作时间，保留文件原权限（time tar -zpcv -f vitest.tar.gz vitest.txt）



![image-20201123135740947](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例一\gzip.png)



> 实例二：利用tar打包bzip2压缩，并显示程式运作时间，保留文件原权限（time tar -jpcv -f vitest.tar.bz2 vitest.txt）



![image-20201123140421962](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例二\bzip2.png)



> 实例三：利用tar打包xz压缩，并显示程式运作时间，保留文件原权限（time tar -Jpcv -f vitest.tar.xz vitest.txt）



![image-20201123140558547](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例三\xz.png)



> 实例四：查阅tar档案资料内容（tar -jtv -f vitest.tar.gz）



![image-20201123140923441](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例四\tar查阅.png)



> 实例五：解压缩到指定目录（tar -jxv -f vitest.tar.bz2 -C /tmp）



![image-20201123141429333](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例五\解压缩1.png)



![image-20201123141429333](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\tar\实例五\解压缩1.png)



### wc实例测试



> 实例一：计算文件Byte数（wc -c man_db.conf.txt）



![image-20201123142627793](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\wc\实例一\计算byte数.png)



> 实例二：计算文件字数（wc -w man_db.conf.txt）



![image-20201123142811979](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\wc\实例二\计算字数.png)



> 实例三：计算文件行数（wc -l man_db.conf.txt）



![image-20201123142934270](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\wc\实例三\计算行数.png)



> 实例四：计算文件行数，字数，byte数（wc man_db.conf.txt）



![image-20201123143108248](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\wc\实例四\行数字数byte数.png)



> 实例五：同时查看多个文件（wc txt1 txt2 ...）



![image-20201123143251034](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\wc\实例五\同时查看多文件.png)



### ss实例测试



> 实例一：显示tcp连接套接字信息（ss -t -a）



![image-20201123143810731](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例一\tcp套接字信息.png)



> 实例二：显示sockets摘要（ss -s）



![image-20201123143931946](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例二\sockets摘要.png)



> 实例三：列出所有打开的网络连接端口（ss -l）



![image-20201123144241414](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例三\列出网络端口.png)



> 实例四：查看进程使用的socket（ss -pl）



![image-20201123144504198](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例四\查看进程socket.png)



> 实例五：找到打开套接字/端口应用程序（ss -pl | grep kernel）



![image-20201123145248045](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例五\打开套接字应用程序.png)



> 实例六：显示所有UDP sockets（ss -u -a）



![image-20201123145358924](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ss\实例六\显示所有UDPsockets.png)



### lsof实例测试



> 实例一：列出打开文件存在的进程（lsof）



![image-20201123150526165](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\lsof\实例一\打开文件进程.png)



> 实例二：列出指定进程所打开的文件（lsof -c 进程名）



![image-20201123151032279](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\lsof\实例二\进程打开的文件.png)



> 实例三： 列出目录下被打开的文件（lsof +d 目录）



![image-20201123151322827](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\lsof\实例三\列出目录下打开的文件.png)



> 实例四： 列出GID号进程详情（lsof -g）



![image-20201123151603397](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\lsof\实例四\列出UID进程详情.png)



### ps实例测试



> 实例一：显示进程信息（ps -A）



![image-20201123152453299](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ps\实例一\显示进程信息.png)



> 实例二：显示root进程用户信息（ps -u root）



![image-20201123152926458](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ps\实例二\显示root进程用户信息.png)



> 实例三：显示所有进程信息，连同命令行（ps -ef）



![image-20201123153445831](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ps\实例三\所有进程信息.png)



> 实例四：ps进程记录行数（ps aux | wc -l）





![image-20201123160950279](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\ps\实例四\ps进程记录行数.png)



### top实例测试



> 实例一：显示进程信息（top）



![image-20201123162412865](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例一\显示进程信息.png)



> 实例二：显示完整命令（top -c）



![image-20201123162341748](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例二\显示完整命令.png)



> 实例三：以批处理模式显示程序信息（top -b）



![image-20201123162308006](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例三\以批处理模式.png)



> 实例四：以累积模式显示程序信息（top -s）



![image-20201123162208767](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例四\以累积模式.png)



> 实例五：设置信息更新次数（top -n 2）



![image-20201123162104808](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例五\设置更新次数.png)



> 实例六：设置信息更新时间（top -d 3）



![image-20201123162033581](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例六\设置更新时间.png)



> 实例七：显示指定的进程信息（top -p 3665）



![image-20201123161957059](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例七\显示指定进程.png)



> 实例八：显示更新十次后退出（top -n 10）



![image-20201123161444175](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\top\实例八\更新十次退出.png)



### awk实例测试



> 示例一：取出登入者的前五条信息第一列和第四列信息（last -n 5 | awk '{print $1 "\t" $4}'）



![image-20201123163319438](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\awk\实例一\取出信息.png)



> 示例二：取出登入者的前五条信息的信息栏总数（last -n 5 | awk '{print $1 "\t lines: " NR "\t columns: " NF}'）



![image-20201123163605230](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\awk\实例二\信息栏数.png)



> 示例三：在/etc/passwd 当中是以冒号":" 来作为栏位的分隔，查阅，第三栏小于10 以下的数据，并且仅列出帐号与第三栏（cat /etc/passwd | awk '{FS=":"} $3 < 10 {print $1 "\t " $3}' ）



![image-20201123164148203](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\awk\实例三\比较运算信息.png)



### sed实例测试



> 实例一：删除输出的内容（ nl /etc/passwd | sed '2,5d'）



![image-20201123170755684](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\sed\实例一\删除输出内容.png)



> 实例二：在第二行后(亦即是加在第三行)加上内容（ nl /etc/passwd | sed '2a drink tea'）



![image-20201123170925034](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\sed\实例二\加上内容.png)



> 实例三：以行为单位的取代与显示（nl /etc/passwd | sed '2,5c No 2-5 number'）



![image-20201123171228577](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\sed\实例三\取代行.png)



> 实例四：仅列出/etc/passwd档案内的第5-7行（ nl /etc/passwd | sed -n '5,7p'）



![image-20201123171859270](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\sed\实例四\列出指定行.png)



> 实例五：搜寻与取代功能（/sbin/ifconfig enp0s3 | grep inet | sed 's/^.*inet //g'）



![image-20201123172718786](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\sed\实例五\搜寻与取代.png)



### find实例测试



> 实例一：将过去系统上面24小时内有更动过内容(mtime)的档案列出（find / -mtime 0）



![image-20201123173332315](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例一\查找更动的内容.png)



> 实例二：寻找/etc底下的档案，如果档案日期比/etc/passwd新就列出（ find /etc -newer /etc/passwd）



![image-20201123173453945](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例二\查找更新的内容.png)



> 实例三：搜寻/home底下属于tim的档案（find /home -user tim）



![image-20201123173717479](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例三\查找用户内容.png)



> 实例四：搜寻系统中不属于任何人的档案（find / -nouser）



![image-20201123173858883](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例四\查找不属于任何人的档案.png)



> 实例五：找出档名为passwd这个档案（ find / -name passwd）



![image-20201123173954017](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例五\找出指定档案.png)



> 实例六：找出档名包含了passwd这个关键字的档案（find / -name "*passwd*"）



![image-20201123174047049](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例六\找出关键字档案.png)



> 实例七：找出/run目录下，档案类型为Socket的档名有哪些（find /run -type s）



![image-20201123174156332](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\find\实例七\根据类型找到目录下的档案.png)



### crontab实例测试



> 实例一:用tim的身份在每天的12:00发信给自己（crontab -e）



![image-20201123180201061](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\crontab\实例一\定期执行.png)



> 实例二:查询使用者目前的crontab 内容（crontab -l）



![image-20201123180320852](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\crontab\实例二\使用者目前的crontab内容.png)



> 实例三:查看/etc/crontab 的内容（cat /etc/crontab）



![image-20201123181038463](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\crontab\实例三\查看crontab.png)



> 实例四:查看/etc/cron.d 里面的内容（ls -l /etc/cron.d）



![image-20201123181204932](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\crontab\实例四\查看cron.d.png)



> 实例五：修改/etc/crontab（vim /etc/crontab）



![image-20201124140714639](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\crontab\实例五\修改资源分配.png)



### grep实例测试



> 实例一：grep查找指定字段（grep ‘...'）



![image-20201124101635857](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例一\字段查找.png)



> 实例二：查找关键字并显示行号和标出颜色（grep -n --color=auto 'man'）



![image-20201124101855095](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例二\显示行号与标出颜色.png)



> 实例三：反向搜寻（grep -vn 'man' man_db.conf.txt）



![image-20201124102126321](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例三\反向搜寻.png)



> 实例四：找出有数字的内容（ grep -n '[0-9]' man_db.conf.txt）



![image-20201124102743884](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例四\找出数字.png)



> 实例五：找出任意字元的内容（grep -n 'g..p' man_db.conf.txt）



![image-20201124103523487](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例五\任意字元.png)



> 实例六：限定连续RE 字符范围（grep -n 'p\\{2\\}' man_db.conf.txt）



![image-20201124104517993](C:\Users\tim.zeng\Desktop\linux学习文件\linux学习image\grep\实例六\限定字符.png)
