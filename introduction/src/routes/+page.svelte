<!-- JS or TS -->
<script lang="ts">
    let word = $state<string>('world');
    let count = $state<number>(0);
</script>

<!-- Normal HTML -->
<h2>Hello {word}!</h2>
<p>Why don't you try clicking on the button</p>
<button onclick={() => {count++}}>Click me</button>
<p>Button clicked {count} times</p>

<!-- Normal css -->
<style>
    h2{color: green;}
    button{
         border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  background-color: #008CBA;
    }
</style>
