<template>
	<div class="">
		<h1>Experience</h1>
		<div class="flex flex-col gap-8">
			<ExperienceItem class="mt-4" position="Software Engineering Intern" company="Lucid"
				date="May 2026 - Aug 2026" location="South Jordan, UT">
				Worked on Lucid's public-facing REST API and developer platform
				<ul class="ml-12 list-inside list-disc">
					<li>Designed and implemented configurable IP allowlisting for the REST API, letting customers
						restrict access to trusted IP ranges</li>
					<li>Redesigned user-search UI flows with autocomplete and smart recommendations, streamlining lookup
						for end users</li>
					<li>Built OAuth2 client management for integrations, including token revocation and client renaming
					</li>
				</ul>
				<TechStack :stack="['TypeScript', 'Scala', 'Angular', 'MySQL']" />
			</ExperienceItem>
			<ExperienceItem position="Web Developer" company="Brigham Young University" date="May 2024 - Present"
				location="Provo, UT">
				Developed and maintained <b>LearningSuite</b>, the university's Learning Management System used
				by <b>34,000+ students and faculty</b>
				<ul class="ml-12 list-inside list-disc">
					<li>Proposed and led a full migration of the legacy build system to Vite, converting
						thousands of files to ES Modules and greatly improving performance:
						<ul class="ml-12 list-outside sm:list-inside list-[circle]">
							<li>Production page load time sped up by <b>2.59x</b> <i aria-hidden="true"
									class="fa-solid fa-angles-up text-green-400"></i></li>
							<li>Compile time sped up by <b>2.55x</b> <i aria-hidden="true"
									class="fa-solid fa-angles-up text-green-400"></i></li>
							<li>Unit test pipeline sped up by <b>3.74x</b> <i aria-hidden="true"
									class="fa-solid fa-angles-up text-green-400"></i></li>
						</ul>
					</li>
					<li>Built core instructor-facing tools including assignment builders, exam question
						editors, grading dashboards, and discussion forum management</li>
				</ul>
				<div class="mt-6 flex gap-8 flex-col sm:flex-row">
					<div class="text-center">
						<Thumbnail :src="LSImage1" />
						<p>Assignment Editor</p>
						<p class="text-gray-300 text-sm">Developed an Assignment Editor tool for creating, editing, and
							managing course assignments, enabling instructors to configure settings, attach resources,
							and streamline the grading workflow.</p>
					</div>
					<div class="text-center">
						<Thumbnail :src="LSImage2" />
						<p>Question Bank</p>
						<p class="text-gray-300 text-sm">Developed a Question Bank tool for creating and organizing
							reusable question pools, enabling instructors, departments, and courses to share resources
							while tracking usage and performance statistics.</p>
					</div>
				</div>
				<TechStack :stack="['JavaScript', 'Vue.js', 'PHP', 'TailwindCSS']" />
			</ExperienceItem>
			<ExperienceItem position="Web Programming Teaching Assistant" company="Brigham Young University"
				date="Jan 2024 - Apr 2024" location="Provo, UT">
				<ul class="list-inside list-disc">
					<li>
						Provided one-on-one guidance to students, helping them debug code and deepen their understanding
						of course material
					</li>
					<li>
						Taught <b>full-stack</b> web development concepts including <b>HTML</b>, <b>CSS</b>,
						<b>JavaScript</b>, <b>React</b>, <b>AWS</b>, <b>MongoDB</b>, etc.
					</li>
					<li>
						<b>Analyzed hundreds</b> of assignment submissions and graded them for <b>quality</b>,
						<b>correctness</b>, and adherence to <b>best practice</b>
					</li>
				</ul>
			</ExperienceItem>
			<ExperienceItem position="Technical Help Desk Intern" company="SolvereOne" date="May 2022 - Jul 2022"
				location="Dulles, VA">
				<ul class="list-inside list-disc">
					<li>
						Provided IT services for<b> U.S. House of Representatives</b> and dozens of private companies in
						the area,
						ensuring <b>productive work environments</b>
					</li>
					<li>
						Resolved sensitive technical problems for clients under <b>time pressure</b>, ensuring <b>client
							satisfaction</b>
					</li>
				</ul>
			</ExperienceItem>
		</div>
	</div>
</template>

<script setup>
import ExperienceItem from '@/components/ExperienceItem.vue'
import LSImage1 from '@/assets/ls-assignmenteditor.png'
import LSImage2 from '@/assets/ls-questionbank.png'
import Thumbnail from './Thumbnail.vue';
import TechStack from './TechStack.vue';
</script>
