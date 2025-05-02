<script lang="ts">
  import { cn } from "$lib/utils";
  import { cva, type VariantProps } from "cva";

  const badgeVariants = cva(
    "inline-flex items-center justify-center rounded-base border-2 border-border px-2.5 py-0.5 text-xs font-base w-fit whitespace-nowrap shrink-0 [&>svg]:size-3 gap-1 [&>svg]:pointer-events-none focus-visible:border-ring focus-visible:ring-ring/50 focus-visible:ring-[3px] overflow-hidden",
    {
      variants: {
        variant: {
          default: "bg-main text-main-foreground",
          neutral: "bg-secondary-background text-foreground",
        },
      },
      defaultVariants: {
        variant: "default",
      },
    }
  );

  export let variant: "default" | "neutral" = "default";
  export let className = "";
</script>

<div class={cn(badgeVariants({ variant }), className)} {...$$restProps}>
  <slot />
</div>
