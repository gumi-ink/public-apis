# 公共 API 仓库（中文本地化版）

> 本仓库是 [public-apis/public-apis](https://github.com/public-apis/public-apis) 的中文本地化 Fork，由 [gumi-ink](https://github.com/gumi-ink) 维护。
> 原始仓库由社区成员和 [APILayer](https://apilayer.com/) 团队精心策划维护。

这是一个精心整理的公共 API 列表，涵盖多个领域的免费接口资源。可以把它看作是一个由社区多年来共同维护的 API 宝库。

---

## 📋 目录

- [项目简介](#项目简介)
- [API 分类索引](#api-分类索引)
- [如何使用](#如何使用)
- [参与贡献](#参与贡献)
- [许可证](#许可证)

---

## 项目简介

Public APIs 项目收集整理了互联网上各类免费的公共 API 接口，涵盖动物、动漫、反恶意软件、艺术与设计、区块链、书籍、商业、日历、云存储、加密货币、数据验证、开发工具、字典、文档与生产力、邮件、娱乐、环境、事件、金融、美食、游戏、地理编码、政府、健康、工作、机器学习、音乐、新闻、开放数据、开源项目、专利、人格测试、电话、摄影、编程、科学与数学、安全、购物、社交、体育、测试数据、文本分析、跟踪、交通、URL 缩短、车辆、视频、天气等 50+ 个分类。

### 主要特点

- ✅ **完全免费** - 所有收录的 API 都有免费使用层级
- ✅ **手工精选** - 每个 API 都经过社区人工审核
- ✅ **信息完整** - 包含认证方式、HTTPS 支持、CORS 支持等关键信息
- ✅ **持续更新** - 社区驱动，定期维护更新
- ✅ **分类清晰** - 按领域分类，方便查找

---

## API 分类索引

| 分类 | 说明 |
|------|------|
| [Animals](#animals) | 动物相关 API（猫、狗、鸟类等） |
| [Anime](#anime) | 动漫、漫画相关 API |
| [Anti-Malware](#anti-malware) | 反恶意软件、安全扫描 API |
| [Art & Design](#art--design) | 艺术与设计 API |
| [Authentication & Authorization](#authentication--authorization) | 认证与授权 API |
| [Blockchain](#blockchain) | 区块链相关 API |
| [Books](#books) | 图书、阅读相关 API |
| [Business](#business) | 商业、企业相关 API |
| [Calendar](#calendar) | 日历、时间相关 API |
| [Cloud Storage & File Sharing](#cloud-storage--file-sharing) | 云存储与文件分享 API |
| [Continuous Integration](#continuous-integration) | 持续集成 API |
| [Cryptocurrency](#cryptocurrency) | 加密货币 API |
| [Currency Exchange](#currency-exchange) | 货币汇率 API |
| [Data Validation](#data-validation) | 数据验证 API |
| [Development](#development) | 开发工具 API |
| [Dictionaries](#dictionaries) | 字典、词典 API |
| [Documents & Productivity](#documents--productivity) | 文档与生产力 API |
| [Email](#email) | 邮件相关 API |
| [Entertainment](#entertainment) | 娱乐相关 API |
| [Environment](#environment) | 环境、气候相关 API |
| [Events](#events) | 活动、事件相关 API |
| [Finance](#finance) | 金融相关 API |
| [Food & Drink](#food--drink) | 美食、饮品相关 API |
| [Games & Comics](#games--comics) | 游戏与漫画 API |
| [Geocoding](#geocoding) | 地理编码、位置 API |
| [Government](#government) | 政府开放数据 API |
| [Health](#health) | 健康、医疗相关 API |
| [Jobs](#jobs) | 求职、招聘 API |
| [Machine Learning](#machine-learning) | 机器学习 API |
| [Music](#music) | 音乐相关 API |
| [News](#news) | 新闻 API |
| [Open Data](#open-data) | 开放数据 API |
| [Open Source Projects](#open-source-projects) | 开源项目 API |
| [Patent](#patent) | 专利相关 API |
| [Personality](#personality) | 人格测试 API |
| [Phone](#phone) | 电话相关 API |
| [Photography](#photography) | 摄影相关 API |
| [Programming](#programming) | 编程相关 API |
| [Science & Math](#science--math) | 科学与数学 API |
| [Security](#security) | 安全相关 API |
| [Shopping](#shopping) | 购物相关 API |
| [Social](#social) | 社交网络 API |
| [Sports & Fitness](#sports--fitness) | 体育与健身 API |
| [Test Data](#test-data) | 测试数据 API |
| [Text Analysis](#text-analysis) | 文本分析 API |
| [Tracking](#tracking) | 跟踪、追踪 API |
| [Transportation](#transportation) | 交通相关 API |
| [URL Shorteners](#url-shorteners) | URL 缩短服务 API |
| [Vehicle](#vehicle) | 车辆相关 API |
| [Video](#video) | 视频相关 API |
| [Weather](#weather) | 天气相关 API |

---

## 如何使用

### 字段说明

每个 API 条目包含以下信息：

| 字段 | 说明 | 可选值 |
|------|------|--------|
| **API** | API 名称和文档链接 | - |
| **Description** | API 功能描述 | - |
| **Auth** | 认证方式 | `No` / `apiKey` / `OAuth` / `X-Mashape-Key` |
| **HTTPS** | 是否支持 HTTPS | `Yes` / `No` |
| **CORS** | 是否支持跨域 | `Yes` / `No` / `Unknown` |

### 认证方式说明

- **No** - 无需认证，直接调用
- **apiKey** - 需要 API 密钥/令牌
- **OAuth** - 支持 OAuth 认证
- **X-Mashape-Key** - 需要特定的请求头

### 使用示例

```javascript
// 无需认证的 API
fetch('https://api.example.com/data')
  .then(response => response.json())
  .then(data => console.log(data));

// 需要 API Key 的 API
fetch('https://api.example.com/data', {
  headers: {
    'X-Api-Key': 'your-api-key-here'
  }
})
  .then(response => response.json())
  .then(data => console.log(data));
```

---

## 参与贡献

欢迎提交 Pull Request 来添加新的 API 或修正现有信息！

### 提交规范

1. **API 要求**：必须有免费使用层级，不能是付费服务的营销工具
2. **格式规范**：遵循表格格式，保持字母顺序
3. **信息完整**：必须包含认证方式、HTTPS、CORS 信息
4. **描述简洁**：描述不超过 100 个字符
5. **PR 标题**：使用 `Add API-name API` 格式，例如 `Add Weather API`

### 提交步骤

1. Fork 本仓库
2. 创建新分支：`git checkout -b add-new-api`
3. 添加 API 到对应分类（保持字母顺序）
4. 提交更改：`git commit -m "Add XXX API to Category"`
5. 推送到你的 Fork：`git push origin add-new-api`
6. 提交 Pull Request 到 `master` 分支

> ⚠️ **注意**：提交 PR 后会自动触发链接有效性检查，请确保所有链接可正常访问。

详细贡献指南请查看 [CONTRIBUTING.md](./CONTRIBUTING.md)（英文）。

---

## 同步上游更新

本 Fork 会定期同步原始仓库的更新：

```bash
# 添加原始仓库为上游
git remote add upstream https://github.com/public-apis/public-apis.git

# 获取上游更新
git fetch upstream

# 合并到本地主分支
git checkout master
git merge upstream/master

# 推送到你的 Fork
git push origin master
```

---

## 相关链接

- 🌐 **原始仓库**：[public-apis/public-apis](https://github.com/public-apis/public-apis)
- 🍴 **本 Fork**：[gumi-ink/public-apis](https://github.com/gumi-ink/public-apis)
- 📝 **贡献指南**：[CONTRIBUTING.md](./CONTRIBUTING.md)
- 📄 **许可证**：[MIT License](./LICENSE)

---

## 许可证

本项目采用 [MIT License](./LICENSE) 开源协议。

原始项目由社区成员和 [APILayer](https://apilayer.com/) 团队维护。本中文本地化 Fork 由 [gumi-ink](https://github.com/gumi-ink) 维护。

---

*最后更新：2026年3月*
