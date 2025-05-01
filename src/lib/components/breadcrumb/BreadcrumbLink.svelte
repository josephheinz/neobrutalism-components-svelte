<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
  export let href = "";
</script>

<a class={cn(className)} {href}>
  <slot />
</a>
