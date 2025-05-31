<script lang="ts">
  interface SectionTitleProps {
    /** Text to show in the title */
    text: string;

    /** Tailwind CSS classes to be applied to the title */
    class: string;
  }

  let { text, class: className }: SectionTitleProps = $props();
</script>

<h2 class={`${className}`}>{text}</h2>
