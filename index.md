***Sustainable Computing Architecture: From Silicon to Datacenter – Co-Designing AI Systems Across the Stack***

AI workloads are fundamentally reshaping computing's energy profile, yet sustainability is still treated as a secondary optimization rather than a first-order design constraint. Worse, current trends show the embodied footprint of computing — from raw-material extraction and semiconductor manufacturing through assembly and end-of-life — is approaching or exceeding the operational footprint, a shift that most architecture and systems research has yet to internalize. 

Sustainability has been established as a cross-cutting architectural concern over the recent years, and a central thesis in achieving sustainable compute system architecture is Architecture-Technology Co-Optimization (ATCO), where architectural decisions, packaging choices, and manufacturing processes must be jointly evaluated against sustainability objectives rather than optimized in isolation.

## Objective

This workshop brings together complementary perspectives to address this gap across the full computing stack and the full product lifecycle. Bridging these layers, the workshop presents cross-stack co-design methodologies for environmentally sustainable computing that decomposes computing's environmental impact into actionable architectural levers. The workshop is intended to turn the attendee towards action, therefore we end the workshop with a hands-on codesign exercise.


## Program

| Time  | Session | Speaker | Topic | Resources |
|---|---|---|---|---|
| 08:00 - 08:05 | Opening | Arindam Malik (imec) | Overview of the Workshop |   |
| 08:05 - 08:20 | Session 1 | Rutwik Jain (Uwisc) | Embrace the Chaos: Harnessing Variability for Large-Scale System Efficiency  |   |
| 08:20 - 08:35 | Session 1 | Mariam Elgamal (Harvard) |   |   |
| 08:35 - 08:50 | Session 1 | August Ning (EPFL) | Metrics for Energy-Efficient Server Design and Operation  |   |
| 08:50 - 09:00 | Buffer + Coffee Break |   |   |   |
| 09:00 - 09:15 | Session 2 | Luca Benini (ETHZ, UNIBO) | Energy efficiency and Power management for AI accelerators - Tackling the MW rack challenge |   |
| 09:15 - 09:30 | Session 2 | Abdulrahman Mahmoud (MBZUAI)   | Brain Computing Interfacing and the Life(time) Argument for Sustainable Computing   |   |
| 09:30 - 09:45 | Session 2 | Vijay Reddi (Harvard) | Flexible electronics for sustainable computing |   |
| 09:45 - 10:00 | Buffer + Coffee break |   |   |   |
| 10:00 - 10:15 | Session 3 | Alex Bruefach (Meta) | Designing Data Foundations for Sustainability at Scale |   |
| 10:15 - 10:30 | Session 3 | Sarah McAllister (UWisc) | Out of sight, but no longer out of mind: tackling stored data’s emissions footprint  |   |
| 10:30 - 10:45 | Session 3 | Timon Evenblij (imec) | The impact of IC manufacturing on the sustainability of AI  |   |
| 10:45- 11:00 | Buffer + Coffee break |   |   |   |
| 11:00 - 11:30 | Panel | All presenters |   |   |
| 11:30 - 12:00 | Codesign exercises | All workshop attendees | Interactive sustainability co-design | [Exercise details](#sustainability-co-design-exercises) |


## Format

<h3 id="speakers">Three sessions with presenters working across the AI stack</h3>

<div class="speakers">
    <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/luca-benini.jpg' | relative_url }}" alt="Headshot of Luca Benini" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Luca Benini</h3>
      <p class="speaker-affiliation">ETH Zürich; Università di Bologna</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Energy efficiency and Power management for AI accelerators - Tackling the MW rack challenge</em></p>
      <details>
        <summary>Abstract</summary>
        <p>Datacenters are moving rapidly toward MW power budgets for a single accelerated computing rack: AI accelerators achieve extremely high performance and utilization, with a strong impact on power management: power density and thermal hotspots primary concerns. In this talk, I will discuss techniques to address and minimize power waste and the evolution of management policies and controllers toward advanced AI-based regulation and planning of power and thermal budgets.</p>
      </details>
      <details>
        <summary>Biography</summary>
        <p>Luca Benini holds the chair of digital Circuits and systems at ETHZ and is Full Professor at the Università di Bologna. He received a PhD from Stanford University. His research interests are in energy-efficient parallel computing systems, smart sensing micro-systems and machine learning hardware. He is a Fellow of the IEEE, of the ACM, a member of the Academia Europaea and of the Italian Academy of Engineering and Technology.</p>
      </details>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/alex-bruefach.jpg' | relative_url }}" alt="Headshot of Alex Bruefach" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Alex Bruefach</h3>
      <p class="speaker-affiliation">Production Systems Engineer, Meta</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Designing Data Foundations for Sustainability at Scale</em></p>
      <details>
        <summary>Abstract</summary>
        <p>One lever for reducing the carbon footprint of a large-scale hardware fleet is design optimization. This talk draws on first-hand experience and the challenges of building a framework end to end, from component-level carbon modeling to embedding sustainability in design practice. We begin at the chip level, presenting a sensitivity analysis of our custom AI accelerators to demonstrate how uncertainty in die manufacturing conditions impacts product carbon estimates.</p>
        <p>AI accelerators, however, are only part of the fleet's footprint. Designing for sustainability at the rack and fleet level requires visibility into a rack's carbon hotspots during the rack design phase. To enable this, we built a pipeline that estimates embodied carbon at the component and subsystem level which accommodates varying data quality and completeness, aggregates estimates across the fleet, and surfaces estimates during hardware design. The estimates highlight hotspots and prioritize reduction opportunities, which feed back into product design: interventions can be evaluated that lower a product's carbon impact before it is committed to production, while maintaining key performance objectives.</p>
      </details>
      <details>
        <summary>Biography</summary>
        <p>Alex Bruefach is a Production Systems Engineer at Meta, building solutions for data center infrastructure, hardware reliability, and sustainability. Alex's work spans component-level embodied carbon modeling through fleet-scale aggregation, driving insights that enable AI hardware programs to scale sustainably. By grounding this accounting in hardware reliability data, Alex builds holistic frameworks for assessing fleet health, efficiency, and sustainability. Alex holds a PhD from UC Berkeley in Materials Science and Engineering with a Designated Emphasis in Computational and Data Science and Engineering.</p>
      </details>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/mariam.jpeg' | relative_url }}" alt="Headshot of Mariam Elgamal" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Mariam Elgamal</h3>
      <p class="speaker-affiliation">PhD candidate, Harvard University</p>
      <details>
        <summary>Biography</summary>
        <p>Mariam Elgamal is a PhD candidate at Harvard University, working with Professors Gage Hills, David Brooks, and Gu-Yeon Wei. Her research interests are at the intersection of computer architecture and circuit design, with a focus on optimizing computing systems for energy efficiency and environmental sustainability across multiple layers of the computing stack. Mariam’s work appears in venues including ISCA, HPCA, ASPLOS, DATE, ICCAD, and IEDM, and has been recognized by multiple awards, including: 2023 IEEE Micro Top Picks, HPCA 2025 Best Paper Honorable Mention, DATE 2025 Best Paper Award Candidate, ASPLOS 2026 Best Paper Award, and 2026 IEEE Micro Top Picks Honorable Mention. She was also recognized as a Heidelberg Laureate Forum Young Investigator, and a NextProf Nexus 2025 Awardee.</p>
      </details>
    </div>
  </article>



  <article class="speaker">
    <div class="photo-name photo-placeholder" aria-hidden="true"></div>
    <div class="bio">
      <h3>Vijay Janapa Reddi</h3>
      <p class="speaker-affiliation">Gordon McKay Professor of Electrical Engineering, John A. Paulson School of Engineering and Applied Sciences, Harvard University</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Flexible electronics for sustainable computing</em></p>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/rutwik-jain.jpg' | relative_url }}" alt="Headshot of Rutwik Jain" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Rutwik Jain</h3>
      <p class="speaker-affiliation">Ph.D. candidate, Computer Sciences, University of Wisconsin-Madison</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Embrace the Chaos: Harnessing Variability for Large-Scale System Efficiency</em></p>
      <details>
        <summary>Abstract</summary>
        <p>Workload scaling has led large-scale systems like datacenters, supercomputers, and hyperscalers to deploy large, accelerator-rich systems with extreme power limits. Current GPU Thermal Design Power limits (TDPs) range from 1400-2000W, scaling to extreme power budgets at scale. Thus, power has displaced performance as the dominant constraint. My works address this challenge by co-optimizing power and performance at scale through cross-stack approaches spanning hardware, firmware, systems, and applications.</p>
        <p>Specifically, my research focuses on variability across GPUs in large-scale systems. I will present key insights from our variability characterization across different clusters and how we developed solutions for harnessing variability at the scheduler level to achieve better job performance and resource utilization. I will also talk about power excursions, where power temporarily spikes over GPU limits, and how excursion management can lead to performance gains and help carry out power optimizations like capping/pinning at scale.</p>
      </details>
      <details>
        <summary>Biography</summary>
        <p>Rutwik Jain is a Ph.D. candidate in the Computer Sciences department at the University of Wisconsin-Madison, advised by Prof. Matt Sinclair and Prof. Shivaram Venkataraman. His research interests are at the intersection of high-performance computing, computer architecture, and systems, with a focus on power management and power-performance co-optimization for large-scale accelerator-rich systems. Rutwik's work has appeared in Supercomputing (SC) and SIGMETRICS and he collaborates with Oakridge National Labs (ORNL) and AMD Research and Advanced Development (RAD) on his research. He was recognized as a Future Leader of AI at the doctoral consortium of the inaugural ACM AI Leadership Summit 2026.</p>
      </details>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/ning_headshot_20261015_compressed.jpeg' | relative_url }}" alt="Headshot of August Ning" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>August Ning</h3>
      <p class="speaker-affiliation">Postdoctoral Researcher, EPFL</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Metrics for Energy-Efficient Server Design and Operation</em></p>
      <details>
        <summary>Abstract</summary>
        <p>The recent unprecedented datacenter build-out has strained power grids and semiconductor economic markets around the world. To continue efficiency gains, server designers and datacenter operators must extract the most performance possible out of the power and hardware available to them. This talk motivates two metrics for designing and operating servers in this resource-constrained paradigm. First, at the server level, server CPU designs must prioritize Silicon Efficiency and optimize for both performance per power and performance per silicon area. Second, at the facility level, operating efficiency should look beyond Power Utilization Effectiveness (PUE) and further break down PUE's IT power using Infrastructure Utilization Efficiency (IUE). We will detail these two metrics and demonstrate how they encourage sustainable server design and operation.</p>
      </details>
      <details>
        <summary>Biography</summary>
        <p>August Ning is a postdoctoral researcher at EPFL working with Prof. Babak Falsafi, PARSA, and EcoCloud. His research interests span computer architecture under broadly defined economic constraints such as datacenters operation, sustainability, TCO, and computing policy. August received his PhD from Princeton University where he was advised by Prof. David Wentzlaff and supported by Princeton’s Gordon Y. S. Wu Fellowship and the NSF GRFP.</p>
      </details>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/abdulrahman.jpg' | relative_url }}" alt="Headshot of Abdulrahman Mahmoud" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Abdulrahman Mahmoud</h3>
      <p class="speaker-affiliation">Assistant Professor, Mohamed bin Zayed University of Artificial Intelligence (MBZUAI)</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Brain Computing Interfacing and the Life(time) Argument for Sustainable Computing</em></p>
      <details>
        <summary>Biography</summary>
        <p>Abdulrahman is an assistant professor at MBZUAI. His work is at the intersection of computer architecture, software system design, and ML, with the goal of co-designing future ML systems for high performance, scalable reliability, and intelligent resource allocation. Prior to joining MBZUAI in Abu Dhabi, he did a postdoc at Harvard University, received his PhD in CS at UIUC, and completed his BSE in EE at Princeton University.</p>
      </details>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name">
      <img class="sara-headshot" src="{{ '/photos/sara-mcallister.png' | relative_url }}" alt="Headshot of Sara McAllister" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Sara McAllister</h3>
      <p class="speaker-affiliation">Assistant Professor, University of Wisconsin-Madison, Computer Science Department</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>Out of sight, but no longer out of mind: tackling stored data’s emissions footprint</em></p>
      <details>
        <summary>Abstract</summary>
        <p>As AI workloads rapidly grow and improve, we will not only see more accelerators and compute, but also more data and more value in that data. While we are beginning to understand the emissions impact of these computing increases and how to mitigate them, storage’s emissions both remain out of sight despite dominating datacenter’s embodied footprint. In this talk, I will discuss the need for storage-specific emissions solutions, the challenges of decreasing storage’s emissions, and techniques to start addressing them.</p>
      </details>
      <details>
        <summary>Biography</summary>
        <p>Sara McAllister is an Assistant Professor at the University of Wisconsin-Madison in the Computer Science Department. Her research focuses on building sustainable datacenters, spanning caching, memory, storage, and AI systems from hardware to software. Her work has appeared at OSDI, SOSP, and ICML, including receiving Best Paper Awards at SOSP 2021 and SIGCSE 2023. She was a 2021 NDSEG Fellow, a 2023 EECS Rising Star, and a 2025 Siebel Scholar.</p>
      </details>
    </div>
  </article>

  {% assign timon_organiser = site.data.organisers | where: "name", "Timon Evenblij" | first %}
  <article class="speaker">
    <div class="photo-name">
      <img src="{{ '/photos/timon-evenblij.jpg' | relative_url }}" alt="Headshot of Timon Evenblij" width="120" height="150" loading="lazy">
    </div>
    <div class="bio">
      <h3>Timon Evenblij</h3>
      <p class="speaker-affiliation">imec</p>
      <p class="speaker-talk"><strong>Talk:</strong> <em>The impact of IC manufacturing on the sustainability of AI</em></p>
      <details>
        <summary>Biography</summary>
        <p>{{ timon_organiser.bio }}</p>
      </details>
      <details>
        <summary>Abstract</summary>
        <p> Assessing the sustainability of AI requires accounting for both operational energy use and the embodied emissions of its hardware. This talk examines how integrated-circuit manufacturing contributes to the life-cycle footprint of AI datacenters. It introduces imec.netzero’s bottom-up virtual fab model, combined in an overall model for performance, energy and emissions for AI datacenters.  We look at a case study of 1024 Nvidia H100 GPU cluster, to illustrates how the assessment scales from individual chips to servers and facility infrastructure, highlighting why sustainable hardware–software design decisions should consider the full life cycle.</p>
      </details>
     
      
    </div>
  </article>
</div>

### Panel Discussion
*Bridging Industry Practice and Academic Research for Sustainable Computing*

In the panel, we synthesize the industry and academic perspectives into actionable next steps for the community. A moderated panel of our invited speakers will address four themes, along with any questions from the audience:

1. **Energy efficiency:** Is energy efficiency still a meaningful sustainability objective for AI?
2. **Total carbon emissions as a metric:** How can researchers reasonably report the total carbon of a chip design?
3. **Avoiding local optimizations:** How do we avoid local microarchitectural optimizations that do not result in global improvements?
4. **Co-designing sustainably across the stack:** What areas of computer architecture should we work on more to improve AI sustainability across the stack?

### Interactive co-design session

The workshop includes hands-on, cross-disciplinary exercises where participants develop and adapt sustainable architecture strategies. [View the session format and assignments](#sustainability-co-design-exercises).


## Sustainability Co-Design Exercises

Participants work in small groups of 4–6 people, depending on workshop attendance, to identify research challenges that become visible when sustainability is considered across the computing stack. Each group develops its thinking around an exercise and reports key considerations to the workshop.

### Exercise 1: Bending Jevons Paradox in the Current AI Demand World

Jevons paradox says that improving resource-use efficiency can increase total resource consumption when a lower effective cost stimulates demand. AI demand may already be very high while deployment is constrained by supply, such as datacenter power capacity. With total datacenter power fixed, increasing accelerator tokens/s/W can increase tokens/s without increasing total datacenter energy use.

**Question:** If AI demand is effectively unlimited but deployment is supply-constrained, what can chip architects do to increase performance without increasing total carbon, or reduce total carbon without decreasing performance?

### Exercise 2: Aligning Total Cost of Ownership and Total Carbon

For AI infrastructure, hardware acquisition can represent the largest part of total cost of ownership (TCO). Assume 90% CAPEX (capital expenditure) and 10% OPEX (operational expenditure). For highly utilized, power-dense AI datacenter systems not operating on low-carbon electricity, use an illustrative lifecycle-carbon split of 30% CAPEM (embodied emissions) and 70% OPEM (operational emissions). These different balances can favor different designs.

**Question:** How can chip architects increase performance per unit of TCO without increasing total carbon, or reduce total carbon without decreasing performance?

### Exercise 3: The Most Sustainable Memory Choice

AI systems need both large memory capacity and high memory bandwidth, and memory can contribute substantially to an accelerator's carbon footprint. For this exercise, assume that in an 80 GB GPU, HBM (high-bandwidth memory) accounts for approximately 50% of embodied GPU emissions and 15% of operational emissions. Large-LLM inference serving concurrent users requires memory for KV caches; batching can improve memory-bandwidth utilization, while each user still needs interactive tokens/s performance.

**Questions:** Which memory architecture offers the lowest total carbon per user while meeting a required tokens/s/user target? Which workload assumptions could change the preferred choice, and when might a hierarchy of memory technologies be more sustainable?

### Exercise 4: Sustainable AI Across the Cloud–Edge Continuum

AI can run across a continuum that includes sensors, phones, personal computers, robots, vehicles, factories, wireless base stations, edge infrastructure, and datacenters, each with different constraints for cost, latency, energy, performance, utilization, and embodied footprint. Moving computation locally can increase lifecycle impact if dedicated hardware replaces infrastructure shared across users.

**Questions:** How should AI workloads be distributed across the cloud–edge continuum to balance useful capability, user-perceived performance, embodied and operational emissions?



## Organisers

<div class="organisers">

  {% for organiser in site.data.organisers %}
  <div class="organiser">
    <div class="photo-name">
      <img src="{{ organiser.photo | relative_url }}" alt="{{ organiser.name }}">
    </div>
    <div class="bio">
      <h4>{{ organiser.name }} ({{ organiser.affiliation }})</h4>
      <p>{{ organiser.bio }}</p>
    </div>
  </div>
  {% endfor %}

</div>



