# Knowledge Inbox

This document stores reusable research knowledge from my LLM-based multi-agent research sprint.

It is not a paper note file.  
It is a semi-structured and expandable knowledge collection.

---

### E001 - Communication Taxonomy in LLM-MAS

**Primary Bucket:** LLM-based Multi-Agent Systems — Communication Taxonomy

**Date:** 17/5/2026

**Source:**  
Paper 2 — *Beyond Self-Talk: A Communication-Centric Survey of LLM-Based Multi-Agent Systems*


**Keywords:**  
LLM-MAS, communication architecture, communication goal, communication protocol, communication strategy, communication paradigm, communication object, communication content, multi-agent coordination, natural language communication, implicit communication, blackboard, message passing

**Content:**  

Paper 2 describes communication in LLM-based multi-agent systems through seven aspects:

1. **Architecture**  
   Architecture describes how agents are organized at the system level and how information can flow among them.

   Main categories:
   - Flat architecture
   - Hierarchical architecture
   - Team architecture
   - Society architecture
   - Hybrid architecture

   Accurate understanding:  
   Architecture is about the overall structure or topology of the agent system. It answers who can communicate with whom and how agents are arranged. It should not be confused with communication strategy, which describes the runtime order or procedure of communication.

2. **Goal**  
   Goal describes why agents communicate.

   Main categories:
   - Cooperation
   - Competition
   - Mixed goal

   Accurate understanding:  
   Communication design should depend on the task goal. Cooperative tasks favor information sharing and joint planning, while competitive tasks may involve debate, persuasion, negotiation, or strategic information control. Mixed settings may combine both.

3. **Protocol**  
   Protocol describes the rules, interfaces, or standards that govern communication.

   Main categories:
   - Model Context Protocol
   - Agent-to-Agent Protocol
   - Agent Network Protocol

   Accurate understanding:  
   Protocol is more infrastructure-oriented. It specifies how messages, context, capabilities, tools, or requests are formatted and exchanged. It is different from architecture: architecture describes system organization, while protocol describes communication rules and interfaces.

4. **Strategy**  
   Strategy describes the runtime procedure or temporal pattern of communication.

   Main categories:
   - One-by-one
   - Simultaneous-talk
   - Simultaneous-talk-with-summarizer

   Accurate understanding:  
   Strategy answers how communication unfolds during execution. For example, agents may speak sequentially, generate responses independently in parallel, or speak simultaneously and then be summarized by another component. Strategy is constrained by architecture but not identical to it.

5. **Paradigm**  
   Paradigm describes the fundamental communication mechanism.

   Main categories:
   - Message passing
   - Speech act
   - Blackboard

   Accurate understanding:  
   Paradigm is more abstract than strategy. Message passing means agents directly send messages to each other. Speech act emphasizes the function of utterances, such as requesting, proposing, criticizing, or commanding. Blackboard means agents interact through a shared workspace or shared information pool.

6. **Object**  
   Object describes the target of communication.

   Main categories:
   - Self
   - Other agents
   - Environment
   - Human

   Accurate understanding:  
   Communication is not limited to agent-agent dialogue. An agent may communicate with itself through reflection, with other agents through messages, with the environment through action-feedback loops, or with humans through feedback and intervention. This aspect is closely related to capability acquisition and human-in-the-loop systems.

7. **Content**  
   Content describes what kind of information is exchanged.

   Main categories:
   - Explicit communication
     - Natural language
     - Code and structured data
   - Implicit communication
     - Behavioral feedback
     - Environmental signal

   Accurate understanding:  
   Natural language is still the dominant form of explicit communication in many LLM-MAS systems, but it is not the only form. Code, structured data, tool outputs, execution traces, environmental feedback, and behavioral signals are also important. Multimodal communication is an emerging extension rather than the default mainstream form.

These seven aspects should not be treated as fully independent dimensions. Some combinations are more natural than others. For example, hierarchical architecture usually supports local simultaneous communication within the same layer, but cross-layer communication often becomes sequential, summarized, or control-oriented. Therefore, communication design in LLM-MAS should be understood as a constrained design space rather than a free combination of independent variables.

---

**Source:**  
Paper 3 — *Survey on Evaluation of LLM-based Agents*

**Keywords:**  
cost-efficiency, safety, robustness, fine-grained evaluation, scalable evaluation, benchmark limitation, process-level evaluation, agent reliability, communication cost, fair baseline

**Content:**  

Key discussion points from Paper 3:

- **Cost-efficiency:** final performance should be considered together with token cost, API calls, tool calls, and inference budget.
- **Safety:** agent evaluation should consider unsafe intermediate actions, not only final answers.
- **Robustness:** agents should remain stable across prompts, tasks, environments, and repeated runs.
- **Fine-grained evaluation:** final task success is insufficient; evaluation should inspect planning, tool use, memory, reflection, and interaction process.
- **Scalable evaluation:** evaluation methods must handle long-horizon tasks, dynamic environments, and complex workflows.
- **Benchmark limitations:** many benchmarks are static, final-answer-oriented, or too narrow to capture real agent behavior.
- **LLM-MAS implication:** multi-agent systems need evaluation of communication quality, coordination quality, cost, robustness, and fair baselines.

---
**Short Title:** Open Problems in Autonomous LLM Agent Memory

**Date:** 19/5/2026

**Source:**  
Paper — *Memory for Autonomous LLM Agents: Mechanisms, Evaluation, and Emerging Frontiers*, Section 9 Open Challenges


**Content:**  

Section 9 lists the main open problems for autonomous LLM agent memory:

- **Principled consolidation:**  
  How to decide what should be kept, compressed, promoted to long-term memory, or discarded. Current systems risk either storing too much noise or forgetting rare but important facts.

- **Causally grounded retrieval:**  
  Current retrieval often relies on semantic similarity, but useful memories may be causally relevant even when they are semantically distant. Future systems may need causal links, temporal structure, and counterfactual relevance.

- **Trustworthy reflection:**  
  Reflective memory can reinforce wrong conclusions. Agents need validation, uncertainty estimation, contradiction checking, adversarial probing, and expiration policies for reflected lessons.

- **Learning to forget:**  
  Forgetting should be selective and purposeful, not just time-based deletion or storage-limit eviction. It matters for robustness, privacy, efficiency, and safety.

- **Multimodal and embodied memory:**  
  Agents in robotics, games, or mixed-reality settings need memory over text, vision, audio, spatial states, tool states, and embodied experience.

- **Multi-agent memory governance:**  
  Multi-agent systems need rules for shared memory, access control, concurrent writes, consensus, memory merging, and knowledge transfer between specialized agents.

- **Memory-efficient architectures:**  
  Memory-augmented agents can be expensive because of long contexts, repeated retrieval, and growing memory stores. Future systems need cheaper retrieval, compression, sparse access, or memory-native architectures.

- **Deeper neuroscience integration:**  
  Current systems borrow cognitive labels superficially. More useful mechanisms may come from spreading activation, reconsolidation, forgetting curves, and spaced repetition.

- **Foundation models for memory management:**  
  A long-term direction is training general memory controllers that can decide when to write, retrieve, summarize, forget, and consolidate across many tasks.

- **Standardized evaluation:**  
  The field lacks shared evaluation protocols and leaderboards for agent memory. Current benchmarks use different datasets, metrics, and settings, making comparisons unreliable.
---
