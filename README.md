<p align="center">
  <a href="#"><img src="https://img.shields.io/github/repo-size/andry81-devops/gh-action--git-checkout" valign="middle" alt="GitHub repo size in bytes" /></a>
• <a href="https://github.com/XAMPPRocky/tokei"><img src="https://tokei.rs/b1/github/andry81-devops/gh-action--git-checkout?category=lines" valign="middle" alt="lines of text by tokei.rs" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/commits/master/traffic/views">
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=Github%20views|all&query=count&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/views/latest-accum.json?raw=True&logo=github" valign="middle" alt="GitHub views|any|total" />
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=count&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/views/latest.json?raw=True" valign="middle" alt="GitHub views|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/commits/master/traffic/views">
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=Github%20views|unq&query=uniques&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/views/latest-accum.json?raw=True&logo=github" valign="middle" alt="GitHub views|unique per day|total" />
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=uniques&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/views/latest.json?raw=True" valign="middle" alt="GitHub views|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/commits/master/traffic/clones">
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=Github%20clones|all&query=count&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/clones/latest-accum.json?raw=True&logo=github" valign="middle" alt="GitHub clones|any|total" />
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=count&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/clones/latest.json?raw=True" valign="middle" alt="GitHub clones|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/commits/master/traffic/clones">
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=Github%20clones|unq&query=uniques&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/clones/latest-accum.json?raw=True&logo=github" valign="middle" alt="GitHub clones|unique per day|total" />
    <img src="https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=uniques&url=https://github.com/andry81-stats/gh-action--git-checkout--gh-stats/raw/master/traffic/clones/latest.json?raw=True" valign="middle" alt="GitHub clones|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--git-checkout/commits">
    <img src="https://img.shields.io/github/commits-since/andry81-devops/gh-action--git-checkout/latest?sort=semver&label=Github%20commits%20since%20latest" valign="middle" alt="GitHub commits since latest version" /></a>
  <a href="https://github.com/andry81-devops/gh-action--git-checkout/releases">
    <img src="https://img.shields.io/github/v/release/andry81-devops/gh-action--git-checkout?include_prereleases&label=latest" valign="middle" alt="latest release name" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81/donate"><img src="https://github.com/andry81/andry81/raw/master/badges/donate.svg" valign="middle" alt="donate" /></a>
</p>

---

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--git-checkout/blob/master/userlog.md">Userlog</a>
• <a href="https://github.com/andry81-devops/gh-action--git-checkout/blob/master/changelog.txt">Changelog</a>
• <a href="#dependecies">Dependencies</a>
• <a href="#known_issues">Known issues</a>
• <a href="#copyright-and-license"><img src="https://github.com/andry81/andry81/raw/master/badges/mit-license.svg" valign="middle" alt="copyright and license" />&nbsp;Copyright and License</a>
</p>

<h4 align="center">GitHub composite action extension of <tt>actions/checkout</tt> action.</h4>

##

# gh-action--git-checkout@master

**Features**:

* Checks if remote repository is exist and has a reference, otherwise call to `mkdir` instead of the checkout.

* If remote repository is exist and has a reference, then delegates all input into https://github.com/actions/checkout action.

# USAGE

## <a name="example-snippet">Example snippet</a>:

```yml
steps:
  - uses: andry81-devops/gh-action--git-checkout@master
    with:
      repository: ...
      ref:        ...

      actions-checkout-ref: HEAD
```

## <a name="known_issues">Known Issues</a>

### Works on a private repository because of GitHub security issue

Implemented to work only with a public repository but currently works on a private repository too because of GitHub security issue and can stop to work in future.

## <a name="copyright-and-license">Copyright and License</a>

Code and documentation copyright 2022 Andrey Dibrov. Code released under [MIT License](https://github.com/andry81-devops/gh-action--git-checkout/blob/master/license.txt)
