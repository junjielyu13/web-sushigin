# SEO 下一步行动清单（SushiGin）

> 网站代码层面的 SEO 已经做完并上线（结构化数据、分享卡片、sitemap、robots）。
> **这份是接下来你要亲自做的部分**——都需要登录店铺的 Google 账号，按顺序做即可。
>
> 准备一个**店铺统一的 Google 账号**（最好不是私人号），下面全部用它。

---

## 任务一：让 Google 尽快重新收录（Search Console）

目的：让搜索结果里的标题/描述尽快换成新版，而不是等几周。

### 1. 添加并验证网站
1. 打开 [Google Search Console](https://search.google.com/search-console)
2. 点左上「添加资源 / Add property」
3. 选右边的「**网址前缀 / URL prefix**」，输入：`https://www.sushigin.es/`
4. 验证所有权（任选一种）：
   - **推荐：HTML 文件**——下载 Google 给的一个 `googuxxxx.html` 文件，发给我，我帮你放到网站根目录再上线，然后回去点「验证」。
   - 或：在你的域名 DNS 后台加一条 TXT 记录（Google 会给内容）。
   - 或：如果网站已接 Google Analytics / Tag Manager，可直接用它验证。

> ✅ 验证成功后才能用下面的功能。

### 2. 提交站点地图
1. 左侧菜单「站点地图 / Sitemaps」
2. 在输入框填：`sitemap.xml` → 点「提交」
3. 状态显示「成功 / Success」即可。

### 3. 请求收录首页
1. 顶部搜索框输入：`https://www.sushigin.es/` → 回车
2. 点「**请求编入索引 / Solicitar indexación**」
3. 等待几天，Google 会重新抓取，搜索结果就会换成新标题/描述。

### 4. 顺手验证结构化数据
1. 打开 [富媒体测试 Rich Results Test](https://search.google.com/test/rich-results)
2. 输入 `https://www.sushigin.es/` → 测试
3. 应识别出 **Restaurant**（餐厅）类型，无报错即可。

---

## 任务二：搞定右侧"知识面板"（Google 商家资料）★评分那块

目的：让搜索右侧出现照片、评分、地址、营业时间、"预约/路线"按钮（就是 Raku 那样）。
**这部分纯在 Google 后台做，和网站代码无关。**

### 1. 认领 / 创建店铺
1. 登录 [Google 商家后台](https://business.google.com)
2. 搜索「SushiGin Les Roquetes del Garraf」
   - 已存在 → 点「认领 / Reclamar」
   - 不存在 → 「添加商家 / Añadir empresa」
3. 验证所有权：Google 通常**寄明信片到店里**（含验证码），收到后输入。**必须完成，否则面板不显示。**

### 2. 填核心信息（务必和网站、Facebook 完全一致）

| 项目 | 填写内容 |
|---|---|
| 商家名称 | SushiGin |
| 主类别 | Restaurante japonés |
| 附加类别 | Bufé libre · Restaurante de sushi |
| 地址 | C.C. En Valentí Village, Rambla del Garraf 48-60, local 6P, 08812 Les Roquetes del Garraf |
| 电话 | +34 932 47 38 71 |
| 网站 | https://www.sushigin.es/ |
| 营业时间 | 每天 13:00–16:30 · 20:00–23:30 |
| 节假日 | 12/24 仅午餐 · 12/25 闭店 · 12/31 仅午餐 |

> ⚠️ 名称/地址/电话三处全网一字不差，Google 才会关联同一家店。

### 3. 填内容（决定面板好不好看）
- [ ] **照片**：门面、店内、招牌菜，≥10 张（面板的图就来自这里）
- [ ] **菜单链接**：`https://www.sushigin.es/#menu`
- [ ] **在线预约**：接入 CoverManager，面板会出现"预约"按钮
      预约链接：`https://www.covermanager.com/reservation/module_restaurant/restaurante-sushigin/spanish`
- [ ] **属性**：如实勾选 可外带 / 堂食 / 适合儿童 等

### 4. 攒评分（★4.8 那种星级）
- 评分只能靠**真实顾客评价**，不能自己设，网站也不能伪造（会被惩罚）。
- 做法：商家后台「获取更多评价」→ 拿到专属评价短链 → 做成二维码贴桌台/收银台，引导满意的客人留评。

### 5. 持续维护
- [ ] 回复每条评论
- [ ] 定期发「动态/优惠」
- [ ] 营业时间变动提前更新

---

## 进度自查表

| 步骤 | 谁做 | 状态 |
|---|---|---|
| 网站 SEO 代码（结构化数据/sitemap/robots/分享卡片） | 已完成（代码） | ✅ 上线 |
| Search Console 验证网站 | 你 | ⬜ |
| 提交 sitemap + 请求收录 | 你 | ⬜ |
| 富媒体测试确认 Restaurant | 你 | ⬜ |
| 认领并验证 Google 商家资料 | 你 | ⬜ |
| 商家资料填信息 + 照片 + 预约 | 你 | ⬜ |
| 引导客人留评攒评分 | 你（持续） | ⬜ |

> 卡在哪一步随时找我。其中「验证网站的 HTML 文件」「需要往网站加任何文件」这类，发给我我直接帮你上线。
