# Rime 朙月拼音輸入法基礎設定

最近重灌 Windows 11，輸入法設定好久。在這裡記錄一些自己 Rime 常用的設定，也給大家參考 ^_^ （其他檔案僅作備份，建議直接找原出處以便獲得最新版本哦！）

--

1. 台灣習慣用字

着、著 兩岸三地使用不同，所以有不同用字。

到 `C:\Users\pen\AppData\Roaming\Rime\` 內新建 `luna_pinyin_tw.schema.yaml`，貼上[這段程式](https://github.com/rime/rime-luna-pinyin/blob/master/luna_pinyin_tw.schema.yaml)。

接著右鍵點擊右下深灰色「中」字重新部署，就可以看到變化。（可以輸入「體」，骨字上面的內部是在右下角就是台灣正體）

--

2. 輸入界面

請到 `C:\Users\pen\AppData\Roaming\Rime\weasel.custom.yaml` 加入下列程式碼

  style/horizontal: true  # 橫向，要直向就不要這條
  style/font_face: "Noto Sans CJK TC Medium"  # 確保電腦有 Noto Sans，沒有的話到記事本內，找你喜歡的字體輸入進來
  style/font_point: 20 
  
接著右鍵點擊右下深灰色「中」字重新部署，就可以看到變化。

--

3. Emoji 表情符號

請到[這裡](https://github.com/rime/rime-emoji)下載檔案，然後將 `opencc` 的資料夾複製到 `C:\Users\pen\AppData\Roaming\Rime` 底下。同時將 `emoji_suggestion.yaml` 的程式貼到 `C:\Users\pen\AppData\Roaming\Rime\default.custom.yaml`。

接著右鍵點擊右下深灰色「中」字重新部署，就可以看到變化。（可以輸入類似「hua」來測試看看）
