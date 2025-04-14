# 📘 Event-Driven Agentic Document Workflows

## 🧭 Course Overview

**Event-Driven Agentic Document Workflows** is a hands-on course created in collaboration with **LlamaIndex** and taught by **Laurie Voss**. It teaches developers how to build intelligent, asynchronous document processing agents using **event-driven architectures** powered by **Retrieval-Augmented Generation (RAG)**.

### 🎯 Key Objectives

- Build modular, asynchronous workflows using LlamaIndex.
- Parse and extract data from complex documents (e.g., resumes, forms).
- Use RAG to semantically answer questions about documents.
- Automate form-filling tasks based on document content.
- Incorporate **human-in-the-loop** feedback via text or voice.
- Extend workflows to support **branching, looping**, and **concurrent execution**.


## 📚 Course Content

### 1. [**Introduction to Agentic Document Workflows**](#)
- What is RAG and why it matters
- Limitations of LLMs and how RAG complements them
- Role of agents and event-based workflows in intelligent automation

### 2. [**Building a Workflow**](./L2-Building-Wrokflow)
- Define workflows using `@step` and `Event` classes
- Support for branching, loops, concurrent execution, and streaming
- Visualize flows with `draw_all_possible_flows()`

### 3. [**Adding RAG**](./L3-Adding-RAG)
- Parse resumes using LlamaParse
- Embed documents using `VectorStoreIndex`
- Set up RAG-powered query engines and wrap them into tools/agents

### 4. [**Form Parsing**](./L4-Form-Parsing)
- Extract form fields with LlamaParse and LLM
- Convert fields to questions and answer them using RAG
- Handle multiple field queries concurrently
- Aggregate results to auto-fill forms

### 5. [**Human in the Loop**](./L5-Human-in-the-Loop)
- Insert feedback points using `InputRequiredEvent` and `HumanResponseEvent`
- Re-trigger field-level RAG based on feedback
- Append feedback to questions for contextual improvements

### 6. [**Use Your Voice**](./L6-Use-Your-Voice)
- Capture voice feedback via **Gradio**
- Transcribe audio using **OpenAI Whisper**
- Integrate voice into the human-feedback loop for agents


## 📓 Notebooks

| Notebook | Description |
|---------|-------------|
| [L2-Building-Workflow](./L2-Building-Wrokflow) | Learn to create event-based workflows with branching, looping, and concurrent tasks. |
| [L3-Adding-RAG](./L3-Adding-RAG) | Integrate RAG into workflows using parsed documents and vector search. |
| [L4-Form-Parsing](./L4-Form-Parsing) | Parse forms, generate field-specific questions, and automate responses. |
| [L5-Human-in-the-Loop](./L5-Human-in-the-Loop) | Add a feedback loop using human-in-the-loop responses for refinement. |
| [L6-Use-Your-Voice](./L6-Use-Your-Voice) | Enable voice feedback using Gradio and OpenAI Whisper. |


## 🚀 Getting Started

### 1. **Clone the Repository**

```bash
git clone <your-repo-url>
cd event-driven-agentic-docs
```

### 2. **Install Requirements**

```bash
pip install -r requirements.txt
```

### 3. **Add API Keys**

Create a `.env` file in the root directory with:

```env
OPENAI_API_KEY=your_openai_key
LLAMA_CLOUD_API_KEY=your_llamaindex_key
```

### 4. **Run Notebooks**

Launch Jupyter or any preferred environment:

```bash
jupyter notebook
```

Then open and run the notebooks cell by cell as instructed.


## 🔗 Resources and References

- 🌐 [Official Course Page](https://www.deeplearning.ai/short-courses/event-driven-agentic-document-workflows/)
- 📘 [LlamaIndex Documentation](https://docs.llamaindex.ai/)
- 🧠 [Blog: Agentic Document Workflows](https://www.llamaindex.ai/blog/introducing-agentic-document-workflows)
- 🧪 [LlamaIndex GitHub Examples](https://github.com/run-llama/llamacloud-demo/tree/main/examples/document_workflows)


## 🛠 Helpers & Utils

The `helper.py` file includes utility functions to support the notebooks:

- `get_openai_api_key()` / `get_llama_cloud_api_key()`: Loads API keys from `.env` file.
- `extract_html_content(filename)`: Loads and wraps HTML content for inline visualization.
- Used for workflow diagram rendering and secure credential loading.


Happy learning and building! 🎉