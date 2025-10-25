# group4Web[Uploading index (1).html…]()
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saibai Learning Gardens: Climate-Ready Food Futures</title>
  <style>
    :root {
      color-scheme: only light;
      --accent: #197278;
      --accent-light: #e9f1ef;
      --secondary: #f4a259;
      --neutral: #f7f7f7;
      --body-color: #1f2a2a;
      --max-width: 1100px;
    }
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      color: var(--body-color);
      background-color: #ffffff;
      line-height: 1.65;
    }
    header {
      background: linear-gradient(135deg, rgba(25,114,120,0.9), rgba(30,86,99,0.92));
      color: #ffffff;
      padding: 80px 20px 120px;
      position: relative;
    }
    header::after {
      content: "";
      position: absolute;
      bottom: -40px;
      left: 50%;
      transform: translateX(-50%);
      width: min(90%, var(--max-width));
      height: 80px;
      background: #ffffff;
      border-radius: 20px;
      box-shadow: 0 20px 50px rgba(31,42,42,0.15);
      z-index: 0;
    }
    header .content {
      position: relative;
      max-width: var(--max-width);
      margin: 0 auto;
      z-index: 1;
    }
    header h1 {
      font-size: clamp(2.2rem, 5vw, 3.2rem);
      margin-bottom: 0.4rem;
      font-weight: 700;
      letter-spacing: 0.02em;
    }
    header p.subtitle {
      font-size: 1.15rem;
      max-width: 700px;
      font-style: italic;
    }
    header .metadata {
      margin-top: 1.8rem;
      display: grid;
      gap: 0.6rem;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    }
    header .metadata div {
      background: rgba(255,255,255,0.15);
      border: 1px solid rgba(255,255,255,0.5);
      padding: 0.8rem 1rem;
      border-radius: 12px;
      backdrop-filter: blur(6px);
      font-size: 0.95rem;
    }
    nav {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(255,255,255,0.95);
      border-bottom: 1px solid #e1e6e5;
    }
    nav ul {
      list-style: none;
      margin: 0 auto;
      padding: 12px 20px;
      max-width: var(--max-width);
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }
    nav a {
      text-decoration: none;
      color: var(--accent);
      font-weight: 600;
      padding: 6px 14px;
      border-radius: 999px;
      transition: background 0.2s, color 0.2s;
    }
    nav a:hover,
    nav a:focus {
      background: var(--accent);
      color: #ffffff;
      outline: none;
    }
    main {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 80px 20px 120px;
    }
    section {
      margin-bottom: 60px;
      position: relative;
      background: #ffffff;
      border-radius: 18px;
      padding: 40px 32px;
      box-shadow: 0 20px 50px rgba(31, 42, 42, 0.08);
    }
    section:nth-child(even) {
      background: var(--neutral);
    }
    section h2 {
      margin-top: 0;
      font-size: 1.75rem;
      color: #144349;
    }
    h3 {
      font-size: 1.25rem;
      margin-top: 2rem;
      color: #1a4f56;
    }
    p {
      margin: 0 0 0.85rem;
    }
    .grid {
      display: grid;
      gap: 1.2rem;
    }
    .grid.two {
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    }
    .pill {
      display: inline-block;
      background: var(--accent-light);
      color: var(--accent);
      padding: 6px 12px;
      border-radius: 999px;
      font-size: 0.85rem;
      font-weight: 600;
      margin-right: 6px;
      margin-bottom: 6px;
    }
    .highlight {
      border-left: 4px solid var(--secondary);
      padding-left: 16px;
      background: rgba(244,162,89,0.09);
      border-radius: 8px;
      margin-bottom: 1rem;
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 1.4rem;
      margin-top: 1.2rem;
    }
    .card {
      background: #ffffff;
      border: 1px solid #e1e6e5;
      border-radius: 14px;
      padding: 20px;
      height: 100%;
      box-shadow: 0 10px 30px rgba(20,67,73,0.08);
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 1.5rem;
      font-size: 0.95rem;
    }
    table thead {
      background: var(--accent);
      color: #ffffff;
    }
    table th, table td {
      border: 1px solid #d8dfde;
      padding: 10px 12px;
      text-align: left;
      vertical-align: top;
    }
    table tbody tr:nth-child(even) {
      background: rgba(25,114,120,0.08);
    }
    .timeline {
      border-left: 3px solid var(--accent);
      padding-left: 24px;
      margin: 1.5rem 0;
    }
    .timeline-item {
      margin-bottom: 1rem;
    }
    .tag {
      font-size: 0.78rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: #6d8687;
    }
    .cost-box {
      background: #ffffff;
      border: 1px solid rgba(25,114,120,0.2);
      border-radius: 16px;
      padding: 20px;
      margin-top: 1.2rem;
      box-shadow: inset 0 0 0 1px rgba(25,114,120,0.05);
    }
    details {
      margin-top: 1rem;
      background: rgba(25,114,120,0.06);
      border-radius: 12px;
      padding: 14px 18px;
    }
    details summary {
      font-weight: 600;
      cursor: pointer;
      color: #144349;
    }
    footer {
      text-align: center;
      padding: 40px 20px 60px;
      color: #5b6d6f;
      font-size: 0.9rem;
    }
    @media (max-width: 720px) {
      header {
        padding: 60px 16px 100px;
      }
      header::after {
        height: 60px;
      }
      section {
        padding: 30px 20px;
      }
      nav ul {
        justify-content: flex-start;
        overflow-x: auto;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="content">
      <p class="pill">5.4 Climate-Adaptive Food System · 2025 EWB Challenge</p>
      <h1>Saibai Learning Gardens: Climate-Ready Food Futures</h1>
      <p class="subtitle">Bilingual youth-led agroecology builds Saibai’s food security while celebrating Ailan Kastom and nurturing climate resilience.</p>
      <div class="metadata">
        <div><strong>Design Area</strong><br />5.4 Climate-Adaptive Food System (EWB, 2024)</div>
        <div><strong>How Might We</strong><br />Empower Saibai youth to co-create a climate-resilient food system that reduces import reliance while honouring Ailan Kastom?</div>
        <div><strong>Keywords</strong><br />Bilingual agroecology · Youth empowerment · Community gardens · Climate resilience · Torres Strait</div>
        <div><strong>Tutorial / Tutor</strong><br />Tutorial 04 – Zone B (Tutor: to be confirmed)</div>
      </div>
    </div>
  </header>

  <nav aria-label="Section navigation">
    <ul>
      <li><a href="#overview">Overview</a></li>
      <li><a href="#considerations">Key Considerations</a></li>
      <li><a href="#cost-summary">Cost Summary</a></li>
      <li><a href="#governance">Governance</a></li>
      <li><a href="#background">Background</a></li>
      <li><a href="#design-options">Design Options</a></li>
      <li><a href="#detailed-design">Detailed Design</a></li>
      <li><a href="#implementation">Implementation</a></li>
      <li><a href="#analysis">Cost &amp; Risks</a></li>
      <li><a href="#journey">Journey Map</a></li>
      <li><a href="#recommendations">Recommendations</a></li>
      <li><a href="#references">References</a></li>
      <li><a href="#appendices">Appendices</a></li>
    </ul>
  </nav>

  <main>
    <section id="overview">
      <h2>Proposal Summary</h2>
      <p>The project responds to saltwater intrusion, fragile supply chains, and declining youth engagement by co-designing a bilingual agroecology program anchored in demonstration gardens on Saibai Island. The initiative intertwines Ailan Kastom with climate-resilient horticulture, training youth mentors and household champions to cultivate salt-tolerant produce and micro-enterprises. Blended learning, scholarships, and cross-island partnerships sustain participation while diversifying diets. The approach aligns with community adaptation plans and strengthens self-determination over food systems (Engineers Without Borders Australia [EWB], 2024; Torres Strait Regional Authority [TSRA], 2022).</p>

      <h3>Overview of Design</h3>
      <div class="cards">
        <article class="card">
          <h4>Program Architecture</h4>
          <p>Two cyclone-ready demonstration gardens are co-managed by Tagai State College Saibai Campus and community rangers. The bilingual (Kala Kawau Ya/Yumplatok–English) curriculum scaffolds climate-adaptive horticulture, nutrition, enterprise, and cultural knowledge transfer.</p>
        </article>
        <article class="card">
          <h4>Capacity Building</h4>
          <p>Youth complete hands-on garden labs, diaries, and group projects, then cascade skills to households via a train-the-trainer model with elders and agronomists. Cultural protocols shape knowledge-sharing agreements.</p>
        </article>
        <article class="card">
          <h4>Digital Support</h4>
          <p>Low-bandwidth modules, printable packs, and a moderated Q&amp;A forum ensure continuity during monsoons or outages. Offline-first tools hedge against coverage gaps (Australian Digital Inclusion Index [ADII], 2023; Food and Agriculture Organization [FAO], 2021).</p>
        </article>
      </div>
    </section>

    <section id="considerations">
      <h2>Key Considerations &amp; Assumptions</h2>
      <ul>
        <li>Secure long-term site tenure and align with TSIRC land management approvals before installing structures (TSRA, 2022).</li>
        <li>Source materials from Cairns suppliers with cyclone ratings and schedule barge deliveries outside king-tide windows.</li>
        <li>Formalise knowledge-sharing agreements to respect cultural intellectual property and data sovereignty commitments.</li>
        <li>Establish maintenance rosters for irrigation, pest management, and digital platform moderation.</li>
        <li>Integrate program hours with Tagai College timetables to protect attendance incentives (Department of Education Queensland [DoE], 2023).</li>
        <li>Embed a feedback loop with the Torres Strait Health Partnership to monitor nutrition outcomes and adapt content.</li>
      </ul>
    </section>

    <section id="cost-summary">
      <h2>Proposed Materials &amp; Cost Summary</h2>
      <div class="grid two">
        <div>
          <h3>Purchased Materials (AUD)</h3>
          <ul>
            <li>Cyclone-rated shade structures – 18,200</li>
            <li>Modular wicking beds and liners – 12,400</li>
            <li>Two 15&nbsp;kL poly rainwater tanks – 8,600</li>
            <li>Solar pump and micro-drip irrigation kit – 6,100</li>
            <li>Chest freezer for produce storage – 3,800</li>
            <li>Garden tools, PPE, soil labs – 4,950</li>
            <li>Tablets and offline server – 5,200</li>
          </ul>
        </div>
        <div>
          <h3>Labour &amp; Training (AUD)</h3>
          <ul>
            <li>Local trades and installation crew – 9,600</li>
            <li>Elder honoraria and knowledge facilitation – 6,000</li>
            <li>Agronomist facilitation and curriculum design – 12,000</li>
            <li>Youth mentor scholarships (12 participants) – 10,800</li>
            <li>Digital content production and translations – 8,500</li>
          </ul>
        </div>
      </div>
      <div class="cost-box">
        <p><strong>Estimated Total Cost (Year&nbsp;1 capital + delivery):</strong> AUD&nbsp;95,150 (approximate). Includes 10% contingency for freight volatility; quoted in Australian dollars (local parity assumed).</p>
        <p><strong>Recurring Operating Cost (from Year&nbsp;2):</strong> AUD&nbsp;41,300 per annum (seeds/soil amendments 3,200; maintenance 2,400; scholarships 10,800; evaluation logistics 5,500; insurance &amp; contingencies 4,000; digital updates 3,200; staffing and stipends 12,200).</p>
      </div>
    </section>

    <section id="governance">
      <h2>Project Governance &amp; Team</h2>
      <div class="grid two">
        <div>
          <h3>Project Metadata</h3>
          <p><strong>Project Opportunity:</strong> Youth-led learning gardens and training hubs (Design Area 5.4).</p>
          <p><strong>Group Name:</strong> Team Learning Gardens Collective.</p>
          <p><strong>Contact Pathways:</strong> Tagai State College Saibai Campus Leadership · Torres Strait Island Regional Council (TSIRC) Climate Adaptation Team · Elders Council (Koedal, Samu, Zagareb).</p>
        </div>
        <div>
          <h3>Group Declaration</h3>
          <table aria-label="Group contributions">
            <thead>
              <tr>
                <th scope="col">Member</th>
                <th scope="col">Project Contributions</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Zijun Lin</td>
                <td>Geographic &amp; socio-economic research, Project Details, stakeholder mapping.</td>
              </tr>
              <tr>
                <td>Xingyu Liu</td>
                <td>Curriculum architecture, incentives strategy, Implementation Plan integration.</td>
              </tr>
              <tr>
                <td>Sheng Han</td>
                <td>Prototype iterations (posters, donation collateral, proposal layouts), user testing synthesis.</td>
              </tr>
              <tr>
                <td>Kefan Xu</td>
                <td>Cost modelling, logistics schedule, risk register, monitoring framework.</td>
              </tr>
              <tr>
                <td>Zhiyuan Sheng</td>
                <td>Community consultation synopsis, Journey Map, Recommendations, editorial coordination.</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

      <h3>Team Acknowledgement</h3>
      <div class="highlight">
        <p>We acknowledge the Saibai Koedal, Samu, and Zagareb clans as custodians of the lands and seas we reference, pay respect to Elders past and present, and recognise the resilience of Ailan Kastom in shaping climate-adaptive futures.</p>
      </div>
    </section>

    <section id="project-details">
      <h2>Project Details</h2>
      <p>Saibai Island sits four kilometres south of Papua New Guinea and hosts a predominantly Torres Strait Islander population of 465 residents with a median age of 23; ninety-six percent identify as Aboriginal and Torres Strait Islander peoples (Australian Bureau of Statistics [ABS], 2022). The island is a low-lying coral cay exposed to king tides, coastal erosion, and saline intrusion that regularly floods gardens, disrupts roads, and threatens potable water stores (TSRA, 2022). Fresh produce freighted from Cairns arrives infrequently and at prices 40–80% higher than mainland Queensland, leaving households dependent on packaged food and limiting diet diversity (EWB, 2024). Tagai State College Saibai Campus serves Prep to Year&nbsp;6 with boarding pathways for secondary students; attendance fluctuates due to weather, cultural obligations, and limited local employment opportunities (DoE, 2023).</p>
      <p>Community aspirations documented in the EWB Challenge emphasise capability-building, cultural continuity, and food sovereignty rather than reliance on external contractors. The Saibai Learning Gardens respond by building community-led education pathways, climate-resilient horticulture infrastructure, and inclusive knowledge systems that celebrate Ailan Kastom while improving nutrition and livelihoods.</p>
    </section>

    <section id="background">
      <h2>Background (Empathy Stage)</h2>
      <p>Consultations summarised in the 2025 EWB brief highlight three interlinked priorities: strengthen local food production; protect culturally significant species; and create meaningful youth pathways (EWB, 2024). Existing household gardens face saline soils, unreliable freshwater, cyclone damage, and limited access to agronomic support. Previous greenhouse pilots proved expensive, fragile, and hard to repair after storms. Elders advocate embedding gardening within cultural practice, language revitalisation, and intergenerational knowledge exchange.</p>
      <p>Comparable Pacific farmer field schools demonstrate that programs combining indigenous knowledge and scientific agronomy improve climate resilience and nutrition outcomes when they feature hands-on learning, peer mentoring, and community markets (FAO, 2021; The Pacific Community, 2021). Digital inclusion in remote Torres Strait communities remains uneven; 4G coverage fails during monsoons, making offline-first delivery vital (ADII, 2023). These insights underscore the project’s emphasis on community-driven learning, low-maintenance infrastructure, and hybrid delivery.</p>
    </section>

    <section id="problem">
      <h2>3. Problem Description</h2>
      <p><strong>User needs statement:</strong> Saibai youth and household champions need a culturally grounded, climate-ready agriculture program that is manageable with local resources so the community can reliably grow fresh produce and reduce reliance on expensive imports despite rising sea levels.</p>
      <p><strong>Problem analysis:</strong> Households contend with saline soils, limited agricultural extension support, and volatile freight that undermine food security and health. Younger residents leave for schooling or employment, weakening knowledge transfer. Without pathways connecting education, culture, and livelihood prospects, community resilience goals stall (EWB, 2024; DoE, 2023). The desired future sees youth leading community gardens, families adapting home plots with salt-tolerant crops, and local organisations coordinating supply chains and markets.</p>

      <h3>3.1 Design Criteria</h3>
      <ul>
        <li><strong>Climate resilience (weight 0.20):</strong> Infrastructure and horticultural practices must withstand cyclones, salt spray, and heat while conserving freshwater (TSRA, 2022).</li>
        <li><strong>Cultural integrity (0.20):</strong> Content must respect Ailan Kastom, be bilingual, and be co-authored with elders to protect knowledge sovereignty (EWB, 2024).</li>
        <li><strong>Youth engagement (0.20):</strong> Activities should align with school timetables, provide incentives, and create leadership pathways that increase attendance and retention (DoE, 2023).</li>
        <li><strong>Maintainability (0.15):</strong> Materials and systems must be repairable locally amid limited technical support.</li>
        <li><strong>Financial sustainability (0.15):</strong> Capital expenditure must remain below AUD&nbsp;100k with operating costs supported through partnerships, grants, or micro-enterprises.</li>
        <li><strong>Scalability &amp; collaboration (0.10):</strong> The model should translate to other Torres Strait communities and align with regional adaptation strategies (TSRA, 2022).</li>
      </ul>
    </section>

    <section id="design-options">
      <h2>3. Design Solution Options (Ideate)</h2>
      <div class="cards">
        <article class="card">
          <h3>Option 1: Cyclone-rated Hydroponic Greenhouses</h3>
          <p>Prefabricated greenhouse cluster with automated irrigation and remote monitoring (East-West Seed Knowledge Transfer, 2021). <strong>Pros:</strong> Controlled environment, high production. <strong>Cons:</strong> High capital (~AUD&nbsp;180k), complex maintenance, cyclone debris risk, limited cultural integration.</p>
        </article>
        <article class="card">
          <h3>Option 2: Subsidised Food Freight &amp; Vouchers</h3>
          <p>Partner with regional suppliers to increase cold-chain deliveries and provide nutrition vouchers. <strong>Pros:</strong> Immediate diet diversification. <strong>Cons:</strong> Deepens external dependency, no capability-building, freight vulnerable to weather (Queensland Government Statistician’s Office [QGSO], 2023).</p>
        </article>
        <article class="card">
          <h3>Option 3: Bilingual Agroecology Learning Gardens</h3>
          <p>Demonstration gardens with peer-led curriculum, train-the-trainer model, incentives, and hybrid delivery. <strong>Pros:</strong> Builds capacity, aligns with culture, moderate cost, scalable, fosters resilience (FAO, 2021; ADII, 2023). <strong>Cons:</strong> Requires sustained facilitation and curriculum development.</p>
        </article>
      </div>

      <h3>Design Selection (Screening)</h3>
      <p>A weighted decision matrix (weights detailed above) produced scores: Option&nbsp;1 – 63/100; Option&nbsp;2 – 58/100; Option&nbsp;3 – 86/100. Option&nbsp;3 outperformed alternatives on cultural fit, maintainability, and fiscal responsibility while maintaining strong production potential. Options&nbsp;1 and 2 remain contingency strategies during extreme events but do not meet long-term community aspirations. The team therefore advanced Option&nbsp;3 for detailed development.</p>
    </section>

    <section id="detailed-design">
      <h2>Detailed Design</h2>
      <div class="grid two">
        <div>
          <h3>Infrastructure &amp; Horticulture</h3>
          <ul>
            <li>Two 400&nbsp;m² demonstration gardens with wicking beds, cyclone-rated shade sails, trellises, and salt-tolerant crop trials (cassava, kangkong, sweet potato, pandanus).</li>
            <li>Rainwater harvesting, solar pumping, and micro-drip irrigation to conserve freshwater and reduce reliance on reticulated supply (TSRA, 2022).</li>
            <li>Soil remediation using biochar and crushed shell amendments co-developed with community rangers.</li>
          </ul>
        </div>
        <div>
          <h3>Learning Ecosystem</h3>
          <ul>
            <li>Eight bilingual modules aligned to the Australian Curriculum: Soil &amp; Water Guardians, Ailan Kastom Foods, Climate Science for Saibai, Household Micro-enterprises, Nutrition &amp; Wellbeing.</li>
            <li>Elders co-facilitate seasonal calendar storytelling and cultural protocols; students maintain garden diaries and micro-learning reflections.</li>
            <li>Youth Garden Mentors (12 participants) receive scholarships, facilitator training, and lead peer circles alongside elders and agronomists.</li>
          </ul>
        </div>
      </div>
      <h3>Digital Delivery</h3>
      <p>The blended platform combines a Google Site hub with downloadable PDF lesson packs, audio stories in Yumplatok, and SMS planting alerts. A portable Lamassu server caches resources to maintain access during outages (ADII, 2023). Content is updated termly with community review to maintain relevance and accuracy.</p>
      <h3>Partnership &amp; Incentives</h3>
      <p>Scholarships funded through NGOs and universities incentivise youth leadership, while micro-grants support household garden expansion. Formal partnerships with TSIRC climate adaptation and the Torres Strait Health Partnership embed monitoring, provide policy alignment, and create pathways to share data-driven insights (TSRA, 2022).</p>
    </section>

    <section id="prototyping">
      <h2>Prototyping &amp; Testing</h2>
      <div class="highlight">
        <p>Prototypes serve to communicate the design and validate functionality. Iterations progressed from low-fidelity sketches to high-fidelity collateral informed by community feedback.</p>
      </div>
      <ul>
        <li><strong>Bilingual Posters &amp; Donation Collateral:</strong> Low-fi hand-drawn posters tested clarity of the “what/why/how” message with six Tagai students and three advisors; high-fi versions incorporated real Saibai imagery, QR donation links, and cultural motifs, improving warmth and engagement (feedback via Sheng Han sessions).</li>
        <li><strong>Curriculum Storyboards:</strong> Module flow tested with Youth Mentors to assess pacing, language, and cultural cues; adjustments included more dual-language prompts and reflective prompts tied to Elders’ narratives.</li>
        <li><strong>Garden Demonstrator:</strong> A wicking-bed prototype built with recycled drums validated tool accessibility, assembly steps, and watering frequency. Testing informed tool procurement (ergonomic handles) and session timing.</li>
        <li><strong>Digital Experience:</strong> Offline-first prototypes trialled caching and SMS scripts; user testing confirmed the need for printable checklists and phonetic Yumplatok spellings for younger learners.</li>
      </ul>
    </section>

    <section id="implementation">
      <h2>Implementation Plan</h2>
      <div class="timeline">
        <div class="timeline-item">
          <span class="tag">Phase 0 · Oct–Dec 2024</span>
          <p>Formalise MOUs with TSIRC, Tagai College, and elders; secure sites and approvals; conduct baseline nutrition and attendance surveys; confirm supplier quotes and freight bookings.</p>
        </div>
        <div class="timeline-item">
          <span class="tag">Phase 1 · Jan–Apr 2025</span>
          <p>Install infrastructure during the dry season; co-design curriculum workshops; develop bilingual resources; train Youth Garden Mentors and adult champions.</p>
        </div>
        <div class="timeline-item">
          <span class="tag">Phase 2 · May–Aug 2025</span>
          <p>Launch weekly garden labs and Saturday community sessions; implement household micro-grants; host first harvest celebration; gather midline data.</p>
        </div>
        <div class="timeline-item">
          <span class="tag">Phase 3 · Sep 2025–Mar 2026</span>
          <p>Expand to second garden site; integrate micro-enterprise module; share learnings via regional forums; conduct final evaluation and publish replication guide.</p>
        </div>
        <div class="timeline-item">
          <span class="tag">Ongoing</span>
          <p>Maintenance rosters, digital updates, seasonal scenario drills, and cross-island exchanges (Boigu, Dauan) to scale insights.</p>
        </div>
      </div>
      <h3>Roles &amp; Responsibilities</h3>
      <ul>
        <li><strong>Tagai State College:</strong> Curriculum integration, youth mentor supervision, facility access.</li>
        <li><strong>Elders Council:</strong> Cultural governance, knowledge validation, storytelling facilitation.</li>
        <li><strong>TSIRC Climate Team:</strong> Land approvals, data sharing into regional adaptation reports.</li>
        <li><strong>Community Rangers:</strong> Garden maintenance, biosecurity, and infrastructure checks.</li>
        <li><strong>External Partners:</strong> Universities and NGOs provide scholarships, agronomic expertise, and monitoring support.</li>
      </ul>
    </section>

    <section id="analysis">
      <h2>Cost Analysis &amp; Risk Management</h2>
      <h3>Financial Overview</h3>
      <p>Capital costs total AUD&nbsp;95,150 (infrastructure 59,250; training and incentives 35,900). Operating costs from Year&nbsp;2 equal AUD&nbsp;41,300 annually. A 10% contingency covers freight fluctuations. Anticipated revenue from produce sales, workshops, and events is AUD&nbsp;9,600 per year after ramp-up (23% of operating costs) based on comparable remote garden programs (FAO, 2021; QGSO, 2023).</p>
      <h3>Funding Pathways</h3>
      <ul>
        <li>TSRA Climate Adaptation Grants and Queensland Indigenous Ranger Program support.</li>
        <li>Philanthropic contributions (Jawun, Good360) and targeted crowdfunding using bilingual collateral.</li>
        <li>Partnership with universities for service-learning placements and research grants.</li>
      </ul>
      <h3>Risk Register Snapshot</h3>
      <table aria-label="Risk register">
        <thead>
          <tr>
            <th scope="col">Risk</th>
            <th scope="col">Likelihood</th>
            <th scope="col">Impact</th>
            <th scope="col">Mitigation</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Cyclone damage to infrastructure</td>
            <td>Medium</td>
            <td>High</td>
            <td>Use demountable shade cloths, secure storage, and pre-season drills; insure assets.</td>
          </tr>
          <tr>
            <td>Freight delays</td>
            <td>High</td>
            <td>Medium</td>
            <td>Pre-order consumables quarterly; maintain buffer stock; explore local composting.</td>
          </tr>
          <tr>
            <td>Digital access outages</td>
            <td>Medium</td>
            <td>Medium</td>
            <td>Offline server, printed packs, radio segments, and SMS updates.</td>
          </tr>
          <tr>
            <td>Knowledge-sharing sensitivities</td>
            <td>Low</td>
            <td>High</td>
            <td>Formal cultural IP agreements, community-led content approvals, data sovereignty protocols.</td>
          </tr>
          <tr>
            <td>Youth attrition</td>
            <td>Medium</td>
            <td>Medium</td>
            <td>Scholarships, recognition events, integration with curriculum credit, mentorship support.</td>
          </tr>
        </tbody>
      </table>
    </section>

    <section id="other-considerations">
      <h2>Other Considerations</h2>
      <ul>
        <li><strong>Waste minimisation:</strong> Compost organic waste; repurpose plastics via TSIRC recycling streams; introduce worm farms for classroom science links.</li>
        <li><strong>Data sovereignty:</strong> Locally governed data storage with informed consent, respecting Torres Strait data protocols.</li>
        <li><strong>Accessibility &amp; Inclusion:</strong> Raised beds at varied heights, quiet reflection spaces, and inclusive roster planning to support girls and students with disability.</li>
        <li><strong>Health integration:</strong> Coordinate with Torres and Cape Hospital and Health Service for nutrition monitoring and health promotion alignment.</li>
      </ul>
    </section>

    <section id="journey">
      <h2>Community Journey Map</h2>
      <div class="cards">
        <article class="card">
          <h3>Discovery</h3>
          <p>Students encounter bilingual posters and taster lessons; elders lead a blessing and share seasonal stories; TSIRC officers review implementation briefs and confirm alignment with adaptation goals.</p>
        </article>
        <article class="card">
          <h3>Engagement</h3>
          <p>Weekly garden labs, household visits, and digital updates build trust. Families witness produce growth and cultural storytelling, anchoring the initiative in community pride.</p>
        </article>
        <article class="card">
          <h3>Ownership</h3>
          <p>Households replicate wicking beds, elders co-lead seasonal planning, and TSIRC integrates data into regional reporting. Youth mentors facilitate harvest markets, reinforcing autonomy.</p>
        </article>
      </div>
    </section>

    <section id="recommendations">
      <h2>Recommendations &amp; Next Steps</h2>
      <ol>
        <li>Confirm tutor allocation and embed program hours within the Tagai College timetable to secure credit and attendance incentives.</li>
        <li>Lock material quotations and freight schedules six months in advance; establish shared procurement tracking with TSIRC.</li>
        <li>Finalize cultural intellectual property agreements, including revenue-sharing for value-added products and media usage protocols.</li>
        <li>Establish a monitoring partnership with Torres and Cape Hospital and Health Service to link diet diversity and health indicators.</li>
        <li>Plan cross-island exchange visits (Boigu, Dauan) in Year&nbsp;2 to pilot replication and share Youth Mentor experiences.</li>
      </ol>
    </section>

    <section id="references">
      <h2>References</h2>
      <ol>
        <li>Australian Bureau of Statistics. (2022). <em>2021 Census QuickStats: Saibai Island (State Suburb)</em>. https://www.abs.gov.au/census</li>
        <li>Australian Digital Inclusion Index. (2023). <em>Australian digital inclusion index 2023</em>. https://digitalinclusionindex.org.au</li>
        <li>Department of Education Queensland. (2023). <em>Far North Queensland region school attendance data</em>. Brisbane, QLD: Author.</li>
        <li>Engineers Without Borders Australia. (2024). <em>2025 EWB Challenge brief: Saibai Island</em>. Melbourne, VIC: Author.</li>
        <li>Food and Agriculture Organization of the United Nations. (2021). <em>School gardens for nutrition and better livelihoods</em>. Rome, Italy: FAO.</li>
        <li>Queensland Government Statistician’s Office. (2023). <em>Queensland regional profiles: Torres Strait Island communities</em>. Brisbane, QLD: Author.</li>
        <li>The Pacific Community. (2021). <em>Fijian farmers better equipped for sustainable agriculture</em>. https://www.spc.int/updates/blog/2021/02/fijian-farmers-better-equipped-sustainable-agriculture</li>
        <li>Torres Strait Regional Authority. (2022). <em>Torres Strait Climate Change Strategy 2022–2032</em>. Thursday Island, QLD: TSRA.</li>
        <li>East-West Seed Knowledge Transfer. (2021). <em>Learning farm in Bukidnon, Philippines</em>. East-West Seed.</li>
      </ol>
    </section>

    <section id="appendices">
      <h2>Supporting Documentation (Appendices)</h2>
      <details open>
        <summary>Appendix 1: Group Charter</summary>
        <p>Week&nbsp;2 charter outlining team values, decision-making processes, communication cadence, and conflict resolution steps (document available on request).</p>
      </details>
      <details>
        <summary>Appendix 2: Meeting Minutes &amp; Consultation Summaries</summary>
        <p>Includes fortnightly meeting records, elder consultation notes, and feedback logs from Tagai College staff and youth participants.</p>
      </details>
      <details>
        <summary>Appendix 3: Decision Matrix, Risk Register, Cost Workbook</summary>
        <p>Provides full scoring tables, underlying assumptions, and cost breakdown spreadsheets supporting selections and financial estimates.</p>
      </details>
      <details>
        <summary>Appendix 4: Prototype Artefacts</summary>
        <p>Contains low-fi and high-fi posters, donation collateral, curriculum storyboards, and testing feedback summaries.</p>
      </details>
      <details>
        <summary>Appendix 5: Monitoring &amp; Evaluation Instruments</summary>
        <p>Baseline survey templates, garden diary samples, diet diversity checklists, and data consent forms.</p>
      </details>
      <details>
        <summary>Appendix 6: Prompt Log (if generative AI used)</summary>
        <p>Log documenting prompts, responses, and human editing decisions, satisfying academic integrity requirements.</p>
      </details>
    </section>
  </main>

  <footer>
    <p>Saibai Learning Gardens · Prepared for the 2025 EWB Challenge · Climate-Adaptive Food Systems</p>
  </footer>
</body>
</html>
