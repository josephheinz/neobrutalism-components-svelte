<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<a class={cn(className)} {...$$restProps}>
  <slot />
</a>
