# 🤝 贡献指南

感谢你愿意为这个项目做出贡献！以下是参与方式。

## 如何贡献

### 方式1：提 Issue（最简单）

如果你发现：
- 某个编码项目**值不对**
- 某个车型**缺少兼容性**标注
- 有**新的编码项目**想添加
- **翻译**有误

直接在 [Issues](https://github.com/StormEye818/porsche-coding-guide-tool/issues) 里提，格式：

```
【类型】纠错 / 新增 / 建议
【车型】你的车型和年款
【模块】涉及的模块名称
【具体描述】详细的编码路径和正确值
【来源】你自己实测 / 来自论坛 / 其他
```

### 方式2：提交 Pull Request

1. **Fork** 本仓库
2. 克隆到本地：
   ```bash
   git clone https://github.com/你的用户名/porsche-coding-guide-tool.git
   ```
3. 修改 `index.html` 中的 `ITEMS` 数据
4. 提交并推送：
   ```bash
   git add .
   git commit -m "描述你的修改"
   git push origin main
   ```
5. 在 GitHub 上发起 **Pull Request**

### 方式3：分享实车测试数据

如果你用 X431 测试了某个编码：
- 在 Issue 里分享你的车型、年款、编码结果
- 标注「已验证可用」或「不可用」

## 编码数据格式

所有编码项目都在 `index.html` 的 `ITEMS` 数组中，格式如下：

### 单模块项目
```javascript
{
  id: 100,                          // 唯一ID
  module: "组合仪表",                // 模块中文名
  name: "功能名称",                  // 项目中文名
  nameEn: "English Name",           // 项目英文名
  compat: ["718","991.2"],          // 适用车型系列
  compatStatus: "ok",               // ok=已验证 / hw=需硬件
  note: "备注说明",                  // 可选备注
  steps: [                          // 编码步骤数组
    {
      pathZh: "中文编码路径",        // X431中文界面路径
      pathEn: "English path",       // X431英文界面路径
      from: "默认值",               // 原始值
      to: "推荐值"                  // 目标值
    }
  ]
}
```

### 跨模块项目
```javascript
{
  id: 9001,
  module: "跨模块",                  // 固定为"跨模块"
  name: "功能名称",
  nameEn: "English Name",
  compat: ["981","991.1","macan"],
  compatStatus: "ok",
  note: "备注",
  multiModule: true,                 // 跨模块标记
  steps: [
    {
      module: "组合仪表",            // 步骤所属模块
      pathZh: "...",
      pathEn: "...",
      from: "...",
      to: "...",
      compat: ["macan"]             // 可选：步骤级车型过滤
    }
  ]
}
```

## 模块名称规范

请使用以下标准模块名（区分大小写）：

| 中文名 | 对应 X431 系统 |
|--------|---------------|
| 组合仪表 | Instrument Cluster |
| 前端电子设备 | Front-End Electronics |
| 后端电子设备 | Rear-End Electronics |
| 空调模块 | Air Conditioning |
| DME模块 | DME (Digital Engine Electronics) |
| PSM模块 | PSM (Porsche Stability Management) |
| 转向助力 | Electric Power Steering |
| 网关模块 | Gateway |
| 方向盘电子设备 | Steering Wheel Electronic |
| 座椅模块 | Driver-side Seat Memory |
| 泊车辅助 | Park Assist |
| 前摄像头 | Front Camera |
| 头灯模块 | Headlight (Central) / Left/Right Headlight |
| 声浪模拟器 | Sound Symposer |
| 跨模块 | （多模块项目专用） |

## compat 车型系列对照

| 值 | 对应车型 |
|----|---------|
| `981` | 2013-2016 Boxster/Cayman |
| `718` | 2017-2025 Boxster/Cayman/Spyder/GT4/GTS |
| `991.1` | 2012-2016 911 Carrera/Turbo/GT3 |
| `991.2` | 2017-2019 911 Carrera/Turbo/GT3 |
| `macan` | 2014-2024 Macan 全系 |

## 注意事项

- 提交前请确保编码路径的**中英文对应正确**
- 如果不确定某个编码是否可用，`compatStatus` 设为 `"hw"`（需硬件）而不是 `"ok"`
- 新增项目请分配一个未使用的 `id`（查看现有 ID 避免冲突）
- 跨模块项目的步骤顺序应按**实际操作顺序**排列（通常先改仪表，再改其他模块）

## 有问题？

不确定怎么改？直接提 Issue 描述你想添加的内容，维护者会帮你加进去。

感谢你的贡献！🏎️