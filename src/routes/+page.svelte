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

  import Card from "$lib/components/card/Card.svelte";
  import CardAction from "$lib/components/card/CardAction.svelte";
  import CardContent from "$lib/components/card/CardContent.svelte";
  import CardDescription from "$lib/components/card/CardDescription.svelte";
  import CardFooter from "$lib/components/card/CardFooter.svelte";
  import CardHeader from "$lib/components/card/CardHeader.svelte";
  import CardTitle from "$lib/components/card/CardTitle.svelte";

  import Input from "$lib/components/input/Input.svelte";

  import Label from "$lib/components/label/Label.svelte";
</script>

<h1>Neobrutalism Components Svelte 5</h1>
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
    <BreadcrumbSeparator />
    <BreadcrumbItem>
      <BreadcrumbLink href="/">Components</BreadcrumbLink>
    </BreadcrumbItem>
    <BreadcrumbSeparator />
    <BreadcrumbItem>
      <BreadcrumbPage>Breadcrumb</BreadcrumbPage>
    </BreadcrumbItem>
  </BreadcrumbList>
</Breadcrumb>

<Card className="w-full max-w-sm">
  <CardHeader>
    <CardTitle>Login to your account</CardTitle>
    <CardDescription>
      Enter your email below to login to your account
    </CardDescription>
  </CardHeader>
  <CardContent>
    <form>
      <div class="flex flex-col gap-6">
        <div class="grid gap-2">
          <Label htmlFor="email">Email</Label>
          <Input id="email" type="email" placeholder="m@example.com" required />
        </div>
        <div class="grid gap-2">
          <div class="flex items-center">
            <Label htmlFor="password">Password</Label>
            <a
              href="#"
              class="ml-auto inline-block text-sm underline-offset-4 hover:underline"
            >
              Forgot your password?
            </a>
          </div>
          <Input id="password" type="password" required />
        </div>
      </div>
    </form>
  </CardContent>
  <CardFooter className="flex-col gap-2">
    <Button className="w-full">Login</Button>
    <Button variant="neutral" className="w-full">Login with Google</Button>
    <div class={"mt-4 text-center text-sm"}>
      Don&apos;t have an account?{" "}
      <a href="#" class={"underline underline-offset-4"}> Sign up </a>
    </div>
  </CardFooter>
</Card>
