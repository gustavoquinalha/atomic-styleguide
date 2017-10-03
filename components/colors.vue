<template>
<div class="size margin">

  <div class="example">
    <div class="title padding-left-20 color-primary">
      <h3>Colors</h3>
    </div>
    <div class="container wrap">
      <div class="box-colors text-center container column align-items-center" v-for="x in colors">
        <div class="box" :style="{ background: x.hex }"></div>
        <div class="text">
          <strong>{{x.name}}</strong>
          <p><small>{{x.hex}}</small></p>
        </div>
      </div>
    </div>
  </div>

  <div class="example">
    <div class="title padding-left-20 color-primary">
      <h3>Gradients</h3>
    </div>
    <div class="container wrap">
      <!-- background: linear-gradient(10deg, #333, #222); -->
      <div v-for="x in gradients" class="flex-basis-300 flex-grow-1">
        <div class="box-gradient text-center container justify-content-center align-items-center" :style="{background: 'linear-gradient(to right,' + x.color + ',' + x.color2 + ')'}">
          <div class="text container column">
            <strong>{{x.name}}</strong>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="example">
    <div class="title padding-left-20 color-primary">
      <h3>Shadows</h3>
    </div>
    <div class="container wrap">
      <div class="box-shadow text-center container justify-content-center align-items-center" v-for="x in shadows" :style="{ boxShadow: '0 ' + '0 ' + x.size + 'px ' + x.smooth + 'px ' +  'rgba(0,0,0,.1)'}">
        <div class="text container column">
          <strong>{{x.name}}</strong>
          <small style="font-size: 10px">box-shadow: 0 0 {{x.size}}px {{x.smooth}}px rgba(0,0,0,.1)</small>
        </div>
      </div>
    </div>
  </div>


</div>
</template>

<script>
export default {
  name: 'colors',
  data() {
    return {
      colors: [{
          name: 'Primary',
          hex: '#50fa7b'
        },
        {
          name: 'Danger',
          hex: '#f2405d'
        },
        {
          name: 'Warning',
          hex: '#ffb721'
        },
        {
          name: 'Black',
          hex: '#000000'
        },
        {
          name: 'Grey',
          hex: '#b3b3b3'
        },
        {
          name: 'Light grey',
          hex: '#e2e2e2'
        },
        {
          name: 'White',
          hex: '#ffffff'
        }],
      shadows: [{
          name: 'Small',
          size: 10,
          smooth: 0
        },
        {
          name: 'Medium',
          size: 20,
          smooth: 5
        },
        {
          name: 'Large',
          size: 30,
          smooth: 10
        }],
      gradients: [{
          name: 'Primary',
          color: '#50fa7b',
          color2: '#457250'
        },
        {
          name: 'Dark',
          color: '#484747',
          color2: '#000000'
        },
        {
          name: 'Light',
          color: '#dddddd',
          color2: '#cccccc'
        }]
    }
  }
}
</script>

<style lang="scss" scoped>
.box-colors {
    flex-basis: 130px;
    box-shadow: 0 0 10px 0 rgba(0,0,0,.1);
    box-sizing: border-box;
    padding-top: 0 !important;
    .box {
        width: 130px;
        height: 100px;
    }
    .text {
        padding-top: 10px;
    }
    &:hover {
        box-shadow: 0 10px 10px 0 rgba(0,0,0,.1);
        transform: translateY(-10px);
    }
}

.box-shadow {
    flex-basis: 300px;
    flex-grow: 1;
    &:hover {
        box-shadow: 0 10px 10px 0 rgba(0,0,0,.1);
        transform: translateY(-10px);
    }
}

.box-gradient {
    flex-basis: 300px;
    flex-grow: 1;
    color: #fff;
    box-shadow: 0 0 10px 0 rgba(0,0,0,.1);
    &:hover {
        box-shadow: 0 10px 10px 0 rgba(0,0,0,.1);
        transform: translateY(-10px);
    }
}

.box-colors,
.box-gradient,
.box-shadow {
    border-radius: 10px;
    overflow: hidden;
    cursor: pointer;
    transition: 0.3s;
    padding: 20px;
    box-sizing: border-box;
    margin: 20px;
    min-height: 130px;
}
</style>
