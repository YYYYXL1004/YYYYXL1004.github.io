# Y的个人学术主页

[![Deploy](https://github.com/YYYYXL1004/YYYYXL1004.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/YYYYXL1004/YYYYXL1004.github.io/actions/workflows/deploy.yml)

这是我的个人学术主页仓库，网站地址为
[https://YYYYXL1004.github.io](https://YYYYXL1004.github.io)。

网站主要展示以下内容：

- 个人简介与近期动态
- 论文与研究成果
- 科研项目和竞赛经历
- 个人简历
- GitHub 项目

## 内容维护

常用内容对应的文件如下：

| 内容     | 文件或目录                      |
| -------- | ------------------------------- |
| 个人简介 | `_pages/about.md`               |
| 近期动态 | `_news/`                        |
| 论文列表 | `_bibliography/papers.bib`      |
| 项目经历 | `_projects/`                    |
| 在线简历 | `_data/cv.yml`                  |
| 简历 PDF | `assets/pdf/cv_yaoxianglin.pdf` |
| 社交链接 | `_data/socials.yml`             |
| 站点设置 | `_config.yml`                   |

## 本地预览

推荐使用 Docker：

```bash
docker compose pull
docker compose up
```

打开 <http://localhost:8080> 查看网站。结束预览后运行：

```bash
docker compose down
```

提交前可运行 Prettier 检查格式：

```bash
npm install
npx prettier . --check
```

## 部署

推送到 `main` 分支后，GitHub Actions 会自动构建并部署到 GitHub Pages。部署状态可在仓库的
Actions 页面查看。

## 技术与致谢

本站基于 [Jekyll](https://jekyllrb.com/) 和
[al-folio](https://github.com/alshedivat/al-folio) 构建，并通过 GitHub Pages 托管。
主题按 MIT License 使用，许可证见 [LICENSE](LICENSE)。
