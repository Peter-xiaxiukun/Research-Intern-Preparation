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

### E002 - [Short Title]

**Date:**  
**Source:**  
**Keywords:**  

**Content:**  


---
