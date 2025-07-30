# Group Intro

We are proudly part of the MIT Computer and Data Science Certificate Project  2024-2025

DATA ALCHEMISTS is dedicated to fostering a culture of trust, respect, and accountability
 while promoting open communication and efficient collaboration. Our goal is to
  create an environment that values diverse perspectives, encourages teamwork,
   and drives success. We support continuous learning and innovative thinking.
    Our shared commitment to growth and development empowers each member to
     contribute and learn from collective experiences, ensuring we work
      together effectively to achieve success.

## 👥 Team Members

* [Raneem Rami](https://github.com/Raneemrami)
* [Viktoriya Haiduk](https://github.com/ViktoriyaHaiduk)
* [Wuor Bhang](https://github.com/WuorBhang)
* [Salem Amassi](https://github.com/salemAmassi)
* [Norbert Busingye](https://github.com/Norbert250)

## Problem statement

In regions affected by war, the education system is one of the first societal
structures to collapse. Students who once demonstrated high academic performance
and consistent attendance often experience a significant decline in both after
conflict begins. Violence, displacement, psychological trauma, and the breakdown
of infrastructure such as internet access or school availability contribute
to reduced academic outcomes and disrupted attendance.

This project investigates how armed conflict affects students'
performance and attendance over time. By comparing pre-conflict
and during-conflict academic records, we aim to understand
the depth of disruption and identify patterns that can inform targeted interventions.

## research question

How does war disruption such as violence, displacement,
and infrastructure breakdown impact students'
academic performance and attendance on online learning
for students in colleges in war affected zones?

## Group Summary of the Problem Domain (with Systems Thinking)

Our group is focused on understanding the effects of the challenges faced by students in war-affected zones on their educational performance. These students are forced to rely on online education under extreme hardships-from exposure to violence,
displacement, and constant unreliable internet.

Using a systems thinking approach, we analyze the student's environment as a complex system, where various elements—physical safety, mental health, access to education, family displacement, and technology
 infrastructure—interact and reinforce one another. For instance:

      Displacement leads to unstable living conditions → Limited or no access to schools.

      Violence and trauma increase stress → Reduced concentration and motivation.

      Interrupted school services → Lower attendance and academic decline.

These effects often create a negative feedback loop, where low performance leads to disengagement, further worsening outcomes. By understanding these relationships, we aim to propose data-driven strategies to identify at-risk students against these effects.

**For further explanation of the problem, the iceberg model is applied** [in this file](/0_domain_study/systems_tkinking.md)

## 5 Ws and 1 H for our problem statement

| **Question** | **Answer** |
| ------------ | ---------------------------------------------------------------- |
| **Who**      | Students in war-affected regions who rely on online platforms for education.|
| **What**     | Their academic engagement and performance are being negatively impacted by conflict-related challenges such as violence, displacement, and unreliable internet access. |
| **Where**    | Conflict zones and war-affected areas where traditional education systems are disrupted.    |
| **When**     | During and after the onset of armed conflicts, particularly when students are displaced or formal schools are shut down.|
| **Why**      | War introduces instability and trauma, while displacement disrupts routine and internet access; these factors collectively harm students’ ability to learn and perform academically.|
| **How**      | By analyzing student interaction and performance data on online platforms,and assessing whether AI tools (e.g., adaptive learning, offline content, emotional support bots) can help mitigate the negative impacts and support effective learning.|

### How are we modeling our problem?

We are collecting data from the Islamic University of Gaza (IUG), this data includes Moodle logs capturing various student interactions in online learning during wartime, with fields such as:

* Timestamp
* Event type (e.g., view, submit, login, forum post)
* Course ID
* Module
* Duration on page
* Grade items
* Cohort or department identifiers
* Gender
* Level of study (when linked via user profiles), we believe these features

We believe these variables are going to be good indicators of college students’ academic engagement and performance during wartime. For example, we can tell how engaged a student is by capturing their number of logins, their duration on the page,
and by considering their grades as well.

We have also gathered  war events data from online websites, we are planning to use these to prove the harsh events going on in Gaza and correlate them with students' performance.

Since we do not have access to these same students’ data before the war (IUG students) to compare their academic performance before and after the war, we are going to be collecting data from another Palestinian university in the West Bank as proxy data.

Taking into consideration college students in the WestBank are not affected by war, but they might be indirectly affected by the situation currently taking place in Gaza from war to starvation to ongoing displacement, we think we can extract much more
valuable insights than if we just used any other proxy data from a non-war affected country.

**Possible flaws**:

* Some of the war events data we collected online contains untrue or misleading values, like the number of fatalities in a lot of datasets is in fact less than the actual number.
* We are going to be trying our best to take into consideration all of the harsh war events that college students in Gaza go through, but
due to a lack of data availability online about war events, we might miss some important effects like starvation.
* Some of the war events data that we have is not really up to date with the situation.

## Milestone 0: Cross-Cultural Collaboration

During this milestone (May 27 – June 2), our team focused on establishing a strong foundation for
 cross-cultural communication and collaborative workflows. Key deliverables include a configured
 repository with project boards, documented group norms, project constraints, communication plans,
  and learning goals. We also maintained meeting notes, set contributor guidelines, and completed a milestone retrospective. All materials were finalized and tagged before the deadline.

### 📄 Collaboration Documents

* [Communication Plan](./collaboration/communication.md)
* [Constraints](./collaboration/constraints.md)
* [Learning Goals](./collaboration/learning_goals.md)

---

## Milestone 1: Problem Identification

Between June 3 and June 16, our team focused on identifying a meaningful, personal, and researchable
 problem related to education in conflict zones. Through guided brainstorming and background
 research, we formulated a clear and actionable research question. We explored how armed conflict
 disrupts learning, damages infrastructure, and affects student performance and attendance. Our work
 during this milestone laid the foundation for the data-driven analysis that followed, integrating
 systems thinking and stakeholder perspectives to ensure relevance and real-world applicability.

### 📂 Domain Research Summary

* **Brainstorming Workflow**: We documented our ideation process using divergent and convergent thinking to explore and narrow down possible problem spaces. This helped us balance creativity with structure at each stage of exploration.
* **Problems Pool**: We compiled a diverse set of research questions centered on the impact of war on education. These were grouped into key themes such as student performance, infrastructure
breakdown, continuity of learning, and use of data in conflict zones.
* **Systems Thinking**: Using the Iceberg Model, we analyzed root causes beneath surface-level issues like absenteeism and low performance, identifying deeper factors such as trauma, displacement, and instability.
* **Five Ws and One H**: We applied this framework to define the core aspects of our problem (Who, What, Where, When, Why, How), ensuring clarity and structure.
* **Research Resources Overview**: We curated a rich collection of academic and field resources, categorized into:
  * War and Academic Performance  
  * Online Learning Barriers  
  * Impact of AI on Education  
  * Stakeholders (NGOs, humanitarian orgs, ministries)  

All documents and research are available in the [`0_domain_research`](/0_domain_research) folder.

---

## Milestone 2: Data Collection

Between June 17 and June 30, our team focused on collecting war events data to measure the effect of war.  We also created documentation, cleaning scripts, and a  cleaned version of all datasets. All
datasets used were obtained from open sources. However, to  enrich our analysis with real-world
academic outcomes, we have submitted data requests to universities for student performance data during wartime.

### 📁 Data Documentation

* All collected datasets and scripts are available in the [`2_data_preparation`](/2_data_preparation) folder.

* A detailed overview of our data sources, structure, and methodology is described in the [`README`](./2_data_preparation/README.md).

---

## Milestone 3: Data Analysis

From July 1 to July 21, our focus was analysing war events data and theirs impact on education system in Gaza . Rather than pursuing complex algorithms, we prioritized clarity, relevance,
 and alignment with the available data and domain context. We used visualizations along with both
  ['technical'](/4_data_analysis/technical_results.md)  and ['non-technical'](/4_data_analysis/non_technical_description.md) summaries to clearly communicate our insights.

### 📊 Analysis Work

During this milestone, we worked across two main folders:

* [`3_data_exploration`](/3_data_exploration/README.md) — initial exploration and early visual patterns.
* [`4_data_analysis`](/4_data_analysis/README.md) — deeper analysis and reproducible code.

### 🔍 Key Findings

Our analysis revealed the severe impact of the ongoing war on Gaza's education system:

* Over **500 schools** (more than **80%** of all schools) have been destroyed or damaged.
* **99.3%** of damaged infrastructure was residential — indicating that many students likely lost their homes. Excluding residential damage, **32.5%** of the remaining damage affected educational infrastructure.
* Most **displacement orders** occurred on weekdays, overlapping with class and exam schedules.
* **Attacks on food and market infrastructure** were highest in **Deir el-Balah** (75+) and **Gaza City** (65+) — areas densely populated by students (Oct 2023 – mid Sep 2024).
* **96.5%** of daily casualties were civilians: **34.7% children**, **41.4% men**, and **23.9% women**.
* **29 attacks** targeted people waiting for or receiving aid; **28** of these were attributed to the Israeli Armed Forces during the same period.

These findings highlight the multilayered disruption faced by students — from destroyed schools and homes to threats during daily routines and humanitarian efforts.

---

## Milestone 4: Communicating Results _(in progress)_

From July 22 to August 11, our focus is on translating our data-driven insights into actionable
messages for a well-defined audience. This milestone is about bridging the gap between technical
analysis and real-world impact through clear, accessible communication. We are currently working on
 identifying our target audience, understanding their needs and constraints, and designing an
 effective communication strategy tailored specifically to them.

 Stay tuned — this section will be updated with the final results and deliverables by
August 11.

### 🛠️ Tools We Use

* **Python** for data processing and analysis  
* **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`
* **Version Control & Collaboration**: Git, VS Code, and GitHub  
