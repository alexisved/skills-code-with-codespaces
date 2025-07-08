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
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->
<!--
  <<< 作者註記：步驟 2 >>>
  從感謝上一步的操作開始這個步驟。
  定義專有名詞並連結到 docs.github.com。
-->

## 步驟 2：為您的 Codespace 加入自訂映像檔！

_做得好！:tada: 您已成功建立第一個 Codespace，並使用 VS Code 推送了程式碼！_

您可以設定儲存庫的開發容器，這樣一來，為該儲存庫建立的任何 Codespace 都會提供您一個量身打造的開發環境，其中包含了您在特定專案上工作所需的所有工具和執行階段 (runtimes)。

**什麼是開發容器 (development containers)？** 開發容器（dev containers）是經過特殊設定的 Docker 容器，用來提供一個功能齊全的開發環境。每當您在 Codespace 中工作時，您其實就是在虛擬機器上使用一個開發容器。

開發容器設定檔 (`devcontainer.json`) 是一個 JSON 檔案，它能讓您客製化執行 Codespace 的預設映像檔、VS Code 設定、執行自訂程式碼、轉發連接埠 (forward ports) 等等，功能非常多！

現在，就讓我們來新增一個 `devcontainer.json` 檔案，並加入一個自訂映像檔吧。

### :keyboard: 動手做：新增 .devcontainer.json 檔案來客製化您的 Codespace

1. 回到您儲存庫的 **Code** 索引標籤，點擊 **Add file** (新增檔案) 下拉按鈕，然後點擊 `Create new file` (建立新檔案)。
2. 在提示的空白文字欄位中，輸入或貼上以下內容來為您的檔案命名。

   ```
   .devcontainer/devcontainer.json
   ```

3. 在新檔案 **.devcontainer/devcontainer.json** 的內容區塊，加入以下內容：

   ```jsonc
   {
     // 為此設定命名
     "name": "Codespace for Skills!",
     // 使用基礎的 codespace 映像檔
     "image": "mcr.microsoft.com/vscode/devcontainers/universal:latest",

     "remoteUser": "codespace",
     "overrideCommand": false
   }
   ```

4. 點擊 **Commit changes** (提交變更)，然後選擇 **Commit changes directly to the `main` branch** (直接提交變更到 `main` 分支)。
5. 回到您儲存庫的 **Code** 索引標籤，來建立一個新的 Codespace。
6. 點擊頁面中間綠色的 **Code** 按鈕。
7. 在跳出的視窗中點擊 **Codespaces** 標籤。
8. 點擊 **Create codespace on main** 按鈕，或是點擊分頁上的 `+` 號。這會在 `main` 分支上建立一個新的 Codespace。(請注意，您先前的 Codespace 也會列在這裡。)

   > 等待約 **2 分鐘**，讓 Codespace 自行啟動。

9. 確認您的新 Codespace 已如先前一樣正常運行。

   請注意，這裡使用的映像檔是 GitHub Codespaces 提供的預設映像檔。它包含了 Python、Node.js、Docker 等等的執行階段和工具。您可以在這裡查看完整列表：https://aka.ms/ghcs-default-image。您的開發團隊可以使用任何已安裝必要先備條件的自訂映像檔。想了解更多資訊，請參閱 [Codespace 映像檔](https://aka.ms/configure-codespace)。

10. 等待約 20 秒，然後重新整理這個頁面（也就是您正在閱讀說明的這個頁面）。[GitHub Actions](https://docs.github.com/en/actions) 將會自動將課程更新到下一個步驟。

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
