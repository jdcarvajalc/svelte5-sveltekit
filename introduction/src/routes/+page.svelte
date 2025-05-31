<!-- JS or TS -->
<script lang="ts">
    let word = $state<string>('world');
    let count = $state<number>(0);
</script>

<!-- Normal HTML -->
<h2 class="text-green-700">Hello {word}!</h2>
<p>Why don't you try clicking on the button</p>
<button class="text-white my-1 mx-0.5 px-8 py-4 text-center bg-[#008CBA] cursor-pointer text-lg" onclick={() => {count++}}>
    Click me
</button>
<p>Button clicked {count} times</p>

