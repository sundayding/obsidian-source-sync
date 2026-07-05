# Obsidian Source Sync

Obsidian Source Sync 是一个 Obsidian 桌面端插件，用于将小红书 / RedNote 的收藏、点赞、我的发布、专辑、图片、视频和评论同步到本地 Obsidian 知识库文件夹（Vault）。

出品：`坦丁|场景化AI知识库`

## 安装方式一：BRAT（推荐，可自动更新）

推荐使用 BRAT 安装。这样后续发布新版本时，BRAT 可以跟随 GitHub Release 自动检测和更新插件。

1. 在 Obsidian 社区插件中安装并启用 `BRAT`。
2. 打开 BRAT，选择 `Add Beta plugin`。
3. 输入这个仓库地址：

```text
https://github.com/sundayding/obsidian-source-sync
```

4. 安装完成后，进入 Obsidian “设置 -> 第三方插件”，启用 `Obsidian Source Sync`。
5. 插件会安装到 `.obsidian/plugins/multi-source-sync/`，这是由插件 ID 决定的正常路径。

## 试用与授权

- 试用版可同步 100 篇笔记。
- 永久版授权后可解锁无限同步、更多评论同步、评论回复、本地视频转文字、AI 分类和评论洞察。
- 永久版授权码通过小红书订单流程发送，在 Obsidian 插件设置页的“授权与试用”区域填写并验证。
- 插件通过 `https://multi-source-sync.pages.dev/v1/license/verify` 校验授权码和设备绑定。

## 手动安装备用方式

如果 BRAT 或 GitHub 暂时不可用，可以使用小红书订单自动发货或私信中的云盘备用包。

手动安装时，把 `multi-source-sync` 文件夹放到你的 Obsidian 知识库文件夹：

```text
Vault/.obsidian/plugins/multi-source-sync/
```

确认 `main.js`、`manifest.json`、`styles.css` 直接位于 `multi-source-sync` 文件夹下，然后重启 Obsidian，并在“设置 -> 第三方插件”中启用 `Obsidian Source Sync`。

已有安装升级时，只需要更新 `.obsidian/plugins/multi-source-sync/` 里的这些插件程序文件：

- `main.js`
- `manifest.json`
- `styles.css`

不要删除或覆盖 `data.json`，也不要删除已同步的 Markdown、媒体目录、账号目录或其他 Vault 内容。

## 本地优先与隐私边界

- 同步后的 Markdown、媒体和评论写入你的本地 Obsidian 知识库文件夹。
- 小红书账号数据、授权码、设备 ID 和 AI API Key 保存在本地插件数据中。
- 授权服务只校验授权码和设备绑定状态，不处理你的同步内容。
- AI 分类和评论洞察只有在你主动开启并配置 API Key 后才会调用。

## 购买与支持

购买、授权码、安装支持和售后问题，请通过小红书订单或私信联系 `坦丁|场景化AI知识库`。
