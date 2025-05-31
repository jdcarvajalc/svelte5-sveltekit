<script lang="ts">
    import GenericButton from "$lib/components/buttons/genericButton.svelte";
    import SectionTitle from "$lib/components/sectionTitle/sectionTitle.svelte";

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

<SectionTitle text={'Hello '+word+'!'} class={'text-green-700'} />
<GenericButton text={'Click me'} class={'bg-[#008CBA] rounded-2xl'} {onClick}/>
<p>{info}</p>

