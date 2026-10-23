# avatar-privacy

「动漫头像制作」（App Store ID `1507739720`，`com.head.anime`）的**官网 + 隐私政策静态站**，纯静态无构建，可直接部署到 GitHub Pages / Cloudflare Pages。

## 路径与 ASC 对应

| 路径 | 内容 | 用途 |
|---|---|---|
| `/` | 产品官网（中英双语，右上角切换） | marketingUrl / 官网 |
| `/privacy-zh.html` | 隐私政策 v2.2 中文 | privacyPolicyUrl（zh-Hans） |
| `/privacy-en.html` | 隐私政策 v2.2 英文（GDPR 口径） | privacyPolicyUrl（en-*） |

## 文件结构

```
index.html        产品官网（根路径）
privacy-zh.html   隐私政策中文（v2.2，含第十章内容安全与举报流程）
privacy-en.html   隐私政策英文（v2.2）
shot1~4.png       App Store 截图（900px 压缩版）
app_icon_1024.png App 图标（256px）
favicon.png       站点图标
404.html          未找到页
_headers          安全响应头（Cloudflare Pages 用）
```

## 部署

**GitHub Pages**：Settings → Pages → Deploy from branch → `main` / root。

**Cloudflare Pages**：连接本仓库，构建命令留空，输出目录 `/`（`_headers` 自动生效）。

## 口径一致性（改动前必读）

- 隐私政策正文与 **App 内弹窗文案、ASC 后台登记、App Store 元数据** 三方对齐，修改需四方同步；
- 支持邮箱：`support@orzjun.com`（正文第九/十章保留，官网页面装饰区不展示）；
- 响应时限：7 个工作日；
- 官网不出现开发者姓名与支持邮箱（页面装饰层面）。

## 同源项目

App 源码仓库：`ningwhy/avatar`（私有）。
