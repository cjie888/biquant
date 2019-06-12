<template lang='pug'>
  section.contain.grd-row
    .grd-row-col-3-6(v-html='left')
    .grd-row-col-3-6.txt--center
      img(src='static/gekko.jpeg')
      p
        em The most valuable commodity I know of is information.
</template>

<script>
import marked from '../../tools/marked';

const left = marked(`

## BiQuant

BiQuant is a Bitcoin trading bot and backtesting platform that
connects to popular Bitcoin exchanges. It is written in javascript
and runs on nodejs.


`);

export default {
  data: () => {
    return {
      left
    }
  }
}
</script>
