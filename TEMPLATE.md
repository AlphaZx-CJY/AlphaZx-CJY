# GitHub Profile 模板使用说明

## 📁 项目结构

```
github-profile/
├── README.md              # 主 Profile 页面（核心文件）
├── assets/
│   └── header.svg         # 自定义 SVG 横幅
├── .github/
│   └── workflows/
│       └── snake.yml      # 贪吃蛇动画生成工作流
└── TEMPLATE.md            # 本说明文档
```

## 🚀 快速开始

### 1. 创建仓库

在 GitHub 上创建一个与您的用户名相同的仓库：
- 仓库名：`AlphaZx`（替换为您的用户名）
- 设置为 Public
- 勾选 "Initialize this repository with a README"

### 2. 上传文件

将本项目的所有文件上传到该仓库：

```bash
# 克隆您的 profile 仓库
git clone https://github.com/AlphaZx/AlphaZx.git
cd AlphaZx

# 复制本项目的文件
cp -r ../github-profile/* .

# 提交并推送
git add .
git commit -m "Initial profile setup"
git push origin main
```

### 3. 启用 GitHub Actions

进入仓库的 **Actions** 标签页，启用 workflows。

### 4. 配置 GitHub Pages（可选）

如需托管资源文件：
- 进入 **Settings → Pages**
- Source 选择 `gh-pages` 分支

## 🎨 自定义修改

### 修改个人信息

编辑 `README.md` 中的以下内容：

1. **用户名** - 将所有 `AlphaZx` 替换为您的 GitHub 用户名
2. **地理位置** - 修改坐标 `N31°14' E121°29'` 和 `Shanghai, China`
3. **技能标签** - 在 Tech Stack 部分添加/删除技能徽章
4. **工作经历** - 在 Experience 部分更新您的工作经历
5. **项目展示** - 在 Featured Projects 部分更新项目卡片

### 技能徽章代码

访问 [shields.io](https://shields.io) 和 [simpleicons.org](https://simpleicons.org) 获取更多徽章：

```markdown
![Name](https://img.shields.io/badge/Name-Color?style=for-the-badge&logo=icon&logoColor=white)
```

### 统计卡片

- **GitHub Stats**: `https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME`
- **Top Languages**: `https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME`
- **Streak Stats**: `https://streak-stats.demolab.com?user=YOUR_USERNAME`
- **贡献图**: `https://github-readme-activity-graph.vercel.app/graph?username=YOUR_USERNAME`

## 🔧 高级配置

### 贪吃蛇动画

`.github/workflows/snake.yml` 会自动生成贡献图的贪吃蛇动画：
- 每天自动更新
- 支持亮色/暗色主题
- 需要开启 GitHub Actions 权限

### 自定义主题颜色

修改所有 URL 中的颜色参数：
- `bg_color=0D1117` - 背景色（深色）
- `title_color=58A6FF` - 标题色（蓝色）
- `text_color=C9D1D9` - 文本色（浅灰）

## 📱 效果预览

![Profile Preview](./assets/preview.png)

## 📝 参考资料

- [GitHub Profile README Generator](https://rahuldkjain.github.io/gh-profile-readme-generator/)
- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)

## ⚠️ 注意事项

1. 外部服务（如 Vercel）可能有访问限制，如遇加载问题请稍后重试
2. 统计卡片数据有缓存，更新可能延迟几小时
3. 建议定期检查链接是否有效

---

Made with ❤️ by AlphaZx
