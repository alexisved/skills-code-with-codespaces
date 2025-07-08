<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->
<!--
  <<< 作者註記：課程標頭 >>>
  閱讀 <https://skills.github.com/quickstart> 以了解更多關於如何使用此範本建立課程的資訊。
  包含一張 1280×640 的圖片、一個句子式大小寫的課程名稱，以及一段以強調樣式呈現的簡潔描述。
  在您的儲存庫設定中：啟用樣板儲存庫、新增您的 1280×640 社群圖片、自動刪除 head 分支。
  在「About」旁邊，新增描述與標籤；停用 releases、packages 與 environments。
  新增您的開源授權條款，GitHub 使用的是 MIT 授權條款。
-->

# 使用 GitHub Codespaces 與 Visual Studio Code 進行程式碼開發

_使用 GitHub Codespaces 和 Visual Studio Code 來開發您的程式碼！_

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->
<!--
  <<< 作者註記：步驟 1 >>>
  為您的課程選擇 3-5 個步驟。
  第一步總是最難的，所以選一些簡單的內容吧！
  連結到 docs.github.com 以獲得更深入的解釋。
  鼓勵使用者為每個步驟開啟新的分頁！
-->

## 步驟 1：建立您的第一個 Codespace 並推送程式碼

_歡迎來到「使用 GitHub Codespaces 與 Visual Studio Code 進行程式碼開發」！ :wave:_

**使用 Codespace 進行軟體開發，到底有什麼了不起的呢？** Codespace 是一個託管在雲端的開發環境。您可以透過將設定檔提交到您的儲存庫（也就是所謂的「設定即程式碼」），來為您的專案客製化 GitHub Codespaces，這樣就能為專案的所有使用者建立一個可重複使用的 Codespace 設定。您建立的每個 Codespace 都由 GitHub 託管在一個運行於虛擬機器上的 Docker 容器中。您可以根據所需的資源，選擇您想要使用的機器類型。

GitHub 提供了一系列功能，幫助您的開發團隊客製化 Codespace，以達到最佳的設定與效能需求。舉例來說，您可以：

- 從您的儲存庫建立一個 Codespace。
- 從 Codespace 將程式碼推送到您的儲存庫。
- 使用 VS Code 進行程式碼開發。
- 使用自訂映像檔來客製化 Codespace。
- 管理 Codespace。

要開始使用 GitHub Codespaces 進行開發，您可以從一個範本，或是從儲存庫中的任何分支或提交來建立一個 Codespace。當您從範本建立 Codespace 時，您可以從一個空白範本開始，或是選擇一個適合您工作的範本。

### :keyboard: 動手做：啟動一個 Codespace

**我們建議您另外開啟一個瀏覽器分頁來進行接下來的活動，這樣您就可以隨時參考這些說明。**

1. 從您的儲存庫首頁開始。
2. 點擊頁面中間綠色的 **Code** 按鈕。
3. 在跳出的視窗中選擇 **Codespaces** 標籤，然後點擊 **Create codespace on main** 按鈕。

   > 等待約 2 分鐘，讓 Codespace 自行啟動。
   > **請注意**：這是在背景啟動一台虛擬機器喔。

4. 確認您的 Codespace 正在運行。瀏覽器中應該會出現一個網頁版的 VS Code 編輯器，並且會有一個終端機視窗，如下圖所示：
   ![codespace 介面範例](https://user-images.githubusercontent.com/26442605/207355196-71aab43f-35a9-495b-bcfe-bf3773c2f1b3.png)

### :keyboard: 動手做：從 Codespace 推送程式碼到您的儲存庫

1. 在 Codespace 的 VS Code 檔案總管視窗中，選擇 `index.html` 檔案。
2. 將 **h1** 標頭替換成以下內容：

   ```html
   <h1>Hello from the codespace!</h1>
   ```

3. 儲存檔案。
   > **請注意**：檔案應該會自動儲存。
4. 使用 VS Code 的終端機，輸入以下的提交訊息來提交檔案變更：

   ```shell
   git commit -a -m "Adding hello from the codespace!"
   ```

5. 將變更推送到您的儲存庫。在 VS Code 終端機中輸入：

   ```shell
   git push
   ```

6. 您的程式碼已經成功推送到儲存庫了！
7. 切換回您儲存庫的首頁，並檢視 `index.html` 來確認新的程式碼已成功推送。
8. 等待約 20 秒，然後重新整理這個頁面（也就是您正在閱讀說明的這個頁面）。[GitHub Actions](https://docs.github.com/en/actions) 將會自動將課程更新到下一個步驟。

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->
<!--
  <<< 作者註記：頁尾 >>>
  新增一個取得支援的連結、GitHub 狀態頁面、行為準則、授權條款連結。
-->

---

尋求協助：[在我們的論壇中發文](https://github.com/orgs/skills/discussions/categories/code-with-codespaces) &bull; [查看 GitHub 狀態頁面](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [行為準則](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT 授權條款](https://gh.io/mit)

</footer>
