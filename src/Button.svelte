<script>
    export let botao = 'botao'

</script>


<button class={botao} on:click>
    <slot></slot>
</button>

<style>

  Button {
  width: 45px;
  margin-bottom: 25px;
  border: 4px;
  border-radius: 9px;
  cursor: pointer;
  text-align: center;
  user-select: none;
}

 Button:hover {
  background-color: darkgray;
  transition: background 0.5s;
  transform: scale(1.4);
}

Button:active {
  transform: translate(1.2px, 1.2px)
}  
</style>