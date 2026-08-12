# Changelog

##### **2026年8月12日（v0.1.3）**

English:
- Bump version to 0.1.3
- Wire task completion notification setting and show an in-panel toast when a turn finishes
- Make Stop kill Grok/Kimi/OpenCode/Pi CLI children; suppress toast/sound after user abort
- Treat Codex Aborted as a quiet interrupt instead of a chat ERROR bubble
- Fix intermittent leftover chat after "new session" (cancel deferred updateMessages, hard clear, remount list)
- Open new chat panels as stacked editor tabs in the same group instead of side-by-side splits

中文:
- 版本升级到 0.1.3
- 打通任务完成通知设置：回合结束时显示面板内 toast
- Stop 可可靠终止 Grok/Kimi/OpenCode/Pi 子进程；用户主动中止后抑制完成 toast/音效
- Codex 中断按安静处理，不再弹出 ERROR 气泡
- 修复偶现「新会话仍显示旧对话」（取消延迟消息回写、强制清空、重挂载列表）
- 新页签改为同一编辑器组叠开，不再左右分屏

##### **2026年8月11日（v0.1.2）**

English:
- Bump version to 0.1.2
- Fix Grok history: restore attached images when reloading sessions
- Fix Grok session titles: prefer typed user_query over English AI generated_title (including image turns)
- Fix Grok image send: pass attachments via `--prompt-file` so the model can see images (UI no longer shows a false optimistic-only image)
- Fix tool spinners stuck pending after multi-step agent turns / stream end

中文:
- 版本升级到 0.1.2
- 修复 Grok 历史重载后用户附件图片丢失
- 修复 Grok 会话标题：优先使用用户输入原文，不再误用英文 AI 标题（含带图消息）
- 修复 Grok 发图：通过 `--prompt-file` 把附件真正传给模型（避免仅 UI 有图、模型看不到）
- 修复多步工具调用结束后转圈不消失的问题

##### **2026年8月10日（v0.1.1）**

English:
- Bump version to 0.1.1
- Fix chat toolbar selectors clipped by overflow (config / provider / mode unclickable)
- Fix revoking local settings.json authorization
- Surface Codex/Claude send failures in chat; swallow success JSON envelopes
- Fix Grok/CLI history isolation

中文:
- 版本升级到 0.1.1
- 修复底部工具栏配置/供应商/模式按钮菜单被裁切导致点不动
- 修复取消本地 settings.json 授权无效
- 发送失败在聊天区展示；成功结果 JSON 不再误入正文
- 修复 Grok/CLI 历史隔离

##### **2026年8月10日（v0.1.0）**

English:
- Bump version to 0.1.0 for Marketplace-compatible SemVer
- Clean packaging ignores (drop tests, sql.js debug builds, non-dist webview files)
- Remove personal local paths from README packaging instructions

中文:
- 版本升级到 0.1.0，符合 Marketplace 的 SemVer 要求
- 收紧打包忽略规则（排除测试、sql.js debug 构建、非 dist 的 webview 文件）
- 移除 README 打包说明中的个人本机路径

##### **2026年8月5日（v0.0.2-fix2）**

English:
- Add `enableDebugLog` setting (default off) and show Webview DevTools only when enabled
- Fix chat input drag-and-drop for files from Explorer (path references and images)
- Improve dependency detection and permission approvals

中文:
- 新增「调试日志」开关（默认关闭），仅开启时显示 Webview 开发者工具按钮
- 修复输入框拖放：支持从资源管理器拖入文件路径引用与图片
- 改进依赖检测与权限审批

##### **2026年8月4日（v0.0.1）**

English:
- Migrate JetBrains CC GUI to VS Code

中文:
- 迁移 JetBrains CC GUI 到 VSCode
