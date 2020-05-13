# EVB_MX_Plus

> [【IOT应用创新大赛】基于 EVB_MX_Plus 的盆栽土壤监测](https://www.yuangezhizao.cn/articles/Linux/TencentOS-tiny/board/EVB-MX-Plus/flower.html)

例程基于[TencentOS-tiny](https://github.com/Tencent/TencentOS-tiny)目录下`\board\TencentOS_tiny_EVB_MX_Plus\KEIL\qcloud_iot_explorer_sdk_data_template\TencentOS_tiny.uvprojx`该工程修改完成

<details><summary>点击此处 ← 查看折叠</summary>

![master](https://i1.yuangezhizao.cn/Win-10/20200513212628.jpg!webp)

[d1b6d1f](https://github.com/Tencent/TencentOS-tiny/tree/d1b6d1f869259d7da8f9662e9aada7af14b9b818)版本编译通过
![build](https://i1.yuangezhizao.cn/Win-10/20200513213537.jpg!webp)
![diff](https://i1.yuangezhizao.cn/Win-10/20200513212158.jpg!webp)

</details>

其中修改过的文件如下，上图已勾选文件仅修改了密钥配置，其余文件均在此仓库`TencentOS-tiny`目录下

1. `board/TencentOS_tiny_EVB_MX_Plus/BSP/Hardware/DHT11/DHT11_BUS.h`：
修改了`DHT11`的接入`PIN`

2. `board/TencentOS_tiny_EVB_MX_Plus/BSP/Inc/main.h`：
修改了`LED`的接入`PIN`，增加了`LED_DBG`和`MOTOR`的接入`PIN`

3. `board/TencentOS_tiny_EVB_MX_Plus/BSP/Src/gpio.c`：
修改了`GPIO`的初始化部分

4. `board/TencentOS_tiny_EVB_MX_Plus/BSP/Src/mcu_init.c`：
增加了`BH1750`的初始化部分

5. `board/TencentOS_tiny_EVB_MX_Plus/KEIL/qcloud_iot_explorer_sdk_data_template/TencentOS_tiny.uvoptx`：
工程文件

6. `board/TencentOS_tiny_EVB_MX_Plus/KEIL/qcloud_iot_explorer_sdk_data_template/TencentOS_tiny.uvprojx`：
工程文件

7. `components/connectivity/qcloud-iot-explorer-sdk/port/TencentOS_tiny/HAL_Device_tencentos_tiny.c`：
修改了设备密匙

8. `examples/qcloud_iot_explorer_sdk_data_template/data_config.c`：
修改了数据配置

9. `examples/qcloud_iot_explorer_sdk_data_template/data_template_sample.c`：
修改了核心交互中的上报、下控部分

10. `examples/qcloud_iot_explorer_sdk_data_template/entry.c`：
修改了配网密匙

持续更新，未完待续……