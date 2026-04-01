# 软件产品经理.skill

工位已空，但产品的逻辑，蒸馏永驻。

### 💡 核心技能
- 物联网产品设计 | IoT Software
- PRD文档生成与研发对接
- 蓝牙/BLE、4G/NB-IoT协议
- 软硬件整合、DP点映射

### 🛠 技术栈
![IoT](https://img.shields.io/badge/IoT-物联网-blue)
![Bluetooth](https://img.shields.io/badge/Bluetooth-蓝牙-green)
![4G](https://img.shields.io/badge/4G-远程通信-orange)
![PRD](https://img.shields.io/badge/PRD-产品需求文档-purple)

## 使用说明
1.  上传SKILL.md到Claude Code技能目录
2.  提供物联网软硬件需求、页面代码、spec文档
3.  一键生成面向研发/测试的结构化PRD

---

## 支持的需求类型

| 类型 | 说明 |
|---|---|
| 数据看板类 | 图表、统计卡片、运营数据 Dashboard |
| 后台列表类 | 数据列表、搜索筛选、表单编辑、详情预览 |
| 用户前台类 | C端设备控制、骑行轨迹、智能服务 |

## 使用方式

在对话中说：

```
帮我生成 PRD
出 PRD
生成需求文档
梳理 DP 功能点
```

Skill 会自动读取当前项目的 `index.tsx`、`spec.md`、`content.md` 等文件，识别页面类型后生成 PRD，并保存至 `src/prototypes/<page-name>/prd.md`。

## 输入文件说明

| 文件 | 作用 |
|---|---|
| `index.tsx` / `index.vue` | 提取功能点和交互逻辑 |
| `spec.md` | 提取技术约定、接口定义、DP 功能点 |
| `content.md` | 提取文案和字段说明 |
| `screenshot.png` | 参考页面布局和 UI 结构 |

## 目录结构

```
prd-generator/
├── SKILL.md                              # Skill 核心工作流
├── spec.md                               # 技术规格文档
├── README.md                             # 本文件
└── assets/
    └── templates/
        ├── data-prd-template.md          # 数据看板类模板
        ├── backend-list-prd-template.md  # 后台列表类模板
        └── user-frontend-prd-template.md # 用户前台类模板
```

## 维护说明

- 修改生成规则和工作流程 → 编辑 `SKILL.md`
- 修改技术规格和字段约定 → 编辑 `spec.md`
- 修改 PRD 模板结构 → 编辑 `assets/templates/` 下对应文件
