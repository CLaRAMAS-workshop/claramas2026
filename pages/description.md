---
layout: page
title: Description
permalink: /description/
feature-img: "assets/img/header/Paphos-Cyprus.jpg"
tags: [aim, scope, motivation, impact]
---

Welcome to the homepage of the 
**1st International Workshop on "Causal Learning and Reasoning in Agents and Multiagent Systems" (CLaRAMAS)**, 
hosted by the [25th International Conference on Agents and Multiagent Systems (AAMAS)](https://cyprusconferences.org/aamas2026/) ☺️

#### Aim

This workshop aims to foster cross-disciplinary exchange 
and synergistic collaboration between two complementary communities: 
the AAMAS community 🤖, 
    focused on advancing the **engineering of autonomous agents and MAS**, 
and the Causal Learning and Reasoning (CLR) community 🔎, 
    dedicated to developing models and methods for **causal discovery an inference**. 

The overarching goal is to **bridge these domains** by exploring the following open questions: 

  * 🤔 *How CLR techniques can enhance agent-based decision-making?* ❓
  * ❓ *How agent-oriented perspectives can leverage the operational deployment of causal models in real-world applications?* 🤔

#### Scope

The concept of an "agent" represents a foundational abstraction in software engineering, 
encapsulating the notion of agency---namely, the capacity of a software entity to bring about effects 
in pursuit of specific goals within its operating environment. 
Exercising agency requires the ability to interpret the structure and dynamics of that environment 
and to anticipate its responses to the agent's actions. 
In essence, 

> **agency hinges on understanding and leveraging the causal relationships** 
> among observable and controllable variables (e.g., through sensors and actuators). 

Such causal reasoning is indispensable for planning actions 
that reliably achieve intended objectives---a principle reinforced by recent research on causal inference in emerging "agentic AI" systems. 

This requirement extends naturally to **multi-agent systems** (MAS), 
a cornerstone of distributed artificial intelligence, 
where multiple agents coexist and interact within a shared environment. 
These interactions -- whether cooperative or competitive -- contribute to individual and systemic goals, 
either through direct communication or indirect influence on the environment. 
Consequently, 

> **effective coordination in multi-agent settings 
> depends on a causal understanding of interdependencies** 
> among agents’ behaviors. 

Only by modeling these reciprocal influences can agents achieve robust and purposeful collaboration 
(or competition) toward their respective objectives.

#### Motivation

> ⚠️ However, this fundamental role of causal modelling 
> of the agent-environment and agent-agent relationships 
> is **not yet widely and deeply discussed in the AAMAS community. ⚠️**

Although Causal Learning and Reasoning (CLR) methods 
-- encompassing techniques for discovering qualitative cause-effect relationships 
(i.e., which variables influence others), 
quantifying their strength 
(how much a variable influences another), 
and exploiting them for tasks such as planning, inference, and prediction -- 
are rapidly expanding beyond their traditional domains 
(e.g., medicine, econometrics) 
into computer science, 
their integration into agent and MAS engineering remains limited. 

In fact, 

> 👉 current approaches largely rely on **implicit or naïve causal modeling**. 😔 
 
For example, the plan library of a BDI agent 
constitutes an implicit causal model 
reflecting the developer's assumptions about environmental dynamics 
and the expected effects of actions on goal achievement. 
However, no theoretically grounded causal model is explicitly constructed or learned, 
nor is **any formal representation** made available to the agent for observation, refinement, or manipulation. 

Similarly, most learning-based agents, 
including those built with reinforcement learning (RL) 
-- where the causal notion of intervention aligns naturally with agents' actions -- 
encode causal knowledge **implicitly** within learned policies 
rather than through explicit, interpretable causal models.

#### Expected impact

> 👉 The availability of an **explicit, 
> mathematically grounded causal model** 
> would bring several key advantages for agent and MAS engineering. 😃 
 
  1. 🧠 It would provide a **unified framework 
for prediction, planning, and diagnosis** of agent behavior, 
based on principled reasoning about the consequences of actions 
and the causes of observed effects. 
  2. 💡 It would enable richer forms of reasoning, 
including **interventional ("What if I do this?") 
and counterfactual** ("What if I had acted differently in that situation?") analyses.
  3. 🤝 It would facilitate **seamless integration between learning-based and programming-based approaches**, 
as causal models can be partially designed and then 
completed, expanded, or refined by learning from data. 
  4. 💪 It would **enhance decision-making robustness** 
in environments characterized by noise and spurious correlations, 
mitigating risks of erroneous decision-making. 
  5. 🔍 It would **improve the transparency and trustworthiness** 
of learned behaviors, offering interpretable models 
that support verification and accountability.

---

If you are persuaded that CRL can notably improve the way we build 
autonomous agents and multi-agent systems,
📝 **consider submitting a paper** 📝 to join this new and promising research direction.

Check the detailed [Call for Papers](/cfp).

---
