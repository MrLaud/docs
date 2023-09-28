---
# 提供三种布局，doc、page和home
# 官方文档相关配置：https://vitepress.dev/reference/default-theme-layout
layout: home
home: true

# 官方文档相关配置：https://vitepress.dev/reference/default-theme-home-page
title: MrLaud
titleTemplate: Hi，终于等到你
editLink: true
lastUpdated: true

hero:
  name: MrLaud
  text: Stay foolish, Stay hungry.
  tagline: /斜杠青年/人间清醒/工具控/
  image:
    # 首页右边的图片  // 表示docs/public/top_left_logo.png
    src: /home_right_logo.png
    # 图片的描述
    alt: avatar
  # 按钮相关
  actions:
    - theme: brand
      text: 进入主页
      link: /markdown-examples
    - theme: alt
      text: 导航标签
      link: /link_tag
# 按钮下方的描述
features:
  - icon: 🤹
    title: Web前端
    details: 大厂程序媛，国内某互联网厂搬砖。
    link: /
  - icon: 🎨
    title: 喜欢美学
    details: 热爱一切美学，喜欢用各种设计工具造图。
    link: /
  - icon: 🧩
    title: 斜杆青年
    details: 是个平平无奇但是又很热爱学习的斜杆青年。
    link: /
---


<!-- 自定义组件 -->
<script setup>
import home from './.vitepress/components/home.vue';
</script>

<home />