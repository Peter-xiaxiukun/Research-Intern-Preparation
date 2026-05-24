# Unanswered Questions

This file records questions that appear during reading and research preparation.


---

## Questions

-  **Which communication structure is currently mainstream in LLM-based multi-agent systems: layered, decentralized, centralized, shared message pool, or something else?**  
  I want to understand the current mainstream communication structure and compare the strengths and weaknesses of layered, decentralized, centralized, and shared-message-pool communication. I also want to know whether recent systems have moved beyond these categories or mainly combine them in hybrid forms.

-  **Is natural language still the dominant communication context in current LLM-based multi-agent systems?**  
  Some modern audio and image generation models are not purely text-based. I want to clarify whether LLM-based multi-agent systems still mainly rely on textual communication, or whether multimodal communication contexts are becoming common in agent-agent interaction.

-  **How is capabilities acquisition implemented in LLM-based multi-agent systems if the model parameters are usually fixed?**  
  My current guess is that since the parameters of LLMs are not easily changed during multi-agent interaction, capabilities acquisition may mainly happen through prompt design, role assignment, tool use, memory, retrieval, external feedback, or coordination among agents rather than direct parameter updates. I need to verify whether this understanding is correct.

-  **Does Paper 2’s communication taxonomy cover all effective communication designs in current LLM-MAS research?**  
  Paper 2 describes communication in LLM-based multi-agent systems through seven aspects: architecture, goal, protocol, strategy, paradigm, object, and content. I want to clarify whether this taxonomy covers all effective communication designs, or whether there are other important mechanisms not captured by these categories, such as adaptive topology, memory sharing, communication cost control, uncertainty expression, tool-mediated communication, or evaluation-driven communication optimization.

  - **How should I fairly evaluate memory systems when raw context is much more information-rich but much more expensive?**  
  Raw data may provide the strongest information baseline, while memory systems trade information completeness for efficiency. I need to decide how to compare accuracy, token usage, API calls, runtime, and memory usefulness without unfairly favoring either full-context input or compressed memory.

- **Can offline memory update hurt performance by merging, deleting, or rewriting useful information?**  
  LightMem’s offline update may improve memory organization, but it may also introduce harmful changes. I need to examine correct → wrong cases after offline update and identify whether they are caused by over-merging, mistaken deletion, over-generalization, or retrieval changes.

- **What is the real-time limitation of buffer-based memory systems like LightMem?**  
  LightMem delays some memory processing through sensory and short-term buffers. I need to clarify whether this creates problems for turn-level freshness, especially when recent information has not yet entered LTM. I also need to distinguish session-level incremental evaluation from true turn-level real-time dialogue evaluation.

- **Should multi-agent memory be shared, individual, hierarchical, role-specific, or hybrid?**  
  Different memory topologies may produce different collaboration behaviors. I need to understand when shared memory helps coordination, when individual memory preserves specialization, when role-specific memory is better, and when shared memory may cause groupthink or error propagation.

- **How can we evaluate whether memory improves collaboration rather than merely increasing available context?**  
  In LLM-MAS, memory may improve performance simply by adding more information to the prompt. I need to design or find evaluations that distinguish genuine memory-enabled collaboration from more tokens, stronger retrieval, longer context, or repeated sampling.

- **Can multi-agent mechanisms reduce self-reinforcing errors in reflective memory?**  
  Reflective memory can turn wrong conclusions into persistent future bias. I suspect that separating memory generation, verification, contradiction checking, and update control across different agents may reduce this risk. I need to check whether existing multi-agent reflexion or memory governance work has already solved this problem.

- **Are graph-structured memories more suitable for reasoning than hierarchical memories?**  
  A-Mem’s network-like structure seems reasoning-friendly because an agent can traverse related memories and perform multi-hop associative retrieval. However, graph memory may also amplify false links or irrelevant associations. I need to compare graph memory, hierarchy-based memory, and hybrid memory in terms of reasoning support, retrieval control, and error propagation.

- **Can xMemory-style hierarchical grouping handle memory components that belong to multiple semantic groups?**  
  A memory component may simultaneously relate to several topics, such as API usage, authentication failure, debugging strategy, and parameter behavior. I need to understand whether strict hierarchy causes retrieval misses, and whether multi-parent references, soft assignment, cross-links, or hybrid graph-hierarchy structures are better.
