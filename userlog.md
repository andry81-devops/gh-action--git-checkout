> :information_source: this log lists user most visible changes

> :warning: to find all changes use [changelog.txt](https://github.com/andry81-devops/gh-action--git-checkout/tree/HEAD/changelog.txt) file in a directory

> :information_source: Legend: :shield: - security; :wrench: - fixed; :new: - new; :pencil: - changed; :twisted_rightwards_arrows: - refactor

## 2023.07.03:
* :twisted_rightwards_arrows: refactor: action.yml: renamed workflow `Git Checkout Extension` to `git-checkout-extension`

## 2023.06.26:
* :wrench: fixed: action.yml: missed to check `inputs.ref` for existence
* :new: new: action.yml: added `actions--checkout-ref` input parameter to use specific `actions/checkout@<ref>` version (default: `v3`, variants: `v2`)
* :pencil: changed: action.yml: parameters updated to latest `actions/checkout` of version `v3` and `v2`

## 2023.06.26:
* :wrench: fixed: action.yml: #1: missed branch reference to use

## 2022.10.30:
* :pencil: changed: action.yml: `set-output` command is replaced in favor of `$GITHUB_OUTPUT` variable usage (details: https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/ )

## 2022.05.12:
* :twisted_rightwards_arrows: refactor: action.yml: rename for unique name on GitHub Marketplace

## 2022.05.04:
* :new: new: action.yml: added `COMMIT_MESSAGE_PREFIX` to split an automated user commit message into prefix and suffix parts

## 2022.04.16:
* :new: new: action.yml: added `mkdir-p` to allocate directories after checkout because the `actions/checkout` action script does cleanup a working copy directory before execution
