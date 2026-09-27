# 字幕檔放置說明

把 yt-dlp 抓下來的 `.vtt`（或 `.srt`）檔直接放在這個資料夾，檔名保留 yt-dlp 的預設格式即可，例如：

```
01_uw971NaMvog.zh-TW.vtt
32_U4CW3YrljDs.zh.vtt
```

檔名中的 11 碼影片 ID 會用來對回 `data/kuo_playlist_videos.json` 裡的標題與頻道。

## 在你的電腦上要做的事

```bash
# 第一次才需要 clone
git clone https://github.com/wcl0503/ML-repo.git
cd ML-repo

git fetch origin
git checkout claude/guo-yuuren-methodology-analysis-uwglql
cp /path/to/kuo-subs/*.vtt data/subtitles/
git add data/subtitles
git commit -m "Add subtitles for Kuo Yu-jen playlist"
git push origin claude/guo-yuuren-methodology-analysis-uwglql
```

音訊與影片檔（m4a、mp3、mp4）不要放進倉庫，已在根目錄 `.gitignore` 排除。
