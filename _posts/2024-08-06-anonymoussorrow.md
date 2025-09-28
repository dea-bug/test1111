---
layout: post
title: "Anonymous Sorrow - Ann Marie Stillion"
author: "Deana Seitz and Aster Teter"
categories: gallery
tags: [gallery, color grading, editing]
image: as-1.jpg
---

<style>
:root {

	--section-spacing-block: 10rem;
	--container-slim-max-wdith: 50rem;
	--container-max-wdith: 100rem;

	background: #080e17;
	color: white;
	line-height: 1.6;
	font-family: system-ui;
}


body {
	margin: 0;
}

p {
	margin: 2em 0;
}

.cover-flow {
	perspective: 100rem;
	// overflow: clip;
	padding: 4rem 0;

	&__track {
		transform-style: preserve-3d;
		display: grid;
	}

	&__space {
		transform-style: preserve-3d;
		view-timeline-name: --name-space;
		view-timeline-axis: block;
	}

	&__cover {
		margin: 0 auto;
		display: block;
		width: 31.25rem;
		max-width: 80wv;
		object-fit: cover;
		animation: linear cover both;
		animation-timeline: view(block);
		transform-style: preserve-3d;
		will-change: transform;
		position: relative;
		user-select: none;
		border-radius: .5rem;
		animation-timeline: --name-space;
		// animation-range: contain 0% contain 100%;

		/*
		animation: cover auto linear both;
		animation-range: contain 0% contain 100%;
		animation-timeline: --sticky-timeline;
		*/
	}

}


.sticky-section_ {
	height: 300vh;
	position: relative;

	view-timeline-name: --sticky-timeline;
	view-timeline-axis: block;

	&__stack {
		position: sticky;
		top: 0;
	}

}


.section {
	margin-block: 10rem;
}

.wrapping {
	padding-inline: var(--wrapper-spacing);
}


.container {
	margin-inline: auto;
	max-width: var(--container-max-wdith);

	&--slim {
		--container-max-wdith: var(--container-slim-max-wdith);
	}

}


@keyframes cover {
	0% {
		transform: translateY(-100%) rotateX(45deg);
	}
	35% {
		transform: translateY(0) rotateX(45deg);
	}
	50% {
		box-shadow: 0 0 1rem .5rem #00000080;
		transform: rotateX(0deg) translateZ(14em) scale(1.2);
	}
	65% {
		transform: translateY(0) rotateX(-45deg);
	}
	100% {
		transform: translateY(100%) rotateX(-45deg);
	}
}

</style>
<div class="section">
	<div class="wrapping">
		<div class="container container--slim">
			<div>
				<h1>Moments by the Sea</h1>
				<p>From the powerful curl of ocean waves to the quiet presence of a lone starfish, these images capture the serene beauty of the shoreline — where sand meets sea and nature speaks in tides.</p>
			</div>
		</div>
	</div>
</div>
<div class="section">
	<div class="wrapping">
		<div class="container container--slim">
			<div class="cover-flow">
				<div class="cover-flow__track">
					<div class="cover-flow__space"><img src="https://images.unsplash.com/photo-1501949997128-2fdb9f6428f1?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wzMjM4NDZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE3NTIyNjYzNTZ8&ixlib=rb-4.1.0&q=80&h=900" alt="Closeup of a curling ocean wave." title="photo by Jeremy Bishop for Unsplash" class="cover-flow__cover"></div>
					<div class="cover-flow__space"><img src="https://images.unsplash.com/photo-1476673160081-cf065607f449?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wzMjM4NDZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE3NTIyNjYzOTJ8&ixlib=rb-4.1.0&q=80&h=900" alt="Foamy waves gently lapping a sandy beach shore." title="photo by Frank McKenna for Unsplash" class="cover-flow__cover"></div>
					<div class="cover-flow__space"><img src="https://images.unsplash.com/photo-1490365728022-deae76380607?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wzMjM4NDZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE3NTIyNjY0Mjd8&ixlib=rb-4.1.0&q=80&h=900" alt="A starfish at the shallow edge of ocean water, alone on a backdrop of white sand." title="photo by Amy Humphries for Unsplash" class="cover-flow__cover"></div>
					<div class="cover-flow__space"><img src="https://images.unsplash.com/photo-1506252374453-ef5237291d83?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3wzMjM4NDZ8MHwxfHJhbmRvbXx8fHx8fHx8fDE3NTIyNjY0NzR8&ixlib=rb-4.1.0&q=80&h=900" alt="An aerial view of waves rolling onto a sandy beach." title="photo by Samuel Scrimshaw for Unsplash" class="cover-flow__cover"></div>

				</div>
			</div>
		</div>
	</div>
</div>


<div class="section">
	<div class="wrapping">
		<div class="container container--slim">
			<div>
				<h2>Reflections from the Shore</h2>
				<p>
					Waves curl and crash in a rhythm older than time, their motion a reminder of nature's quiet strength.
				</p>
				<p>
					Foam traces the shoreline in gentle pulses, smoothing the sand and softening the edges of the world.
				</p>
				<p>
					At the water’s edge, a lone starfish rests — still, patient, and perfectly placed in the morning light.
				</p>
				<p>
					From above, the sea paints patterns on the beach, each wave a brushstroke on the canvas of the coast.
				</p>
				<p>
					These moments are fleeting, but in their stillness, they hold something lasting — peace, motion, and the simple poetry of tide and sand.
				</p>
			</div>
		</div>
	</div>
</div>


<br>

<iframe src="https://player.vimeo.com/video/997865296?h=715e669524&color=7a1818&title=0&byline=0&portrait=0" width="640" height="360" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>

Gallery video of Ann Marie Stillion's "Anonymous Sorrow" <br>

https://www.arttrek.com/ <br>
https://www.coregallery.org/ann-marie-stillion <b>

Director: Ann Marie Stillion @annmariestillion <br>
Editor: Deana Seitz @joybirdstudios <br>
Cinematography & Color Grade: Aster Teter @joybirdstudios <br>
Camera Assistant: Drew Boysen @drew.boysen <br>


<img src="{{site.baseurl}}/assets/img/as-2.jpg">