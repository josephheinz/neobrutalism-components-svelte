<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div class={cn("text-sm font-base", className)} {...$$restProps}>
  <slot />
</div>
