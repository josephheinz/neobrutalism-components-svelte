<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div
  class={cn(
    "rounded-base flex flex-col shadow-shadow border-2 gap-6 py-6 border-border bg-background text-foreground font-base",
    className
  )}
  {...$$restProps}
>
  <slot />
</div>
