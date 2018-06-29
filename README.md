# linux的常用命令

more -dc /etc/profile<br>              打开文件<br>
cksum file<br>                         查看文件大小<br>
ls -all<br>                            查看隐藏文件<br>
ls -a<br>                              显示隐藏文件<br>
tar zcvf FileName.tar.gz DirName<br>   压缩命令<br>
tar zxvf FileName.tar.gz<br>           解压命令<br>     

mv jdk1.7.0_80/ /usr/local/<br>        移动命令<br>
mv a.txt b.txt<br>                     将一个名为a.txt的文件重命名为b.txt<br>
mv A B<br>                             将目录A重命名为B<br>
mv a.txt /b/c.txt<br>                  将a.txt移动到/b下，并重命名为c.txt<br>

cp file /usr/men/tmp/file1<br>         将文件file复制到目录/usr/men/tmp下，并改名为file1<br>
cp -r /usr/men /usr/zh<br>             将目录/usr/men下的所有文件及其子目录复制到目录/usr/zh中<br>

查看进程
------

ps aux 是用BSD的格式来显示 java这个进程，显示的项目有：USER , PID , %CPU , %MEM , VSZ , RSS , TTY , STAT , START , TIME , COMMAND<br>
ps -ef 是用标准的格式显示java这个进程，显示的项目有：UID , PID , PPID , C , STIME , TTY , TIME , CMD<br>
参考资料：https://blog.csdn.net/a12345555555/article/details/72770789<br>

### pid进程编号和进程名字查询
pkill - 9 java<br>                    停止所有java进程命令<br>
kill -9 java进程序号<br>               根据java进程序号强制关闭进程<br>
ps -ef  | grep redis<br>              查看进程<br> 
ps -aux | grep redis<br>              看看进程<br>
ps -aux | grep pid<br>                根据进程pid查看<br>
### 端口和进程名字查询
netstat -antp<br>                     查看所有端口和服务<br> 
netstat -antp |grep port<br>          查看端口<br> 
netstat -antp |grep redis<br>         查看服务<br> 



搜索命令search
------
(1)find命令是根据文件的属性进行查找，如文件名，文件大小，所有者，所属组，是否为空，访问时间，修改时间等。<br>
(2)grep是根据文件的内容进行查找，会对文件的每一行按照给定的模式(patter)进行匹配查找。<br>


find / -name redis.conf <br> 　　        在根目录下查找文件redis.conf，表示在整个硬盘查找<br>
find / -name '*redis.conf*'<br>        使用通配符*,表示在/目录下查找文件名中含有字符<br>
参考资料：https://www.cnblogs.com/zhangmo/p/3571735.html

grep -rn "0.0.0.0" *<br>               在当前目录下，查找"0.0.0.0"字符串<br>
grep -rn man *<br>                     会匹配 ‘Batman’、‘manic’、‘man’等<br>
grep -rn '\<man' *<br>                 匹配‘manic’和‘man’，但不是‘Batman’<br>
grep -rn '\<man\>'<br>                 只匹配‘man’，而不是‘Batman’或‘manic’等其他的字符串<br>


vi命令
------
:wq<br>            保存文件并退出vi<br>
:wq!<br>           强制保存文件，并退出vi<br>
:q!<br>            不保存文件，强制退出vi<br>
:set number<br>    设置行号<br>
:set nonumber<br>  关闭行号显示<br>


