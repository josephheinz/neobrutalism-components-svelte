<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<span
  class={cn(className)}
  aria-disabled="true"
  aria-current="page"
  {...$$restProps}
>
  <slot />
</span>
