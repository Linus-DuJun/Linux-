##用法
&emsp;&emsp;secure copy(远程拷贝文件或文件夹)
##格式
    scp 本地文件路径 User＠远程地址：需要拷贝到的目标地址
    scp User@远程地址：需要拷贝的文件 需要拷贝到本地的目标路径
##示例
    //将本地Desktop文件夹下的nginx.conf文件拷贝到132.232.249.97服务器的linus用户的家目录下
    scp Desktop/nginx.conf linus@132.232.249.97:.

    //将本地Desktop文件夹下的nginx.conf文件拷贝到132.232.249.97服务器的linus用户的家目录下并重命名为nginx.conf.bak
    scp Desktop/nginx.conf linus@132.232.249.97:./nginx.conf.bak

    //将132.232.249.97服务器上的linus用户的家目录下的data文件夹拷贝到本地Desktop文件夹
    scp -r linus@132.232.249.97:data Desktop
##常用选项
    -r 递归拷贝，用于拷贝文件夹
    -P 指定端口，一般用默认端口：22 (ssh默认端口号也是22)
##注意事项
    远程路径是远程服务器的User的家目录的相对路径
