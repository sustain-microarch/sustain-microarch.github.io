***Sustainable Computing Architecture: From Silicon to Datacenter – Co-Designing AI Systems Across the Stack***

AI workloads are fundamentally reshaping computing's energy profile, yet sustainability is still treated as a secondary optimization rather than a first-order design constraint. Worse, current trends show the embodied footprint of computing — from raw-material extraction and semiconductor manufacturing through assembly and end-of-life — is approaching or exceeding the operational footprint, a shift that most architecture and systems research has yet to internalize. 

Sustainability has been established as a cross-cutting architectural concern over the recent years, and a central thesis in achieving sustainable compute system architecture is Architecture-Technology Co-Optimization (ATCO), where architectural decisions, packaging choices, and manufacturing processes must be jointly evaluated against sustainability objectives rather than optimized in isolation.

## Objective

This workshop brings together complementary perspectives to address this gap across the full computing stack and the full product lifecycle. Bridging these layers, the workshop presents cross-stack co-design methodologies for environmentally sustainable computing that decomposes computing's environmental impact into actionable architectural levers. The workshop is intended to turn the attendee towards action, therefore we end the workshop with a hands-on codesign exercise.


## Program

| Time  | Session | Speaker | Topic | Resources |
|---|---|---|---|---|
| 08:00 - 08:05 | Opening | Arindam Malik (imec) | Overview of the Workshop |   |
| 08:05 - 08:20 | Session 1 | Rutwik Jain (Uwisc) |   |   |
| 08:20 - 08:35 | Session 1 | Mariam Elgamal (Harvard) |   |   |
| 08:35 - 08:50 | Session 1 | August Ning (EPFL) |   |   |
| 08:50 - 09:00 | Buffer + Coffee Break |   |   |   |
| 09:00 - 09:15 | Session 2 | Luca Benini (ETHZ, UNIBO) | Energy efficiency and Power management for AI accelerators - Tackling the MW rack challenge |   |
| 09:15 - 09:30 | Session 2 | Abdulrahman Mahmoud (MBZUAI)   |   |   |
| 09:30 - 09:45 | Session 2 | Vijay Reddi (Harvard) | Flexible electronics for sustainable computing |   |
| 09:45 - 10:00 | Buffer + Coffee break |   |   |   |
| 10:00 - 10:15 | Session 3 | Alex Bruefach (Meta) | Designing Data Foundations for Sustainability at Scale |   |
| 10:15 - 10:30 | Session 3 | Sarah McAllister (UWisc) |   |   |
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
    <div class="photo-name photo-placeholder" aria-hidden="true"></div>
    <div class="bio">
      <h3>Rutwik Jain</h3>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name photo-placeholder" aria-hidden="true"></div>
    <div class="bio">
      <h3>August Ning</h3>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name photo-placeholder" aria-hidden="true"></div>
    <div class="bio">
      <h3>Abdulrahman Mahmoud</h3>
    </div>
  </article>

  <article class="speaker">
    <div class="photo-name photo-placeholder" aria-hidden="true"></div>
    <div class="bio">
      <h3>Sarah McAllister</h3>
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



