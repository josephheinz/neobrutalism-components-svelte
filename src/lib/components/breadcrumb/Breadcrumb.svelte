<script lang="ts">
  import { cn } from "$lib/utils";

  export let className = "";
</script>

<nav
    class={cn(className)}
>
    <slot/>
</nav>