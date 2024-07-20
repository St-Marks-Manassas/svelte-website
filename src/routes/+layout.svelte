<script>
	import '../app.css';
	import { page } from '$app/stores';
	import {
		DarkMode,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		Button,
		Heading,
		P,
	} from 'flowbite-svelte';
		import { Cog } from 'svelte-heros-v2';

	let backdrop = false;
	const toggleDrawer = () => {
		drawerHidden = false;
	};
	$: activeUrl = $page.url.pathname;
	let spanClass = 'pl-2 self-center text-md text-gray-900 whitespace-nowrap dark:text-white';
	let divClass = 'w-full ml-auto lg:block lg:w-auto order-1 lg:order-none';
	let ulClass =
		'flex flex-col py-3 my-4 lg:flex-row lg:my-0 text-sm font-medium gap-4 dark:lg:bg-transparent lg:bg-white lg:border-0';
	let navDivClass =
		'bg-white dark:bg-gray-800 text-gray-500 dark:text-gray-400 border-gray-200 dark:border-gray-700 divide-gray-200 dark:divide-gray-700 flex items-center justify-between w-full mx-auto py-1.5 px-4';
</script>


<svelte:head>
    <script src="https://www.youtube.com/iframe_api"></script>
</svelte:head>


<header class="flex-none w-full mx-auto bg-white dark:bg-slate-950">
	<Navbar let:hidden let:toggle>
		<NavBrand href="/" >
			<Cog />
			<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white pl-4">
				St Marks UMC
			</span>
		</NavBrand>
 	   <div class="flex md:order-2">
 		<Button size="sm">Prayer Request</Button>
 		<NavHamburger />
	  </div>
		<NavUl>
			<NavLi class="lg:px-2 lg:mb-0" active={activeUrl === '/'} href="/">Home</NavLi>
			<NavLi class="lg:px-2 lg:mb-0" active={activeUrl === '/pages/about'} href="/pages/about">About</NavLi>
			<NavLi class="lg:px-2 lg:mb-0" href="https://github.com/shinokada/flowbite-sveltekit-responsive-sidebar-layout">GitHub</NavLi>
		</NavUl>
	</Navbar>
</header>
<div class="flex px-4 mx-auto w-full">
	<main class="w-full mx-auto">
		<slot />
	</main>
</div>
<footer class="flex-none mx-auto bg-white dark:bg-slate-950">
	<div class="grid xl:grid-cols-2 sm:grid-cols-1 gap-4 mx-auto w-4/5 place-items-start">
		<div>
			<Heading tag="h4">Location</Heading>
		</div>
		<div>
			<Heading tag="h4">Site</Heading>
		</div>
	</div>
</footer>

