***Silicon to Datacenter — Co-Designing AI Systems Across the Stack***

AI workloads are fundamentally reshaping computing's energy profile, yet sustainability is still treated as a secondary optimization rather than a first-order design constraint. Worse, current trends show the embodied footprint of computing — from raw-material extraction and semiconductor manufacturing through assembly and end-of-life — is approaching or exceeding the operational footprint, a shift that most architecture and systems research has yet to internalize. 

Sustainability has been established as a cross-cutting architectural concern over the recent years, and a central thesis in achieving sustainable compute system architecture is Architecture-Technology Co-Optimization (ATCO), where architectural decisions, packaging choices, and manufacturing processes must be jointly evaluated against sustainability objectives rather than optimized in isolation.

## Objective

This workshop brings together complementary perspectives to address this gap across the full computing stack and the full product lifecycle. At the silicon and package level, we examine how advanced packaging and 3D integration can reduce both operational energy and manufacturing waste. At the datacenter level, we address cloud-scale efficiency through inference serving disaggregation, power stabilization for AI training clusters, and hardware memory compression. 

Bridging these layers, we present cross-stack co-design methodologies for environmentally sustainable computing — from specialized hardware for recommendation and agentic AI workloads with open-source benchmarking through MLPerf, that decomposes computing's environmental impact into actionable architectural levers. The holistic lifecycle perspective — spanning extraction, manufacturing, use, and end-of-life — provides the conceptual spine that connects every technical contribution. We also extend this trajectory by integrating [IMEC's SSTS initiative](https://www.imec-int.com/en/expertise/cmos-advanced/sustainable-semiconductor-technologies-and-systems-ssts), closing the loop between architecture-level design exploration and quantitative manufacturing footprint assessment.


## Program

| Time  | Session | Speaker | Topic | Resources |
|---|---|---|---|---|
| 08:00 - 08:05 | Opening | Arindam Malik (imec) | Overview of the Workshop |   |
| 08:05 - 08:20 | Session 1 | Rutwik Jain (Uwisc) |   |   |
| 08:20 - 08:35 | Session 1 | Mariam Elgamal (Harvard) |   |   |
| 08:35 - 08:50 | Session 1 | August Ning (EPFL)) |   |   |
| 08:50 - 09:00 | Buffer + Coffee Break |   |   |   |
| 09:00 - 09:15 | Session 2 | Luca Benini (ETHZ)   |   |   |
| 09:15 - 09:30 | Session 2 | Abdulrahman Mahmoud (MBZUAI)   |   |   |
| 09:30 - 09:45 | Session 2 | Vijay Reddi (Harvard)   |   |   |
| 09:45 - 10:00 | Buffer + Coffee break |   |   |   |
| 10:00 - 10:15 | Session 3 | Alex Bruefach (Meta) |   |   |
| 10:15 - 10:30 | Session 3 | Sarah McAllister (UWisc) |   |   |
| 10:30 - 10:45 | Session 3 | Timon Evenblij (imec) |   |   |
| 10:45- 11:00 | Buffer + Coffee break |   |   |   |
| 11:00 - 11:30 | Panel | All presenters |   |   |
| 11:30 - 12:00 | Codesign exercises | All workshop attendees |   |   |


## Topics

* Holistic lifecycle sustainability: embodied vs. operational footprint, and full-lifecycle LCA
* Quantifying the manufacturing footprint: imec.netzero virtual fab modeling and the SSTS industry consortium
* Energy-efficient silicon: advanced packaging (chiplets, DRAM-on-Logic, 3D integration) and SoC/SiP design for sustainability
* Cloud-scale AI efficiency: Splitwise inference disaggregation, power stabilization, hardware memory compression
* Cross-stack co-design: specialized systems for recommendation and agentic AI, democratizing AI on resource-constrained hardware
* Manufacturing sustainability R&D (PFAS-free materials, process gas abatement)


## Format

### 3 Sessions with presenters from practitioners across the AI stack
Titles and abstracts of each presenter will be uploaded soon.

### Panel Discussion
*Bridging Industry Practice and Academic Research for Sustainable Computing*

In this session, we synthesize the industry and academic perspectives into actionable next steps for the community. A moderated panel of our invited speakers from the industry and academia, with audience participation, will address three provocations:

1. What sustainability metrics should architecture conferences require in paper evaluations?
2. How do we close the gap between manufacturing-level LCA data and system-level design decisions?
3. Is the embodied-vs-operational crossover a temporary trend or a permanent shift — and what does that mean for research priorities?

### Co-Design Exercise -- Where do we go from here?*

This session concludes beyond the panel discussion with a *hands-on co-design exercise* where cross-disciplinary groups develop sustainable architecture strategies for a representative AI workload.



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


## Speakers

Speaker bio's will be updated soon

<!-- <div class="speakers">

  {% for speaker in site.data.speakers %}
  <div class="speaker">
    <div class="photo-name">
      <img src="{{ speaker.photo | relative_url }}" alt="{{ speaker.name }}">
    </div>
    <div class="bio">
      <h4>{{ speaker.name }} ({{ speaker.affiliation }})</h4>
      <p>{{ speaker.bio }}</p>
    </div>
  </div>
  {% endfor %}

</div> -->
