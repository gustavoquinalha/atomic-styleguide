<template>
<div class="size margin">

  <div class="example">
    <titleComponent>
      <span slot="title">Buttons</span>
    </titleComponent>
    <div class="container wrap padding-top-20 border-box padding-20">

      <div class="container column">



        <div class="esp">
          <atomic-button value="Botão 1" size="small" type="" color="" font-color="" border-radius="" width=""></atomic-button>
        </div>

        <div class="esp">
          <atomic-button value="Medium" size="medium" type="" color="" font-color="" border-radius="" width=""></atomic-button>
        </div>

        <div class="esp">
          <atomic-button value="Conferir " size="large" type="" color="" font-color="" border-radius="" width=""></atomic-button>
        </div>





      </div>

    </div>
    <table>
      <tr>
        <th><h4>Attribute</h4></th>
        <th><h4>Type</h4></th>
        <th><h4>Default</h4></th>
        <th><h4>Options</h4></th>
        <th><h4>Description</h4></th>
      </tr>

      <tr>
        <td>Value</td>
        <td>String</td>
        <td></td>
        <td></td>
        <td>Texto dentro do botão</td>
      </tr>

      <tr>
        <td>Size</td>
        <td>String</td>
        <td>Medium</td>
        <td>small / medium / large</td>
        <td>Define a proporção do botão</td>
      </tr>

      <tr>
        <td>Type</td>
        <td>String</td>
        <td>Default</td>
        <td>primary / danger</td>
        <td>Define o tipo</td>
      </tr>

      <tr>
        <td>Color</td>
        <td>String</td>
        <td>#ddd</td>
        <td>Qualquer tipo de cor(red, #ff4455, rgb(23,154, 16))</td>
        <td>Define a cor do background</td>
      </tr>

      <tr>
        <td>Font-color</td>
        <td>String</td>
        <td>#333</td>
        <td>Qualquer tipo de cor, Ex: (red, #ff4455, rgb(23,154, 16))</td>
        <td>Define a cor da fonte</td>
      </tr>

      <tr>
        <td>Border-radius</td>
        <td>String</td>
        <td>4px</td>
        <td>Número + medida, Ex: (4px, 50%)</td>
        <td>Define o radius da borda</td>
      </tr>

    </table>


  </div>

</div>
</template>

<script>
import titleComponent from '@/components/titleComponent'
import atomicButton from '@/components/btn/buttonComponent'

export default {
  components: {
    titleComponent,
    atomicButton
  },
  name: 'buttons',
  data() {
    return {}
  }
}
</script>

<style lang="scss" scoped>
.esp {
  margin-bottom: 10px
}
table {
    border-collapse: collapse;
    width: 100%;
}

td, th {
    border: 1px solid #ccc;
    text-align: left;
    padding: 8px;
}

tr:nth-child(even) {
    background-color: #ddd;
}
</style>
