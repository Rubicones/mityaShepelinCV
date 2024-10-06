<script>
	import fc from '$lib/assets/fc.jpg';
	import mw from '$lib/assets/mw.webp';
	import {
		Mail,
		Instagram,
		Linkedin,
		Target,
		MessageSquare,
		Cog,
		Bug,
		GraduationCap,
		BookOpen,
		Gauge,
		X
	} from 'lucide-svelte';
	import TypingText from '../components/TypingText.svelte';
</script>

<div class="w-full h-full">
	<div class="w-full h-[calc(100dvh-40px)] bg-white no-scrollbar p-16">
		<div class="w-full h-full flex gap-32">
			<div class="w-[55%] flex flex-col justify-center gap-16">
				<div class="flex flex-col">
					<TypingText caret={false} classList="text-7xl font-extrabold" text="Hi! I am Mitya," />
					<TypingText
						latency={800}
						classList="text-7xl font-extrabold"
						text="a software engineer."
					/>
				</div>

				<span class="text-2xl"
					>My 3 years of experience include working on a startup project, contributing at Yandex (a
					major tech company in Eastern Europe), and being part of the teams behind Call of Duty:
					Modern Warfare III and FC25. I'm now engaged in an exciting new AAA project!</span
				>
				<button
					class="p-2  border-2 border-black rounded-md text-lg flex items-center justify-center gap-3 w-40"
					>Get in touch
					<div
						class="w-6 h-6 rounded-full border-2 border-[#0070CC] flex justify-center items-center"
					>
						<X class="text-[#0070CC]" strokeWidth={2} />
					</div>
				</button>
			</div>
			<div class="w-[35%] h-full flex flex-col justify-center items-center gap-20">
				<div class="relative w-full group">
					<Target
						class="group-hover:blur-sm transition-all duration-[1s] absolute bottom-5 right-5 text-white animate-pulse z-30"
						size={45}
					/>
					<img
						class="w-full z-10 group-hover:blur-sm transition-all duration-[1s] rounded-lg"
						src={mw}
						alt="Call Of Duty: Modern Warfare game poster"
					/>
					<div
						class="absolute top-0 left-0 group-hover:opacity-100 opacity-0 transition-all duration-[1s] w-full h-full bg-neutral-900/50 z-20 p-4 text-white text-center text-lg rounded-md"
					>
						Call of Duty is a major AAA title that is played by over 100 million players every
						month. It includes mutiplayer and several singleplayer modes. The quality of solutions
						is very important for the game, because there are a lot of mechanics, modes, also
						performance should be taken into account. I worked on UI in multiple places of the game.
						If you want to find out more - reach the resume in the end of the website.
					</div>
				</div>
				<div class="relative w-full group">
					<Target
						class="group-hover:blur-sm transition-all duration-[1s] absolute bottom-5 right-5 text-white animate-pulse z-30"
						size={45}
					/>
					<img
						class="w-full z-10 group-hover:blur-sm transition-all duration-[1s] rounded-lg"
						src={fc}
						alt="Football Club 2025 game poster"
					/>
					<div
						class="absolute top-0 left-0 group-hover:opacity-100 opacity-0 transition-all duration-[1s] w-full h-full bg-neutral-900/50 z-20 p-4 text-white text-center text-lg rounded-md"
					>
						FC25 is a successful football simulator that was sold with more than 6 millions of
						copies over the world. Each time FC releases it’s a multi-national event. I was lucky to
						participate in development of UI for FC25, if you are curious about details - wait for
						the end of the website to check more info in the resume.
					</div>
				</div>
			</div>
		</div>
	</div>
	<div class="w-full h-[calc(100dvh-40px)] bg-white no-scrollbar px-16">
		<div class="w-full h-full flex flex-col justify-start items-center">
			<span class="text-6xl font-semibold text-center"
				>What do I do? <br />
				Flip the cards to find out more</span
			>
			<div class="h-full w-full grid grid-cols-3 grid-rows-2 pt-16">
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="relative tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20"
									>Gather requirements with designers and engineers</span
								>
								<MessageSquare size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>This also includes a feature breakdown, estimating delivery time, analyzing
									possible risks.</span
								>
							</div>
						</div>
					</div>
				</div>
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20">Design systems and logic</span
								>
								<Cog size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>By following best practices, I ensure the final solution is simple, scalable, and
									maintainable.</span
								>
							</div>
						</div>
					</div>
				</div>
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20">Fix bugs</span>
								<Bug size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>I have experience with fixing visual defects, crashes, concurrency issues,
									platform-specific bugs.</span
								>
							</div>
						</div>
					</div>
				</div>
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20">Perform optimizations</span>
								<Gauge size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>Collecting data about memory consumption and frame runtime allows me to choose
									better algorithms.</span
								>
							</div>
						</div>
					</div>
				</div>
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20">Write documentaiton</span>
								<BookOpen size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>For me, knowledge sharing isn't just about mentoring junior developers—it's a
									vital part of my daily routine.</span
								>
							</div>
						</div>
					</div>
				</div>
				<div class="tileDropShadow w-full flex justify-center">
					<div class="tile">
						<div class="tile-inner">
							<div
								class="tile-front self-center bg-neutral-100 border-2 flex flex-col p-2 items-center justify-around"
							>
								<span class="text-3xl font-semibold text-center z-20">Share knowledge</span>
								<GraduationCap size={200} class="absolute top-0 left-5 text-neutral-200 z-10" />
							</div>
							<div class="tile-back self-center bg-neutral-100 border-2 flex flex-col p-2">
								<span class="text-2xl font-light text-center"
									>I've created clear, structured documentation with visuals and helpful tips for
									developers and designers.</span
								>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="w-full h-[40px] sticky bottom-0 bg-black flex justify-center items-center gap-6">
		<a href=""><Mail class="text-white" size={25} /></a>
		<a href=""><Instagram class="text-white" size={25} /></a>
		<a href=""><Linkedin class="text-white" size={25} /></a>
	</div>
</div>

<style lang="sass">
	.tileDropShadow
		position: relative
	
		.tile
			.tile-inner
				text-align: center
				transition: transform 0.8s
				transform-style: preserve-3d
				position: relative
				width: 350px
				height: 200px
				background-color: #faf8f8
				text-align: center
				perspective: 1000px
				
	
			.tile-front, .tile-back
				position: absolute
				width: 100%
				height: 100%
				-webkit-backface-visibility: hidden
				backface-visibility: hidden
				border-radius: 8px

	
			.tile-back
				transform: rotateY(180deg)
				box-sizing: border-box
	
			&:hover
				.tile-inner
					transform: rotateY(180deg)
	
	

</style>
