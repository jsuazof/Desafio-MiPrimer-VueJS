<template>
  <div>
    <div class="container">
      <table class="table">
        <thead>
          <tr>
            <th scope="col">#</th>
            <th scope="col">Nombre</th>
            <th scope="col">Rut</th>
            <th scope="col">Teléfono</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="cliente in clientes" :key="cliente">
            <th scope="row"></th>
            <td>{{ cliente.nombre }}</td>
            <td>{{ cliente.rut }}</td>
            <td>{{ cliente.telefono }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>


export default {
  name: "App",
  data() {
    return {
      clientes: [
        { nombre: "Jose", 
          rut: 11111111 - 1, 
          telefono: 231312321 
        },
        {
          nombre: "Carlos",
          rut: 22222233 - 2,
          telefono: 432425526,
        },
        {
          nombre: "Juan",
          rut: 435353534 - 2,
          telefono: 325435354,
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
