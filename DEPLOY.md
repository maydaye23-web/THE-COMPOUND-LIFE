# 🚀 5 分钟发布速查卡

不想读长 README? 跟着这 7 步, 5 分钟把网站跑起来。

## 准备

- 一个 GitHub 账号（github.com 免费注册）
- 这个项目的所有文件（你已经有了）

## 7 步发布

### 1. 创建仓库

打开 https://github.com/new

- Repository name: `compound-life` （或你喜欢的名字）
- Public（必须公开, GitHub Pages 免费版不支持私有）
- ❌ 不要勾 "Add a README file"（我们已经有了）
- 点 "Create repository"

### 2. 上传文件

在新建的仓库页面点 **"uploading an existing file"** 链接

把这 4 个文件拖进去：
- `index.html`
- `README.md`
- `LICENSE`
- `.gitignore`

底下点 **"Commit changes"**。

### 3. 开启 GitHub Pages

仓库页面 → 顶部 **Settings** → 左边栏 **Pages**

- Source: 选 **Deploy from a branch**
- Branch: 选 **main** + **/ (root)**
- 点 **Save**

### 4. 等 1-2 分钟

GitHub 在后台部署。刷新 Settings → Pages 页面, 上方会出现:

```
Your site is live at https://YOUR_USERNAME.github.io/compound-life/
```

### 5. 打开链接验证

点那个链接, 应该看到你的网页。试试:

- 调整年龄、年薪、消费
- 切换三种职业剧本
- 第 04 幕里点"收益率对比"
- 滚到底点"生成分享图"

### 6. (可选) 加自定义域名

如果你有自己的域名 (比如 `compound.example.com`):

在域名 DNS 管理面板加一条 CNAME 记录:
- Name: `compound` (或你想要的子域)
- Value: `YOUR_USERNAME.github.io`

回到 Settings → Pages, 在 Custom domain 里填 `compound.example.com`, Save。

等 DNS 生效（10 分钟到几小时不等），就可以用自己的域名访问了。

### 7. 把链接发给朋友

完成。

复制 `https://YOUR_USERNAME.github.io/compound-life/` 这个链接, 转发到微信群、朋友圈、X、小红书……

## 后续修改

修改 `index.html` 后:

**网页方式（不用命令行）**:
- 仓库里点 `index.html`
- 右上角铅笔图标 ✏️ 编辑
- 改完滚到底点 "Commit changes"
- 1-2 分钟后线上自动更新

**命令行方式**:
```bash
git clone https://github.com/YOUR_USERNAME/compound-life.git
cd compound-life
# 修改 index.html
git add index.html
git commit -m "your changes"
git push
```

## 常见问题

**Q: 链接打开是 404?**
A: 等 1-2 分钟。第一次部署需要时间。

**Q: 字体加载很慢?**
A: 中国大陆访问 Google Fonts CDN 可能慢。如果是给国内用户为主用, 可以考虑后续把字体文件本地化 (TODO).

**Q: 怎么换二维码?**
A: 把你的二维码图片传到仓库根目录 (比如 `qrcode.png`), 然后编辑 `index.html`, 搜索 `<div class="sc-qr"></div>`, 替换为 `<img src="qrcode.png" style="width:140px;height:140px;border-radius:16px">`。

**Q: 想用 Vercel / Netlify 而不是 GitHub Pages?**
A: 都行, 这就是个静态文件。Netlify 最快: 直接拖 `index.html` 到 https://app.netlify.com/drop 即可。

---

有问题 → 提 Issue
觉得好 → Star ⭐
