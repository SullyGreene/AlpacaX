<p align="center">
  <img src="https://raw.githubusercontent.com/SullyGreene/AlpacaX/refs/heads/main/Static/logo.png" alt="TinyAGI Logo">
</p>

## 📚 AlpacaX Dataset Documentation

The **AlpacaX** dataset is crafted specifically for integration with **TinyAGI**, utilizing an advanced form of the Alpaca methodology to enhance model responses with structured, contextually-aware, and logically sequenced data. Through its unique tagging and data format, AlpacaX empowers TinyAGI agents to handle complex tasks with improved reasoning and clarity in responses.

---

### 📝 Dataset Summary

AlpacaX organizes data into three core fields — **System**, **Request**, and **Response** — that guide TinyAGI models to deliver rich, insightful, and structured answers:

- **System**: Provides overarching guidance or contextual settings to align the model’s response style.
- **Request**: Captures the user’s instruction or question along with additional input details.
- **Response**: Contains the model’s structured response, crafted based on the system prompt and user’s request.

This structure encourages TinyAGI agents to approach queries step-by-step, fostering clear, context-sensitive responses in complex interactions.

### 🔖 Example Format

Each entry in the AlpacaX dataset follows a structured, standardized format:

```json
{
  "system": "<prompt>\n{system_prompt}\n</prompt>",
  "request": "<instruction>\n{instruction}\n</instruction>\n<input>\n{input_text}\n</input>",
  "response": "<output>\n{output}\n</output>"
}
```

#### Example Prompt Template

AlpacaX’s format ensures consistency across training samples, allowing TinyAGI to interpret and generate responses in a predictable structure:

```plaintext
<s><system>
{{ .system }}
</system>
<request>
{{ .request }}
</request>
<response>
{{ .response }}
</response></s>
```

### 📂 Dataset Structure

With three distinct fields, AlpacaX provides TinyAGI agents with a structured approach to interpret and respond to inputs effectively:

- **System**: Frames the model’s approach, setting the context for its reasoning and tone.
- **Request**: Contains the user’s instruction with supplementary input for depth.
- **Response**: The model’s output, crafted based on the information provided, aiming for clarity and relevance.

### 🚀 Usage in TinyAGI

AlpacaX’s integration into **TinyAGI** unlocks new possibilities for fine-tuning and evaluation within the AGI framework:

- **Fine-Tuning**: TinyAGI agents, trained on AlpacaX, gain enhanced abilities to deliver responses with structured depth and reflection, ideal for tasks requiring multi-step reasoning.
- **Evaluation**: AlpacaX serves as a benchmark for assessing TinyAGI’s capacity to handle structured prompts, evaluate complex instructions, and respond with well-rounded outputs.

### 🛠 Dataset Creation

The AlpacaX dataset was developed using a unique data structuring approach that allows TinyAGI agents to gain a deep understanding of context and logical flow. Each entry is formatted to promote clarity, making AlpacaX a robust choice for training TinyAGI models to handle intricate queries and nuanced contexts effectively.

---

### 📜 License

AlpacaX is distributed under the **Apache 2.0 License**, making it accessible for both academic and commercial use. This license supports open-source contributions to TinyAGI, allowing widespread adoption and further refinement of AlpacaX's structured approach within AI ecosystems.
