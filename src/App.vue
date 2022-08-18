
<script>
export default {
  data: () => ({
    contador: 0,
    }),

    methods: {
      aumentar() { this.contador += 1},
      disminuir() {this.contador -= 1}, 
      reset(){this.contador = 0}
    }


}
</script>

 <template>
  <div container>
    <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
    <small>
      <h1> Hola mundo desde Vue3.j</h1>
    </small>  
    <hr />
    <h2> Contador:  {{contador}}</h2>
    <!--<button v-on:click="aumentar()">+1</button>-->
    <button @click="aumentar()">+1</button>
    <button @click="disminuir()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
 </template>


<style scoped >

small{
  color: #D4D4D4;
}
h1{
  font-weight: bolder;
}
h2 {
  font-size: 2.5rem;
}
button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
.container {
  text-align: center;
  background-color: #C2C2C2;
}

</style>