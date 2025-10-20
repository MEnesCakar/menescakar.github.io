<script lang="ts">
	import SunIcon from '@lucide/svelte/icons/sun';
	import MoonIcon from '@lucide/svelte/icons/moon';
	import SlingUpCover from '$lib/assets/covers/Sling_Up_Cover.7464e25a.jpg';
	import ZombieDefenseCover from '$lib/assets/covers/Zombie_Defense_Cover.d850343d.jpg';
	import SpaceSurvivorCover from '$lib/assets/covers/Space_Survivor_Cover.ec1d128e.png';
	import SuperKillCover from '$lib/assets/covers/SuperKill_IO_Cover.45a710bd.jpg';
	import ChillerCover from '$lib/assets/covers/ChillerCover.png';
	import KineuralCover from '$lib/assets/covers/KineuralCover.png';
	import TesaCover from '$lib/assets/covers/TesaCover.png';
	import TRLCover from '$lib/assets/covers/TRLCover.png';
	import PixelParrotCover from '$lib/assets/covers/PixelParrotCover.png';

	import { toggleMode } from 'mode-watcher';
	import { Button } from '$lib/components/ui/button/index.js';
	import ProjectItem from '$lib/components/custom/project-item-card.svelte';
</script>

<Button
	onclick={toggleMode}
	variant="outline"
	size="icon"
	class="sticky left-full shrink-1  mr-2 mt-2 hover:text-card-foreground hover:bg-card-foreground/1  !transition-all"
>
	<SunIcon
		class="h-[1.2rem] w-[1.2rem] scale-100 rotate-0 !transition-all dark:scale-0 dark:-rotate-90"
	/>
	<MoonIcon
		class="absolute h-[1.2rem] w-[1.2rem] scale-0 rotate-90  !transition-all dark:scale-100 dark:rotate-0 dark:text-card"
	/>
	<span class="sr-only">Toggle theme</span>
</Button>

<div
	class=" relative left-1/2 -translate-x-1/2 flex align-middle gap-5 justify-around w-full md:w-2/3 flex-wrap"
>
	<ProjectItem
		imgSrc={SpaceSurvivorCover}
		title="Space Survior"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
	<ProjectItem
		imgSrc={SuperKillCover}
		title="Super Kill"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
	<ProjectItem
		imgSrc={ZombieDefenseCover}
		title="Zombie Defense"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
	<ProjectItem
		imgSrc={SlingUpCover}
		title="Sling Up"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
	<ProjectItem
		imgSrc={TesaCover}
		title="T Dispenser"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
	<ProjectItem
		imgSrc={ChillerCover}
		title="Glaciem"
		description="Fast paced arcade game with simple gameplay, the level is procedurally generated"
		link="youtube.com"
	></ProjectItem>
</div>
