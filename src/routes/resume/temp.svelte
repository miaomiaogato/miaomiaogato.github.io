<script>
  import WorkCard from '$lib/WorkCard.svelte';
  import { resolve } from "$app/paths";
</script>

<h1>Resume</h1>
<p>A fuller, more professional resume can be downloaded <a href="/files/Miao_Daniel_Resume.pdf" download>here</a>. Might not be as up-to-date as this website!</p>

<h3>Jobs</h3>

<div class="work-column">
  <WorkCard
    logo="/images/resume/rdi.png"
    alt="Example Co."
    title="Software Engineer, Example Co."
    dates="Jun 2025 – Aug 2025"
    location="Remote"
  >
    <p>Description of what you did at this job goes here.</p>
  </WorkCard>

  <WorkCard
    logo="/images/resume/happylemon.png"
    alt="Another Co."
    title="Software Engineer, Another Co."
    dates="Jun 2024 – Aug 2024"
    location="Remote"
  >
    <p>Description of what you did at this job goes here.</p>
  </WorkCard>
</div>

<h3>Internships</h3>

<div class="work-column">
  <WorkCard
    logo="/images/resume/rdi.png"
    alt="Intern Co."
    title="Software Engineering Intern, Intern Co."
    dates="Jun 2023 – Aug 2023"
    location="Remote"
  >
    <p>Description of what you did during this internship goes here.</p>
  </WorkCard>
</div>

<style>
  .work-column {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
</style>

<h3>Projects & Publications</h3>
<p>View <a href={resolve('/projects')}>here!</a></p>

<h3>Honors & Certifications</h3>
<p><b>2025 USAPhO Honorable Mention</b> - Top ~280/5850. Did mostly for fun.</p>
<p><b>2024 AIME Qualifier</b> - The usual.</p>
<p><b>CompTIA Security+</b> - Did for fun when I was interested in security.</p>
<p><b>CompTIA Network+</b> - Same as Security+.</p>