注意：

默认串口0不能配置为485模式。
在115200波特率下150us的延时较为合适，如果使用其他波特率可能要自己用示波器看看io口切换时机对不对
在dts的串口里加上 rs485_ctrl_gpio = <&gpio_chip5 7 GPIO_ACTIVE_HIGH>;即可，其中 GPIO_ACTIVE_HIGH 表示485发送时io为高电平。
