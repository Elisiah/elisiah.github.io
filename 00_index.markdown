---
layout: page
title: About Me
permalink: /
---

<style>
/* Unified rectangular button style */
.portfolio-btn {
  display: inline-block;
  background-color: #007acc;  /* primary blue */
  color: white;
  padding: 0.8rem 1.5rem;
  border-radius: 0;           /* rectangular */
  font-weight: 600;
  text-decoration: none;
  box-shadow: 2px 2px 6px rgba(0,0,0,0.15);
  transition: background 0.2s ease, transform 0.2s ease;
  font-size: 0.95rem;
}

.portfolio-btn:hover {
  background-color: #005f99;
  transform: translateY(-2px);
}
</style>



# Hi, I’m Ellie 👋

I’m a **First Class BSc Computer Science Graduate** from the University of Exeter, passionate about **software development, reverse engineering, and data analysis**.  

Since much of my work involves **reverse engineering**, I can’t always post full source code; but here are a few of my key projects with detailed write-ups.

---
<br/>
## Skills & Technologies
<div style="display: flex; flex-wrap: wrap; gap: 0.5rem; justify-content: left; margin-bottom: 1.5rem;">
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/C-00599C?logo=c&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/C%23-239120?logo=csharp&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white&style=flat-square">
  <img src="https://img.shields.io/badge/CI/CD-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white&style=flat-square">
</div>

---
<br/>
## Get in Touch

<div style="text-align:center; margin: 2rem 0;">
<p style="font-size:0.95rem; margin-top:1rem; color:#333;">
    <a href="mailto:Ellie.Vallard@outlook.com" class="portfolio-btn">
      Email me: Ellie.Vallard@outlook.com
    </a>
  </p>

  <a href="/assets/EllieVallard_CV.pdf" download class="portfolio-btn">
    📄 Download CV
  </a>
</div>

  




---
<br/>
## Featured Projects

<div style="display: flex; flex-wrap: wrap; gap: 1.5rem; justify-content: center;">

<div style="flex: 1 1 300px; max-width: 350px; border: 1px solid #ddd; border-radius: 10px; padding: 1rem; box-shadow: 2px 2px 6px rgba(0,0,0,0.1); transition: transform 0.2s ease, box-shadow 0.2s ease;">
  <a href="https://siege.rip" style="text-decoration:none; color:inherit;">
    <img src="/assets/siegerip.png" alt="Siege.Rip stats and inventory platform" style="width:100%; border-radius: 8px; margin-bottom: 0.5rem;">
    <span class="portfolio-btn" style="font-size:0.8rem; padding:0.2rem 0.6rem; background-color:#28a745;">
  Professional Project Environment
</span>
    <h3 style="margin-top: 0.5rem;">Siege.Rip Web Platform</h3>
    <p><strong>Tech:</strong> MySQL, RESTful API, Node.js, Python</p>
    <p><strong>Role:</strong> Backend Engineer & Database Designer</p>
    <p>Handled backend and database development for <em>Siege.Rip</em>, a live inventory tracker for <em>Rainbow Six Siege</em>.  
    Designed relational schemas ensuring efficient entity relationships, and implemented REST APIs supporting scalable real-time data handling.  
    Collaborated with frontend developers using Git-based workflows and integrated unit testing into CI pipelines for API validation.</p>
    <p style="margin-top: 0.5rem;">
      <img src="https://img.shields.io/badge/status-live-success?style=flat-square">
    </p>
  </a>
</div>

<div style="flex: 1 1 300px; max-width: 350px; border: 1px solid #ddd; border-radius: 10px; padding: 1rem; box-shadow: 2px 2px 6px rgba(0,0,0,0.1); transition: transform 0.2s ease, box-shadow 0.2s ease;">
  <a href="https://jumpkingplus.github.io/#team" style="text-decoration:none; color:inherit;">
    <img src="/assets/jkpluslogo.png" alt="Jump King Plus modding project" style="width:100%; border-radius: 8px; margin-bottom: 0.5rem;">
    <span class="portfolio-btn" style="font-size:0.8rem; padding:0.2rem 0.6rem; background-color:#FFA500;">
  Team Collaboration Project (OSS)
</span>
    <h3 style="margin-top: 0.5rem;">Jump King Plus</h3>
    <p><strong>Tech:</strong> C#, Mono Modding</p>
    <p><strong>Role:</strong> Gameplay Mod Developer</p>
    <p>Collaborative modding project for <em>Jump King</em>, extending game mechanics and adding new features including multiplayer. Developed custom tools and gameplay modules later integrated into the official Steam Workshop by Nexile.</p>
    <p style="margin-top: 0.5rem;">
      <img src="https://img.shields.io/github/downloads/JumpKingPlus/JumpKingPlus/total?style=flat-square">
      <img src="https://img.shields.io/github/stars/JumpKingPlus/JumpKingPlus?style=flat-square">
    </p>
  </a>
</div>


<div style="flex: 1 1 300px; max-width: 350px; border: 1px solid #ddd; border-radius: 10px; padding: 1rem; box-shadow: 2px 2px 6px rgba(0,0,0,0.1); transition: transform 0.2s ease, box-shadow 0.2s ease;">
  <a href="/decomp/" style="text-decoration:none; color:inherit;">
    <img src="/assets/ctwistlogo.png" alt="Chameleon Twist reverse engineering project" style="width:100%; border-radius: 8px; margin-bottom: 0.5rem;">
    <span class="portfolio-btn" style="font-size:0.8rem; padding:0.2rem 0.6rem; background-color:#FFA500;">
  Team Collaboration Project (OSS)
</span>
    <h3 style="margin-top: 0.5rem;">N64 Reverse Engineering</h3>
    <p><strong>Tech:</strong> C, MIPS Assembly, Python, Blender API</p>
    <p><strong>Role:</strong> Reverse Engineer & Tool Developer</p>
    <p>Reconstructed the original <em>Chameleon Twist</em> Nintendo 64 game in C to enable source-level modifications and recompilation. Created supporting tooling such as a Blender plugin for model extraction and custom gameplay mod experiments.</p>
    <p style="margin-top: 0.5rem;">
      <img src="https://github.com/chameleonTwistRet/chameleonTwistv1.0-JP/actions/workflows/ci.yml/badge.svg">
      <img src="https://img.shields.io/endpoint?label=Code%20JP&url=https%3A%2F%2Fprogress.deco.mp%2Fdata%2Fchameleontwist%2Fjp%2Fdefault%2F%3Fmode%3Dshield%26measure%3Dfuncs&color=yellow">
    </p>
  </a>
</div>

<div style="flex: 1 1 300px; max-width: 350px; border: 1px solid #ddd; border-radius: 10px; padding: 1rem; box-shadow: 2px 2px 6px rgba(0,0,0,0.1); transition: transform 0.2s ease, box-shadow 0.2s ease;">
  <a href="https://github.com/Elisiah/XSerialOne" style="text-decoration:none; color:inherit;">
    <img src="/assets/xseriesone_deadzones.png" alt="XSerialOne Framework project preview" style="width:100%; border-radius: 8px; margin-bottom: 0.5rem;">
    <span class="portfolio-btn" style="font-size:0.8rem; padding:0.2rem 0.6rem; background-color:#6f42c1;">
  Solo Personal Project
</span>
    <h3 style="margin-top: 0.5rem;">XSerialOne Framework</h3>
    <p><strong>Tech:</strong> Python, Serial I/O, Custom Hardware Interface</p>
    <p><strong>Role:</strong> Solo Developer</p>
    <p>A modular Python framework enabling real-time Xbox controller emulation and input automation through custom serial hardware. Used for advanced applications such as AI-driven gameplay, image-recognition-based control, and automated testing on real consoles.</p>
    <p style="margin-top: 0.5rem;">
      <img src="https://img.shields.io/github/stars/Elisiah/XSerialOne?style=flat-square">
      <img src="https://img.shields.io/badge/last_commit-Nov_2025-blue?style=flat-square">
    </p>
  </a>
</div>

<div style="flex: 1 1 300px; max-width: 350px; border: 1px solid #ddd; border-radius: 10px; padding: 1rem; box-shadow: 2px 2px 6px rgba(0,0,0,0.1); transition: transform 0.2s ease, box-shadow 0.2s ease;">
  <a href="/dissertation/" style="text-decoration:none; color:inherit;">
    <img src="/assets/speedrun_logo.png" alt="Speedrun Data Analysis Dissertation" style="width:100%; border-radius: 8px; margin-bottom: 0.5rem;">
    <span class="portfolio-btn" style="font-size:0.8rem; padding:0.2rem 0.6rem; background-color:#6f42c1;">
      Solo Dissertation Research Project
    </span>
    <h3 style="margin-top: 0.5rem;">Speedrun Data Analysis (Dissertation)</h3>
    <p><strong>Tech:</strong> Python, MySQL, Network Analysis</p>
    <p><strong>Role:</strong> Solo Research & Data Analyst</p>
    <p>Modeled Speedrun.com as a bipartite network connecting players and games. Maintained a relational database with millions of records, performed data cleaning, SQL aggregation, and statistical network analysis to extract insights on speedrunning trends and player-game relationships.</p>
  </a>
</div>



</div>