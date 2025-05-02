<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<div class={cn("font-heading leading-none", className)} {...$$restProps}>
  <slot />
</div>
