# Recommendations

## Apple Mac

Mac基於Unix，同Linux一樣，但比起唔同Linux distribution軟件應用生態更加豐富，對於開發者嚟講係非常好嘅選擇。
[Homebrew on Mac](Homebrew.md) 係一個非常好嘅package manager，可以方便咁安裝各種軟件。單憑呢一點已經方便過Windows好多。

## GitHub Student

強烈建議拎咗個 [GitHub Student Developer Pack](https://education.github.com/pack/offers)先。
Github為學生提供咗唔少優惠同資源，用學校email開個新account然後去認證就可以。
單憑可以免費用Github Copilot，就值得去搞。
> 試過用safari申請， 試過有Step有bug，BTW你唔得先轉用其他，可能已經Fix咗

## JetBrains全家桶

喺呢個SPEED program我哋會寫唔同Languages，如果每個Language都用唔同IDE就會好麻煩，所以我會用建議用JetBrains。
寫唔同嘅Language但係統一嘅介面同用法，仲有大量好用嘅plugin，例如入邊內置咗Git同埋DB GUI client。
可以用 [JetBrains Toolbox](https://www.jetbrains.com/toolbox-app/) 去裝JetBrains全家桶。 \
<br/>
用Mac嘅同學:

```bash
brew install jetbrains-toolbox
```

## Docker

Docker可以話係現代developer必學嘅嘢，詳情可以自己去了解。呢度都有安裝教學: [Docker](Docker.md)。
Mac同Linux用Docker都方便，但Windows就唔係咁方便，所以建議有能力嘅都買部Mac，或者唔鍾意可以裝個Linux，當然都可以用WSL2。

## Git

Git都係developer必學嘅嘢，詳情可以自己去了解，呢度就唔多講。我認為要團隊合作得更好至少要掌握以下幾個概念：
<img height="600" src="git-basic.png" alt="git concept"/>
- 有咩係唔需要版本控制: Ignore (`.gitignore`)
- 有咩係需要版本控制: Stage (add)
- 類似遊戲存檔，每做一步就Save一下: Local Repository (commit)
- 最終儲存同步嘅地方: Remote Repository (push/pull)
- 分支，開多個Save，畀你去做一系列唔同嘅嘢: Branch (checkout/merge)
- 交貨畀大佬: Pull Request (PR)

## 待續