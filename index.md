---
layout: default
title: "A Multivocal Review of MLOps Practices, Challenges and Open Issues"
description: "MLR of 150 academic and 48 grey-literature works on MLOps — synthesising definitions, activities, roles, practices, challenges, and open issues."
---

<section class="hero">
  <div class="hero-inner">
    <p class="venue-badge">
      <span class="venue-name">ACM Computing Surveys</span>
      <span class="venue-sep">·</span>
      <span>Vol. 58</span>
      <span class="venue-sep">·</span>
      <span>Issue 2</span>
      <span class="venue-sep">·</span>
      <span>Article 1</span>
      <span class="venue-sep">·</span>
      <span>pp. 1–35</span>
      <span class="venue-sep">·</span>
      <span>2025</span>
    </p>

    <h1 class="paper-title">A multivocal review of MLOps practices, challenges and open issues</h1>
    <p class="paper-subtitle">Synthesising 150 academic and 48 grey-literature works into a unified conceptualisation of MLOps</p>

    <p class="authors">
      <span><strong>Beyza Eken</strong><sup>1,*</sup></span>
      <span class="dot">·</span>
      <span><strong>Samodha Pallewatta</strong><sup>2,*</sup></span>
      <span class="dot">·</span>
      <span><strong>Nguyen Khoi Tran</strong><sup>2</sup></span>
      <span class="dot">·</span>
      <span><strong>Ayse Tosun</strong><sup>3</sup></span>
      <span class="dot">·</span>
      <span><strong>Muhammad Ali Babar</strong><sup>2</sup></span>
    </p>

    <p class="affiliations">
      <sup>1</sup> Faculty of Computer and Information Sciences, Sakarya University, Turkey &nbsp;
      <sup>2</sup> CREST — The Centre for Research on Engineering Software Technology, The University of Adelaide, Australia &nbsp;
      <sup>3</sup> Faculty of Computer and Informatics Engineering, Istanbul Technical University, Turkey
    </p>
    <p class="affiliations" style="font-size: 0.82rem; margin-top: -0.5rem;">
      <sup>*</sup> Equal contribution.
    </p>

    <div class="hero-actions">
      <a class="btn btn-primary" href="{{ '/assets/pdf/main.pdf' | relative_url }}">⬇ Download PDF</a>
      <a class="btn btn-ghost" href="https://doi.org/10.1145/3747346" rel="noopener">View on ACM Digital Library ↗</a>
    </div>
  </div>
</section>

<section class="section section--alt">
  <div class="container">
    <h2>TL;DR</h2>
    <p>
      We conducted a <strong>Multivocal Literature Review (MLR)</strong> of <strong>150 peer-reviewed studies</strong>
      and <strong>48 grey-literature works</strong> to build a unified, evidence-based conceptualisation of MLOps. We
      identified <strong>eight definitions</strong> of MLOps in the literature, organised the primary activities across
      the ML lifecycle, mapped <strong>20 practitioner roles</strong>, and catalogued seven categories of state-of-the-art
      practices and techniques — together with the socio-technical, pipeline, and platform challenges that practitioners
      face when adopting MLOps. The review closes with an agenda for future research on domain-specific architectures,
      responsible-AI tooling, and secure pipelines.
    </p>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>At a glance</h2>
    <div class="stat-grid">
      <div class="stat">
        <div class="stat-value">150</div>
        <div class="stat-label">peer-reviewed studies analysed</div>
      </div>
      <div class="stat">
        <div class="stat-value">48</div>
        <div class="stat-label">grey-literature works analysed</div>
      </div>
      <div class="stat">
        <div class="stat-value">8</div>
        <div class="stat-label">distinct definitions of MLOps synthesised</div>
      </div>
      <div class="stat">
        <div class="stat-value">20</div>
        <div class="stat-label">practitioner roles mapped across the lifecycle</div>
      </div>
    </div>
  </div>
</section>

<section class="section section--alt">
  <div class="container">
    <h2>Research method</h2>
    <p>
      Following Garousi et al.'s MLR guidelines, the review ran in three stages — <em>planning</em>,
      <em>conducting</em>, and <em>reporting</em>. Academic literature was harvested from IEEE Xplore, ACM Digital Library,
      Web of Science, and Scopus with complex Boolean queries; grey literature was collected via Google Search and arXiv
      with flexible strings, until theoretical saturation. Selection used pilot-calibrated inclusion / exclusion and
      quality criteria, with three reviewers resolving conflicts by consensus. Forward and backward snowballing extended
      coverage. Data extraction was driven by a shared spreadsheet and an Obsidian vault; coding followed Braun et al.'s
      thematic analysis to surface themes, sub-themes, and codes. The final corpus: <strong>150 academic + 48 grey
      literature</strong>, published up to September 2023.
    </p>
    <figure class="figure">
      <img src="{{ '/assets/figures/ResearchMethodology.png' | relative_url }}" alt="Overview of the three-stage MLR methodology: planning, conducting, and reporting the review">
      <figcaption>
        Overview of the MLR methodology: planning, conducting, and reporting the review.
      </figcaption>
    </figure>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Eight conceptualisations of MLOps</h2>
    <p>
      Rather than a single definition, the literature converges on <strong>eight conceptualisations</strong> of MLOps —
      each foregrounding a different facet of operationalising ML. They are not mutually exclusive; real-world adoptions
      typically blend several of them.
    </p>

    <figure class="figure">
      <img src="{{ '/assets/figures/RQ11.png' | relative_url }}" alt="Eight MLOps definitions and the ML productionalization problems each one addresses">
      <figcaption>
        The eight MLOps definitions identified in the literature and the ML productionalisation problems each one targets.
      </figcaption>
    </figure>

    <ul class="framework-list">
      <li><strong>Continuous ML</strong> (34 studies) — continuous engineering practices (CI/CD + Continuous Training) applied across the ML lifecycle.</li>
      <li><strong>DevOps for ML</strong> (32 studies) — DevOps practices and cultural shifts extended to ML systems.</li>
      <li><strong>Pipeline Automation</strong> (30 studies) — automating repetitive lifecycle activities via managed pipelines.</li>
      <li><strong>Culture</strong> (18 studies) — tools and managerial practices enabling cross-team collaboration.</li>
      <li><strong>Agile Data Science</strong> (15 studies) — intersection of data engineering, data science, ML, and operations.</li>
      <li><strong>ML Productionalisation</strong> (15 studies) — bringing ML models into a production environment reliably and at scale.</li>
      <li><strong>ML Life-Cycle Management</strong> (15 studies) — managing artefacts, workflows, and triggers across the lifecycle.</li>
      <li><strong>Unified Engineering Practice</strong> — unifying development, deployment, and operations of ML-enabled systems.</li>
    </ul>
  </div>
</section>

<section class="section section--alt">
  <div class="container">
    <h2>The MLOps pipeline and 20 practitioner roles</h2>
    <p>
      The review synthesises a comprehensive MLOps pipeline spanning <em>project initiation</em>,
      <em>ML lifecycle activities</em> (data collection, preparation, analysis, model development), <em>application
      development</em>, <em>deployment</em>, <em>monitoring</em>, <em>pipeline management</em>, <em>artifact
      management</em>, <em>quality assurance</em>, and <em>team management</em> — with twenty distinct practitioner
      roles collaborating across them.
    </p>
    <figure class="figure">
      <img src="{{ '/assets/figures/Pipeline.png' | relative_url }}" alt="A pipeline for ML development and operations with associated roles labelled DME, BA, DE, DS, MLE, MLOE, DOE, SE, QAE, OPE, ARC, SE, BM, PM, DGO, DQB, DST">
      <figcaption>
        The MLOps pipeline, with the 20 practitioner roles that collaborate across each lifecycle phase.
      </figcaption>
    </figure>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Practices, techniques, and the challenges they target</h2>
    <p>
      The review catalogues seven categories of state-of-the-art MLOps practices — from team-structure adaptations and
      version-control discipline to continuous monitoring, infrastructure-as-code, containerised deployment, automated
      pipelines, and integrated platforms — and maps them to the specific <em>productionalisation challenges</em>
      they address.
    </p>

    <figure class="figure">
      <img src="{{ '/assets/figures/RQ2.png' | relative_url }}" alt="Mapping of MLOps practices and techniques to the ML productionalization challenges they address">
      <figcaption>
        MLOps practices and techniques mapped to the corresponding ML productionalisation challenges.
      </figcaption>
    </figure>

    <p>Highlights from the synthesis:</p>

    <div class="finding">
      <h3>Work practices</h3>
      <div class="finding-grid">
        <div class="finding-item"><span class="num">2</span><span class="lbl">team structures: <strong>balanced project teams</strong> and <strong>specialised ML engineering teams</strong></span></div>
        <div class="finding-item"><span class="num">4</span><span class="lbl">cross-silo concerns to integrate: <strong>fairness</strong>, <strong>explainability</strong>, <strong>security</strong>, <strong>compliance</strong></span></div>
        <div class="finding-item"><span class="num">1</span><span class="lbl">Git-based workflow coordinating training, testing, and deployment via two stable branches (<code>dev</code> + <code>main</code>)</span></div>
      </div>
    </div>

    <div class="finding">
      <h3>Transparency and provenance</h3>
      <div class="finding-grid">
        <div class="finding-item"><span class="num">5</span><span class="lbl">artifact axes: <strong>code</strong>, <strong>data</strong>, <strong>features</strong>, <strong>models</strong>, <strong>experiments</strong></span></div>
        <div class="finding-item"><span class="num">4</span><span class="lbl">provenance tools surveyed: <strong>Vamsa</strong>, <strong>Geyser</strong>, <strong>MLflow2PROV</strong>, <strong>IBM AI Factsheets</strong></span></div>
        <div class="finding-item"><span class="num">2</span><span class="lbl">centralised repositories recommended: <strong>data</strong> and <strong>feature stores</strong></span></div>
      </div>
    </div>

    <div class="finding">
      <h3>Continuous monitoring</h3>
      <figure class="figure figure--small">
        <img src="{{ '/assets/figures/PublicationCountsByYear.png' | relative_url }}" alt="Distribution of selected academic and grey literature by publication year, showing growth of MLOps research since 2019">
        <figcaption>Growth of MLOps research: selected studies by year and literature type (academic vs. grey).</figcaption>
      </figure>
    </div>
  </div>
</section>

<section class="section section--alt">
  <div class="container">
    <h2>Adoption challenges and open issues</h2>
    <p>The review groups practitioner challenges into three families:</p>
    <ul class="framework-list">
      <li><strong>Socio-technical challenges</strong> — cultural change, MLOps fragmentation (complexity + diversity), and Responsible MLOps (compliance, fairness, security, transparency).</li>
      <li><strong>Pipeline-related challenges</strong> — setup overhead and expertise required, optimised deployment to distributed environments, managing large-scale pipelines, continual learning under high-velocity streams, and the automation decision dilemma.</li>
      <li><strong>Platform-related challenges</strong> — customisation vs. managed platforms, scalability, artifact management, distributed computing environments (TinyML, Federated Learning), and migration from existing DevOps toolchains.</li>
    </ul>
    <p>
      Solutions increasingly emphasise human-centric, transparent communication strategies; domain-specific reference
      architectures; systematic artifact management with governance; and structured human-in-the-loop interventions.
      Future work called out in the paper includes evaluation frameworks for MLOps platforms, automation-impact
      analysis frameworks, conjugated artifact management, and tools for responsible AI.
    </p>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Abstract</h2>
    <p>
      With the increasing trend of Machine Learning (ML) enabled software applications, the paradigm of ML Operations
      (MLOps) has gained tremendous attention of researchers and practitioners. MLOps encompasses the practices and
      technologies for streamlining the resources and monitoring needs of operationalizing ML models. Software
      development practitioners need access to the detailed and easily understandable knowledge of MLOps workflows,
      practices, challenges and solutions to effectively and efficiently support the adoption of MLOps. Whilst the
      academic and industry literature on the MLOps has been growing rapidly, there have been relatively a few attempts
      at systematically synthesizing and analyzing the vast amount of existing literature of MLOps for improving ease
      of access and understanding. We conducted a Multivocal Literature Review (MLR) of 150 relevant academic studies
      and 48 gray literature to provide a comprehensive body of knowledge on MLOps. Through this MLR, we identified the
      emerging MLOps practices, adoption challenges and solutions related to various areas, including development and
      operation of complex pipelines, managing production at scale, managing artifacts, and ensuring quality, security,
      governance, and ethical aspects. We also report the socio-technical aspect of MLOps relating to diverse roles
      involved and collaboration practices across them through the MLOps lifecycle. We assert that this MLR provides
      valuable insights to researchers and practitioners seeking to navigate the rapidly evolving landscape of MLOps.
      We also identify the open issues that need to be addressed in order to advance the current state-of-the-art of
      MLOps.
    </p>
    <p>
      MLOps has emerged as a key solution to address many socio-technical challenges of bringing ML models to
      production, such as integrating ML models with non-ML software, continuous monitoring, maintenance, and retraining
      of deployed models. Despite the utility of MLOps, an integrated body of knowledge regarding MLOps remains
      elusive because of its extensive scope due to the diversity of ML productionalization challenges it addresses.
      Whilst the existing literature reviews provide valuable snapshots of specific practices, tools, and research
      prototypes related to MLOps at various times, they focus on particular facets of MLOps, thus fail to offer a
      comprehensive and invariant framework that can weave these perspectives into a unified understanding of MLOps.
      This paper presents a Multivocal Literature Review that systematically analyzes a corpus of 150 peer-reviewed
      and 48 grey literature to synthesize a unified conceptualization of MLOps and develop a snapshot of its best
      practices, adoption challenges, and solutions.
    </p>
  </div>
</section>

<section class="section section--alt">
  <div class="container">
    <h2>Cite this paper</h2>
    <p>BibTeX entry (verbatim from the manuscript's <code>BIBTEX</code> file):</p>
    <pre class="bibtex"><code>@article{eken2025multivocal,
  title={A multivocal review of MLOps practices, challenges and open issues},
  author={Eken, Beyza and Pallewatta, Samodha and Tran, Nguyen and Tosun, Ayse and Babar, Muhammad Ali},
  journal={ACM Computing Surveys},
  volume={58},
  number={2},
  pages={1--35},
  year={2025},
  publisher={ACM New York, NY}
}</code></pre>

    <p class="doi-line">
      DOI: <a href="https://doi.org/10.1145/3747346" rel="noopener">10.1145/3747346</a>
    </p>
  </div>
</section>