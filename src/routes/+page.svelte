<script>
    import Button from "$lib/components/button/Button.svelte";
    import Badge from "$lib/components/badge/Badge.svelte";
    import Alert from "$lib/components/alert/Alert.svelte";
    import AlertDescription from "$lib/components/alert/AlertDescription.svelte";
    import AlertTitle from "$lib/components/alert/AlertTitle.svelte";
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>
<Button>Button</Button>
<Badge variant="neutral">Neutral</Badge>
<Alert>
    <AlertTitle>Uh oh</AlertTitle>
    <AlertDescription>Something went wrong</AlertDescription>
    <Button size="sm" className="absolute top-2.5 right-3 h-6 bg-secondary-background text-foreground">Try Again</Button>
</Alert>