<template>
  <div>
    <h3>Mis Paneles</h3>
    <div class="board-collection">
      <input 
      type="text"
      placeholder="Añade un nuevo panel"
      v-model = "boardName"
      @keyup.enter="add()"
      />
      <board-card
      v-for = "(board, index) in boards" :key = "index"
      :name = "board.name"
      :id = "board.id">      
      </board-card>
  
    </div>
  </div>
  </template>
  <script>
    export default {
      name: 'about-view'
    }
  </script>

<style lang = "scss" scoped>
/* @media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
} */
h3 {
    text-align: left;
    margin: 1.5rem;
  }
  .boards-collection {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    padding-top: 1rem;
  }
  input {
    box-sizing: border-box;
    background-color: #546e7a;
    border: 2px solid #546e7a;
    border-radius: 3px;
    font-size: 1.1rem;
    outline:0;
    padding: 0.5rem;
    transition: all 600ms ease;

  
  }

</style>
