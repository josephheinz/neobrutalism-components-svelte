<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div
  class={cn(
    "flex size-full items-center justify-center rounded-full bg-secondary-background text-foreground font-base",
    className
  )}
>
  <slot />
</div>
