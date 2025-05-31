<script lang="ts">
    interface GenericButtonInterface{
        /** The text inside the button */
        text: string;

        /** Tailwind CSS classes to be applied to the button */
        class: string;

        /** Callback function for when clicking on the button */
        onClick: () => void;
    }

    let {text, class: className, onClick}: GenericButtonInterface = $props();
</script>

<button class={`${className} text-white my-1 mx-0.5 px-8 py-4 text-center cursor-pointer text-lg`} onclick={onClick}>
    {text}
</button>