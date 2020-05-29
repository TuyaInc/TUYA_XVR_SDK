# Overview

涂鸦NVR/DVR SDK

# Release Note

### XVR SDK v1.4.6
* 修复子设备上报skill不一致
* [MAX_MEDIA_FRAME_SIZE]放大到500K
### XVR SDK v1.4.2
* 支持三方增值服务，需要调用tuya_ipc_upload_skills(NVR_SUB_DEV_NUM);
* 扫码配网region设置调整到sdk初始化前调用
### XVR SDK v1.4.0
* 增加早期nodeId开通增值服务兼容
* p2p库更新
### XVR SDK v1.3.7
* 云存储增加2s预录
* 支持三方增值服务（echoshow+chromecast）TUYA_APP_Enable_EchoShow_Chromecast
### XVR SDK v1.3.4
* 移除设备删除子设备管理配置
* 放开音视频开关p2p回调
* 云存储修改chn不下发不对应问题
* CHANNEL管理修改，消除与ringbuffer理解
* 查询子设备上下线异常修复
* ringbuffer最大支持10s数据缓存
* 修复子设备升级异常提示问题
### XVR SDK v1.2.8
* 修改子设备binds接口，tuya_ipc_sub_dev_binds_4_CVI(tp, uddd, NVR_SUB_DEV_NUM, IPC_APP_SUB_DEV_PID, IPC_APP_SUB_DEV_VERSION);<br>
* 持云存储功能<br>
### XVR SDK v1.2.6
* 增加本地扫码添加功能；tuya_ipc_set_region(REGION_CN)和IPC_APP_get_qrcode_info();<br>
* 增加子设备升级进度上报；tuya_ipc_upgrade_progress_report<br>
* 修改子设备bind接口，增加tp和uddd参数，tuya_ipc_sub_dev_bind_4_CVI(tp, uddd, NVR_SUB_DEV_NUM, IPC_APP_SUB_DEV_PID, IPC_APP_SUB_DEV_VERSION);<br>
* 支持云存储功能，推荐使用tuya_ipc_sub_dev_bind_4_CVI绑定子设备<br>
### XVR SDK v1.2.4
* 批量绑定子设备接口增加最大路数16限制；<br>
* 子设备清晰度切换cb开放；<br>
* 增加子设备上下线demo；<br>
* 支持云存储+echoshow+chromecast增值服务；<br>

# Supported Platforms

## ubuntu x64 laptop
* linux-ubuntu-6.2.0_64Bit

## Hisilicon Linux
* arm-hisiv500-linux-ev100
* arm-hisiv510-linux
