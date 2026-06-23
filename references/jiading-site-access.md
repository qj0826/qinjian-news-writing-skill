# jiading.gov.cn 网站访问调研记录

> 调研日期：2026年6月22日（初次）/ 2026年6月23日（更新）
> 目标URL：https://www.jiading.gov.cn/xinwen/jddt1/shxw/
> 当前状态：✅ 可访问（HTTP 200）

## 访问状态更新（2026-06-23）

**网站已恢复可访问**。之前的403地理封锁已于2026年6月23日解除，curl和浏览器均可正常获取页面内容。

### 已验证的访问方式

| 方法 | 状态 | 说明 |
|------|------|------|
| curl + Chrome UA | ✅ 200 | 正常返回HTML |
| 浏览器导航 (Browserbase) | ✅ 200 | 页面完整渲染，含JavaScript分页 |
| 分页访问 (/shxw_N) | ✅ 200 | N=1~487，共12172篇文章 |

### URL模式

- 列表首页：`https://www.jiading.gov.cn/xinwen/jddt1/shxw/`
- 列表分页：`https://www.jiading.gov.cn/xinwen/jddt1/shxw_N`（N=2~487）
- 文章详情：`https://www.jiading.gov.cn/xinwen/jddt1/shxw/content_XXXXXX`

### HTML结构

- 文章元数据（作者/编辑/日期）位于 `<div class="contArticle_author">` 内
- 文章正文位于 `<div id="ivs_content">` 内
- 部分文章（机构供稿/系列稿）的编辑信息在正文末尾的 `<p>` 内，不在顶部信息栏
- 列表页面同时包含侧边栏（嘉定动态/民生新闻等）和主内容区（社会新闻）

## 历史记录（保留供参考）

### 2026年6月22日调研结论（已过时）

该网站曾对非中国大陆IP实施严格地理封锁，所有请求返回403 Forbidden。26种访问方法均告失败。详见下方原始记录。

<details>
<summary>原始调研记录（06-22，已过时）</summary>

| 项目 | 值 |
|------|-----|
| 域名 | www.jiading.gov.cn |
| IP地址 | 58.34.40.88（中国大陆） |
| Web服务器 | nginx |
| 防火墙行为（当时） | 对所有非中国大陆请求返回 403 Forbidden |
| RSS/API | 不存在 |

已测试的26种访问方法（当时全部失败，略）
</details>
