华为设备的配置
==========
# 交换机配置
## 配置登陆用户，口令。
'''
[Quidway]system-view #进入配置视图
[Quidway]sysname xxx #设置主机名称
[Quidway]aaa  #进入aaa认证模式定义用户账户
[Quidway-aaa]local--user wds password cipher wds # 
[Quidway-aaa]local--user wds level 15 #
[Quidway-aaa]local--user wds service type telnet terminal ssh#
[Quidway-aaa]quit

'''
