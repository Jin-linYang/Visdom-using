# Cyclegan -    Visdom-using
1、
http://localhost/ 页面能否出现
否：打开 控制面板\程序， 启用或关闭windows功能，将internet information services下的三栏都选中，系统会自动安装IIS组件
https://www.codenong.com/cs106490942/

2、
打开一个screen  python -m visdom.server -p 8097
打开另一个screen python train.py --dataroot ./datasets/maps --name maps_cyclegan --model cycle_gan --display_port 8097


3、
在本地终端输入  ssh -L 1234:127.0.0.1:8097 -p 端口号 username@server_ip
ifconfig可查看IP

4、
打开网页   http://localhost:1234/   

！！！！完成！！！！

参考博客
https://www.codenong.com/cs106490942/
https://blog.csdn.net/weixin_41870042/article/details/120888209
https://blog.csdn.net/qq_42971035/article/details/118547151
