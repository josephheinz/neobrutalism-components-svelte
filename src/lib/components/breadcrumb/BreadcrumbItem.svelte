<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<li class={cn("inline-flex items-center gap-1.5", className)}>
  <slot />
</li>
