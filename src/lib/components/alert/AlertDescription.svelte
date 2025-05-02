<script lang="ts">
  import { cn } from "$lib/utils";
  import { cva, type VariantProps } from "cva";

  export let className = "";
</script>

<div
  class={cn(
    "col-start-2 grid justify-items-start gap-1 text-sm font-base [&_p]:leading-relaxed",
    className
  )}
  {...$$restProps}
>
  <slot />
</div>
