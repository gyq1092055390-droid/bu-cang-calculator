补仓计算器（GitHub Pages 发布说明）

将本项目放到一个 GitHub 仓库后，可通过 GitHub Pages 把 `index.html` 作为静态页面发布：

1. 在仓库根目录推送这些文件（`index.html`、`manifest.json`，可选：图标文件 `icon-192.png`/`icon-512.png`）。
2. 在 GitHub 上打开仓库设置 -> Pages（或在 `Settings` -> `Pages`）：
   - Source 选择 `main` 或 `master` 分支，目录选择 `/ (root)`。
   - 保存后几分钟会生成一个 `https://<your-username>.github.io/<repo>/` 地址。
3. 访问该地址即可看到页面。

本地测试：在包含 `index.html` 的目录运行（Windows PowerShell）：

```powershell
# 在当前目录启动一个简单的静态服务器（需要已安装 Python）
python -m http.server 8000
# 然后在浏览器打开 http://localhost:8000/index.html
```

注意：历史数据保存在浏览器的 `localStorage`，只存在于本地浏览器与设备上；不同设备/浏览器不会同步。