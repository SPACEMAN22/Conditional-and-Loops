# Conditional-and-Loops
HTML 
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.5.13/vue.min.js"></script>
<div id="app">
  <button @click="change()">Set Strawberry</button>
  <select v-model="selectedFlavor">
    <option v-for="flavor in flavors" :value="flavor">{{flavor}}</option>
  </select>
</div>

JavaSCript/Vue

new Vue({
  el: '#app',
  data: function() {
    return {
      selectedFlavor: 'lime',
      flavors: ['blueberry', 'lime', 'strawberry']
    }
  },
  methods: {
    change: function() {
      this.selectedFlavor = 'strawberry';
    }
  }
})
