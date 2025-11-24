# 💡 Which Model Should I Run?

This guide summarizes the key differences between **unsloth/gpt-oss-20b** (an optimized MoE model) and **Mistral 7B** (a highly efficient dense model) to help you choose the best fit for your Linode deployment.

---

## 🔬 Core Architecture and Performance

| Feature | Mistral 7B (Dense) | unsloth/gpt-oss-20b (MoE) |
| :--- | :--- | :--- |
| **Total Parameters** | ~7.3 Billion | ~21 Billion |
| **Active Parameters** | ~7.3 Billion (Dense: all parameters active) | **~3.6 Billion** (MoE: only a fraction active per token) |
| **Inference Speed (General)** | **Extremely Fast** (High tokens/sec) | Fast (Efficient decode, but MoE routing adds overhead) |
| **Primary VRAM Need** | **Very Low** (Can run on minimal VRAM/RAM for its performance class) | Low/Moderate (Requires ~16GB of VRAM/RAM for efficient running) |
| **Max Context Window** | Up to **32K** tokens | Up to **131K** tokens |

---

## 🧠 Reasoning & Capability

| Capability | Mistral 7B (Dense) | unsloth/gpt-oss-20b (MoE) |
| :--- | :--- | :--- |
| **Reasoning Depth** | Strong for its size, but limited on highly complex, multi-step problems. | **Superior.** Deliberately trained for complex reasoning and agentic tasks. |
| **Agentic Features** | Generally requires external frameworks (e.g., LangChain) for tool-use/function calling. | **Native Tool Use.** Built-in support for function calling, web browsing, and code execution. |
| **Customization** | Excellent model for general-purpose fine-tuning (e.g., QLoRA). | Excellent for agent-style fine-tuning, but requires the specific **Harmony response format** for best results. |
| **Adjustable Effort** | No. | **Yes** (Low, Medium, High). You can trade latency for reasoning performance via prompting. |

---

## 🎯 Which Model Should I Run?

The choice depends entirely on your project's **priorities for performance vs. complexity**.

### Choose **Mistral 7B** if:

* **You need Speed and Low Cost:** Your application is **latency-critical** (e.g., real-time chat, quick suggestions) and must be as fast as possible.
* **You are resource-constrained:** You are targeting the **cheapest Linode instance** possible and need the most performance for the least VRAM/RAM.
* **Your tasks are general:** You focus on high-quality text generation, summarization, or simple question-answering.

### Choose **unsloth/gpt-oss-20b** if:

* **You need Deep Reasoning & Logic:** Your application requires **complex problem-solving**, code generation, or financial/mathematical analysis.
* **You are building an Agent:** You need **native support for tool-calling** (function calling, web search) or full **Chain-of-Thought (CoT)** outputs for debugging.
* **You need a Massive Context:** Your workflow deals with very long documents or threads (up to 131K tokens).
* **You have a budget for a slightly larger Linode** (e.g., 16GB VRAM/RAM minimum for optimal performance).