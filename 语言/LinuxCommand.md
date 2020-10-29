## 查找文件
```find / -name mysql```    寻找名为mysql的文件夹的位置

```less /apollo/env/ES2Service-beta/var/output/logs/application.log.timestamp```
less 与 more 类似，但使用 less 可以随意浏览文件，而 more 仅能向前移动，却不能向后移动，而且 less 在查看之前不会加载整个文件。

```ls | grep "^app”```   ls查看以app开头的所有文件

```awk '{print NR}’ 1.txt | tail -n1``` 文件行数

## zip
```zip -r test.zip test```    把test文件夹打包成test.zip

```zip test.zip test.jpg test.png```    这条命令是将test.jpg和test.png压缩成一个zip包

## vim
```gg```    命令将光标移动到文档开头 

```G```    命令将光标移动到文档末尾

```x```       删除当前光标下的字符

```dw```      删除光标之后的单词剩余部分

```d$```       删除光标之后的该行剩余部分

```dd```       删除当前行

```c```        功能和d相同，区别在于完成删除操作后进入INSERT MODE

```cc```       也是删除当前行，然后进入INSERT MODE

```%s/^.//g```    删除每行第一个字符 

```shift+4```    即$ 行末

```shift+6```    即^ 行首

```a```    第一行

```G```    最后一行

## scp
```scp src des```

```-r``` 表示文件夹

```scp lizyun@***.com:/ccc* ./```

```scp -r CCCModelTraining/  lizyun@***.com:~/workspace/```
