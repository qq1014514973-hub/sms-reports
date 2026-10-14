# AICRM 只读侦察记录

- 侦察时间：2026-10-14（Asia/Shanghai）
- 站点：`https://wjwjs.cc`
- 租户：`AICRM Default (aicrm-default)`
- 安全边界：仅查看、切换筛选、读取页面和分析公开前端模块；未调用任何创建、修改、删除、发信或上传接口。
- 关键结论：计划中心的“暂无活动”是数据加载完成前的瞬时空态，不是选错实例。34 个可选后端实例均有计划，合计 **8,185** 条。

## 1. 左侧模块与 URL

| 分组 | 模块 | URL |
|---|---|---|
| - | 工作台 | `https://wjwjs.cc/` |
| 运营中心 | 计划管理 | `https://wjwjs.cc/campaigns` |
| 运营中心 | 模板管理 | `https://wjwjs.cc/texts` |
| 运营中心 | 发送监控 | `https://wjwjs.cc/delivery-monitor` |
| 运营中心 | 普通发信监控 | `https://wjwjs.cc/plain-campaign-center` |
| 运营中心 | 号码中心 | `https://wjwjs.cc/recipient-shortlinks` |
| 运营中心 | 号码包收录中心 | `https://wjwjs.cc/collected-phone-packs` |
| 数据分析 | 运营驾驶舱 | `https://wjwjs.cc/ops-workbench` |
| 数据分析 | 异常事件 | `https://wjwjs.cc/exception-center` |
| 数据分析 | 资源健康 | `https://wjwjs.cc/resource-health` |
| 数据分析 | AI 智能助手 | `https://wjwjs.cc/ai-assistant` |
| 数据分析 | 复盘看板 | `https://wjwjs.cc/replay-dashboard` |
| 数据分析 | 智能分析中心 | `https://wjwjs.cc/intelligence` |
| 数据分析 | 运营报表 | `https://wjwjs.cc/operations-report` |
| 数据分析 | 管理看板 | `https://wjwjs.cc/management-dashboard` |
| 数据分析 | 归因看板 | `https://wjwjs.cc/attribution` |
| 号码管理 | 号码包中心 | `https://wjwjs.cc/phone-packs` |
| 号码管理 | 一键分包 | `https://wjwjs.cc/phone-packs/one-click` |
| 号码管理 | 数据标签中心 | `https://wjwjs.cc/phone-pack-labels` |
| 号码管理 | 黑名单 | `https://wjwjs.cc/phone-blacklist` |
| 号码管理 | 通道号段黑名单 | `https://wjwjs.cc/channel-prefix-blacklists` |
| 号码管理 | 运营商配置 | `https://wjwjs.cc/carrier-prefixes` |
| 资源中心 | 代理账号 | `https://wjwjs.cc/agent-accounts` |
| 资源中心 | 域名配置 | `https://wjwjs.cc/domain-config` |
| 资源中心 | 落地页管理 | `https://wjwjs.cc/landing-pages` |
| 资源中心 | 短链 Loading 模板 | `https://wjwjs.cc/shortlink-loading-templates` |
| 系统管理 | 短信测试设备 | `https://wjwjs.cc/platform/sms-test-devices` |
| 系统管理 | 适配器 | `https://wjwjs.cc/adapters` |
| 系统管理 | 市场管理 | `https://wjwjs.cc/platform/markets` |
| 系统管理 | 自动编排发送中心 | `https://wjwjs.cc/platform/auto-send-plans` |
| 系统管理 | 主代理管理 | `https://wjwjs.cc/master-agents` |
| 系统管理 | 用户权限 | `https://wjwjs.cc/users` |
| 系统管理 | 账单中心 | `https://wjwjs.cc/billing` |
| 系统管理 | 租户管理 | `https://wjwjs.cc/tenants` |
| 系统管理 | 审计中心 | `https://wjwjs.cc/audit` |
| 系统管理 | 敏感审批中心 | `https://wjwjs.cc/sensitive-approvals` |
| 系统管理 | 任务中心 | `https://wjwjs.cc/jobs` |
| 系统管理 | IP 白名单 | `https://wjwjs.cc/ip-whitelist` |
| 系统管理 | 全局配置 | `https://wjwjs.cc/global-config` |
| 系统管理 | 平台公告 | `https://wjwjs.cc/platform-announcements` |
| 字典查询 | API 字典 | `https://wjwjs.cc/api-dictionary` |
| 字典查询 | Skills 字典 | `https://wjwjs.cc/skills-dictionary` |
| 字典查询 | 通道费用 | `https://wjwjs.cc/channel-costs` |
| - | Telegram 绑定 | `https://wjwjs.cc/telegram-binding` |

## 2. 后端实例（backendInstanceId）

计划页中实例选择器显示为“筛选包网”。顶部的 `AICRM Default` 下拉框是租户选择器，并不是后端实例选择器。

| 名称 | backendInstanceId | 计划数 |
|---|---|---:|
| PH World02 | `14b30aca-f6b1-46f5-bdea-1f9efe5897a5` | 145 |
| PK05(巴基斯坦地区） | `1bc869bc-2a0e-4905-abfc-8a392177dbc0` | 2 |
| MM02包网 MMK (短信需要70字符内） | `215b339b-4463-4509-a1f9-d27c07cdd4a9` | 29 |
| PH18 | `25c59ca9-f12d-414c-b4d9-9fb6fedefcef` | 244 |
| PH03 | `2a193ae9-846a-47e1-8aa5-2d0142d47630` | 21 |
| MM05包网 jilievo (短信需要70字符内） | `2b372e89-00a6-4032-9a69-01213f05c0a9` | 27 |
| BD05 | `2ea0e9e5-15ba-460f-a30a-1c00ba9dcb8e` | 411 |
| BD18 | `347f7069-39e1-4565-a6a8-2f159dfab42c` | 28 |
| PH01 | `44bf2e3a-f896-47c3-a8d3-ff2944167985` | 58 |
| PH35 | `485ff653-109e-46c3-a2e2-083b53f8b3f6` | 687 |
| PHAG | `4abb39c9-632f-43f6-a805-f9671ed107f8` | 7 |
| MM01包网 123 (短信需要70字符内） | `4c875b34-e186-408b-a65d-855aa392b8f5` | 3 |
| MM07包网 MMK (短信需要70字符内 | `4d1d9556-a5cd-4b2b-8272-6af23ad791fc` | 73 |
| MM00包网 MMK (短信需要70字符内 | `54551f30-97a3-494f-8910-50264a3f7959` | 124 |
| PH25 | `5dd46f03-b7d2-4d9a-86cd-1db9196854f2` | 290 |
| PH23 | `69e86fdb-8ebe-451f-928f-004057104980` | 8 |
| BD09 | `710cac14-dd7c-469d-a4c3-dd9b1f839dbd` | 332 |
| PH31 | `77df27c5-3f21-4755-9730-1928c0a71e77` | 1,663 |
| PK01(巴基斯坦地区） | `882a2e3a-b4d3-47a7-8d8f-77476c119802` | 130 |
| PH22 | `8ac5824a-f8b9-4646-a6b1-0db0ce05542a` | 30 |
| PH16 | `9e9dd7d3-b0fe-4df7-be8c-3c37c59203c4` | 53 |
| mm21 包网 MMK (短信需要70字符内 | `aa329430-c8c7-4854-bd03-16615883d4c8` | 2 |
| PH05 | `ab965792-a0dd-4c3f-b6cf-19b9471078a9` | 3 |
| PH30 | `c971dd74-47ea-41c6-9022-a0284762140c` | 1,210 |
| PH11 | `d3f85849-fca7-4024-bffd-9a3bb05f3e25` | 142 |
| BD11 | `e019513d-d40e-4e6a-844e-6594b72fc188` | 299 |
| mx01 墨西哥 | `e2e7a042-0b23-4bee-a00f-a12b63bc91b8` | 33 |
| PH33 | `e69f6c9a-06a9-4315-9845-5830c6aa810d` | 140 |
| PH07 | `ed38345f-848e-4e63-995a-ca76504c4dce` | 43 |
| PH09 | `f00e6133-8bd8-4779-85cd-70a16b4c7906` | 540 |
| BD02 | `f73ca118-ed6b-4c11-82b3-d7aaee7eaa8b` | 685 |
| TH18 | `f7e435f1-434e-4c04-827f-ab459b63b31a` | 20 |
| MM03包网（缅甸市场MGLA） H1 | `fa8f5a43-bccd-47b8-ab83-c0b04fe6a752` | 66 |
| PH21 | `0738c46d-5ee5-4796-a3af-69ddcd620f15` | 637 |
| **合计** | **34 个实例** | **8,185** |

## 3. 创建人（creatorId）

URL/接口参数名为 `creatorId`（大写 `I`），不是 `creatorid`。

| 名称 | creatorId |
|---|---|
| Jeff - 南昌组 | `4378053f-11d0-46db-9b99-c567b1d5d67f` |
| YOYO - 南昌组 | `da32c277-c556-4edb-9a30-2dc0ba2ae719` |
| AICRM Super Admin | `1b0f95ea-c814-433a-a1a4-f46f1908536a` |
| 阿伟 - 运营组 | `de81f7e5-917e-4a0f-bc89-cf6c971374c8` |
| 北北 - 深圳组 | `db2f2e71-d027-4878-acf9-9d581254842d` |
| 小财财【jack组】 | `b9bc5b16-775d-4b55-8147-6a6390a8b5aa` |
| 小发 - 运营组 | `953313a5-dd70-463a-893e-4bb1d69c1999` |
| 小高 - 运营组 | `84e740c5-09cf-46fa-a847-c2742f0ecd4d` |
| 基挖 - 运营组 | `6e39b8b2-e677-404c-adcd-bc75d337b452` |
| 吉米 - 运营组 | `45f2e555-8b9f-4a33-b8a0-9147c419e26b` |
| 客服30 - 阿西组 | `91794c12-61c6-4703-bcf3-c7765349ce0f` |
| 客服36 - 阿西组 | `f92b4048-7efb-41aa-a619-7400ef82e4ea` |
| 客服39 - 阿西组 | `4b024b53-6de4-40f6-b9de-d80e76cc8650` |
| 阿正 - 运营组 | `dbd84cc4-e8b5-4791-9cbf-693c77c5e83e` |
| 芋头 - 运营组 | `e7c016d7-9a5b-4b45-a72d-fb5e78e11fdb` |
| Mark - 运营组 | `3e0a69f5-e907-43a1-8967-99a24688dd1e` |
| 杰森 - 南昌组 | `57dab362-e2c0-4f38-928d-a69abd4b8f2b` |
| 红中 - 运营组 | `ffba6099-2951-4815-bbf4-b8abd63db867` |
| 莹莹 - 南昌组 | `cd302f42-80b4-4864-ae0e-511d7cac2b7f` |
| 钱钱 - 深圳组 | `f67c4b0b-098b-4185-b22b-3d4a69db13f7` |
| 阿木 - 运营组 | `19173dfb-2994-403b-b132-83956ad9b7a2` |
| 小木 - 南昌组 | `a8308617-fc60-4cff-b513-d4ef9c29599a` |
| 蛙声 - 运营组 | `5dac86af-2806-4284-a237-357cb7194c60` |
| 泡泡 - 南昌组 | `509420bc-5138-48f9-83f9-931374099581` |
| 威龙 | `1e41b8ba-778c-4a15-ade7-b086b47e5d33` |
| 大陈 - 南昌组 | `9a215763-d70a-4bde-a92b-476348c0e6f4` |
| 阿璃 - 运营组 | `a859fac6-9135-471f-84cd-86179ebb6f36` |
| 明石 - 运营组 | `b98d2c00-ea4d-4fbb-9818-76c2f769a524` |
| 阿咩 - 运营组 | `19b988c1-1cdb-4959-aa8b-90989edbd27f` |
| wtt689 | `ec7fbe8c-3a0e-4823-b1da-0afc88c76f89` |
| 小K - 南昌组 | `a561d633-5990-4c9e-9d7c-1a245c7a6867` |
| 小刀 - 广告组 | `49c9edb8-4bad-4811-9377-a9d2925d00a1` |
| 阿西 - 阿西组 | `f684c6de-8afd-4efc-9ad8-14367601a577` |
| 叶子回流 | `4313d2c0-ed9f-486c-a1db-ed81ddc1ef83` |
| 叶子【NN33组】 | `096d82e9-757a-4fff-b0be-35719278e0b1` |
| 阿跃 - 运营组 | `ad4ced0e-3ce6-4fb8-8f50-9854e8994202` |
| 眼睛 - 运营组 | `d08acf8b-eb5f-4fcb-af82-da80937445b0` |

## 4. 只读 XHR / GET 接口

站点前端使用 `Authorization: Bearer <aicrm_token>`。下表只列 GET 接口；未调用写接口。

### 4.1 计划列表与筛选面

`GET https://wjwjs.cc/api/campaigns`

查询参数：

- `page`：页码，从 1 开始。
- `pageSize`：每页数量；前端上限为 200。
- `campaignType`：空、`activity` 或 `plain`。
- `q`：批次名、内容或创建人关键词。
- `backendInstanceId`：后端实例 ID。
- `creatorId`：创建人 ID。
- `launchStatus`：`draft`、`launched`、`scheduled`、`launching`、`launch_failed`、`sending`、`sent`、`partial_failed`、`failed`。

返回结构（值省略）：

```json
{
  "items": [
    {
      "id": "string",
      "displayTitle": "string|null",
      "campaignType": "activity|plain",
      "status": "string",
      "launchStatus": "string",
      "batchTaskCount": "number|null",
      "backendInstanceId": "string|null",
      "createdBy": { "id": "string", "name": "string|null", "email": "string|null" },
      "createdAt": "ISO-8601 string",
      "plannedAt": "ISO-8601 string|null",
      "scheduleEnabled": "boolean",
      "completedSentAt": "ISO-8601 string|null",
      "sentAt": "ISO-8601 string|null",
      "sendChannelIds": ["string"],
      "smsContentOverride": "string|null",
      "text": { "content": "string" }
    }
  ],
  "page": 1,
  "pageSize": 200,
  "total": 8185
}
```

`GET https://wjwjs.cc/api/campaigns/filter-facets`

查询参数：`campaignType`（可选）。

```json
{
  "backendInstanceIds": ["string"],
  "creators": [
    { "id": "string", "name": "string|null", "email": "string|null" }
  ]
}
```

### 4.2 计划详情与统计

`GET https://wjwjs.cc/api/campaigns/{campaignId}`

主要字段：

```json
{
  "id": "string",
  "campaignId": "string|null",
  "displayTitle": "string|null",
  "campaignType": "string",
  "status": "string",
  "launchStatus": "string",
  "createdAt": "ISO-8601 string",
  "createdBy": "object|null",
  "backendInstanceId": "string|null",
  "finalSmsContent": "string|null",
  "smsContentOverride": "string|null",
  "text": { "content": "string" },
  "phonePack": "object|null",
  "phonePackId": "string|null",
  "phonePackTitle": "string|null",
  "agentAccount": "object|null",
  "agentAccountId": "string|null",
  "shortUrl": "string|null",
  "relatedCampaigns": ["Campaign"],
  "sendLogs": ["object"],
  "plannedAt": "ISO-8601 string|null",
  "sentAt": "ISO-8601 string|null",
  "completedSentAt": "ISO-8601 string|null",
  "failureReason": "string|null"
}
```

详情页已验证“最终短信文案”直接渲染自详情数据；最终文案可能包含非拉丁字符和短链，应按原文保存，不能做 trim、Unicode 规范化或 HTML 解码后的二次改写。

相关只读统计接口：

- `GET https://wjwjs.cc/api/campaigns/{campaignId}/dashboard?period=DATE|WEEK|MONTH`
- `GET https://wjwjs.cc/api/campaigns/{campaignId}/sms-analytics`
- `GET https://wjwjs.cc/api/campaigns/{campaignId}/sms-send-hours?start=<ISO>&end=<ISO>`
- `GET https://wjwjs.cc/api/campaigns/{campaignId}/sms-submission-exports`
- `GET https://wjwjs.cc/api/send-verification-sessions?ids=<comma-separated-ids>`

### 4.3 后端实例

`GET https://wjwjs.cc/api/adapters/instances`

常用字段：`id`、`name`、`type`、`enabled`。该响应还可能包含 `configJson` 等敏感配置；巡检程序必须白名单选择字段，禁止原样落盘或写入 GitHub。

计划页将 `type === "gaming_backend" && enabled === true` 的实例作为包网后端候选。

### 4.4 人员与代理账号

`GET https://wjwjs.cc/api/users`

用于运营报表的创建人选择器。返回用户数组；建议巡检只保留 `id` 与显示名，不落盘邮箱等非必要字段。

`GET https://wjwjs.cc/api/agent-accounts`

查询参数：

- `backendInstanceId`
- `keyword`
- `status`
- `page`
- `pageSize`

```json
{
  "items": [
    {
      "id": "string",
      "agentName": "string",
      "affiliateCode": "string|null",
      "backendInstanceId": "string",
      "status": "string",
      "upline": "string|null",
      "customerId": "string|null",
      "masterAgentId": "string|null",
      "domainConfigId": "string|null",
      "rawRegisterUrl": "string|null",
      "shortUrl": "string|null",
      "createdAt": "ISO-8601 string"
    }
  ],
  "total": "number"
}
```

### 4.5 运营报表

`GET https://wjwjs.cc/api/operations-report`

查询参数：

- `dateFrom`
- `dateTo`
- `groupBy`
- `agentLineId`（可选）
- `activityId`（可选）
- `backendInstanceId`（必选）
- `createdByUserId`（可选）

```json
{
  "items": [
    {
      "dimension": "string",
      "sentCount": "number",
      "submitSuccessCount": "number",
      "clicks": "number",
      "uv": "number",
      "ctr": "number",
      "registrations": "number",
      "ftdCount": "number",
      "ftdCost": "number",
      "registrationCost": "number",
      "depositAmount": "number",
      "withdrawAmount": "number",
      "netAmount": "number",
      "roi": "number",
      "roas": "number",
      "batchSmsText": "string|null"
    }
  ],
  "summary": "object（数值汇总，字段与 items 的指标口径对应）"
}
```

## 5. 建议的 24 小时巡检

1. 每 5 分钟请求 `filter-facets`，确认实例集合与创建人集合未意外减少。
2. 对每个 `backendInstanceId` 分页读取 `/api/campaigns`，记录 `total`、状态分布、最新 `createdAt`、`launchStatus` 异常以及 `failureReason`。
3. 对新增或状态变化的计划再请求详情，保存 `finalSmsContent` 原始字节对应的 Unicode 字符串，并计算 GSM-7、UCS-2、零宽字符、弯引号和 Emoji。
4. 监控项建议：实例计划数突然归零、连续分页空响应、详情 404/5xx、`launch_failed`/`partial_failed`/`failed` 增长、计划超过阈值时间仍停留在 `launching` 或 `sending`、最终文案为空、后端实例缺失。
5. `adapters/instances`、`users`、`agent-accounts` 响应只保留巡检所需白名单字段；禁止存储令牌、密码、OTP、`configJson` 或完整注册链接。

