<template>
	<div class="">
		<h1>Experience</h1>
		<div class="flex flex-col gap-4">
			<ExperienceItem class="mt-4" position="Web Developer" company="Brigham Young University"
				date="May 2024 - Present" location="Provo, UT"
			>
				<ul class="list-inside list-disc">
					<li>
						Developed LearningSuite, the university's learning platform used by <b>all 34,000 students</b>
						<ul class="ml-12 list-inside list-[circle]">
							<li>Implemented new features in assignment editing and grading exams, allowing instructors to score student submissions</li>
							<li>Built 5 new pages used by instructors to create assignments, grade exams, and view course data</li>
							<li>Rewrote several existing pages to use the <b>Vue.js</b> framework</li>
						</ul>
					</li>
				</ul>
			</ExperienceItem>
			<ExperienceItem class="mt-4" position="Web Programming Teaching Assistant" company="Brigham Young University"
				date="Jan 2024 - Apr 2024" location="Provo, UT"
			>
				<ul class="list-inside list-disc">
					<li>
						Educated students in a one-on-one setting frequently; helped students debug and understand their code to 
						improve their understanding and grades
					</li>
					<li>
						Taught <b>full-stack</b> web development topics including <b>HTML</b>, <b>CSS</b>, 
						<b>JavaScript</b>, <b>React</b>, <b>AWS</b>, <b>MongoDB</b>, etc.
					</li>
					<li>
						<b>Analyzed hundreds</b> of assignment submissions of dozens of students, graded them for <b> 
						quality and adherence</b> to instructions
					</li>
				</ul>
			</ExperienceItem>
			<ExperienceItem class="mt-4" position="Technical Help Desk Intern" company="SolvereOne"
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
</script>
