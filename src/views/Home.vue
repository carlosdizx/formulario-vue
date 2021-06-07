<template>
  <form>
    <input
        type="text"
        class="form-control my-2"
        placeholder="Ingrese nommbre"
        v-model="tarea.nombre"
    />
    <div class="form-check form-check-inline">
      <input class="form-check-input" type="checkbox" id="check-1"
             v-model="tarea.categorias" value="JavaScript"/>
      <label class="form-check-label" for="check-1">JavaScript</label>
    </div>
    <div class="form-check form-check-inline">
      <input class="form-check-input" type="checkbox" id="check-2"
             v-model="tarea.categorias" value="NodeJS"/>
      <label class="form-check-label" for="check-2">NodeJS</label>
    </div>
  </form>
  <hr>
  <p>{{ tarea }}</p>
</template>

<script>

export default {
  name: 'Home',
  components: {
  },
  data() {
    return {
      tarea:{
        nombre: '',
        categorias: []
      }
    }
  },
}
</script>
