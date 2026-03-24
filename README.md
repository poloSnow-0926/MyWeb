# 极简高级个人网站

这是一套可以直接部署到 `Cloudflare Pages` 的静态个人网站模板，适合第一次做个人站的人起步。

## 文件说明

- `index.html`：页面结构和文案
- `style.css`：页面样式
- `script.js`：年份和滚动显现动画

## 你最先要改的地方

打开 `index.html`，优先替换这些内容：

- `你的名字`
- `中国 · 你的城市`
- `hello@example.com`
- `https://github.com/yourname`
- `https://www.linkedin.com/in/yourname`

你也可以把各个段落文案改成你自己的介绍、兴趣和项目。

## 本地预览

直接双击 `index.html` 就能看静态效果。

如果你想用本地服务预览，可以在当前目录执行：

```bash
python -m http.server 8080
```

然后打开 [http://localhost:8080](http://localhost:8080)。

## 部署到 Cloudflare Pages

1. 把当前目录上传到 GitHub 仓库。
2. 登录 `Cloudflare` 后台。
3. 进入 `Workers & Pages`。
4. 选择 `Create application` -> `Pages` -> `Connect to Git`。
5. 连接你的 GitHub 仓库。
6. 部署配置填写：

```text
Production branch: main
Build command: exit 0
Build output directory: .
```

7. 点击 `Save and Deploy`。
8. 部署完成后，先访问 `*.pages.dev` 地址确认页面正常。
9. 再去 `Custom domains` 里绑定你自己的域名。

## 建议

第一版别贪多，先把名字、介绍、联系方式和 3 个重点方向改成自己的内容，能上线就已经赢了一大半。
