<script>
	import HamburgerIcon from '../assets/icons/hamburger-icon.svelte';
	import UserIcon from './../assets/icons/user-icon.svelte';
	import { AppBar } from '@skeletonlabs/skeleton';
</script>

<AppBar slotTrail="place-content-end" slotDefault="place-self-center">
	<svelte:fragment slot="lead">
		<HamburgerIcon />
	</svelte:fragment>
	My Skelton App
	<svelte:fragment slot="trail">
		<UserIcon />
	</svelte:fragment>
</AppBar>
