<!-- JS or TS -->
<script lang="ts">
    let word = $state<string>('world');
    let count = $state<number>(0);
    
    let info = $derived.by<string>(()=>{
        if(count === 0){
            return "Why don't you try clicking on the button";
        }
        if(count === 1){
            return "You clicked the button once";
        }
        return "You clicked the button " + count + " times";
    })

    function onClick(){
        count++;
    }
</script>

<!-- Normal HTML -->
<h2 class="text-green-700">Hello {word}!</h2>
<button class="text-white my-1 mx-0.5 px-8 py-4 text-center bg-[#008CBA] cursor-pointer text-lg" onclick={onClick}>
    Click me
</button>
<p>{info}</p>

