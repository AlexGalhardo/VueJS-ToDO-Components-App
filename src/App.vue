<template>
  <div id="app">
     <section class="hero is-primary is-bold is-fullheight">

      <!-- Hero content: will be in the middle -->
      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="row">
            <div class="columns">
              <div class="column is-half is-offset-one-quarter">
                <!-- segundo component principal da aplicação -->
                <todo-card></todo-card>
              </div>
            </div>
          </div>
        </div>
      </div>

    </section>
  </div>
</template>

<script>
// component filho necessário para esse component root/raíz App.vue
import TodoCard from './components/TodoCard'

export default {
  // nome deste component
  name: 'app',
  // components filhos necessários 
  components: {
    TodoCard
  },
  // dados imutáveis
  data () {
    return {
      msg: 'Hello, World!'
    }
  }
}
</script>

<style></style>