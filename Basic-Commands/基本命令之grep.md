##用法
    查找文件内容，可以正则匹配
##格式
    grep [OPTIONS] PATTERN [FILE...]
    grep [OPTIONS] [-e PATTERN | -f FILE] [FILE...]
##示例
    grep hello fileToFind
    grep ^start fileToFind   //在fileToFind文件中查找以start开头的行
    grep end$ fileToFind    //在fileToFind文件中查找以end结尾的行
##常用选项
  -i: 不区分大小写
  -n： 添加行号
  -v: 查询结果取反
