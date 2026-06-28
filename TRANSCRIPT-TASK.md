# 任务 spec：YouTube 逐字稿抓取 + 四点提炼

> 给"放宽网络策略后的新 session"用。当前环境网络策略封禁 youtube.com（代理 403），
> 拿不到逐字稿。用户已同意放宽策略。新 session 冷启动，照本文件执行即可。

## 一、前置：确认网络已放行
```bash
curl -sS -o /dev/null -w "%{http_code}\n" --max-time 15 https://www.youtube.com
# 期望 200/301/302；若仍是 000 + CONNECT 403，说明策略未生效，停止并告知用户。
pip install -q yt-dlp   # 若未装
```

## 二、抓逐字稿（自动字幕）
```bash
# 单个测试
yt-dlp --skip-download --write-auto-sub --write-sub --sub-lang "en.*" \
  --sub-format vtt --convert-subs srt -o "%(id)s" \
  "https://www.youtube.com/watch?v=<ID>"
# 批量：对下方 ID 列表循环，sleep 2s 防限流；抓到的 .srt 去掉时间轴合并成纯文本逐字稿。
```
注：只抓字幕不下视频（--skip-download），无需 googlevideo.com。优先 en，其次自动翻译字幕。

## 三、四点提炼格式（每个视频产出一段）
对每个视频，基于**真实逐字稿**输出：
1. **提到了什么能力？** —— 视频里展示/主张的设计能力点
2. **通过什么方式实现？** —— 用了哪些工具/模型/插件（Figma/PS/Nano Banana/ComfyUI…）
3. **具体怎么做？** —— 关键操作步骤（可复现的 how）
4. **能否迁移到 CapCut Web Design？** —— 判断：可直接迁移 / 需改造 / 不适用，并说明理由（结合画布后编辑 + Seed 模型协同的定位）

最终：① 每视频一段卡片；② 整组一段总结；③ 汇总"最该迁移进 CapCut 的 N 个能力"排序。
产物可写成 markdown，并按需并入 kr4-framework.html 模块7（每条 details 下加"四点提炼"正文）。

## 四、优先级与视频清单

### 优先批（用户截图所示"整体 AI 设计工作流"组，先做这 8 个）
- mrXOSXLb8-g  UI/UX 极简 AI 工作流
- idPrScvnSro  4 小时完整 AI 设计流程大课
- 1ClbYm_mgpk  UX 设计师 2026 完整工具链
- gihVEnsh2Ls  构建"会思考/自适应"AI 工作流 5 步法
- GcNwDqqoafo  UI/UX 终极 AI 工作流
- AfmFnzg6pZ0  "像作弊"的工作流
- 6JInQYdSWAc  AI 平面设计工具排名（横评）
- dUZqxumtaTs  AI 工作流的未来形态（Framia Pro）

### 全量 88 个 YouTube ID（按主题，二期）
整体工作流: ni19lPH_wy0 WpkOJ-4sTlw XfezMs8B-O8 mrXOSXLb8-g BLW5NLtQVHM idPrScvnSro ItsKfNAoqTU 1ClbYm_mgpk gihVEnsh2Ls GcNwDqqoafo 2u6bH17NIQk AfmFnzg6pZ0 6JInQYdSWAc dUZqxumtaTs
Figma/UI: C7U_hMSCgZI IPHN7K58Bdw QzbB5yG0kq4 nx_j4y6Zakg tty90cDna3A _-FEgdQ_L4I Q7CABljHMEs tBK4pmNUoBc NqNjx7KEKPw 09VgyFFLrOw
批量自动化: zT68U_u8EBI 5GW9AhLZDV4 a9iTBgQfgF4 DLFPuXFSnQE XvR7uxRH_Fo kxziDfysBbs L2MyYrYcqN4 5FWAFawSEWQ 5kS-c3ayiVU
电商产品图: 9b6fl3oHamo JSj64pGcr94 g0x0rqgv3sU UPZppv0gX70 fLnGlP7mLqw 1sIejUSfytg oyVczeHm7hY qDwgNnPLboM 4yqxpCPn91s -bHhPgiU1UM
Nano Banana/MJ: 1L9TehBIhZ4 dkkcX6gmnlQ 64bOxqzQ0pg uJN59t3SvGI tmwkWnRZkUg xWObTbZgbW4 RP-KurR9KvY vOLiOgZvd-A tSDSSJlHFL4 EQd0U0ohPZc
品牌Logo: JRAGi9AUWic NBZAHaE5jQk 99dGOIM09Vc UTaKkj_GE6Q N6fDPP0UFQk SF5K4weDGlg 26Vi9qy_nW4 vUNQx7cqt7I
社媒批量: VEaJkjf0cvE yEUkiU7tIT0 ekP4ov3z6Q4 J_WbmeHnbSQ f-0_j-f1TuQ 3ysZujOI-NE 4sk0idYZ2RU _hp-DITrwzU pT_8EuBHMQc
调色字体: IooTBRwce2s iDgMb8cX7i8 VggyXZPEmdg sYnW9R4qoqg
GenerativeFill: 86s7AhpOIII ZUJSIzCW5L4 9e8aOzwDPr4 pgBjkr2X6wI
一致性: Uls_jXy9RuU grtmiWbmvv0 h5kjDJrHw_g 5pa3vTWGBuc
动态/演示/设计系统: 8gbkoavLHIg vqTQPKQPv0o 0e8jNWKU-5k nafNPuElCtY X2CpBOoYblg Z0O3lmWghsA

## 五、若策略仍无法放行
退路：用户用浏览器"显示转写"复制逐字稿粘贴/传文件，或我用 WebSearch 做"基于摘要的低保真提炼"（明确标注非逐字稿）。
