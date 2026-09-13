<!-- ==========================================================================
     ABOUT ME SECTION
     ========================================================================== -->
<h1 id="about-me" class="section-title">🌟 About Me</h1>

<p class="lead">
  Hello! I am <strong>Alex Chen (陈晨)</strong>, a fourth-year Ph.D. candidate in Computer Science at
  <strong>Stanford University</strong>, where I am very fortunate to be advised by Prof.
  <a href="https://example.edu/~advisor" target="_blank" rel="noopener noreferrer">Sarah Jenkins</a>.
  Previously, I obtained my B.S. in Computer Science & Applied Mathematics from <strong>Carnegie Mellon University</strong>.
  During the summers of 2024 and 2025, I was a research scientist intern at <strong>DeepMind Robotics</strong>.
</p>

<p>
  My research lies at the intersection of <strong>Computer Vision, Robotics, and Multimodal Foundation Models</strong>.
  My ultimate goal is to build intelligent physical agents capable of perceiving unstructured 3D environments,
  reasoning about physical dynamics, and executing dexterous manipulation tasks in the real world.
</p>

<p>
  To achieve this, my current projects explore three synergistic directions:
</p>

<ul class="modern-list" style="margin-top: 8px; margin-bottom: 14px;">
  <li><strong>Neural Scene Representations:</strong> Building real-time dynamic radiance fields and Gaussian splatting primitives for metric-scale 3D mapping and novel view synthesis.</li>
  <li><strong>Vision-Language-Action Models (VLA):</strong> Training cross-embodiment transformer policies conditioned on continuous visual observations and open-vocabulary natural language instructions.</li>
  <li><strong>Physics-Informed World Simulators:</strong> Developing differentiable physics engines to generate synthetic sensor rollouts and accelerate sim-to-real transfer.</li>
</ul>

<div class="collab-callout">
  📬 I am actively open to research discussions, academic talks, and collaborating on open-source robotics benchmarks. Feel free to reach out via email!
</div>

<!-- ==========================================================================
     NEWS SECTION
     Add your latest news items here. Newest on top.
     ========================================================================== -->
<h1 id="news" class="section-title">🔥 News</h1>
<ul class="modern-list">
  <li><span class="modern-list-date">2026.04</span><span class="modern-list-content">Excited to announce that <em>GaussianGrasp</em> received the <strong>Best Paper Award Finalist</strong> at <strong>CVPR 2026</strong>!</span></li>
  <li><span class="modern-list-date">2026.01</span><span class="modern-list-content">Our paper on open-world robotic manipulation was accepted to <strong>ICRA 2026</strong> as an <strong>Oral Presentation</strong>!</span></li>
  <li><span class="modern-list-date">2025.10</span><span class="modern-list-content">Gave an invited talk on <em>"From Photorealism to Physical Action"</em> at the <strong>CoRL Workshop on Robot Learning</strong>.</span></li>
  <li><span class="modern-list-date">2025.07</span><span class="modern-list-content">Started my second research internship at <strong>DeepMind (Mountain View)</strong> working on foundation models for manipulation!</span></li>
</ul>

<!-- ==========================================================================
     PUBLICATIONS SECTION
     Each paper card accepts attributes:
       - data-selected="true" : Displayed in the default "Selected" tab.
       - data-author-rank="1" : Authorship position (1 for 1st author, 2 for 2nd, etc.). Used for sorting in "All".
       - data-year="2026"     : Publication year. Used for secondary sorting in "All".
     ========================================================================== -->
<h1 id="publications" class="section-title">📝 Publications</h1>
<div class="publications-toolbar">
  <p class="muted-note">(<sup>*</sup> denotes equal contribution, <sup>#</sup> denotes corresponding author.)</p>
  <div class="paper-toggle" role="tablist" aria-label="Publication filter">
    <button type="button" class="paper-toggle-btn is-active" data-filter="selected" role="tab" aria-selected="true">Selected</button>
    <button type="button" class="paper-toggle-btn" data-filter="all" role="tab" aria-selected="false">All</button>
  </div>
</div>

<div id="published-papers">

<!-- Paper 1 -->
<div class="paper-card" data-selected="true" data-author-rank="1" data-year="2026">
  <div class="paper-image-container">
    <img src="images/paper-placeholder.svg" alt="GaussianGrasp teaser figure">
  </div>
  <div class="paper-content">
    <div class="paper-title">GaussianGrasp: 3D Gaussian Splatting as Universal Representation for Dexterous Robotic Grasping</div>
    <div class="paper-authors"><strong>Alex Chen<sup>*</sup></strong>, Maya Patel<sup>*</sup>, Lucas Vance, Sarah Jenkins<sup>#</sup></div>
    <div class="paper-meta">
      <span class="conf-badge">CVPR 2026 (Oral & Best Paper Finalist)</span>
      <span class="ccf-badge">CCF-A</span>
    </div>
    <div class="paper-links">
      <a href="https://arxiv.org/" class="paper-btn paper-btn-primary" target="_blank" rel="noopener noreferrer">Paper</a>
      <a href="https://github.com/" class="paper-btn paper-btn-secondary" target="_blank" rel="noopener noreferrer">Code</a>
      <a href="#" class="paper-btn" target="_blank" rel="noopener noreferrer">Project Page</a>
      <a href="#" class="paper-btn" target="_blank" rel="noopener noreferrer">Video Demo</a>
    </div>
  </div>
</div>

<!-- Paper 2 -->
<div class="paper-card" data-selected="true" data-author-rank="1" data-year="2025">
  <div class="paper-image-container">
    <img src="images/paper-placeholder.svg" alt="VLA-Scale teaser figure">
  </div>
  <div class="paper-content">
    <div class="paper-title">VLA-Scale: Cross-Embodiment Robot Learning with Differentiable Trajectory Diffusion</div>
    <div class="paper-authors"><strong>Alex Chen</strong>, Ethan Walker, Hiroshi Tanaka, Sarah Jenkins</div>
    <div class="paper-meta">
      <span class="conf-badge">NeurIPS 2025 (Spotlight)</span>
      <span class="ccf-badge">CCF-A</span>
    </div>
    <div class="paper-links">
      <a href="https://arxiv.org/" class="paper-btn paper-btn-primary" target="_blank" rel="noopener noreferrer">Paper</a>
      <a href="https://github.com/" class="paper-btn paper-btn-secondary" target="_blank" rel="noopener noreferrer">Code</a>
      <a href="#" class="paper-btn" target="_blank" rel="noopener noreferrer">Poster</a>
    </div>
  </div>
</div>

<!-- Paper 3 -->
<div class="paper-card" data-selected="true" data-author-rank="1" data-year="2025">
  <div class="paper-image-container">
    <img src="images/paper-placeholder.svg" alt="OmniDepth figure">
  </div>
  <div class="paper-content">
    <div class="paper-title">OmniDepth: Zero-Shot Monocular Metric Depth Estimation across Extreme Weather Conditions</div>
    <div class="paper-authors"><strong>Alex Chen<sup>*</sup></strong>, Daniel Kim<sup>*</sup>, Elena Rostova, Marcus Zhang</div>
    <div class="paper-meta">
      <span class="conf-badge">ICCV 2025</span>
      <span class="ccf-badge">CCF-A</span>
    </div>
    <div class="paper-links">
      <a href="https://arxiv.org/" class="paper-btn paper-btn-primary" target="_blank" rel="noopener noreferrer">Paper</a>
      <a href="https://github.com/" class="paper-btn paper-btn-secondary" target="_blank" rel="noopener noreferrer">Dataset</a>
    </div>
  </div>
</div>

<!-- Paper 4 (Collaborative paper, hidden in Selected tab by default) -->
<div class="paper-card" data-author-rank="3" data-year="2026">
  <div class="paper-image-container">
    <img src="images/paper-placeholder.svg" alt="TactileFlow figure">
  </div>
  <div class="paper-content">
    <div class="paper-title">TactileFlow: Visuotactile Sensor Fusion for Slippage Detection in Deformable Object Handling</div>
    <div class="paper-authors">Sofia Romero<sup>*</sup>, Jordan Lee<sup>*</sup>, <strong>Alex Chen</strong>, Sarah Jenkins</div>
    <div class="paper-meta">
      <span class="conf-badge">ICRA 2026</span>
      <span class="ccf-badge">CCF-B</span>
    </div>
    <div class="paper-links">
      <a href="https://arxiv.org/" class="paper-btn paper-btn-primary" target="_blank" rel="noopener noreferrer">Paper</a>
      <a href="https://github.com/" class="paper-btn paper-btn-secondary" target="_blank" rel="noopener noreferrer">Code</a>
    </div>
  </div>
</div>

</div>

<!-- ==========================================================================
     WORKING PAPERS & PREPRINTS (MINI CARDS)
     ========================================================================== -->
<h2 id="working-papers" class="section-title subsection-title">Working Papers</h2>

<div class="mini-card">
  <div class="mini-card-title">Sim2World: Scalable Synthetic Data Generation via Generalizable Physics Simulators</div>
  <div class="mini-card-authors"><strong>Alex Chen<sup>*</sup></strong>, Chloe Nguyen<sup>*</sup>, Liam Brooks, Sarah Jenkins</div>
  <div class="mini-card-status">Under review at CoRL 2026 · Preprint on arXiv</div>
</div>

<div class="mini-card">
  <div class="mini-card-title">DexterBench: A Photorealistic Benchmark for Multi-Finger In-Hand Manipulation</div>
  <div class="mini-card-authors">Maya Patel, <strong>Alex Chen</strong>, Kenji Sato, Sarah Jenkins</div>
  <div class="mini-card-status">Preprint available · Benchmark code released</div>
</div>

<!-- ==========================================================================
     EXPERIENCE / INTERNSHIPS
     ========================================================================== -->
<h1 id="experience" class="section-title">💻 Experience</h1>

<div class="exp-card">
  <div class="exp-header">
    <div class="exp-title">Research Scientist Intern</div>
    <div class="exp-date">Jun. 2025 - Sep. 2025</div>
  </div>
  <div class="exp-org">
    <img class="company-logo" src="images/org-placeholder.svg" alt="DeepMind Logo" loading="lazy">
    <span>Google DeepMind · Robotics & Embodied AI Team</span>
  </div>
  <div class="exp-desc">Mentored by Dr. Arthur Clark. Researched scalable vision-language-action policies for real-world dual-arm manipulators.</div>
</div>

<div class="exp-card">
  <div class="exp-header">
    <div class="exp-title">Computer Vision Research Intern</div>
    <div class="exp-date">Jun. 2024 - Sep. 2024</div>
  </div>
  <div class="exp-org">
    <img class="company-logo" src="images/org-placeholder.svg" alt="Company Logo" loading="lazy">
    <span>NVIDIA Research · Autonomous Driving Lab</span>
  </div>
  <div class="exp-desc">Mentored by Dr. Rebecca Stone. Developed efficient neural volume rendering algorithms for surround-view camera rigs.</div>
</div>

<!-- ==========================================================================
     EDUCATION
     ========================================================================== -->
<h1 id="education" class="section-title">📖 Education</h1>

<div class="exp-card">
  <div class="exp-header">
    <div class="exp-title">Ph.D. in Computer Science</div>
    <div class="exp-date">2022 - Present</div>
  </div>
  <div class="exp-org">Stanford University</div>
  <div class="exp-desc">Stanford AI Lab (SAIL). Advised by Prof. Sarah Jenkins. Focus: Robot Learning, 3D Vision & Embodied AI.</div>
</div>

<div class="exp-card">
  <div class="exp-header">
    <div class="exp-title">B.S. in Computer Science & Applied Mathematics</div>
    <div class="exp-date">2018 - 2022</div>
  </div>
  <div class="exp-org">Carnegie Mellon University</div>
  <div class="exp-desc">School of Computer Science. University Honors, Magna Cum Laude. GPA: 3.94 / 4.0.</div>
</div>

<!-- ==========================================================================
     HONORS & AWARDS
     ========================================================================== -->
<h1 id="honors" class="section-title">🎖 Honors and Awards</h1>
<ul class="modern-list">
  <li><span class="modern-list-date">2026</span><span class="modern-list-content">CVPR 2026 Best Paper Award Finalist (Top 0.5% of submissions)</span></li>
  <li><span class="modern-list-date">2024</span><span class="modern-list-content">Qualcomm Innovation Fellowship Finalist</span></li>
  <li><span class="modern-list-date">2022</span><span class="modern-list-content">Stanford Graduate Fellowship (SGF) in Science & Engineering</span></li>
  <li><span class="modern-list-date">2022</span><span class="modern-list-content">CMU Allen Newell Award for Undergraduate Research Excellence</span></li>
</ul>

<!-- ==========================================================================
     ACADEMIC SERVICES
     ========================================================================== -->
<h1 id="services" class="section-title">🤝 Academic Services</h1>

<h2 class="section-title subsection-title" style="margin-top: 18px; margin-bottom: 12px; font-size: 1.05rem; color: #1e293b;">Conference Reviewer</h2>
<div class="service-grid">
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">CVPR</span>
      <div class="tile-years">
        <span class="tile-year-pill">2026</span>
        <span class="tile-year-pill">2025</span>
        <span class="tile-year-pill">2024</span>
      </div>
    </div>
    <div class="tile-full-name">IEEE/CVF Conference on Computer Vision and Pattern Recognition</div>
  </div>
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">NeurIPS</span>
      <div class="tile-years">
        <span class="tile-year-pill">2025</span>
        <span class="tile-year-pill">2024</span>
      </div>
    </div>
    <div class="tile-full-name">Conference on Neural Information Processing Systems</div>
  </div>
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">ICCV</span>
      <div class="tile-years">
        <span class="tile-year-pill">2025</span>
      </div>
    </div>
    <div class="tile-full-name">IEEE/CVF International Conference on Computer Vision</div>
  </div>
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">ECCV</span>
      <div class="tile-years">
        <span class="tile-year-pill">2026</span>
        <span class="tile-year-pill">2024</span>
      </div>
    </div>
    <div class="tile-full-name">European Conference on Computer Vision</div>
  </div>
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">CoRL</span>
      <div class="tile-years">
        <span class="tile-year-pill">2025</span>
      </div>
    </div>
    <div class="tile-full-name">Conference on Robot Learning</div>
  </div>
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">ICRA</span>
      <div class="tile-years">
        <span class="tile-year-pill">2026</span>
        <span class="tile-year-pill">2025</span>
      </div>
    </div>
    <div class="tile-full-name">IEEE International Conference on Robotics and Automation</div>
  </div>
</div>

<h2 class="section-title subsection-title" style="margin-top: 24px; margin-bottom: 12px; font-size: 1.05rem; color: #1e293b;">Journal Reviewer & Workshop Organization</h2>
<ul class="modern-list">
  <li><span class="modern-list-date">Journal</span><span class="modern-list-content">IEEE Transactions on Pattern Analysis and Machine Intelligence (TPAMI), International Journal of Computer Vision (IJCV)</span></li>
  <li><span class="modern-list-date">Workshop</span><span class="modern-list-content">Co-Organizer, CVPR 2025 Workshop on Neural Representations for Physical Interaction</span></li>
</ul>

<!-- ==========================================================================
     TEACHING ASSISTANTSHIPS
     ========================================================================== -->
<h1 id="teaching" class="section-title">📚 Teaching Assistantships</h1>
<ul class="modern-list">
  <li><span class="modern-list-date">Spring 2025</span><span class="modern-list-content">CS231N: Deep Learning for Computer Vision (Head TA, ~450 students)</span></li>
  <li><span class="modern-list-date">Fall 2024</span><span class="modern-list-content">CS224N: Natural Language Processing with Deep Learning (TA)</span></li>
  <li><span class="modern-list-date">Winter 2023</span><span class="modern-list-content">CS131: Computer Vision Foundations & Applications (TA)</span></li>
</ul>
