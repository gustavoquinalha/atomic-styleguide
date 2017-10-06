<template>
<div class="size margin">

  <div class="example">
    <titleComponent>
      <span slot="title">Buttons</span>
    </titleComponent>
    <div class="container column padding-top-20 border-box padding-20">

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Value</h4>
        </div>
        <div class="esp container align-items-center">
          <atomic-button value="Digite seu texto"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="Digite seu texto"&gt;&lt;/atomic-button&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Size</h4>
        </div>
        <div class="esp container wrap align-items-center">
          <atomic-button value="Small" size="small"></atomic-button>
          <atomic-button value="Medium" size="medium"></atomic-button>
          <atomic-button value="Large" size="large"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="Small" size="small"&gt;
&lt; atomic-button value="Medium" size="medium"&gt;
&lt; atomic-button value="Large" size="large"&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Type</h4>
        </div>
        <div class="esp container wrap align-items-center">
          <atomic-button value="Default" type=""></atomic-button>
          <atomic-button value="Primary" type="primary"></atomic-button>
          <atomic-button value="Danger" type="danger"></atomic-button>
          <atomic-button value="Warning" type="warning"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="Default" type=""&gt;
&lt; atomic-button value="Primary" type="primary"&gt;
&lt; atomic-button value="Danger" type="danger"&gt;
&lt; atomic-button value="Warning" type="warning"&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Color</h4>
        </div>
        <div class="esp container align-items-center">
          <atomic-button value="color: purple" color="purple"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="color: purple" color="purple"&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Font-color</h4>
        </div>
        <div class="esp container align-items-center">
          <atomic-button value="font-color: #fff" color="purple" font-color="#fff"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="font-color: #fff" color="purple" font-color="#fff"&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Border-radius</h4>
        </div>
        <div class="esp container align-items-center">
          <atomic-button value="Border Radius" border-radius="30px"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="Border Radius" border-radius="30px"&gt;
    </code>
  </pre>
        </div>
      </div>

      <div class="container column esp flex-grow-1">
        <div class="subtitle">
          <h4>Width</h4>
        </div>
        <div class="esp container align-items-center">
          <atomic-button value="Width: 300px" width="300px"></atomic-button>
        </div>
        <div class="ex-btn">
          <pre>
    <code class="html">
&lt; atomic-button value="Width: 300px" width="300px"&gt;
    </code>
  </pre>
        </div>
      </div>

    </div>

    <div class="table">
      <table>
        <thead>
          <tr>
            <th>
              <h4>Attribute</h4>
            </th>
            <th>
              <h4>Type</h4>
            </th>
            <th>
              <h4>Default</h4>
            </th>
            <th>
              <h4>Options</h4>
            </th>
            <th>
              <h4>Description</h4>
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Value</td>
            <td>String</td>
            <td></td>
            <td>Ex: "Texto do botão"</td>
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

          <tr>
            <td>Width</td>
            <td>String</td>
            <td></td>
            <td>Número + medida, Ex: (200px, 100%)</td>
            <td>Define o tamanho do botão</td>
          </tr>

        </tbody>
      </table>
    </div>


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
.ex-btn {
    padding-bottom: 100px;
}
.esp {
    margin-bottom: 10px;
}
table {
    border-collapse: collapse;
    width: 100%;
}

td,
th {
    border: 1px solid #ccc;
    text-align: left;
    padding: 8px;
}
tr:nth-child(even) {
    background-color: #ddd;
}
.table {
    width: 1200px;
    max-width: 100%;
    overflow-x: scroll;
}
table,
td,
th,
tr {}
</style>
