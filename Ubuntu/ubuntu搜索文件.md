###ubuntu搜索文件
1. `whereis `文件名
　　
　　特点:快速,但是是模糊查找,例如 找 #whereis mysql 它会把mysql,mysql.ini,mysql.*所在的目录都找出来.我一般的查找都用这条命令.
　　

2. `find / -name` 文件名

　　特点:准确,但速度慢,消耗资源大,例如我想找到php.ini的准确位置,就需要用

　　#find / -name php.ini

3. `locate` 文件名

　　强力推荐的方法,最快,最好的方法.
