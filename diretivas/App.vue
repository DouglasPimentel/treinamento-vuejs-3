<template>
  <div>
    <h1>Minha Lista de Tarefas!</h1>
    <button
      @click="() => showList = !showList"
    >
      Ver a lista!
    </button>
    <br />
    <ul v-if="showList">
      <li
        v-for="(task, index) in task"
        :key="`${task}-${index}`" 
      >
        {{ task.name }}
      </li>
    </ul>
    <p v-else>
      Lista de tarefas escondidas
    </p>
  </div>
</template>

<script>
export default {
  data: () => ({
    showList: false,
    task: [
      {
        name: 'Fazer o curso',
        isDone: false
      },
      {
        name: 'Fazer compras',
        isDone: false
      },
      {
        name: 'Ler um livro',
        isDone: false
      }
    ]
  })
}
</script>