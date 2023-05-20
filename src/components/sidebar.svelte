<script>
	import { AppRail, AppRailTile } from '@skeletonlabs/skeleton';
	import UserIcon from '../assets/icons/user-icon.svelte';
	import { derived } from 'svelte/store';
	import { page } from '$app/stores';

    const selected = derived(page, $page => $page.url.pathname)

</script>

<AppRail {selected}>
	<AppRailTile label="Page 1" href="/1">
		<UserIcon />
	</AppRailTile>
	<AppRailTile label="Page 2" href="/2">
		<UserIcon />
	</AppRailTile>
	<AppRailTile label="Page 3" href="/3">
		<UserIcon />
	</AppRailTile>
</AppRail>
