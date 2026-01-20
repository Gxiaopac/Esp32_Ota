# Web Client - BLE OTA 测试工具

本文件夹包含用于测试 ESP32-S3 BLE OTA 升级功能的网页客户端工具。

## 📁 文件说明

- **`ble_ota_test.html`** - 完整的 BLE OTA 测试网页
  - 使用 Web Bluetooth API 连接 ESP32-S3 设备
  - 支持固件文件选择和上传
  - 实时显示升级进度和日志
  - 美观的现代化 UI 界面

- **`BLE_OTA_TEST_GUIDE.md`** - 详细的使用指南
  - 前置要求说明
  - 使用步骤详解
  - 故障排除指南
  - 技术细节说明

## 🚀 快速开始

### 方法一：直接打开（最简单）

1. 双击 `ble_ota_test.html` 文件
2. 浏览器会自动打开（Chrome/Edge）
3. 点击"连接设备"开始使用

### 方法二：本地服务器（推荐）

```bash
# 进入 web_client 目录
cd web_client

# 使用 Python 3 启动服务器
python -m http.server 8000

# 或使用 Node.js
npx http-server -p 8000
```

然后访问: `http://localhost:8000/ble_ota_test.html`

## 📋 使用流程

1. **连接设备** - 点击"连接设备"按钮，选择 ESP32-S3 设备
2. **选择固件** - 选择要升级的 `.bin` 固件文件
3. **开始升级** - 点击"开始升级"按钮，观察进度
4. **等待完成** - 设备会自动重启到新固件

## 🔧 系统要求

- **浏览器**: Chrome 56+, Edge 79+, Opera 43+
- **设备**: ESP32-S3 运行 BLE OTA 固件
- **固件**: `.bin` 格式的固件文件

## 📚 更多信息

详细的使用说明请参考 `BLE_OTA_TEST_GUIDE.md` 文件。

## 🔗 相关文档

- 项目根目录的 `BLE_OTA_CLIENT_REQUIREMENTS.md` - 客户端开发需求文档
- 项目根目录的 `README_OTA.md` - OTA 功能说明文档

