# 考研助手

考研备考打卡 + 计时 + 伴侣监督 PWA 应用

## GitHub Pages 部署步骤（iPhone可用）

### 第一步：创建 GitHub 仓库

1. 打开 [github.com](https://github.com) 注册/登录
2. 点击右上角 `+` → `New repository`
3. Repository name 填 `kaoyan-helper`（可自定义）
4. 选择 `Public`
5. 点击 `Create repository`

### 第二步：上传文件

**方法A - 网页直接上传（最简单）：**

1. 在新仓库页面点击 `uploading an existing file`
2. 把本文件夹内**所有文件和文件夹**（index.html、assets文件夹、bg-mountain.jpg、icon-192.png、manifest.json、sw.js）拖进去
3. 点击 `Commit changes`

**方法B - 命令行上传：**

```bash
git clone https://github.com/你的用户名/kaoyan-helper.git
cd kaoyan-helper
# 把所有文件复制进来
git add .
git commit -m "init"
git push origin main
```

### 第三步：启用 GitHub Pages

1. 仓库页面 → `Settings`（顶部标签）
2. 左侧菜单 → `Pages`
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `main`，文件夹选 `/ (root)`
5. 点击 `Save`
6. 等待1-2分钟，刷新页面，会看到绿色提示：
   `Your site is live at https://你的用户名.github.io/kaoyan-helper/`

### 第四步：iPhone 添加到主屏幕

1. Safari 打开上面的链接
2. 点击底部分享按钮（方框+向上箭头）
3. 选择「添加到主屏幕」
4. 点击「添加」

桌面会出现「考研助手」图标，以后直接点开使用。

### 功能介绍

- **今日** - 学习时长仪表盘、快速开始、打卡、名言、意图、任务清单
- **计时** - 多项目正计时（支持暂停/继续）、每日上限提醒
- **伴侣** - 双角色切换（备考者/监督人）、查看对方数据、留言互动
- **统计** - 周/月/200天统计、每日趋势图、备考打卡热力图
- **设置** - 角色切换、项目编辑、定时提醒

### 数据存储

所有数据保存在手机本地（localStorage），换手机或清除浏览器数据会丢失。
