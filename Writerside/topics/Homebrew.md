# Homebrew Installation

## Instructions

> ❗❗❗ 此教學只適用Apple Silicon，Intel用戶請自研

### Option 1

Install [Homebrew](https://brew.sh) by executing the following command in your terminal

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

裝完之後仲會叫你行兩句command，跟住Terminal做就得，下面只係參考，唔好跟住copy！

```bash
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/$USER/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

> ❗❗❗ 經同學反映，冇行到佢跟畀你嘅commands，會產生大麻煩，請不要忘記！

### Option 2

Follow the official download instruction [https://docs.brew.sh/Installation](https://docs.brew.sh/Installation) and
choose a method for youself

## References

- [https://electrify.tw/archives/395/homebrew-for-mac/](https://electrify.tw/archives/395/homebrew-for-mac/)