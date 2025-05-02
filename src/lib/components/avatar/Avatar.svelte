<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div
  class={cn(
    "relative flex size-10 shrink-0 overflow-hidden rounded-full outline-2 outline-border",
    className
  )}
  {...$$restProps}
>
  <slot />
</div>
