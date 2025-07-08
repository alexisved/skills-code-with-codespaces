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
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->
<!--
  <<< 作者註記：步驟 3 >>>
  從感謝上一步的操作開始這個步驟。
  定義專有名詞並連結到 docs.github.com。
-->

## 步驟 3：客製化您的 Codespace！

_做得好！:tada: 您已成功建立一個帶有自訂映像檔的 Codespace！_

您可以透過新增 VS Code 擴充套件、加入新功能、設定主機需求等等，來客製化您的 Codespace。

現在，就讓我們來客製化 `devcontainer.json` 檔案裡的一些設定吧！

### :keyboard: 動手做：在 `devcontainer` 檔案中加入客製化設定

1. 前往 `.devcontainer/devcontainer.json` 檔案。
2. 在檔案內容的最後一個 `}` 之前，加入以下客製化設定。

   ```jsonc
    ,
    // Add the IDs of extensions you want installed when the container is created.
    "customizations": {
        "vscode": {
            "extensions": [
                "GitHub.copilot"
            ]
        },
        "codespaces": {
            "openFiles": [
                "codespace.md"
            ]
        }
    }
   ```

3. 點擊 **Commit changes** (提交變更)，然後選擇 **Commit changes directly to the `main` branch** (直接提交變更到 `main` 分支)。
4. 回到您儲存庫的首頁，來建立一個新的 Codespace。
5. 點擊頁面中間的 **Code** 按鈕。
6. 在跳出的視窗中點擊 **Codespaces** 標籤。
7. 請確保運行中的 Codespace 數量未達到上限（通常是 2 個）。想了解更多資訊，請參閱[了解 Codespace 的生命週期](https://docs.github.com/en/codespaces/getting-started/understanding-the-codespace-lifecycle)。

   > **小提示**：要停止一個運行中的 Codespace，請點擊 **<span>&#x25cf;</span>Active** 旁邊的 **•••** 圖示，然後從選單中選擇 **Stop codespace**。
   
8. 點擊 **Create codespace on main** 按鈕。

   > 等待約 **2 分鐘**，讓 Codespace 自行啟動。

9. 確認您的 Codespace 已如先前一樣正常運行。
10. `codespace.md` 檔案應該會出現在 VS Code 編輯器中。
11. `copilot` 擴充套件應該會出現在 VS Code 擴充套件列表中。

    這樣就會在 Codespace 啟動時，新增一個 VS Code 擴充套件並開啟一個檔案。

接下來，讓我們加入一些程式碼，讓它在 Codespace 建立時自動執行！

### :keyboard: 動手做：在 Codespace 建立時執行程式碼

1. 編輯 `.devcontainer/devcontainer.json` 檔案。
2. 在檔案內容的最後一個 `}` 之前，加入以下的 `postCreateCommand`。

   ```jsonc
    ,
    "postCreateCommand": "echo '# Writing code upon codespace creation!'  >> codespace.md"
   ```

3. 點擊 **Commit changes** (提交變更)，然後選擇 **Commit changes directly to the `main` branch** (直接提交變更到 `main` 分支)。
4. 回到您儲存庫的首頁，來建立一個新的 Codespace。
5. 點擊頁面中間的 **Code** 按鈕。
6. 在跳出的視窗中點擊 **Codespaces** 標籤。
7. 點擊 **Create codespace on main** 按鈕。

   > 等待約 **2 分鐘**，讓 Codespace 自行啟動。

8. 確認您的 Codespace 已如先前一樣正常運行。
9. 確認 `codespace.md` 檔案現在已經包含了 `Writing code upon codespace creation!` 的文字。
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
