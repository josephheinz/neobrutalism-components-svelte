<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<ol
  class={cn(
    "flex flex-wrap items-center gap-1.5 text-sm font-base break-words text-foreground sm:gap-2.5",
    className
  )}
  {...$$restProps}
>
  <slot />
</ol>
