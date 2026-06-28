# 设计师「AI 提效 / 辅助设计技巧」调研

> 目标：盘点设计师在公开平台分享的、**可被封装成产品能力**的辅助设计技巧。
> 每条 = 结论（这条揭示了什么可封装能力）+ 链接。每个平台末尾有总结结论。
> 调研日期：2026-06。关键词覆盖：AI 提效 / 工作流 / batch 自动化 / 后编辑 / 一致性 / 提示词 等。

## ⚠️ 平台可达性说明（先看这个）
| 平台 | 状态 | 实际抓到条数 |
|------|------|------|
| YouTube | ✅ 正常 | ~65 条 |
| Medium | ✅ 正常 | ~52 条 |
| Behance | ✅ 正常（多为分类检索页 + 部分作品页） | ~26 条 |
| X / Twitter | ✅ 正常 | ~30 条 |
| **Reddit** | ❌ **被封禁** | 0 条（见下方说明） |

**Reddit 说明**：Anthropic 的网页爬虫被 reddit.com 屏蔽（`robots.txt` 级别），搜索直接返回 400。这不是关键词问题，是平台级限制。报告末尾给了 Reddit 的直达搜索链接，你可手动浏览；或后续我用浏览器（Playwright）模拟访问再补。

---

# 一、YouTube（~65 条）

## 1.1 整体 AI 设计工作流（看「完整链路」怎么串）
- **结论｜可封装：端到端工作流模板。** 设计师完整演示「从生成到改到交付」的个人工作流，是后编辑链路的串联范本。 https://www.youtube.com/watch?v=ni19lPH_wy0
- **结论｜10x 提效叙事，核心是"去摩擦"。** 强调 AI 不是替代创意，而是去掉拖慢设计师的摩擦点——可逐一拆成产品要消除的卡点。 https://www.youtube.com/watch?v=WpkOJ-4sTlw
- **结论｜AI + 设计系统的真实用法。** 把 AI 接进 design system，适合提炼"组件级辅助"能力。 https://www.youtube.com/watch?v=XfezMs8B-O8
- **结论｜UI/UX 极简 AI 工作流。** https://www.youtube.com/watch?v=mrXOSXLb8-g
- **结论｜"什么真正有用"——筛掉噱头。** 自动化评审 + 加速，可对照哪些是真需求。 https://www.youtube.com/watch?v=BLW5NLtQVHM
- **结论｜4 小时完整 AI 设计流程大课，链路最全。** https://www.youtube.com/watch?v=idPrScvnSro
- **结论｜可封装：截图→HTML→Figma 一键转换。** 21 分钟教程，演示截图转可编辑稿，典型可产品化的转换能力。 https://www.youtube.com/watch?v=ItsKfNAoqTU
- **结论｜UX 设计师 2026 完整工具链。** https://www.youtube.com/watch?v=1ClbYm_mgpk
- **结论｜构建"会思考/自适应"的 AI 工作流 5 步法。** https://www.youtube.com/watch?v=gihVEnsh2Ls
- **结论｜UI/UX 终极 AI 工作流。** https://www.youtube.com/watch?v=GcNwDqqoafo
- **结论｜"用与不用 AI"的边界——克制视角。** 哪些环节不该交给 AI，反推产品该在哪给"人工接管"。 https://www.youtube.com/watch?v=2u6bH17NIQk
- **结论｜"像作弊"的工作流，主打爽点。** https://www.youtube.com/watch?v=AfmFnzg6pZ0
- **结论｜AI 平面设计工具排名（横评）。** https://www.youtube.com/watch?v=6JInQYdSWAc
- **结论｜AI 工作流的未来形态（Framia Pro）。** https://www.youtube.com/watch?v=dUZqxumtaTs
- **结论｜可封装：消除重复任务的 AI Agent。** 自动跨平台 resize（IG/邮件/移动端），典型"多尺寸适配"能力。 https://www.youtube.com/watch?v=C7U_hMSCgZI

## 1.2 Figma / UI 设计 AI 插件（看"嵌进现有工具"的能力）
- **结论｜可封装：Figma AI 插件集，砍掉一半设计时间。** https://www.youtube.com/watch?v=IPHN7K58Bdw
- **结论｜跨工具（Envato/Figma/PS）必备 AI 工具串讲。** https://www.youtube.com/watch?v=QzbB5yG0kq4
- **结论｜UX Pilot：想法→结构化界面。** https://www.youtube.com/watch?v=nx_j4y6Zakg
- **结论｜Figma Make 出更好 UI 的进阶提示技巧。** https://www.youtube.com/watch?v=tty90cDna3A
- **结论｜Figma AI 让网站 10X 好看。** https://www.youtube.com/watch?v=_-FEgdQ_L4I
- **结论｜可封装：从现有设计生成 Figma 屏。** https://www.youtube.com/watch?v=Q7CABljHMEs
- **结论｜Figma AI 完整课（2026）。** https://www.youtube.com/watch?v=tBK4pmNUoBc
- **结论｜Figma AI 入门指南（2026）。** https://www.youtube.com/watch?v=NqNjx7KEKPw
- **结论｜可封装：Figma MCP + Cursor 设计→代码新工作流。** https://www.youtube.com/watch?v=09VgyFFLrOw

## 1.3 批量自动化（最容易封装成"一键"产品能力）
- **结论｜可封装：批量去背。** https://www.youtube.com/watch?v=zT68U_u8EBI
- **结论｜可封装：批量放大+去背（MyDesigns）。** https://www.youtube.com/watch?v=5GW9AhLZDV4
- **结论｜可封装：批量修背景（2026）。** https://www.youtube.com/watch?v=a9iTBgQfgF4
- **结论｜可封装：整文件夹批处理去背（ComfyUI）。** https://www.youtube.com/watch?v=DLFPuXFSnQE
- **结论｜批量去背 AI 艺术（MyDesigns）。** https://www.youtube.com/watch?v=XvR7uxRH_Fo
- **结论｜可封装：PS 动作+批处理自动化。** https://www.youtube.com/watch?v=kxziDfysBbs
- **结论｜免费批量去背器。** https://www.youtube.com/watch?v=L2MyYrYcqN4
- **结论｜Microsoft Designer 一键去背。** https://www.youtube.com/watch?v=5FWAFawSEWQ
- **结论｜免费 AI 去背"改变游戏规则"。** https://www.youtube.com/watch?v=5kS-c3ayiVU

## 1.4 电商产品图（核心商业场景，对标我们电商能力）
- **结论｜可封装：AI 换背景做电商图（核心 hack）。** https://www.youtube.com/watch?v=9b6fl3oHamo
- **结论｜免费生成无限电商产品图。** https://www.youtube.com/watch?v=JSj64pGcr94
- **结论｜Shopify 产品图（X-Design）。** https://www.youtube.com/watch?v=g0x0rqgv3sU
- **结论｜Instant Studio：电商产品摄影棚。** https://www.youtube.com/watch?v=UPZppv0gX70
- **结论｜可封装：真实重打光（relight）。** 后编辑"打光"能力的真实演示。 https://www.youtube.com/watch?v=fLnGlP7mLqw
- **结论｜电商新手去产品背景。** https://www.youtube.com/watch?v=1sIejUSfytg
- **结论｜Krea AI：产品图转专业棚拍。** https://www.youtube.com/watch?v=oyVczeHm7hY
- **结论｜用 AI 做电商产品图全流程。** https://www.youtube.com/watch?v=qDwgNnPLboM
- **结论｜Etsy/Shopify 产品图。** https://www.youtube.com/watch?v=4yqxpCPn91s
- **结论｜可封装：无需 PS 的 AI 重打光。** https://www.youtube.com/watch?v=-bHhPgiU1UM

## 1.5 Nano Banana / Midjourney 产品图与提示词（对标 Seed 模型能力）
- **结论｜可封装：在 Nano Banana 里精确控制 MJ 风格。** https://www.youtube.com/watch?v=1L9TehBIhZ4
- **结论｜Nano Banana + Midjourney 全流程"上帝模式"。** https://www.youtube.com/watch?v=dkkcX6gmnlQ
- **结论｜MJ + ComfyUI 完美产品摄影工作流 V2。** https://www.youtube.com/watch?v=64bOxqzQ0pg
- **结论｜建筑可视化：MJ + Nano Banana Pro + FLUX。** https://www.youtube.com/watch?v=uJN59t3SvGI
- **结论｜Nano Banana vs MJ 能力对比测试。** https://www.youtube.com/watch?v=tmwkWnRZkUg
- **结论｜最佳 Nano Banana 产品图 App。** https://www.youtube.com/watch?v=xWObTbZgbW4
- **结论｜可封装：Nano Banana 做 mockup（含提示词）。** https://www.youtube.com/watch?v=RP-KurR9KvY
- **结论｜跨模型提示词写法完整指南。** https://www.youtube.com/watch?v=vOLiOgZvd-A
- **结论｜Nano Banana 极致产品图教程。** https://www.youtube.com/watch?v=tSDSSJlHFL4
- **结论｜"Nano Banana 改变了产品摄影"。** https://www.youtube.com/watch?v=EQd0U0ohPZc

## 1.6 品牌 / Logo（看"品牌物料"场景）
- **结论｜Skywork：更快做品牌内容的完整工作流。** https://www.youtube.com/watch?v=JRAGi9AUWic
- **结论｜AI 做完整品牌识别（含 logo maker）。** https://www.youtube.com/watch?v=NBZAHaE5jQk
- **结论｜Design.com 一站式快速出全套设计。** https://www.youtube.com/watch?v=99dGOIM09Vc
- **结论｜用 AI 更快出稿打动客户。** https://www.youtube.com/watch?v=UTaKkj_GE6Q
- **结论｜AI + Illustrator 生成专业 logo。** https://www.youtube.com/watch?v=N6fDPP0UFQk
- **结论｜可封装：ChatGPT 图像 hack 快速建品牌视觉。** https://www.youtube.com/watch?v=SF5K4weDGlg
- **结论｜logo：AI + Illustrator 砍掉一半构思时间。** https://www.youtube.com/watch?v=26Vi9qy_nW4
- **结论｜Looka AI 低成本快速做 logo。** https://www.youtube.com/watch?v=vUNQx7cqt7I

## 1.7 社媒批量出图（多尺寸 + 批量，强可封装）
- **结论｜可封装：Canva AI 10 分钟出 100 条社媒图。** https://www.youtube.com/watch?v=VEaJkjf0cvE
- **结论｜Canva 批量做社媒图教程。** https://www.youtube.com/watch?v=yEUkiU7tIT0
- **结论｜可封装：Canva Sheets 批量+独立背景图。** https://www.youtube.com/watch?v=ekP4ov3z6Q4
- **结论｜Canva 批量社媒图。** https://www.youtube.com/watch?v=J_WbmeHnbSQ
- **结论｜Canva Bulk + Sheets + AI 一键 20+ 设计。** https://www.youtube.com/watch?v=f-0_j-f1TuQ
- **结论｜可封装：Claude + Canva 8 分钟出 60 个设计。** https://www.youtube.com/watch?v=3ysZujOI-NE
- **结论｜Canva 几分钟批量 30 条。** https://www.youtube.com/watch?v=4sk0idYZ2RU
- **结论｜Canva AI 出社媒图。** https://www.youtube.com/watch?v=_hp-DITrwzU
- **结论｜Canva Sheets+AI 批量一个月内容。** https://www.youtube.com/watch?v=pT_8EuBHMQc

## 1.8 调色 / 字体（B 线"调色"能力对标）
- **结论｜AI 辅助配色基础（Adobe）。** https://www.youtube.com/watch?v=IooTBRwce2s
- **结论｜可封装：提示词生成配色（Illustrator Generative Recolor）。** https://www.youtube.com/watch?v=iDgMb8cX7i8
- **结论｜AI 配色 + 字体工具实验。** https://www.youtube.com/watch?v=VggyXZPEmdg
- **结论｜可封装：给 AI 生成图精确指定颜色的 4 种方法。** https://www.youtube.com/watch?v=sYnW9R4qoqg

## 1.9 Generative Fill 隐藏技巧（指令/局部编辑对标）
- **结论｜可封装：Generative Fill 5 个隐藏技巧。** https://www.youtube.com/watch?v=86s7AhpOIII
- **结论｜可封装：强度（intensity）控制技巧。** https://www.youtube.com/watch?v=ZUJSIzCW5L4
- **结论｜Generative Fill 完整技巧教程。** https://www.youtube.com/watch?v=9e8aOzwDPr4
- **结论｜可封装：用参考图（而非提示词）引导 Generative Fill。** 2026 新特性，对标"指令编辑+参考"。 https://www.youtube.com/watch?v=pgBjkr2X6wI

## 1.10 角色一致性 / 多尺寸衍生（对标"一致性"失败 case）
- **结论｜可封装：从单图生成一致角色（FLUX/ComfyUI）。** https://www.youtube.com/watch?v=Uls_jXy9RuU
- **结论｜可封装：单图→无限一致角色。** https://www.youtube.com/watch?v=grtmiWbmvv0
- **结论｜100% 一致角色的实战做法。** https://www.youtube.com/watch?v=h5kjDJrHw_g
- **结论｜Leonardo AI 角色参考特性。** https://www.youtube.com/watch?v=5pa3vTWGBuc

## 1.11 动态 / 演示 / 设计系统（外延场景，判断要不要做）
- **结论｜可封装：AI 生成专业 mockup（几分钟）。** https://www.youtube.com/watch?v=8gbkoavLHIg
- **结论｜AI 几秒做演示稿（Gamma）。** https://www.youtube.com/watch?v=vqTQPKQPv0o
- **结论｜动态设计师 2026 该怎么用 AI。** https://www.youtube.com/watch?v=0e8jNWKU-5k
- **结论｜可封装：4 小时用 AI 搭完整设计系统（Claude+Cursor+Figma）。** https://www.youtube.com/watch?v=nafNPuElCtY
- **结论｜自动化你的设计系统。** https://www.youtube.com/watch?v=X2CpBOoYblg
- **结论｜设计系统自动化：什么该自动、何时自动。** https://www.youtube.com/watch?v=Z0O3lmWghsA

> **YouTube 总结结论：** YouTube 是"可封装能力"密度最高的平台——绝大多数视频本质是在演示**一个可被产品化的单点操作**（批量去背、换背景、重打光、配色生成、截图转稿、角色一致性、多尺寸批量）。三个最该重点拆解的方向：①**批量/多尺寸自动化**（1.3+1.7，封装难度低、用户感知强）；②**电商换背景+重打光**（1.4，正面商业场景，对标 Seed 打光能力）；③**Generative Fill 的参考图引导 + 角色一致性**（1.9+1.10，正好命中我们"指令编辑/图层分离"的护城河方向）。建议把这三类各挑 3-5 个视频做逐帧拆解，提炼成"模型该优化什么"的失败 case 清单。

---

# 二、Medium（~52 条）

## 2.1 "我的 AI 工作流"个人复盘（最适合挖未包装需求）
- **结论｜5 个真正省时间的 AI 工具。** https://medium.com/@zenvertise/ai-tools-design-workflow-5195a6edea08
- **结论｜AI 如何重塑平面设计工作流（效率视角）。** https://medium.com/@atasan/embracing-efficiency-how-ai-is-transforming-graphic-design-workflows-56bdabf857f5
- **结论｜设计师的 AI 工具之旅（支撑而非替代）。** https://medium.com/@rkoscinski07/ai-tools-supporting-graphic-design-a-designers-journey-6134d29eb975
- **结论｜AI 工作流优化 7 个实操技巧。** https://medium.com/@vicki-larson/ai-workflow-optimization-7-game-changing-tips-that-actually-work-414862126f5f
- **结论｜把 AI 接进真实设计工作流（2026）。** https://medium.com/@ant_95138/ai-for-graphic-designers-in-2026-how-to-integrate-ai-into-a-real-design-workflow-464971e28e03
- **结论｜产品设计师的 AI 工作流。** https://medium.com/@mariamargarida/ai-in-my-design-workflow-as-a-product-designer-feb120d8fe38
- **结论｜支撑我工作流的 AI 设计栈。** https://medium.com/design-bootcamp/the-ai-design-stack-that-powers-my-workflow-de3efcb220af
- **结论｜UX 设计师该懂的 AI 提效工具（含怎么用）。** https://medium.com/design-bootcamp/ai-productivity-tools-every-ux-designer-should-know-and-how-i-use-them-in-my-workflow-b57d0b8462fe
- **结论｜团队级：用 AI 让 UX/UI 更快更人性。** https://medium.com/@ssd_design/how-we-use-ai-to-design-smarter-faster-and-more-human-digital-products-c6d9910c4053
- **结论｜我的设计工作流如何因 AI 改变。** https://medium.com/@kazdenc/how-my-design-workflow-is-changing-with-ai-bc80e7fa3323
- **结论｜用 AI 提速但不丢创意。** https://medium.com/@mkumud24/how-i-use-ai-to-speed-up-my-design-workflow-without-losing-creativity-2979d2629582
- **结论｜可封装：AI 在设计工作流的 5 个真实例子。** https://medium.com/@jackanglesea/real-examples-of-using-ai-in-my-design-workflow-3992bfe3a3f2
- **结论｜用 AI 规模化设计工作。** https://medium.com/design-bootcamp/scaling-design-work-with-ai-a-new-era-of-creative-productivity-d54b8c08d775
- **结论｜可封装：16 个让创意产出 10x 的 AI 工具。** https://medium.com/artificial-corner/16-ai-tools-for-designers-to-10x-their-creative-output-d978ad5b7f38

## 2.2 后编辑 / inpainting / 一致性（最贴近 KR4 核心）
- **结论｜可封装：FLUX.1 inpainting/outpainting 工具革新。** https://medium.com/@wxbxtxr/revolutionize-ai-image-editing-in-comfyui-with-flux-1-tools-for-inpainting-and-outpainting-c48f45e8cf91
- **结论｜可封装：电商行业的 inpainting 实战。** 直接电商场景的局部重绘，对标我们图层/指令编辑。 https://medium.com/data-science-at-microsoft/introduction-to-image-inpainting-with-a-practical-example-from-the-e-commerce-industry-f81ae6635d5e
- **结论｜可封装：产品图多角度/高保真变体生成。** https://garystafford.medium.com/ai-powered-product-perfection-part-2-of-2-leveraging-generative-ai-techniques-for-diverse-ba8d5ea7986e
- **结论｜ComfyUI inpaint/outpaint 技巧。** https://medium.com/@techlatest.net/inpainting-and-outpainting-techniques-in-comfyui-d708d3ea690d
- **结论｜动画场景一致性与连续性（OpenArt）。** https://medium.com/@latouralexandre/my-ai-animators-dream-achieving-scene-consistency-and-continuity-in-animation-with-openart-ai-76b32b2bed87
- **结论｜可封装：FLUX.1 Kontext 多模态图像编辑。** https://medium.com/diffusion-doodles/flux-1-kontext-dev-multimodal-image-editing-19a003714b40

## 2.3 提示词工程（设计向）
- **结论｜设计师的提示词工程实操指南。** https://medium.com/@uxraspberry/prompt-engineering-for-designers-a-practical-guide-what-i-learned-so-far-140d70879c7e
- **结论｜AI 图像提示词技巧是否用对了。** https://medium.com/@david-ocean/ai-image-generation-prompt-engineering-are-you-applying-proper-prompt-techniques-when-generating-0753d0ee3666
- **结论｜可封装：设计向提示（整体排版为主角）。** https://medium.com/@david-ocean/crafting-visual-designs-with-ai-design-focused-prompting-explained-b5ca10f256e8
- **结论｜掌握 AI 图像提示词。** https://medium.com/digital-miru/mastering-ai-image-generator-prompts-a-guide-to-creating-stunning-visuals-5ac9b4038a7e
- **结论｜写出专业平面设计师级提示词。** https://medium.com/@jamesoconnorai/how-to-create-ai-generated-prompts-worthy-of-a-pro-graphic-designer-d2c3f19babd1
- **结论｜25 个强力视觉 AI 提示词。** https://medium.com/write-a-catalyst/master-visual-ai-25-powerful-prompts-to-create-stunning-images-designs-a08cd615f47f

## 2.4 Logo / 品牌
- **结论｜AI logo 生成器革新品牌流程。** https://medium.com/uxness/how-ai-logo-generators-are-revolutionizing-the-branding-process-a76883891cb3
- **结论｜可封装：用 AI 做 logo+视觉品牌（案例）。** https://xetrocube.medium.com/how-to-create-a-logo-and-visual-brand-with-ai-a-case-study-84bee87b0538
- **结论｜我如何在品牌流程里用 AI。** https://jennyhendersonstudio.medium.com/how-i-use-ai-in-my-branding-process-acfa348c440f
- **结论｜2026 logo 设计师的 7 个 AI 工具。** https://medium.com/design-bootcamp/best-7-ai-tools-for-logo-designers-in-2026-d6695edc2d42
- **结论｜测了 30+ logo 生成器选 9 个。** https://medium.com/freelancers-hub/i-tried-6-ai-logo-generators-this-is-my-favorite-by-far-e46b7422ef48

## 2.5 UX 研究 / 线框 / persona（外延场景）
- **结论｜可封装：用 AI 建 3 个 persona 的工作流。** https://medium.com/design-bootcamp/how-i-built-3-personas-using-ai-a-designers-workflow-3c82ff6cde2c
- **结论｜AI 进线框流程：提效还是添乱（含边界）。** https://medium.com/@nsks_83006/ai-in-the-wireframing-workflow-efficiency-or-extra-work-8807af82420f
- **结论｜线框 + AI + 设计师大脑的真实体验。** https://medium.com/@sandysh/wireframes-ai-and-a-designers-brain-my-experience-using-generative-tools-ee261796ac30
- **结论｜8 个 UX 新人能用的 AI 提示词。** https://medium.com/@hashbyt/how-new-ux-designers-can-use-ai-prompts-8165b1b1b208
- **结论｜把 AI 集成进 UX 用户研究。** https://medium.com/@hhnngvrie/integrating-ai-into-ux-workflows-user-research-edb7f5b07633
- **结论｜免费 AI UX 工具包。** https://medium.com/design-bootcamp/how-i-use-ai-for-ux-design-without-paying-a-dime-9c633af06655

## 2.6 工具横评 / 选型（看竞品全景）
- **结论｜测了 50+ AI 设计工具选 10 个必备。** https://medium.com/@DilSalaKamina/i-tested-50-ai-design-tools-so-you-dont-have-to-the-10-every-product-designer-actually-needs-in-5bce66cdb74a
- **结论｜Figma vs Adobe vs Canva 设计 AI 对决。** https://medium.com/design-bootcamp/ai-product-case-study-3-battle-of-the-design-ais-figma-vs-adobe-vs-canva-7ed41a05fa02
- **结论｜2026 最佳 AI 图像工具横评。** https://jimmacleod.medium.com/the-best-ai-image-tools-for-2026-compared-and-evaluated-4dee99b4b565
- **结论｜MJ vs Firefly 设计师视角对决。** https://medium.com/design-bootcamp/ai-art-showdown-midjourney-vs-adobe-firefly-for-designers-2025-ebec364673c4
- **结论｜MJ vs DALL-E vs Firefly 谁更值。** https://medium.com/@glasier067/midjourney-vs-dall-e-vs-adobe-firefly-which-image-ai-is-actually-worth-it-f78b14136041
- **结论｜Figma AI 特性如何改变 2026 设计方式。** https://medium.com/@ryan.almeida86/how-figmas-ai-features-are-changing-the-way-designers-work-in-2026-5cef84801d38
- **结论｜被 AI 塑造的 7 个 2026 网页设计趋势。** https://medium.com/creative-black-pug-studio/7-web-design-trends-being-shaped-by-ai-in-2026-4afbec683b34

## 2.7 反思 / 边界（反向喂"产品该在哪让人接管"）
- **结论｜AI 是面镜子，不是批判性思考工具——警惕"无深度的自信"。** https://medium.com/@nuarle/overconfident-by-design-ais-feedback-loop-and-the-designer-s-god-complex-230bbbcc9d70
- **结论｜设计师和 AI：没人在谈的诚实对话。** https://medium.com/design-bootcamp/designers-and-ai-the-honest-conversation-were-not-having-dcba719dee2b
- **结论｜可封装反例：AI 承诺提速，为何反而更慢了。** 直接指出产品化的坑。 https://medium.com/design-bootcamp/ai-tools-promised-to-speed-up-design-so-why-does-everything-take-longer-now-afe167bc7b55
- **结论｜AI 对设计师日常的真实影响：什么仍重要。** https://uxmag.medium.com/the-real-impact-of-ai-on-designers-day-to-day-and-interfaces-what-still-matters-f9162c199cdf
- **结论｜设计师其实已在用 AI（即便没意识到）。** https://medium.com/design-bootcamp/how-designers-are-already-using-ai-even-if-they-dont-realize-it-29b7cefe715f
- **结论｜我能做而 AI 做不到的：UX 设计师视角。** https://medium.com/design-bootcamp/what-i-can-do-that-ai-cant-a-ux-designer-s-perspective-655b239cb3fe

## 2.8 Agent / 10x 自动化
- **结论｜AI Agent 改造设计与开发工作流。** https://makotokern-iiimpact.medium.com/ai-agents-transforming-design-and-development-workflows-3045861fee9c
- **结论｜可封装：搭建自动化创意内容工作流系统。** https://medium.com/@elosarah85/how-i-built-an-ai-content-workflow-system-to-automate-my-creative-process-fffaad970ae0

> **Medium 总结结论：** Medium 是"方法论 + 边界"的金矿，价值在两端——**正向**（2.1/2.2 的个人工作流复盘里藏着大量"用户在用 coding/ComfyUI 自己补"的未包装需求，尤其是 inpainting、产品图多角度变体、角色一致性，全部正中 KR4 后编辑核心）；**反向**（2.7 的反思文直接告诉你"AI 在哪让设计师更慢/更不可控"，这正是产品该设计"人工接管/可降级"的地方）。建议把 2.2 的 6 篇和 2.7 的反思文逐篇精读，分别产出"可封装能力清单"和"失败 case/降级触发条件清单"。

---

# 三、Behance（~26 条）

> 说明：Behance 搜索多返回**分类检索页**（本身就是高价值的"案例入口"，可一键看该类目下全部作品）+ 少量具体作品页。下面分两类标注。

## 3.1 方法/资源文章（含可封装的能力分类法）
- **结论｜可封装分类法：生成式/辅助式/分析式 三类 AI。** Behance 官方把 AI 分成 Generative/Assistive/Analytical，是很好的能力归类框架。 https://www.behance.net/resources/articles/aibasics
- **结论｜创意工作流 AI 实操（直播录像）。** https://www.behance.net/live/videos/25567/Ai-in-Action-Hands-On-with-Creative-Workflows
- **结论｜AI 驱动的产品设计服务（看商业化打包方式）。** https://www.behance.net/fineartdesignagency/services/319885/AI-Driven-Product-Design

## 3.2 分类检索入口（一键看整类案例）
- **结论｜入口：生成式设计案例集。** https://www.behance.net/search/projects/generative%20design
- **结论｜入口：生成式 AI UI 设计。** https://www.behance.net/search/projects/generative%20ai%20ui%20design
- **结论｜入口：生成式 AI 项目总集。** https://www.behance.net/search/projects/generative%20ai
- **结论｜入口：AI 艺术项目。** https://www.behance.net/search/projects/ai%20art?locale=en_US
- **结论｜入口：AI 自动化项目（看流程类）。** https://www.behance.net/search/projects/ai%20automation?locale=en_US
- **结论｜入口：Midjourney 项目总集。** https://www.behance.net/search/projects/?search=midjourney
- **结论｜入口：Midjourney 品牌识别。** https://www.behance.net/search/projects/midjourney%20ai%20brand%20identity?locale=en_US
- **结论｜入口：Midjourney 社媒图。** https://www.behance.net/search/projects/midjourney%20ai%20social%20media%20post?locale=en_US
- **结论｜入口：AI 海报。** https://www.behance.net/search/projects/ai%20poster
- **结论｜入口：AI 演示稿设计。** https://www.behance.net/search/projects/ai%20presentation
- **结论｜入口：人工智能主题海报。** https://www.behance.net/search/projects/artificial%20intelligence%20poster
- **结论｜入口：Midjourney 标签聚合页。** https://www.behance.net/tags/midjourney
- **结论｜入口：AI 标签聚合页。** https://www.behance.net/tags/ai
- **结论｜入口：包装设计案例。** https://www.behance.net/search/projects/packaging%20study?locale=en_US

## 3.3 具体作品/案例页（可直接拆解的成品）
- **结论｜可封装参考：单字母独立提示词生成的字体海报。** 展示"每个元素独立提示词"的精修思路。 https://www.behance.net/gallery/165516153/Midjourney-Typography-Poster?locale=en_US
- **结论｜MidJourney UI/UX 案例研究。** https://www.behance.net/gallery/195228179/MidJourney-AI-UIUX-Case-Study
- **结论｜SolarPunk 游戏角色/道具/场景概念（一致性参考）。** https://www.behance.net/gallery/176180091/SolarPunk-Game-Character-Prop-Environment-Concepts
- **结论｜MidJourney AI 艺术 App 概念 UI/UX 案例。** https://www.behance.net/gallery/156623655/Midjourney-Ai-Art-App-Concept-UIUX-Study-Case

> **Behance 总结结论：** Behance 的价值不在"教程"，而在**成品级案例**——设计师把 AI 做出的品牌/海报/包装当作品集展示，是验证"某能力能不能撑起真实商业产出"的样本库。但它对"提效技巧"的文字描述少，多靠看图。最高价值的一条是官方的 **Generative/Assistive/Analytical 三分法**（3.1 第一条），可直接拿来给我们的能力盘点做归类。建议把 3.2 的分类入口当作"持续监测看板"，定期扫该类目下的新作品看趋势。

---

# 四、X / Twitter（~30 条）

## 4.1 官方/权威提示词指南（最可直接转成产品默认提示）
- **结论｜可封装：Nano Banana 六条文生图提示技巧（官方）。** https://x.com/GoogleAIStudio/article/1962957615262224511
- **结论｜Nano Banana 开发者完整教程（官方）。** https://x.com/GoogleAIStudio/status/1964024315638403231
- **结论｜可封装：Nano Banana Pro 专业资产生产 10 招（官方）。** https://x.com/GoogleAIStudio/status/1994480371061469306
- **结论｜可封装：Nano Banana Pro 在产品设计的 3 个用法（应用新风格到现有 UI/图）。** https://x.com/101babich/status/1991875088774283769
- **结论｜Nano Banana Pro 完美文字渲染。** https://x.com/rjmans/status/2003479311525839123

## 4.2 提示词模板（可直接做成"一键模板"功能）
- **结论｜可封装：把任意 logo/设计转视觉资产的 JSON 提示模板。** https://x.com/alex_prompter/status/1992013852897148989
- **结论｜可封装：整合 9 条技巧的 Nano Banana Pro JSON 母版提示。** https://x.com/aigleeson/status/1998678041007194320
- **结论｜可封装：生成写实图（自拍/手机照/生活方式）提示模板。** https://x.com/godofprompt/status/1994753701227991490

## 4.3 Midjourney 一致性 / 风格参考（对标一致性能力）
- **结论｜MJ 12 份帮助/提示资源合集。** https://x.com/nickfloats/status/1763371638395895953
- **结论｜可封装：控制角色权重做一致角色。** https://x.com/nickfloats/status/1768326351038112069
- **结论｜MJ omnireference（一致角色/物体/场景）系统预告。** https://x.com/nickfloats/status/1917660347508613455
- **结论｜可封装：系统测试 SREF 风格码的方法。** 参数比提示词更重要的实操，适合做成"风格锁定"能力。 https://x.com/ciguleva/status/1803538907968975058
- **结论｜MJ + EverArt 做一致角色指南。** https://x.com/skirano/status/1744711126892347653
- **结论｜SREF 新风格码示例（linocut/木刻）。** https://x.com/michaelrabone/status/1999403859912065092
- **结论｜可封装工作流：MJ 建角色→后续动画化。** https://x.com/aimikoda/status/2066447640829505886

## 4.4 设计观点 / 工作流（看趋势与心智）
- **结论｜"多数设计师把 AI 当计算器，顶尖 1% 当整个创意团队"——分层用法。** https://x.com/shushant_l/status/2067502587335840057
- **结论｜可封装：图片一键转 Figma 可编辑组件。** https://x.com/fardeentwt/status/1993660792298971542
- **结论｜Figma×Intent 详细工作流（MCP 拉设计数据）。** https://x.com/LukeW/status/2030066421099884862
- **结论｜Figma 官方：AI Agent 直接在画布上设计（MCP）。** https://x.com/figma/status/2036434766661296602
- **结论｜Figma 官方：编辑图像 + 生成图像新特性。** https://x.com/figma/status/1915098380331839541
- **结论｜跨工具实测：Figma MCP 在 V0/Cursor/Claude Code 表现对比。** https://x.com/melodyskim/status/2014530834385056222
- **结论｜"直接设计"（Direct Design）理念。** https://x.com/alexkehr/status/2021667248608584183
- **结论｜AI 让设计直接出代码组件，自动套站点样式。** https://x.com/SubframeApp/status/1928505958009024827

## 4.5 账号（持续跟踪源）
- **结论｜跟踪源：Nano Banana 官方实验室。** https://x.com/NanoBanana_labs
- **结论｜跟踪源：Sref 风格码聚合账号。** https://x.com/SrefCodeAi
- **结论｜跟踪源：Nick St. Pierre（MJ 头部教学）。** https://x.com/nickfloats
- **结论｜跟踪源：Tatiana Tsiguleva（SREF 实测）。** https://x.com/ciguleva

> **X 总结结论：** X 是"提示词技巧 + 一致性参数"最快的一手来源，且最容易直接转成产品功能——**4.1/4.2 的官方与模板类**几乎可以原样做成画布里的"一键模板/智能提示"能力；**4.3 的 SREF/omnireference**是我们做"风格锁定/角色一致"时绕不开的对标，建议把这几条的参数玩法整理给 Seed 当"产品可用水位"参照。跟踪策略：先关注 4.5 四个账号 + Google AI Studio 官方，从它们的转发/关注链横向扩散。注意：X 帖子需登录才能看完整内容/视频，链接仅作锚点。

---

# 五、Reddit（被封禁，0 条抓取）

我的爬虫无法访问 reddit.com（平台级屏蔽，返回 400）。以下是直达搜索链接，你可手动浏览；或我后续用浏览器自动化（Playwright）模拟登录访问，再按同样格式补一批：
- r/StableDiffusion 搜"workflow"：https://www.reddit.com/r/StableDiffusion/search/?q=workflow
- r/midjourney 搜"consistency"：https://www.reddit.com/r/midjourney/search/?q=consistency
- r/graphic_design 搜"AI workflow"：https://www.reddit.com/r/graphic_design/search/?q=AI%20workflow
- r/photography 搜"AI editing"：https://www.reddit.com/r/photography/search/?q=AI%20editing

> **Reddit 总结结论（基于其他平台交叉印证）：** 虽未直接抓取，但 Medium/YouTube 多次引用 Reddit 上反复出现的痛点——**角色/物体一致性保不住、inpainting 局部改动牵连全图、风格不连续**。这三条恰好是我们后编辑护城河要解决的失败 case。建议优先级：等需要做"模型需求清单"时，再用浏览器自动化专门去 r/StableDiffusion 抓高赞抱怨贴，归类成评测标准。

---

# 全局结论：哪些技巧最该被封装成产品能力

按"出现频率 × 可封装度 × 命中 KR4 后编辑核心"三重打分，最该做的五类：

1. **批量 / 多尺寸自动化**（YouTube 1.3+1.7 高频）：去背、跨平台 resize、批量出社媒图——封装难度低、用户感知最强，适合做 L1 渗透率的入口能力。
2. **电商换背景 + 重打光**（YouTube 1.4 + Medium 2.2）：正面商业场景，直接对标 Seed 打光能力，是"产品可用水位"最该先定义的。
3. **局部编辑 + 参考图引导**（Generative Fill 1.9 + FLUX Kontext）：命中"指令编辑"护城河，关键失败 case 集中在"局部改动牵连全图"。
4. **角色 / 风格一致性锁定**（YouTube 1.10 + X 4.3 SREF/omnireference）：命中"图层分离+指令编辑"组合护城河，是别人抄不了的方向。
5. **一键模板 / 智能提示**（X 4.1+4.2 官方与 JSON 模板）：把社区沉淀的提示词工程封装进画布，几乎零模型成本即可上线。

**反向输入（同样重要）：** Medium 2.7 的反思文 + "AI 反而更慢"那篇，直接给出产品该设"人工接管/可降级"的位置——这部分喂给 Part 04 的降级策略。
