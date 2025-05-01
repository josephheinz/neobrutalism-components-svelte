<script>
  import Alert from "$lib/components/alert/Alert.svelte";
  import AlertDescription from "$lib/components/alert/AlertDescription.svelte";
  import AlertTitle from "$lib/components/alert/AlertTitle.svelte";

  import Avatar from "$lib/components/avatar/Avatar.svelte";
  import AvatarFallback from "$lib/components/avatar/AvatarFallback.svelte";
  import AvatarImage from "$lib/components/avatar/AvatarImage.svelte";

  import Breadcrumb from "$lib/components/breadcrumb/Breadcrumb.svelte";
  import BreadcrumbEllipsis from "$lib/components/breadcrumb/BreadcrumbEllipsis.svelte";
  import BreadcrumbItem from "$lib/components/breadcrumb/BreadcrumbItem.svelte";
  import BreadcrumbLink from "$lib/components/breadcrumb/BreadcrumbLink.svelte";
  import BreadcrumbList from "$lib/components/breadcrumb/BreadcrumbList.svelte";
  import BreadcrumbPage from "$lib/components/breadcrumb/BreadcrumbPage.svelte";
  import BreadcrumbSeparator from "$lib/components/breadcrumb/BreadcrumbSeparator.svelte";

  import Badge from "$lib/components/badge/Badge.svelte";
  import Button from "$lib/components/button/Button.svelte";
</script>

<h1>Welcome to SvelteKit</h1>
<p>
  Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
  documentation
</p>
<Button>Button</Button>
<Badge variant="neutral">Neutral</Badge>
<Alert>
  <AlertTitle>Uh oh</AlertTitle>
  <AlertDescription>Something went wrong</AlertDescription>
  <Button
    size="sm"
    className="absolute top-2.5 right-3 h-6 bg-secondary-background text-foreground"
    >Try Again</Button
  >
</Alert>
<Avatar>
  <AvatarImage src="https://github.com/shadcn.png" alt="@shadcn" />
  <AvatarFallback>CN</AvatarFallback>
</Avatar>

<Breadcrumb>
  <BreadcrumbList>
    <BreadcrumbItem>
      <BreadcrumbLink href="/">Home</BreadcrumbLink>
    </BreadcrumbItem>
    <BreadcrumbSeparator />
    <BreadcrumbItem>
      <BreadcrumbEllipsis />
    </BreadcrumbItem>
    <BreadcrumbItem>
      <BreadcrumbSeparator />
    </BreadcrumbItem>
    <BreadcrumbItem>
      <BreadcrumbLink href="/">Components</BreadcrumbLink>
    </BreadcrumbItem>
    <BreadcrumbSeparator />
    <BreadcrumbItem>
      <BreadcrumbPage>Breadcrumb</BreadcrumbPage>
    </BreadcrumbItem>
  </BreadcrumbList>
</Breadcrumb>
