title: About
---
This is about page

## here is code 

```bash
appearance:
  # Accent color, default '#2a2b33'
  accent_color:
  # Font color, default '#363636'
  foreground_color:
  # Border color, default '#e0e0e0'
  border_color:
  # body background, default '#f5f7fa'
  background:
  # Sidebar background (when opened), default to accent_color
  sidebar_background:
  # Card background, default '#fff'
  card_background:

  # All background settings above support image, e.g.,
  # '//www.toptal.com/designers/subtlepatterns/patterns/confectionary.png #f5f7fa' or
  # 'url(//www.toptal.com/designers/subtlepatterns/patterns/confectionary.png) #f5f7fa'

  # 内容区域最大宽度
  content_width: 640

  # 字体设置
  font:
    # 字体 CSS 文件的 URL
    url: //fonts.googleapis.com/css?family=Baloo+Bhaijaan|Inconsolata|Josefin+Sans|Montserrat

    # 基础字体，作用于 body 元素
    base: "'Josefin Sans', 'PingFang SC', Microsoft YaHei"
    # 作用于 sidebar 上方的 LOGO
    logo:
    # 作用于 sidebar 菜单栏
    menu: 'Baloo Bhaijaan'
    # 作用于文章百分比、归档页月份、分类文字数、分页、目录索引等地方
    label: Montserrat
    # 作用于标题
    heading:
    # 作用于代码及代码块
    code: Inconsolata, monospace
    # Base font for printing which applied to body
    print:

  # 代码语法高亮
  # 接受设置值为 16 个 hex 色值的数组，具体请参考 base16 (https://github.com/chriskempson/base16)
  # 默认配色方案为 Atelier Dune Light
  highlight: [
    '#ffffff', '#e0e0e0', '#d6d6d6', '#8e908c',
    '#969896', '#4d4d4c', '#282a2e', '#1d1f21',
    '#c82829', '#f5871f', '#eab700', '#718c00',
    '#3e999f', '#4271ae', '#8959a8', '#a3685a'
  ]

  # 启用 darkmode
  darkmode:
    accent_color: '#539bf5'
    foreground_color: '#adbac7'
    border_color: '#373e47'
    background: '#22272e'
    sidebar_background: '#22272e'
    card_background: '#2d333b'
    highlight: [
      '#2d333b', '#444c56', '#3e4451', '#545862',
      '#565c64', '#abb2bf', '#b6bdca', '#c8ccd4',
      '#e06c75', '#d19a66', '#e5c07b', '#98c379',
      '#56b6c2', '#61afef', '#c678dd', '#be5046'
    ]
```