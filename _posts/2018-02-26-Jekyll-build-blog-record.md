---
title: Github Page x Jekyll 架站紀錄
layout: post
date: '2018-02-26 23:00:00'
img: githubXjekyll.png
tags: Jekyll GithubPage
---

### 個人需求

開始使用 Github 多多少少有些品牌忠誠度，特別是當知道 Github 有網站託管功能時，真的造福像我喜歡簡單的個性，像之前嘗試過 Wordpress ，因為操作介面太複雜，不太適合只需要基本需求的我，基本上我的需求只需要寫文章，弄個分類、標籤，就好。

### 環境 & 工具需求
- 個人環境
	- Linux Mint 18.3 (如果在 Windows , Mac OS 也是沒問題的，不過本文就僅參考用)
- 環境
	- [GithubPage](https://pages.github.com/) (需 Github 帳號)
- 工具
	- [git](https://git-scm.com/) (需安裝,透過套件庫安裝) 這邊假設你已經熟悉 git
	- [Jekyll](https://jekyllrb.com/)  (需安裝,透過 gem 或 套件庫安裝)
		- 
	- [bundler](http://bundler.io/) (需安裝,透過 gem 或 套件庫安裝)
- 樣版
	- [Jekyll themes](http://jekyllthemes.org/) (想要自幹也沒問題，如果想要抽換樣版也是很容易的)

### 工具安裝 

套件庫安裝
```
sudo apt -y install jekyll
sudo apt -y install bundler
```

### 建立初始網站

```
jekyll new [blog-name] // 請無視[]符號
```

### 樣版外掛安裝

請將樣版資料夾內的檔案複製到[blog-name]。
```
cd [blog-name]
bundle install 
```

### 啟動網站

```
bundle exec jekyll serve // bundler 可以避免因為版本差異，而無法運行。
```

### 注意事項

_config.yml 's plugin & Gemfile 這兩邊插件必須一致，避免啟動時，因為插件內容沒有樣版所需要的，而無法啟動。

### Github Page

在 Github 建立一個以 [username].github.io 為名 repository，並將剛才做的網站 push 此 repository。

### 常用套件

- jekyll-admin

### 封面引用
[How to setup your Jekyll website with free web hosting, SSL, and a custom domain](https://hackernoon.com/how-to-setup-your-jekyll-website-with-free-web-hosting-ssl-and-a-custom-domain-4056ff862ca1)
### 文章參考
[Jekyll 介紹](https://wcc723.github.io/jekyll/2014/01/04/what-is-jekyll/)