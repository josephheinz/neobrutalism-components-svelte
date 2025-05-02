<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div
  class={cn(
    "col-start-2 row-span-2 row-start-1 self-start justify-self-end",
    className
  )}
  {...$$restProps}
>
  <slot />
</div>
