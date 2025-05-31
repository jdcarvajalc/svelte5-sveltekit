<!-- JS or TS -->
<script lang="ts">
    let word = $state('world')
</script>

<!-- Normal HTML -->
<p>Hello {word}!</p>
<button onclick={() => console.log('Button clicked')}>Click me</button>

<!-- Normal css -->
<style>
    p{color: green;}
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
