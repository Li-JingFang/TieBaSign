# 贴吧签到Github Action版

## 今日签到状态

![Baidu Tieba Auto Sign](https://github.com/gwtak/TieBaSign/workflows/Baidu%20Tieba%20Auto%20Sign/badge.svg)

## 使用说明1

1. Fork 本仓库，然后点击你的仓库右上角的 Settings，找到 Secrets 这一项，添加一个库秘密变量。其中 `BDUSS` 存放你的 BDUSS。支持同时添加多个帐户，BDUSS 之间用 `#` 隔开即可。

![添加库秘密变量](/img/new_repository_secret.png)
![添加BDUSS](/img/add_BDUSS.png)

2. 设置好环境变量后点击你的仓库上方的 `Actions` 选项，第一次打开需要点击 `I understand...` 按钮，确认在 Fork 的仓库上启用 GitHub Actions 。

3. 任意发起一次commit，可以参考下图流程修改readme文件。

- 打开`README.md`，点击修改按钮

![修改README](/img/edit.png)

- 修改任意内容，这里在末尾插入了空格。移动到最下面，点击提交。

![添加空行](/img/update.png)

4. 至此自动签到就搭建完毕了，可以再次点击`Actions`查看工作记录，如果有`Baidu Tieba Auto Sign`则说明workflow创建成功了。点击右侧记录可以查看详细签到情况。

![查看Action](/img/check.png)

## 报错修改

1.报错信息:Version 3.6 with arch x64 not found
Available versions:

3.10.8 (x64)
3.11.0 (x64)
3.7.15 (x64)
3.8.14 (x64)
3.9.15 (x64)

修改:在main.yml文件中把python的3.6换成3.7.15


