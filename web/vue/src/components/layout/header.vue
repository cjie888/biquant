<template lang='pug'>
  div
    #top
    header.bg--off-white.grd
      .contain.grd-row
        h3.py1.px2.col-2 比特币量化平台（基于Gekko）
    nav.bg--light-gray
      .menu.contain
        router-link(to='/home').py1 介绍
        router-link(to='/live-gekkos').py1 实盘
        router-link(to='/backtest').py1 回测
        router-link(to='/data').py1 数据
        router-link(to='/config').py1 配置
        a(href='https://gekko.wizb.it/docs/introduction/about_gekko.html', target='_blank').py1 Gekko文档

</template>

<script>
export default {}
</script>

<style>
.menu {
  display: flex;
  flex-direction: row;
  margin-top: 0;
  margin-bottom: 2rem;
}

.menu a {
  flex: 1 1 100%;
  display: block;
  text-align: center;
  text-decoration: none;
  color: inherit;
}

.menu .router-link-active {
  background-color: rgba(250,250,250,.99);
}

.menu a:hover {
  text-decoration: underline;
}

</style>
