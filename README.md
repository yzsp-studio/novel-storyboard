<div align="center">

# 🎬 novel-storyboard

## 镜头认领剧本节拍，18 道质量门当场对账
## Shots claim story beats, and 18 quality gates audit every cut

📮 **商务合作 / Business：wow.vip@foxmail.com**
🎬 **抖音 / Douyin：[v.douyin.com/07EjIDGVErY](https://v.douyin.com/07EjIDGVErY/)**

</div>

---

## 🇨🇳 中文

这是一个给 AI 短剧出分镜的三层结构工具：段（一次视频生成，≤15 秒）→ 分镜（段内 2–5 秒的剪切，认领剧本节拍）→ 分镜图（每切一张关键帧，主分镜图钉 0.00 秒，子分镜图钉各自切点）。每个镜头声明覆盖剧本某场的哪几个连续节拍，镜头不许跨场次，换景必换镜，剧本改动后重跑校验会当场点名失效镜头。每段自带一条 H3 视频提示词，对齐指令与 [Shot k] 切点时刻由分镜结构推导并逐字对账，台词逐字进 <d> 块。产出 storyboard.json、Markdown 与单页评审报告，18 道质量门由脚本确定性检查，export 一键导出投产包；零依赖、零 API key。

### ✨ 能做什么

- 镜头认领剧本节拍（sceneIndex + beats 起止），不许跨场次，换景必换镜
- 单镜头时长上限按模型设置（默认 ≤15 秒），长对话强制拆镜；台词秒数 ≤ 镜头秒数逐镜检查
- 每段一条 H3 视频提示词：对齐指令、台词 <d> 块、声景、配乐一次带全
- 分镜图提示词与镜头正文分离，中文景别词必须写进画面提示词
- 输出 storyboard.json + Markdown + 单页评审报告（分镜节奏带 / 分集分镜表 / 生成批次单 / 配音对齐单）
- 18 道质量门脚本确定性检查，export 一键导出投产包；零依赖、零 API key

### 📦 包含的技能

- `novel-storyboard` —— 见 [`novel-storyboard/SKILL.md`](novel-storyboard/SKILL.md)

### 🚀 安装

```bash
git clone https://github.com/yzsp-studio/novel-storyboard.git
cp -r novel-storyboard/* "$DSH_HOME/skills/"
```

> 技能是**纯文本说明**（`SKILL.md` + `references/`），零依赖、零 API key，用你当前 agent 的会话额度。

---

## 🇬🇧 English

This is a three-layer storyboard tool for AI short drama: segment (one video generation, up to 15 seconds), shot (a 2-5 second cut inside the segment that claims story beats), and storyboard frame (one keyframe per cut, with the main frame pinned at 0.00s and sub-frames pinned at their cut points). Every shot declares which consecutive beats of which scene it covers; shots may not cross scenes, so a scene change always means a new shot, and re-running validation after a script edit names the shots that went stale. Each segment carries one H3 video prompt where the alignment instruction and [Shot k] cut times are derived from the storyboard structure and reconciled word by word, with dialogue going verbatim into <d> blocks. It outputs storyboard.json, Markdown, and a one-page review report; 18 quality gates are checked deterministically by script, and export produces the production pack—zero dependencies, zero API keys.

### ✨ What it does

- Shots claim story beats (sceneIndex plus beat start/end); no shot crosses scenes, so a scene change forces a new shot
- Per-shot duration cap is model-driven (15 seconds by default) with forced splitting, and dialogue seconds are checked against shot seconds cut by cut
- One H3 video prompt per segment: alignment instruction, dialogue in <d> blocks, soundscape, and score all in one
- Storyboard frame prompts stay separate from shot body text, with Chinese shot-size terms required in the frame prompt
- Outputs storyboard.json, Markdown, and a one-page review report (rhythm band, per-episode table, generation batch sheet, dubbing alignment sheet)
- 18 quality gates checked deterministically by script, plus one-command export of the production pack; zero dependencies, zero API keys

### 📦 Skills included

- `novel-storyboard` — [`novel-storyboard/SKILL.md`](novel-storyboard/SKILL.md)

### 🚀 Install

```bash
git clone https://github.com/yzsp-studio/novel-storyboard.git
cp -r novel-storyboard/* "$DSH_HOME/skills/"
```

> Skills are **plain-text instructions** (`SKILL.md` + `references/`). Zero dependencies, no API keys — they run on your agent's existing session quota.

---

## 📮 联系 / Contact

| | |
|---|---|
| 🎬 **抖音 / Douyin** | [https://v.douyin.com/07EjIDGVErY/](https://v.douyin.com/07EjIDGVErY/) |
| 📮 **商务合作 / Business** | **wow.vip@foxmail.com** |
| 🐙 **GitHub** | [https://github.com/yzsp-ai](https://github.com/yzsp-ai) |
| 💖 **打赏 / Support** | [afdian.com/a/yzsp-ai](https://afdian.com/a/yzsp-ai) |

## 📄 License

[MIT](LICENSE) · © 2026 [yzsp-ai](https://github.com/yzsp-ai)
