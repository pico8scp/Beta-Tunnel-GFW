# Beta-Tunnel-GFW  
仅在centos7.6-7.9环境下测试  

测试版，将于2022年12月1日过期，下次更新时测试时间相应延长，请及时关注频道内消息及时更新文件

将Beta-Tunnel-GFW与c.json放入root目录并赋予777权限  
按照使用需求修改c.json配置文件  
"ServerConfig"填写服务端IP：1080  
  
客户端启动命令：./Beta-Tunnel-GFW start --uc  
服务端启动命令：./Beta-Tunnel-GFW -s start --udp  
  
Beta-Tunnel-GFW-s.service 【是服务端的进程保护】    
Beta-Tunnel-GFW-c.service 【是客户端的进程保护】  
将文件放到/usr/lib/systemd/system目录下  

//客户端停止服务：systemctl stop Beta-Tunnel-GFW-c  
//服务端停止服务：systemctl stop Beta-Tunnel-GFW-s  
  
//客户端开始服务：systemctl start Beta-Tunnel-GFW-c  
//服务端开始服务：systemctl start Beta-Tunnel-GFW-s  
  
//查看客户端实时运行日志：journalctl -f -u Beta-Tunnel-GFW-c -o cat  
//查看服务端实时运行日志：journalctl -f -u Beta-Tunnel-GFW-s -o cat  
  

飞机：https://t.me/DNZSD
