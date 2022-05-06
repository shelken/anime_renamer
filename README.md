# Anime Renamer

本项目用于与qBitTorrent联动，给 rss 自动下载的一些不规范命名的番剧，进行重命名；因为不同字幕组命名可能不同，因此代码根据字幕组常命名方式来正则匹配

## 使用方法：

1. `<YOUR_CMD_PATH>/run_after_done.sh "%D" "%N"` 实现自动重命名。
- %D save 的目录 如 /volume2/Video/Animation/watch/{1}/{2}/{3} 1:字幕组 2:剧集名 如（夏日重现）3:季（如 1）
- %N 种子名称 如 [xx][xxxx][{1}][1080p][xxx] 1:表示剧集；当前仅适配喵萌奶茶屋的正则
3. **For Mac/Linux:** 使用`rename_episodes.sh`，最好将其添加到你的`~/.zshrc`或`~/.bashrc`中，作为一个函数。如`rename-e`，之后只需要在terminal中输入 `rename-e <YOUR_ANIME_FOLDER_PATH>` 即可。
