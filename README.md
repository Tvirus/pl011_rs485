# 注意：

* 默认串口0不能配置为485模式。
* 在dts的串口里加上 rs485_ctrl_gpio = <&gpio_chip5 7 GPIO_ACTIVE_HIGH>;即可，其中 GPIO_ACTIVE_HIGH 表示485发送时io为高电平。
