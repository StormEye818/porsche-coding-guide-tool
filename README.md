# 🏎️ 保时捷 X431 刷隐藏编码助手 / Porsche X431 Coding Assistant

[中文](#中文) | [English](#english)

---

## 中文

一个免费、开源的保时捷隐藏功能编码查询工具，支持通过 X431 诊断设备激活保时捷车辆的隐藏功能。

### ✨ 功能特点

- **覆盖全系车型**：981 Boxster/Cayman、718 Boxster/Cayman/Spyder/GT4、991.1/991.2 Carrera/Turbo/GT3、Macan
- **100+ 编码项目**：涵盖仪表、灯光、舒适、驾驶辅助、发动机等全部模块
- **多步骤项目合并**：一个功能包含所有编码步骤，不会遗漏
- **跨模块自动分组**：如 Sport Chrono 激活涉及多个模块，自动按模块分组显示
- **车型智能过滤**：选择车型后自动隐藏不兼容的项目
- **中英双语切换**：一键切换中文/英文界面，英文模式纯英文编码路径
- **X431 使用教程**：内置 Launch CRP919x/E 和 Thinkdiag 操作指南
- **移动端适配**：手机浏览器可直接使用

### 🚀 在线使用

**[👉 点击这里直接打开工具](https://stormeye818.github.io/porsche-coding-guide-tool/)**

无需安装，手机/电脑浏览器直接使用。

### 📖 使用方法

1. **选择车型**：依次选择系列（981/718/991/Macan）→ 型号 → 年款
2. **筛选项目**：通过模块标签或搜索框找到想刷的功能
3. **勾选项目**：支持复选，可全选当前筛选
4. **生成方案**：点击「生成编码方案」，按模块输出完整的 X431 编码步骤
5. **对照刷写**：打开 X431 设备，按方案逐项编码

### 🔧 支持的编码项目（部分）

| 类别 | 项目举例 |
|------|---------|
| **仪表显示** | 真实水温、性能/G力图、涡轮压力、油耗显示、车型变量 |
| **灯光系统** | 日行灯菜单、斯堪的纳维亚DRL、自动远光灯、PDLS+功能 |
| **舒适功能** | 钥匙控制车窗/敞篷、锁车收后视镜、启停记忆、座椅舒适进出 |
| **驾驶辅助** | PSM Sport、PTV扭矩分配、Servotronic转向助力、刹车助力map |
| **运动功能** | Sport Chrono直刷(含弹射)、运排控制激活、换挡辅助调优 |
| **安全相关** | 安全带警告关闭、紧急刹车灯闪烁、车内监控关闭 |
| **进阶调优** | 性能显示图调优、981换挡辅助齿比调优、Macan涡轮压力激活 |

### 📋 X431 设备推荐

| 设备 | 价格 | 说明 |
|------|------|------|
| **Launch CRP919x / E** | ~$400 | 到期后仍可编码，不支持更新 |
| **Thinkdiag** | ~$100 | 需安卓手机，年费~$40 |

⚠️ 购买时确认支持 **Ecu Coding**，Lite 版不支持。

### 🤝 如何贡献

欢迎车友一起完善这个工具！你可以：

1. **补充编码数据**：添加新的编码项目或修正错误的编码值
2. **验证兼容性**：用你的车型测试并反馈哪些能用哪些不能
3. **翻译优化**：改进中英文编码路径的翻译
4. **UI 改进**：优化界面设计和用户体验

详细贡献方式请查看 [CONTRIBUTING.md](./CONTRIBUTING.md)。

### ⚠️ 免责声明

- 本工具仅供参考，编码前请**备份所有原始值**
- **一次只改一项**，改完验证再改下一项
- 编码操作存在风险，请自行承担后果
- 安全模块（Airbag/PSM）请谨慎操作
- 本项目不对因使用本工具造成的任何损失负责

### 📄 开源协议

本项目基于 [MIT License](./LICENSE) 开源。

### 🙏 致谢

感谢以下贡献者和社区：

- **Ken G** — 原始编码数据库和 X431 Coding Guide
- **Santirx, 718socal, z06jerry, Treemagnet, Mani** 等 718 Forum 车友
- **Rennlist** 社区的各种编码分享
- 所有提供实车测试反馈的车友

---

## English

A free, open-source Porsche hidden feature coding lookup tool. Activate hidden functions on your Porsche using an X431 diagnostic device.

### ✨ Features

- **Full model coverage**: 981 Boxster/Cayman, 718 Boxster/Cayman/Spyder/GT4, 991.1/991.2 Carrera/Turbo/GT3, Macan
- **100+ coding items**: Covers instrument cluster, lighting, comfort, driver assist, engine, and all other modules
- **Multi-step project grouping**: One feature with all coding steps shown together — no steps missed
- **Cross-module grouping**: Features like Sport Chrono activation span multiple modules, automatically grouped by ECU
- **Smart car filtering**: Select your car model and incompatible items are hidden automatically
- **Bilingual toggle**: Switch between Chinese and English UI — English mode shows English-only coding paths
- **X431 tutorial**: Built-in step-by-step guide for Launch CRP919x/E and Thinkdiag
- **Mobile-friendly**: Works directly in mobile browsers

### 🚀 Use Online

**[👉 Click here to open the tool](https://stormeye818.github.io/porsche-coding-guide-tool/)**

No installation needed — works in any browser on phone or desktop.

### 📖 How to Use

1. **Select your car**: Choose series (981/718/991/Macan) → model → year
2. **Filter items**: Use module tags or search bar to find the feature you want
3. **Select items**: Multi-select supported, or select all in current filter
4. **Generate plan**: Click "Generate Plan" to output complete X431 coding steps grouped by module
5. **Code your car**: Open your X431 device and follow the steps one by one

### 🔧 Supported Coding Items (Partial)

| Category | Examples |
|----------|----------|
| **Instrument Cluster** | Real coolant temp, Performance/G-force display, boost pressure, fuel consumption |
| **Lighting** | DRL menu, Scandinavian DRL, auto high beam, PDLS+ features |
| **Comfort** | Key fob window/roof control, mirror fold on lock, ASS memory, comfort entry |
| **Driver Assist** | PSM Sport, PTV torque vectoring, Servotronic steering, brake booster map |
| **Sport** | Sport Chrono activation (incl. Launch Control), exhaust valve control, shift assist tuning |
| **Safety** | Seatbelt warning off, emergency brake flash, interior monitor off |
| **Advanced** | Performance display tuning, 981 shift assist gear ratio tuning, Macan boost activation |

### 📋 Recommended X431 Devices

| Device | Price | Notes |
|--------|-------|-------|
| **Launch CRP919x / E** | ~$400 | Still works for coding after subscription expires |
| **Thinkdiag** | ~$100 | Android only, ~$40/year renewal |

⚠️ Make sure the device supports **Ecu Coding** — Lite versions do NOT.

### 🤝 How to Contribute

We welcome contributions from the Porsche community! You can:

1. **Add coding data**: Submit new coding items or correct existing values
2. **Verify compatibility**: Test on your car and report what works/doesn't
3. **Improve translations**: Fix Chinese/English coding path translations
4. **UI improvements**: Enhance design and user experience

See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed contribution guidelines.

### ⚠️ Disclaimer

- This tool is for reference only — **backup all original values** before coding
- **One change at a time** — verify before making the next change
- Coding carries risk — proceed at your own discretion
- Safety modules (Airbag/PSM) — proceed with extra caution
- The authors are not liable for any damage caused by using this tool

### 📄 License

This project is licensed under the [MIT License](./LICENSE).

### 🙏 Acknowledgments

- **Ken G** — Original coding database and X431 Coding Guide
- **Santirx, 718socal, z06jerry, Treemagnet, Mani** and other 718 Forum contributors
- **Rennlist** community for various coding shares
- All car owners who provided real-world testing feedback

---

🚗 Happy coding! Open an Issue if you have questions.