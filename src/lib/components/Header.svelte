<script>
    import { AppBar, TabGroup, TabAnchor, LightSwitch } from "@skeletonlabs/skeleton";
    import { page } from "$app/stores";
</script>

<AppBar gridColumns="grid-cols-3 px-4" slotDefault="place-self-center px-4" slotTrail="place-content-end px-4">
    <svelte:fragment slot="lead">
        <h1 class="h1">edGGG</h1>
    </svelte:fragment>
    <TabGroup
        justify="justify-center"
        active="variant-filled-primary"
        hover="hover:variant-soft-primary"
        flex="flex-1 lg:flex-none"
        rounded=""
        border=""
        class="bg-surface-100-800-token w-full"
    >
    <TabAnchor href="/about" selected={$page.url.pathname === '/about'}>
        <span>About</span>
    </TabAnchor>
    <TabAnchor href="/" selected={$page.url.pathname === '/'}>
        <span>Home</span>
    </TabAnchor>
    <TabAnchor href="/search" selected={$page.url.pathname === '/search'}>
        <span>Search</span>
    </TabAnchor>
    </TabGroup>
    <svelte:fragment slot="trail">
        <LightSwitch />
    </svelte:fragment>
</AppBar>