<script lang="ts">
  import { cn } from "$lib/utils";
  import ChevronRight from "@lucide/svelte/icons/chevron-right";

  export let className = "";
</script>

<li
  class={cn("[&>svg]:size-3.5", className)}
  aria-hidden="true"
  {...$$restProps}
>
  <ChevronRight />
</li>
