## LEDC 工程集成 BLE OTA 说明（简要）

- 已在 `E:\project2\OTA\ledc` 工程中集成 BLE OTA：
  - 通过 `EXTRA_COMPONENT_DIRS` 复用 `gatt_server_s3/components/ble_ota` 组件
  - 在 `main.c` 中新增 BLE OTA 初始化和 OTA 任务
  - 保留原有 LEDC 呼吸灯逻辑，并放到单独的 FreeRTOS 任务中运行

- 构建方式（在 `E:\project2\OTA\ledc` 目录）：
  - `idf.py build`
  - `idf.py -p COMxx flash`

- BLE OTA 行为与 `gatt_server_s3` 工程保持一致，可直接复用现有 Web 页面 `web_client/ble_ota_test.html` 进行固件升级。


