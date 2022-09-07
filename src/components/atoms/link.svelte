<script lang="ts">
	export let to: string;

	const links: { [key: string]: string } = {
		home: "Home",
		about: "About",
		platform: "Platform",
		team: "Team",
		contact: "Contact Us",
	};
</script>

<a
	href={`/${to === "home" ? "" : to}`}
	class="bg-transparent font-sans rounded-md text-lg">{links[to]}</a
>

<style>
	a {
		color: rgba(48, 25, 110, 1);
	}
	a:hover {
		color: rgba(240, 150, 13, 1);
	}
	a:visited {
		color: rgba(240, 150, 13, 1);
	}
</style>
