<script lang="ts">
  import { cn } from "$lib/utils";
  import Ellipsis from "@lucide/svelte/icons/ellipsis";

  export let className = "";
</script>

<span
  class={cn("flex size-9 items-center justify-center", className)}
  aria-hidden="true"
  {...$$restProps}
>
  <Ellipsis class="size-4" />
  <span class="sr-only">More</span>
</span>
