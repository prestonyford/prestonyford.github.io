<template>
	<div class="">
		<h1>Experience</h1>
		<div class="flex flex-col gap-8">
			<ExperienceItem class="mt-4" position="Web Developer" company="Brigham Young University"
				date="May 2024 - Present" location="Provo, UT"
			>
				<ul class="list-inside list-disc">
					<li>
						Developed and maintained <b>LearningSuite</b>, the university's Learning Management System used by <b>34,000+ students and faculty</b>
						<ul class="ml-12 list-outside sm:list-inside list-[circle]">
							<li>Built and enhanced instructor-facing tools for assignment creation, exam grading, and feedback workflows</li>
							<li>Led development of <b>core features</b> including assignment builders, exam question editors, grading dashboards, and discussion forum management</li>
							<li>Refactored and migrated <b>5+ legacy pages</b> to <b>Vue.js</b>, improving maintainability and user experience</li>
							<li>Created <b>PHP API endpoints</b> for handling data retrieval and submission</li>
						</ul>
					</li>
				</ul>
				<div class="mt-6 flex gap-8 flex-col sm:flex-row">
					<div class="text-center">
						<img :src="LSImage1">
						<p>Assignment Editor</p>
					</div>
					<div class="text-center">
						<img :src="LSImage2">
						<p>Question Bank</p>
						<p class="text-gray-300 text-sm">Developed a Question Bank tool for creating and organizing reusable question pools, enabling instructors, departments, and courses to share resources while tracking usage and performance statistics.</p>
					</div>
				</div>
			</ExperienceItem>
			<ExperienceItem position="Web Programming Teaching Assistant" company="Brigham Young University"
				date="Jan 2024 - Apr 2024" location="Provo, UT"
			>
				<ul class="list-inside list-disc">
					<li>
						Provided one-on-one guidance to students, helping them debug code and deepen their understanding of course material
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
			<ExperienceItem position="Technical Help Desk Intern" company="SolvereOne"
				date="May 2022 - Jul 2022" location="Dulles, VA"
			>
				<ul class="list-inside list-disc">
					<li>
						Provided IT services for<b> U.S. House of Representatives</b> and dozens of private companies in the area, 
						ensuring <b>productive work environments</b>
					</li>
					<li>
						Resolved sensitive technical problems for clients under <b>time pressure</b>, ensuring <b>client satisfaction</b>
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
</script>
