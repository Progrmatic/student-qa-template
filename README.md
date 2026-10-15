# 學員提問 repo

**繁體中文** | [English](README.en.md)

這個 repo 是空的，是讓你和講師討論用的模板。請照下面的步驟，用它建立**你自己的** repo，把你的作業程式碼放進去，之後的提問與 code review 都在你的 repo 裡進行。你的 repo 是私人的，只有你和講師看得到。

> **請不要在這個 repo 發問。** 這裡是所有學員共用的模板，請在你自己建立的 repo 開 issue。

## 一、建立你自己的 repo

### 1. 用「Use this template」建立你的 repo

這個 repo 是公開的，不用等任何邀請就能開始。購買課程後 GitHub 可能會寄來加入這個 repo 的邀請，接受或忽略都可以，不影響後面的步驟。

在這個 repo 的頁面右上角，按 **Use this template** → **Create a new repository**，然後：

| 欄位 | 怎麼填 |
|---|---|
| Owner | 你自己的 GitHub 帳號 |
| Repository name | 自己取，例如課程名稱 |
| Visibility | **Private**（建議） |
| Include all branches | 不用勾 |

按 **Create repository** 就完成了。

> **請不要用 Fork。** 從公開 repo fork 出來的 repo 一定是公開的，你的作業和提問會被所有人看到；平台也不接受連結這個 repo 的 fork。用「Use this template」建立的 repo 可以設成 Private，完全屬於你自己。

### 2. 在課程頁連結你的 repo

1. 回到 Progrmatic 的課程頁，找到「GitHub 協作」區塊。
2. 貼上你剛建立的 repo 網址，例如 `https://github.com/你的帳號/repo名稱`。
3. 按 **連結並安裝 App**，會帶你到 GitHub 安裝課程的 GitHub App。
4. 在 GitHub 上選 **Only select repositories**，**只選你剛建立的這個 repo**，然後儲存。
5. GitHub 會自動帶你回到平台。講師會以可寫入（push）的權限加入你的 repo，通常幾秒內完成。

### 3. 確認 Issues 已開啟

平台通常會自動幫你開啟 Issues。如果你的 repo 上方沒有 **Issues** 分頁，請到 **Settings → General → Features**，勾選 **Issues**。

## 二、遇到問題：開一個 issue

到你的 repo 的 **Issues → New issue**，選一個模板。每個模板都有中文版和英文版，選你習慣的語言即可：

| 模板 | 什麼時候用 |
|---|---|
| **卡關／提問** | 作業或實作卡住了、測試過不了、看不懂某段程式 |
| **請講師 review** | 寫好了，想請講師看寫法、設計或還能怎麼改 |
| **教材勘誤** | 影片、投影片或課程的範例程式碼有錯字、錯誤或過時的地方 |

模板會一格一格引導你，把講師需要的資訊寫清楚。幾個小訣竅：

- **一個 issue 只問一件事**，標題寫出重點，例如「[提問] 背包問題第 3 筆測資答案多 1」。
- **錯誤訊息貼文字，不要截圖**，講師才能複製、搜尋。模板裡的欄位會自動排版；在留言裡貼的話，前後用 ``` 包起來。
- **附上程式碼的位置**：分支名稱、commit，或檔案行數的連結（在 GitHub 上點行號就能複製）。
- **寫下你已經試過的方法**，包括問 AI 得到的答案。講師能更快知道問題卡在哪裡。
- **不要貼上密碼、token、API key 或個人資料**，即使 repo 是私人的。

講師回覆後，你可以直接在 issue 裡繼續討論；問題解決了就把 issue 關掉。

## 三、請講師 review：開 Pull Request

講師在程式碼上逐行留言，比在 issue 裡貼程式碼清楚得多。建議的流程：

```bash
# 1. 從 main 開一個新分支
git switch main
git pull
git switch -c feat/你的作業名稱

# 2. 寫程式、commit
git add .
git commit -m "說明這次做了什麼"

# 3. 推上 GitHub
git push -u origin feat/你的作業名稱
```

然後：

1. 到你的 repo，GitHub 會提示剛推上的分支，按 **Compare & pull request**，目標選 `main`。
2. 依照 PR 模板寫下你做了什麼、想請講師特別看哪裡。
3. 再用「**請講師 review**」模板開一個 issue，附上 PR 的編號，講師就知道該看了。
4. 講師在 PR 上留言後，你在同一個分支繼續 commit、push，PR 會自動更新。

## 常見問題

**課程頁說 GitHub App 無法存取我的 repo？**
安裝 App 時沒有選到這個 repo。照課程頁的說明到 GitHub App 設定，把 repo 加進授權清單，再回到課程頁按「重新連結」。

**我想換一個 repo？**
在課程頁的 GitHub 協作區塊可以更換連結的 repo，講師會從舊的 repo 移出、加入新的。

**平台本身的問題（網站、影片播放）？**
請到公開的 [平台問題回報](https://github.com/Progrmatic/progrmatic-feedback) 回報。那裡是公開的，請不要貼上個人資料或你的程式碼。
