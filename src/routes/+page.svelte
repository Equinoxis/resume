<script>
	function downloadPDF() {
		window.print();
	}
</script>

<main class="relative mx-auto flex h-full w-full max-w-4xl flex-col gap-4 bg-white p-4">
	<section class="flex flex-col gap-2 text-center">
		<h1 class="text-xl font-bold">Mathieu Renaud</h1>

		<p class="font-medium">IT Engineer - Cybersecurity and Electronic Banking</p>

		<div class="flex flex-col items-center justify-center gap-1 text-sm sm:flex-row sm:gap-4">
			<a
				class="inline-flex items-center gap-1"
				aria-label="Call me at +33641504249"
				href={`tel:+33641504249`}
			>
				<img
					src="/fontawesome/phone-solid.svg"
					class="h-4 w-4"
					alt="Phone icon"
					aria-hidden="true"
				/>
				+33641504249
			</a>
			<a
				class="inline-flex items-center gap-1"
				aria-label="Send me an email at mathieu.renaud29@gmail.com"
				href={`mailto:mathieu.renaud29@gmail.com`}
			>
				<img
					src="/fontawesome/envelope-solid.svg"
					class="h-4 w-4"
					alt="Envelope icon"
					aria-hidden="true"
				/>
				mathieu.renaud29@gmail.com
			</a>

			<p class="sr-only">Location:</p>
			<address
				aria-label="Send me a mail at 45 Rue de Bras, Caen, France"
				class="inline-flex items-center gap-1 not-italic"
			>
				<img
					src="/fontawesome/location-dot-solid.svg"
					class="h-4 w-4"
					alt="Location dot icon"
					aria-hidden="true"
				/>
				45 Rue de Bras, Caen, France
			</address>
		</div>

		<div class="flex items-center justify-center gap-2 text-sm sm:gap-4">
			<a
				href="https://github.com/Equinoxis"
				aria-label="See my GitHub"
				title="Github"
				target="_blank"
				rel="noreferrer"
				class="inline-flex items-center gap-[2px] text-blue-600 transition-colors hover:text-blue-800"
			>
				<span class="text-sm">
					<img
						src="/fontawesome/github-brands.svg"
						class="h-4 w-4"
						alt="GitHub icon"
						aria-hidden="true"
					/>
				</span>
				Equinoxis
			</a>

			<a
				href="https://www.linkedin.com/in/mathieu-renaud-inge/"
				aria-label="See my Linkedin"
				title="Linkedin"
				target="_blank"
				rel="noreferrer"
				class="inline-flex items-center gap-[2px] text-blue-600 transition-colors hover:text-blue-800"
			>
				<span class="text-sm">
					<img
						src="/fontawesome/linkedin-brands.svg"
						class="h-4 w-4"
						alt="LinkedIn icon"
						aria-hidden="true"
					/>
				</span>
				Mathieu Renaud
			</a>

			<a
				href="https://mathieurenaud.fr/"
				aria-label="See my website"
				title="Website"
				target="_blank"
				rel="noreferrer"
				class="inline-flex items-center gap-[2px] text-blue-600 transition-colors hover:text-blue-800"
			>
				<span class="text-sm">
					<img
						src="/fontawesome/globe-solid.svg"
						class="h-4 w-4"
						alt="Globe icon"
						aria-hidden="true"
					/>
				</span>
				mathieurenaud.fr
			</a>
		</div>
	</section>

	<article class="flex flex-col gap-2">
		<section class="">
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Summary</h2>

			<p class="text-sm font-normal">
				Computer science engineer with three years of experience in development. Passionate about
				DevOps and Web, with a keen interest in automating the development process. Currently
				studying computer engineering at ENSICAEN. My goal is to explore new experiences and take on
				exciting challenges.
			</p>
		</section>

		<section class="">
			<div>
				<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Education</h2>

				<div class="mb-1">
					<h3 class="text-sm font-semibold">
						École nationale supérieure d'ingénieurs de Caen (ENSICAEN)
					</h3>
					<p class="text-sm font-normal">IT Engineer - Cybersecurity and electronic banking</p>
					<p class="text-xs font-normal whitespace-nowrap text-gray-600">2022 - 2025</p>
				</div>
				<div class="mb-1">
					<h3 class="text-sm font-semibold">EM Normandie Business School</h3>
					<p class="text-sm font-normal">Master in Management - Grande Ecole Program</p>
					<p class="text-xs font-normal whitespace-nowrap text-gray-600">2023 - 2025</p>
				</div>
				<div class="mb-1">
					<h3 class="text-sm font-semibold">IT Carlow - South East Technological University</h3>
					<p class="text-sm font-normal">Bachelore of science - Software Development</p>
					<p class="text-xs font-normal whitespace-nowrap text-gray-600">2021 - 2022</p>
				</div>
				<div class="mb-1">
					<h3 class="text-sm font-semibold">IT Saint-Lô</h3>
					<p class="text-sm font-normal">Two year diploma - Multimédia and Internet</p>
					<p class="text-xs font-normal whitespace-nowrap text-gray-600">2019 - 2021</p>
				</div>
			</div>
		</section>

		<section class="">
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Projects</h2>

			<div class="flex flex-col gap-2">
				<div class="">
					<div class="flex items-center justify-between gap-2">
						<h3 class="text-sm font-bold">DevOps</h3>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2024 - 2025</p>
					</div>
					<p class="text-sm font-normal">
						Actively learning and applying DevOps methods in my free time by exploring CI/CD
						pipelines, containerization, and cloud deployment. While communicating with a team of
						developper.
					</p>
					<ul class="list-disc pl-4 text-sm font-normal">
						<li class="text-sm font-normal">
							Hosting an Apache2 multi-service Web server with Ubuntu Linux and a reverse proxy.
						</li>
						<li class="text-sm font-normal">
							Experimenting with automation tools such as Docker with Git and GitLab.
						</li>
						<li class="text-sm font-normal">
							Continuously improving my knowledge of monitoring, security, and scalability best
							practices to enhance system reliability and efficiency.
						</li>
					</ul>
				</div>

				<div class="">
					<div class="flex items-center justify-between gap-2">
						<div class="flex items-center gap-2">
							<h3 class="text-sm font-bold">Yellow Dot Decoder</h3>
							<a
								target="_blank"
								aria-label="See Yellow Dot Decoder's website"
								rel="noopener noreferrer"
								class="text-blue-600 hover:text-blue-800"
								title="https://yellow-dots-decoder.mathieurenaud.fr/"
								href="https://yellow-dots-decoder.mathieurenaud.fr/"
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
						</div>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2025</p>
					</div>
					<p class="text-sm font-normal">
						Developed an open-source tool to analyze yellow dot patterns in printed documents. These
						dots, embedded by laser printers, can encode details such as the printer's serial number
						and print date, raising privacy concerns.
					</p>
					<ul class="list-disc pl-4 text-sm font-normal">
						<li class="text-sm font-normal">
							Built an interactive web application for decoding yellow dot patterns.
						</li>
						<li class="text-sm font-normal">
							Implemented image processing techniques to enhance dot visibility.
						</li>
						<li class="text-sm font-normal">
							Contributed to raising awareness about forensic tracking in printed documents.
						</li>
					</ul>
				</div>

				<div class="">
					<div class="flex items-center justify-between gap-2">
						<div class="flex items-center gap-2">
							<h3 class="text-sm font-bold">Course project - engineering school</h3>
						</div>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2022 - 2025</p>
					</div>
					<p class="text-sm font-normal">
						Practice the different engineering notions seen in class through projects
					</p>
					<ul class="list-disc pl-4 text-sm font-normal">
						<li class="text-sm font-normal">
							Use SOLID principles and Software design patterns for application development
						</li>
						<li class="text-sm font-normal">
							Project management and analysis of project feasibility and risks
						</li>
						<li class="text-sm font-normal">
							Team management, practice the concepts acquired during the master's degree at EM
							Normandie
						</li>
					</ul>
				</div>
				<div class="">
					<div class="flex items-center justify-between gap-2">
						<div class="flex items-center gap-2">
							<h3 class="text-sm font-bold">Data science, Capture The Flag - TRACS</h3>
							<a
								target="_blank"
								aria-label="See TRACS's website"
								rel="noopener noreferrer"
								class="text-blue-600 hover:text-blue-800"
								title="https://tracs.viarezo.fr/"
								href="https://tracs.viarezo.fr/"
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
						</div>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2024</p>
					</div>
					<p class="text-sm font-normal">
						Participated at TRACS, a cybersecurity and data science competition organized by ViaRézo
						and the DGSE, tackling challenges in data science, cryptanalysis, and cybersecurity.
					</p>
					<ul class="list-disc pl-4 text-sm font-normal">
						<li class="text-sm font-normal">
							Solved complex cybersecurity and data science challenges, including cryptanalysis,
							data processing, anomaly detection and OSINT.
						</li>
						<li class="text-sm font-normal">
							Collaborated in a team environment, applying analytical and problem-solving skills
							under time constraints.
						</li>
					</ul>
				</div>

				<div class="">
					<div class="flex items-center justify-between gap-2">
						<div class="flex items-center gap-2">
							<h3 class="text-sm font-bold">Start-up weekend</h3>
							<a
								target="_blank"
								aria-label="See Start-up weekend's website"
								rel="noopener noreferrer"
								class="text-blue-600 hover:text-blue-800"
								title="https://startupsweekend.fr/"
								href="https://startupsweekend.fr/"
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
						</div>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2020</p>
					</div>
					<p class="text-sm font-normal">
						Participated in a 54-hour Startup Weekend, collaborating with a multidisciplinary team
						to develop a startup idea, build a prototype, and pitch to a panel of judges.
					</p>
					<ul class="list-disc pl-4 text-sm font-normal">
						<li class="text-sm font-normal">Imagine and develop a business project, as a team</li>
						<li class="text-sm font-normal">
							Managing a significant amount of work and information within a given time frame
						</li>
					</ul>
				</div>
			</div>
		</section>

		<section class="">
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Work Experience</h2>

			<div class="flex flex-col gap-2">
				<div class="">
					<div class="flex items-center justify-between gap-2">
						<h3 class="text-sm font-normal">
							<span class="font-bold">AIOA</span><span class="mx-1">-</span><span
								>Full stack developer - Apprenticeship</span
							>
						</h3>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2022 - 2025</p>
					</div>
					<p class="text-sm font-normal">
						Develop, and deploy web solutions, websites, and web-based applications, ensuring high
						performance. Implement user-friendly interfaces, and integrate backend services.
					</p>
					<p class="text-sm font-normal">
						Practice different engineering concepts, apply and experiment with various engineering
						concepts across development, automation, and system architecture.
					</p>
				</div>

				<div class="">
					<div class="flex items-center justify-between gap-2">
						<h3 class="text-sm font-normal">
							<span class="font-bold">LEEROY</span><span class="mx-1">-</span><span
								>Front-End developer - Internship abroad</span
							>
						</h3>
						<p class="text-xs font-normal whitespace-nowrap text-gray-600">2024 - 2024</p>
					</div>
					<p class="text-sm font-normal">
						Maintain and enhance websites by implementing new features and updates using Svelte or
						Vue.js. Collaborate with designers and backend developers to ensure seamless
						integration, optimal performance, and a responsive user experience.
					</p>
					<p class="text-sm font-normal">
						Gained international experience in Montreal, Canada, working in a multicultural
						environment.
					</p>
				</div>
			</div>
		</section>

		<section class="">
			<div>
				<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Technical Skills</h2>
				<p class="text-sm font-normal">
					Linux, Git, Docker, Apache2, JavaScript, TypeScript, C, C++, Java, Flutter, Android,
					Scala, SvelteKit, Vue.js, PHP, HTML, CSS, SASS, Tailwind CSS, Python, PostgreSQL,
					Firebase, Node.js, Github, Gitlab
				</p>
			</div>
		</section>

		<section class="">
			<div>
				<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Soft Skills</h2>
				<p class="text-sm font-normal">Communication, Resilience, Rigor, Curiosity, Team Spirit</p>
			</div>
		</section>

		<section class="">
			<div>
				<h2 class="mb-1 border-b-2 border-gray-300 font-bold">Languages</h2>
				<p class="text-sm font-normal">French, English - TOIEC (930/990)</p>
			</div>
		</section>

		<section class="">
			<h2 class="mb-1 border-b-2 border-gray-300 font-bold">References</h2>

			<h3 class="text-sm font-normal">Nicholas Charbonneau</h3>
			<p class="flex items-center gap-2 text-sm font-normal">
				Technical Director at LEEROY<a
					target="_blank"
					rel="noopener noreferrer"
					aria-label="See Leeroy's website"
					class="text-blue-600 hover:text-blue-800"
					title="Leeroy"
					href="https://www.leeroy.ca/"
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
			</p>
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
