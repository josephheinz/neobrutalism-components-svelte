<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<span
  class={cn(
    "text-sm font-heading leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70",
    className
  )}
  {...$$restProps}
>
  <slot />
</span>
