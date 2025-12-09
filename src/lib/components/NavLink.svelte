<script lang="ts">
	export let title: string;
	export let href: string = "#";
</script>

<a {href} class="text-sm font-medium text-gray-600 hover:text-black transition-colors">
	{title}
</a>
