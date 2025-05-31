<script lang="ts">
  interface GenericButtonInterface {
    /** The text inside the button */
    text: string;

    /** Tailwind CSS classes to be applied to the button */
    class: string;

    /** Callback function for when clicking on the button */
    onClick: () => void;
  }

  let { text, class: className, onClick }: GenericButtonInterface = $props();
</script>

<button
  class={`${className} mx-0.5 my-1 cursor-pointer px-8 py-4 text-center text-lg text-white`}
  onclick={onClick}
>
  {text}
</button>
