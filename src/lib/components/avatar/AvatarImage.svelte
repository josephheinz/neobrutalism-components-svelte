<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
  export let src = "";
  export let alt = "";
</script>

<img
  {src}
  {alt}
  class={cn("aspect-square size-full absolute", className)}
  {...$$restProps}
/>
