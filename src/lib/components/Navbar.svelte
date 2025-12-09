<script lang="ts">
	import NavLink from './NavLink.svelte';
    import Logo from './Logo.svelte';
</script>

<nav class="flex items-center justify-between px-6 py-5 max-w-7xl mx-auto w-full">
	<Logo color="black" />

	<div class="hidden md:flex items-center gap-8">
		<NavLink title="Home" />
		<NavLink title="Sourcing" />
		<NavLink title="Evaluation" />
		<NavLink title="Tracking" />
		<NavLink title="Communication" />
		<NavLink title="Early access" />
	</div>
</nav>
