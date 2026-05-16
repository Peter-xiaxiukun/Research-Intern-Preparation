# Unanswered Questions

This file records questions that appear during reading and research preparation.

Rule:
- Normal text = unresolved
- ~~Strikethrough~~ = resolved
- **Bold** = important / worth revisiting

---

## Questions

- [2026-05-16] **What are the characteristics of the three agent profiling methods mentioned in Paper 1: pre-defined, model-generated, and data-derived?**  
  I want to understand the practical differences among these three profiling methods. Specifically, I need to clarify their advantages, limitations, typical use cases, and how they affect agent diversity, controllability, and realism in LLM-based multi-agent systems.

- [2026-05-16] **Which communication structure is currently mainstream in LLM-based multi-agent systems: layered, decentralized, centralized, shared message pool, or something else?**  
  I want to understand the current mainstream communication structure and compare the strengths and weaknesses of layered, decentralized, centralized, and shared-message-pool communication. I also want to know whether recent systems have moved beyond these categories or mainly combine them in hybrid forms.

- [2026-05-16] **Is natural language still the dominant communication context in current LLM-based multi-agent systems?**  
  Some modern audio and image generation models are not purely text-based. I want to clarify whether LLM-based multi-agent systems still mainly rely on textual communication, or whether multimodal communication contexts are becoming common in agent-agent interaction.

- [2026-05-16] **How is capabilities acquisition implemented in LLM-based multi-agent systems if the model parameters are usually fixed?**  
  My current guess is that since the parameters of LLMs are not easily changed during multi-agent interaction, capabilities acquisition may mainly happen through prompt design, role assignment, tool use, memory, retrieval, external feedback, or coordination among agents rather than direct parameter updates. I need to verify whether this understanding is correct.
---