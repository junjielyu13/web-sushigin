# Google 商家资料补全清单（SushiGin）

> 目标：让 SushiGin 在 Google 搜索右侧出现"知识面板"（照片、评分、地址、营业时间、"预约/路线"按钮），就像 Raku 那样。
>
> ⚠️ 这部分**全程在 Google 后台完成，不涉及网站代码**。网站的结构化数据（JSON-LD）已经做好，会和商家资料相互印证。

---

## 第一步：认领 / 创建店铺
1. 用店铺的 Google 账号登录 [business.google.com](https://business.google.com)
2. 搜索 "SushiGin Les Roquetes del Garraf"
   - **已存在** → 点"认领此商家 / Reclamar"
   - **不存在** → "添加商家 / Añadir empresa"
3. 验证所有权：Google 通常寄**明信片到店里**（含验证码），也可能用电话/邮件验证。
   - 👉 **必须完成**，否则面板不会显示。

## 第二步：核心信息（务必和网站、Facebook 完全一致）

| 项目 | 填写内容 |
|---|---|
| 商家名称 | SushiGin |
| 主类别 | Restaurante japonés |
| 附加类别 | Bufé libre · Restaurante de sushi |
| 地址 | C.C. En Valentí Village, Rambla del Garraf 48-60, local 6P, 08812 Les Roquetes del Garraf |
| 电话 | +34 932 47 38 71 |
| 网站 | https://www.sushigin.es/ |
| 营业时间 | 每天 13:00–16:30 · 20:00–23:30 |
| 节假日 | 12/24 仅午餐 · 12/25 全天闭店 · 12/31 仅午餐 |

> ⚠️ **NAP（名称 Name / 地址 Address / 电话 Phone）三处必须一字不差**，Google 才会把网站、地图、Facebook 关联到同一家店。

## 第三步：内容（决定面板好不好看）
- [ ] **照片**：门面、店内环境、招牌菜，建议 ≥10 张（面板左上的图就来自这里）
- [ ] **菜单链接**：贴 PDF（`https://www.sushigin.es/images/SushiGin_ES.pdf`）或 `https://www.sushigin.es/#menu`
- [ ] **在线预约**：在"预订/Reservas"里接入 CoverManager，面板会出现"预约"按钮
      - 预约链接：`https://www.covermanager.com/reservation/module_restaurant/restaurante-sushigin/spanish`
- [ ] **属性**：如实勾选 可外带 / 堂食 / 适合儿童 / 无障碍 等

## 第四步：评分（★4.8 那种星级）
- 评分**只能靠真实顾客评价积累**，不能自行设置；网站上也不能伪造 ★ 结构化数据（会被 Google 惩罚）。
- 做法：
  1. 在 Google 商家后台获取**专属评价短链**（"获取更多评价 / Solicitar reseñas"）
  2. 做成二维码贴在桌台/收银台/小票上，引导满意的客人留评
- 攒到一定数量后，面板自动显示星级和评论数。

## 第五步：持续维护
- [ ] 及时回复每一条评论（好评差评都回）
- [ ] 定期发"动态/优惠 Novedades"
- [ ] 营业时间变动、节假日提前更新
- 资料越活跃，Google 越愿意展示。

---

## 验证（网站侧，已完成的部分）
部署后做一次检查：
- [Google 富媒体测试](https://search.google.com/test/rich-results) → 输入 `https://www.sushigin.es/`，确认识别出 `Restaurant` 结构化数据
- [Google Search Console](https://search.google.com/search-console) → 提交 `https://www.sushigin.es/sitemap.xml`，并对首页"请求编入索引"

---

## 名词对照
- **知识面板 (Knowledge Panel)**：搜索结果右侧的店铺信息卡 = 来自 Google 商家资料
- **Sitelinks**：标题下方的子链接 = Google 自动生成，单页网站较难出全套
- **结构化数据 (JSON-LD)**：网站里告诉 Google 店铺信息的代码 = 已在 `index.html` 实现
- **NAP**：Name / Address / Phone，全网保持一致是本地 SEO 基础
