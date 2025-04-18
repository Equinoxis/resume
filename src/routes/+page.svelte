<script>
	import resume from '$lib/data/resume.json';
	const references = JSON.parse(import.meta.env.VITE_REFERENCES_JSON);

	function downloadPDF() {
		window.print();
	}
</script>

<main class="relative mx-auto flex h-full w-full max-w-4xl flex-col gap-4 bg-white p-4">
	<section class="flex flex-col gap-2 text-center">
		<h1 class="text-xl font-bold">{resume.personal.name}</h1>
		<p class="font-medium">{resume.personal.title}</p>

		<div class="flex flex-col items-center justify-center gap-1 text-sm sm:flex-row sm:gap-4">
			<a href={`tel:${resume.personal.phone}`} class="inline-flex items-center gap-1">
				<img
					src="/fontawesome/phone-solid.svg"
					class="h-4 w-4"
					alt="Phone icon"
					aria-hidden="true"
				/>
				{resume.personal.phone}
			</a>
			<a href={`mailto:${resume.personal.email}`} class="inline-flex items-center gap-1">
				<img
					src="/fontawesome/envelope-solid.svg"
					class="h-4 w-4"
					alt="Envelope icon"
					aria-hidden="true"
				/>
				{resume.personal.email}
			</a>
			<address class="inline-flex items-center gap-1 not-italic">
				<img
					src="/fontawesome/location-dot-solid.svg"
					class="h-4 w-4"
					alt="Location icon"
					aria-hidden="true"
				/>
				{resume.personal.address}
			</address>
		</div>

		<div class="flex items-center justify-center gap-2 text-sm sm:gap-4">
			<a
				href={resume.personal.github.url}
				target="_blank"
				class="inline-flex items-center gap-[2px] text-blue-600 hover:text-blue-800"
			>
				<img
					src="/fontawesome/github-brands.svg"
					class="h-4 w-4"
					alt="GitHub icon"
					aria-hidden="true"
				/>
				{resume.personal.github.username}
			</a>
			<a
				href={resume.personal.linkedin.url}
				target="_blank"
				class="inline-flex items-center gap-[2px] text-blue-600 hover:text-blue-800"
			>
				<img
					src="/fontawesome/linkedin-brands.svg"
					class="h-4 w-4"
					alt="LinkedIn icon"
					aria-hidden="true"
				/>
				{resume.personal.linkedin.username}
			</a>
			<a
				href={resume.personal.website.url}
				target="_blank"
				class="inline-flex items-center gap-[2px] text-blue-600 hover:text-blue-800"
			>
				<img
					src="/fontawesome/globe-solid.svg"
					class="h-4 w-4"
					alt="Website icon"
					aria-hidden="true"
				/>
				{resume.personal.website.display}
			</a>
		</div>
	</section>

	<article class="flex flex-col gap-2">
		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Summary</h2>
			<p class="text-sm font-normal">{resume.summary}</p>
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Education</h2>
			{#each resume.education as edu}
				<div class="mb-1">
					<h3 class="text-sm font-semibold">{edu.school}</h3>
					<p class="text-sm font-normal">{edu.degree}</p>
					<p class="text-xs font-normal text-gray-600">{edu.years}</p>
				</div>
			{/each}
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Projects</h2>
			{#each resume.projects as project}
				<div class="mb-2 {project.noprint ? 'print:hidden' : ''}">
					<div class="flex items-center justify-between">
						<div class="flex items-center gap-2">
							<h3 class="text-sm font-bold">{project.title}</h3>
							{#if project.url}
								<a
									href={project.url}
									target="_blank"
									class="text-blue-600 hover:text-blue-800"
									aria-label="See {project.title}'s website"
								>
									<svg
										stroke="currentColor"
										fill="currentColor"
										stroke-width="0"
										viewBox="0 0 512 512"
										height="12"
										width="12"
										xmlns="http://www.w3.org/2000/svg"
									>
										<path
											d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
										></path>
									</svg>
								</a>
							{/if}
						</div>
						<p class="text-xs font-normal text-gray-600">{project.year}</p>
					</div>
					<p class="text-sm font-normal">{project.description}</p>
					<ul class="list-disc pl-4 text-sm">
						{#each project.bullets as bullet}
							<li>{bullet}</li>
						{/each}
					</ul>
				</div>
			{/each}
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Work Experience</h2>

			{#each resume.experience as exp}
				<div class="mb-2 {exp.noprint ? 'print:hidden' : ''}">
					<div class="flex items-center justify-between">
						<h3 class="text-sm font-bold">{exp.company} - {exp.title}</h3>
						<p class="text-xs font-normal text-gray-600">{exp.years}</p>
					</div>

					{#each exp.description as desc}
						<p class="text-sm font-normal">{desc}</p>
					{/each}
				</div>
			{/each}
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Technical Skills</h2>
			<p class="text-sm font-normal">{resume.skills.technical.join(', ')}</p>
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Soft Skills</h2>
			<p class="text-sm font-normal">{resume.skills.soft.join(', ')}</p>
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Languages</h2>
			<p class="text-sm font-normal">{resume.languages.join(', ')}</p>
		</section>

		<section>
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">References</h2>

			<div class="grid grid-cols-2 gap-2">
				{#each references as ref}
					<div class="">
						<h3 class="text-sm font-normal">{ref.name}</h3>

						<p class="flex flex-col text-sm font-normal sm:flex-row sm:items-center sm:gap-2">
							<span>{ref.title}</span>

							{#if ref.link}
								<a
									href={ref.link}
									target="_blank"
									class="text-blue-600 hover:text-blue-800"
									aria-label="See person"
								>
									<svg
										stroke="currentColor"
										fill="currentColor"
										viewBox="0 0 512 512"
										height="12"
										width="12"
										xmlns="http://www.w3.org/2000/svg"
									>
										<path
											d="M432,320H400a16,16,0,0,0-16,16V448H64V128H208a16,16,0,0,0,16-16V80a16,16,0,0,0-16-16H48A48,48,0,0,0,0,112V464a48,48,0,0,0,48,48H400a48,48,0,0,0,48-48V336A16,16,0,0,0,432,320ZM488,0h-128c-21.37,0-32.05,25.91-17,41l35.73,35.73L135,320.37a24,24,0,0,0,0,34L157.67,377a24,24,0,0,0,34,0L435.28,133.32,471,169c15,15,41,4.5,41-17V24A24,24,0,0,0,488,0Z"
										></path>
									</svg>
								</a>
							{/if}
						</p>

						<div class="flex flex-col text-sm text-gray-800 sm:flex-row sm:gap-4">
							{#if ref.email}
								<a href={`mailto:${ref.email}`} class="inline-flex items-center gap-1">
									<img src="/fontawesome/envelope-solid.svg" class="h-4 w-4" alt="Email icon" />
									{ref.email}
								</a>
							{/if}

							{#if ref.phone}
								<a href={`tel:${ref.phone}`} class="inline-flex items-center gap-1">
									<img src="/fontawesome/phone-solid.svg" class="h-4 w-4" alt="Phone icon" />
									{ref.phone}
								</a>
							{/if}
						</div>
					</div>
				{/each}
			</div>
		</section>
	</article>

	<button
		class="fixed right-2 bottom-2 aspect-square cursor-pointer rounded-full border border-black bg-white sm:right-8 sm:bottom-8 print:hidden"
		on:click={downloadPDF}
	>
		<span class="sr-only">Download my resume as a PDF</span>
		<img
			src="/fontawesome/download-solid.svg"
			class="m-3 h-4 w-4"
			alt="Download icon"
			aria-hidden="true"
		/>
	</button>
</main>
