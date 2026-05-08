# 复利人生 · The Compound Life

> 写给所有相信 **FIRE** 的年轻人 —— 一个属于你自己的复利梦

[![Made for FIRE](https://img.shields.io/badge/Made_for-FIRE-2A8F47?style=flat-square)]()
[![Pure HTML](https://img.shields.io/badge/Stack-Pure_HTML-1A1A1A?style=flat-square)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-D4AF5A?style=flat-square)]()

---

## 这是什么

如果你是一个相信 FIRE（Financial Independence, Retire Early）、希望有一天**让钱替你工作**的年轻人 —— 这个工具是给你的。

它不是计算器，是一面镜子。

填几个数字 —— 你的年龄、年薪、本金、消费、期望收益率 —— 它会告诉你：

> **再过 X 年，你就能让钱替你工作。那一年，你 X 岁。**

然后画出两条曲线，一条是"复利的你"，一条是"不投资的你"。30 年后，它们之间的差距可能是几百万、上千万 —— **这就是你和复利的距离**。

## 为什么要做这个

我相信一件事：**复利是把普通人从"为钱工作"中解放出来的最重要手段**。

但大多数人对复利的理解停留在公式层面。看到 "8% 年化、30 年" 不会有任何感觉。直到他们**亲眼看见两条命运曲线发散的瞬间**，那个"卧槽，原来差这么多"的瞬间，才会真正开始行动。

这个工具想做的，就是**制造那个瞬间**。

3 分钟，让你看见自己未来的财务形状。然后，希望你今天就开始做点什么。

## 核心理念

**1. 真实，不浪漫化**

不会告诉你"长期投资稳赚 10%"这种话。事实上工具里写得很清楚：A 股个人投资者的中位数甚至是亏损的。**收益率只是假设，不是承诺**。

**2. 故事，不仅是数字**

每张图、每个数字背后都有一个具体的人生场景：
- "再过 9 年，你就能让钱替你工作 —— 那一年你 37 岁"
- "45 岁那年，你离开了职场主战场。但你不慌 —— 复利账户里有 830 万"
- "★ 财富自由那一年" / "⚠ 退休那一年"

**3. 普通人的逻辑**

不是给金融从业者用的高级工具。是给一个 28 岁、月薪两万、不太懂理财、但想为自己未来做点什么的年轻人用的。

## 它能做什么

- ✅ **职业剧本** — 奋斗型 / 稳健型 / 温和型，三种人生轨迹一键切换
- ✅ **完全可调参数** — 涨薪频率、顶薪封顶、退休年龄、之后的收入，全部可改
- ✅ **消费随年龄上涨** — 把"结婚、买房、生娃"摊到每年的消费上涨里，比一次性算冲击更接近真实
- ✅ **起始本金支持负数** — 学贷、信用卡债，如实呈现
- ✅ **收益率四档对比** — 0% / 3% / 6% / 10% 同图叠加，外加自定义档位
- ✅ **可编辑的逐年表** — 表格里点击任何一年，可以直接改"年薪"或"消费"，模拟跳槽、买房等人生大事件，曲线实时同步
- ✅ **时间轴叙事** — 拖动看每一年的故事，关键节点会自动高亮
- ✅ **一键分享** — 生成 9:16 竖版分享图，曲线版 / 表格版双版本，朋友圈适配

## 设计哲学

> 复利是世界第八大奇迹。懂它的人 —— 赚到它。不懂它的人 —— 付给它。
>
> — Albert Einstein

工具做了一些**刻意的简化**，因为我相信"清晰的故事"比"精确的预测"更有力量：

- 收益率取常数，不模拟波动
- 不计算通胀和税
- 不考虑社保 / 公积金
- 不推荐具体投资产品

这些都是取舍。如果你需要严肃的退休规划，请咨询持牌财务顾问。这个工具的目标是**让你产生想咨询的冲动**。

## 技术栈

纯前端单文件应用，**零构建依赖**：

- 原生 HTML / CSS / JavaScript
- [Chart.js](https://www.chartjs.org/) —— 数据可视化
- [html2canvas](https://html2canvas.hertzen.com/) —— 分享图生成
- 字体：Inter、Manrope、思源黑体、思源宋体（Google Fonts CDN）

整个项目就是一个 `index.html` 文件，没有 build、没有依赖管理、没有服务器，**双击就能跑**。

## 本地运行

```bash
git clone https://github.com/YOUR_USERNAME/compound-life.git
cd compound-life
# 直接打开 index.html
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

或者用静态服务器：

```bash
python3 -m http.server 8000   # 然后访问 http://localhost:8000
```

## 部署到 GitHub Pages

这是一个完全静态的网页，部署成本为零。

1. **创建仓库** —— GitHub 上新建一个公开仓库（比如叫 `compound-life`）
2. **上传文件** —— 把项目里的 `index.html` 和 `README.md` 传上去
3. **开启 Pages** —— 仓库 Settings → Pages → Source 选 `main` 分支 → Save
4. **等待部署** —— 1-2 分钟后访问 `https://YOUR_USERNAME.github.io/compound-life/`

完成。把链接发给你身边正在思考"还要打多少年工"的朋友。

### 自定义域名

Settings → Pages → Custom domain 填入你的域名，再在域名 DNS 里加一条 CNAME 记录指向 `YOUR_USERNAME.github.io` 即可。

## 自定义你自己的版本

### 替换分享图里的二维码和品牌

分享图底部有一个二维码占位框和"复利人生 / The Compound Life"品牌文字。打开 `index.html`，搜索 `sc-qr` 找到位置：

```html
<div class="sc-footer-brand">
  <div class="sc-qr"></div>                <!-- 替换为你的二维码 -->
  <div class="sc-brand-text">
    <div class="sc-brand-name">复利人生</div>      <!-- 你的品牌名 -->
    <div class="sc-brand-tag">扫码体验你自己的曲线</div>  <!-- 你的标语 -->
  </div>
</div>
```

把空的 `<div class="sc-qr"></div>` 替换成 `<img src="qrcode.png" />`，把图片放到项目根目录即可。

### 调整职业剧本默认值

搜索 `const SCENARIOS =`，根据你的目标人群修改起薪、涨薪频率、顶薪等参数。

### 调整收益率档位

搜索 `data-return="0"`，可以改成你想要的档位组合。

## 路线图

短期想加的：

- [ ] 真实二维码集成（指向工具本身）
- [ ] 多人生路径并排对比（保存 A / B 两套配置）
- [ ] 数据导出（导出为 CSV）
- [ ] 黑暗模式

长期可能加的：

- [ ] 蒙特卡洛模拟（让收益率有不确定性）
- [ ] 通胀调整开关
- [ ] 税收 / 社保的可选模型

欢迎提 Issue 说你想要什么。

## 给我反馈

如果这个工具让你 "卧槽" 了一下，或者让你今天就打开了券商 App —— 告诉我。

如果你觉得哪里看不懂、哪里数字不对、哪里设计反人类 —— 也告诉我。

提 Issue、发 PR，或者 [其他联系方式]。

## License

[MIT License](LICENSE) —— 你可以自由使用、修改、分发。如果对你有帮助，请考虑保留一行 "Powered by 复利人生" 或类似的来源说明。

---

> *能让你今天就开始投资的工具，胜过让你 30 年后才后悔的工具。*

*Made with ☕ and a deep respect for compound interest.*
