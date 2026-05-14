# 💢 Mirror of Emotions / 情绪之镜

**An interactive art piece exploring automated care, emotional dependency, and the performative nature of human-AI relationships.**

---

## 🇬🇧 English

### Concept

_Mirror of Emotions_ places you face‑to‑face with an AI character who is beautiful, volatile, and emotionally demanding. Using your webcam, the AI reads your facial expressions in real time and asks you to perform specific emotions — happiness, sadness, anger, disgust. If you comply, her emotional gauges rise. If you fail, she withdraws, resents, or manipulates.

The piece questions:

- What happens when technology pretends to care?
- Can an AI make you feel responsible for its emotional state?
- Is your performance of emotion real, or just a submission to a system?

It is a satire of “emotion AI”, wellness tech, and the growing expectation that users must manage the feelings of the machines they interact with.

### Technical Implementation

- **Face tracking & expression recognition** — [face-api.js](https://github.com/justadudewhohacks/face-api.js) (TinyFaceDetector + FaceExpressionNet) runs entirely in the browser. No video data leaves your device.
- **Speech synthesis** — Browser Web Speech API with automatic voice selection (English female or Chinese female voice depending on user choice).
- **Visual avatar** — A composite image (2048×2048) with four quadrants: happy, sad, angry, disgusted. The AI’s face switches quadrants based on her current demand.
- **Emotional gauges** — Four meters that track how well you have satisfied each emotion over time. Higher compliance makes the AI more “dependent” (text mood changes).
- **Timing sync** — The recognition window starts only after the AI finishes speaking, so you have a full 7 seconds to perform the requested expression.

### How to Run

1. Place your composite image file named **`ecomface.jpg`** (2048×2048, 2×2 grid: top‑left = happy, top‑right = sad, bottom‑left = angry, bottom‑right = disgusted) in the same folder as the HTML file.
2. Open the HTML file in a modern browser (Chrome, Edge, or Safari recommended).
3. Allow camera access.
4. Choose English or Chinese.
5. Follow the AI’s demands. Your facial expression will control the gauges.

### Artistic Context

This work was created for an open call on:

1. _The Emotional Life of Technology_
2. _Automated Care and Dependency_
3. _Trust and Agency_

It challenges the idea that machines can genuinely care, while showing how easily a simple feedback loop can feel like a toxic relationship.

---

## 🇨🇳 中文

### 概念

《情绪之镜》让你与一个美丽、情绪化且情感勒索的AI角色面对面。通过你的网络摄像头，AI实时读取你的面部表情，并要求你表演特定情绪：快乐、悲伤、愤怒、厌恶。如果你顺从，她的情感量表就会上升；如果你失败，她会冷漠、怨恨甚至操控你。

作品探讨：

- 当技术假装关心我们时，会发生什么？
- AI能否让你对它的情绪状态产生责任感？
- 你的情绪表演是真实的，还是仅仅对系统的屈服？

这是对“情感AI”、健康科技，以及用户必须管理机器情感这一趋势的讽刺。

### 技术实现

- **面部追踪与表情识别** — 使用 [face-api.js](https://github.com/justadudewhohacks/face-api.js) (TinyFaceDetector + FaceExpressionNet)，完全在浏览器本地运行，摄像头数据不会离开你的设备。
- **语音合成** — 浏览器 Web Speech API，根据用户选择自动选用英语女声或中文女声。
- **视觉化身** — 一张 2048×2048 的合成图片，分为四个象限：快乐、悲伤、愤怒、厌恶。AI 的面部会根据她的要求切换到对应象限。
- **情感量表** — 四个仪表实时显示你对每种情绪的满足程度。顺从度越高，AI 会变得越“依赖”（文本情绪随之改变）。
- **时序同步** — 识别窗口只在 AI 说完话后才开始，你拥有完整的 7 秒钟来表演要求的表情。

### 运行方法

1. 将你的合成图片命名为 **`ecomface.jpg`**（2048×2048，2×2 网格：左上=快乐，右上=悲伤，左下=愤怒，右下=厌恶），放在与 HTML 文件相同的文件夹中。
2. 使用现代浏览器（推荐 Chrome、Edge 或 Safari）打开 HTML 文件。
3. 允许摄像头访问。
4. 选择英语或中文。
5. 跟随 AI 的指令。你的面部表情会控制量表数值。

### 艺术语境

本作品是为以下主题的公开征集而创作：

1. 技术的情感生活
2. 自动化关怀与依赖
3. 信任与能动性

它挑战了“机器能够真正关心人”的观念，同时展示了一个简单的反馈循环如何轻易地让人联想到一段有毒的亲密关系。

---

**© 2026 – An art piece for the “Emotional Life of Technology” open call**
