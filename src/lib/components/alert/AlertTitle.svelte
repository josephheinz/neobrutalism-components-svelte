<script lang="ts">
  import { cn } from "$lib/utils";
  import { cva, type VariantProps } from "cva";

  export let className = "";
</script>

<div
  class={cn(
    "col-start-2 line-clamp-1 min-h-4 font-heading tracking-tight",
    className
  )}
  {...$$restProps}
>
  <slot />
</div>
