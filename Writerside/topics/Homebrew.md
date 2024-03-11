# Homebrew Installation

## Instructions

Install [Homebrew](https://brew.sh) by executing the following command in your terminal

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

裝完之後仲會叫你行兩句command，跟住Terminal做就得，下面只係參考。

```bash
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/$USER/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## References

- [https://electrify.tw/archives/395/homebrew-for-mac/](https://electrify.tw/archives/395/homebrew-for-mac/)