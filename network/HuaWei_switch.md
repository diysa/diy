华为交换机的配置
==========
> system-view #进入配置视图
> sysname xxx #设置主机名称
> aaa  #进入aaa认证模式定义用户账户
> [Quidway-aaa]local--user wds password cipher wds #
> [Quidway-aaa]local--user wds level 15 #
> [Quidway-aaa]local--user wds service type telnet terminal ssh#
> [Quidway-aaa]quit

