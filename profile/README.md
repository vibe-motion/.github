# 欢迎来到 Vibe Motion 👋

> Prompts → code → motion graphics.

Vibe Motion 专注于用代码创作动画、动态图形和视频。

## 快速开始

- **根据 srt 字幕文件全自动生成视频画面**

  [`vibe-motion/auto-motion`](https://github.com/vibe-motion/auto-motion) 是一个自动视频生成工作流：提供 `transcription.srt`，然后让 Codex 执行 `PROMPT.md`，自动拆分镜头、调用 Claude Code 制作 MG 动画，并拼接生成 `final.mp4`。

  ```bash
  codex exec \
    --cd . \
    --sandbox danger-full-access \
    --ask-for-approval never \
    - < PROMPT.md
  ```

  目前仅支持hyperframes，后续可能会支持remotion或者我改进的vibe-motion

  [查看auto-motion仓库](https://github.com/vibe-motion/auto-motion)

- **2D 动画 -> 手动 vibe coding 2D 动画**

  基于 [Remotion](https://www.remotion.dev/) 的程序化视频与动态图形脚手架。

  ```bash
  npm create vibe-motion@latest my-app
  ```

  [查看create-vibe-motion仓库](https://github.com/vibe-motion/create-vibe-motion)

- **3D 动画 -> 手动 vibe coding 3D 动画**

  基于 [Three.js](https://threejs.org/) 和 [Puppeteer](https://pptr.dev/) 的 3D 动画脚手架，用于确定性地渲染和导出帧序列。

  ```bash
  npm create vibe-motion-3d@latest my-app
  ```

  [查看create-vibe-motion-3d仓库](https://github.com/vibe-motion/create-vibe-motion-3d)

### AI Agent Skills

[`vibe-motion/skills`](https://github.com/vibe-motion/skills) 是给 AI agent 使用的 Vibe Motion skills 集合，适合配合 Claude Code 等智能体快速生成动效。

```bash
npx skills add vibe-motion/skills
```

仓库里已经包含尺子进度动画、Claude Code CLI 打字动画、procedural fish、SVG 组装动效、聚光灯文字 reveal、3D 照片滚动墙、黑胶唱片机、Three.js 地球飞线、微信聊天动效等示例效果。

进群信息和交流方式也在 [`vibe-motion/skills`](https://github.com/vibe-motion/skills#交流) 里。

## join vibe-motion dev team

- 点击 [提交加入申请](https://github.com/vibe-motion/.github/issues/new?title=%E7%94%B3%E8%AF%B7%E5%8A%A0%E5%85%A5%20Vibe%20Motion&body=%E4%BD%A0%E5%A5%BD%EF%BC%8C%E6%88%91%E6%83%B3%E5%8A%A0%E5%85%A5%20Vibe%20Motion%20%E7%BB%84%E7%BB%87%E3%80%82%0A%0A%E6%88%91%E7%9A%84%20GitHub%20%E8%B4%A6%E5%8F%B7%EF%BC%9A%40%0A%0A%E6%88%91%E6%84%9F%E5%85%B4%E8%B6%A3%E7%9A%84%E6%96%B9%E5%90%91%20/%20%E6%83%B3%E5%81%9A%E7%9A%84%E5%86%85%E5%AE%B9%EF%BC%9A%0A)，填写你的 GitHub 账号、感兴趣的方向或想参与的内容，然后创建 Issue。
- 等待维护者审核并添加 `invite-to-org` 标签(好像github没给我推送邮件，可以加我微信主动催我加tag）。
- GitHub Actions 会自动发送组织邀请、留言并关闭 Issue。
- 在 GitHub 通知或注册邮箱中接受邀请，即可加入 Vibe Motion。

## 更多

- [官方网站](https://vibe-motion.github.io/)
