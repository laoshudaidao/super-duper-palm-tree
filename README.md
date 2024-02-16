名称:IPTV All
开启:
推送:
分支:
 -主要的
工作:
构建:
运行:Ubuntu-最新版
步骤:
 -名称:结账代码
用途:actions/checkout@v2
 -名称:设置Python
用途:操作/设置-python@v2
使用:
python版本:3.x
 -名称:安装依赖项
运行:pip安装selenium请求
 -名称:安装Chrome网络驱动程序
运行:|
最新的CHROMEDRIVER版本=120.0.6099.109
curl-sS-o chrome driver _ Linux 64 . zip“https://edge dl . me . gvt 1 . com/edge dl/chrome/chrome-for-testing/120 . 0 . 6099 . 109/Linux 64/chrome-headless-shell-Linux 64 . zip“
sudo unzip chrome driver _ Linux 64 . zip-d/usr/local/bin
rm chromedriver_linux64.zip
 -名称:设置chrome驱动程序路径
运行:|
sudo ln-SF/usr/local/bin/chrome-headless-shell-Linux 64/chrome-headless-shell/usr/local/bin/chrome driver
sudo chmod+x/usr/local/bin/chrome driver
 -名称:运行脚本
run:python $ { { github . workspace } }/IPTV . py
 -姓名:提交更改
运行:|
git配置-本地用户。电子邮件“278391333@qq.com"
git配置-本地用户名“laoshudaidao"
git添加。
git提交*。txt -m“添加生成的文件”
git推出
