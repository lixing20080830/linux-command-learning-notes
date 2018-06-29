# linux的常用命令

kill -9 8142 强制关闭进程<br>
ps -ef  | grep zookeeper          查看进程<br> 
ps -aux | grep 'zookeeper'        看看进程<br>

cksum file                        查看文件大小<br>
ls -all                           查看隐藏文件<br>
ls -a                             显示隐藏文件<br>
tar zcvf FileName.tar.gz DirName  压缩命令<br>
tar zxvf FileName.tar.gz          解压命令<br>     

mv jdk1.7.0_80/ /usr/local/       移动命令<br>
mv abc.txt 1234.txt               将一个名为abc.txt的文件重命名为1234.txt<br>
mv A B                            将目录A重命名为B<br>
mv a.txt /b/c.txt                 将a.txt移动到/b下，并重命名为c.txt<br>

cp file /usr/men/tmp/file1        将文件file复制到目录/usr/men/tmp下，并改名为file1<br>
cp -r /usr/men /usr/zh            将目录/usr/men下的所有文件及其子目录复制到目录/usr/zh中<br>

grep -rn "hello,world!" *         在当前目录下，查找"hello,world!"字符串<br>
grep -rn man *                    会匹配 ‘Batman’、‘manic’、‘man’等<br>
grep -rn '\<man' *                匹配‘manic’和‘man’，但不是‘Batman’<br>
grep -rn '\<man\>'                只匹配‘man’，而不是‘Batman’或‘manic’等其他的字符串<br>


vi命令
------
:wq  保存文件并退出vi<br>
:wq! 强制保存文件，并退出vi<br>
:q! 不保存文件，强制退出vi<br>
:set number 设置行号
:set nonumber 关闭行号显示


