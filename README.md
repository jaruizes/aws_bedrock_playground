# 🚀 AWS Generative AI Developer Professional - Practical Cookbook

This repository is a comprehensive collection of practical implementations, design patterns, and real-world use cases using **Amazon Bedrock** and the AWS Generative AI ecosystem.

The content is strictly aligned with the exam domains of the **AWS Certified Generative AI Developer - Professional** certification, covering everything from basic model invocation to complex Agent architectures and advanced RAG.

---

## 📂 Repository Structure

The project is organized into progressive modules:

### 1. Invocation & Fundamentals (`/01-invocation`)
* **InvokeModel API**: Handling model-specific payloads (JSON) for Anthropic Claude, Meta Llama, and Amazon Nova.
* **Converse API**: Implementing the unified Bedrock interface for maximum code portability.
* **Streaming Responses**: Implementing real-time "typing" effects for better UX using `ConverseStream`.
* **Multimodal Prompts**: Processing images and documents (PDF/Docx) directly within the prompt.

### 2. Security & Governance (`/02-guardrails`)
* **Content Filtering**: Configuring thresholds for hate, violence, and sexual content.
* **PII Masking**: Automatic detection and redaction of sensitive data (Emails, SSNs, Phone numbers).
* **Denied Topics**: Restricting specific conversation themes using custom word filters.
* **Contextual Grounding**: Detecting hallucinations by validating model responses against source data.



### 3. Advanced RAG & Knowledge Bases (`/03-rag-knowledge-bases`)
* **Data Ingestion**: Pipeline from S3 to Vector Engine (OpenSearch Serverless).
* **Chunking Strategies**:
    * Fixed-size vs. Hierarchical chunking.
    * **Semantic Chunking**: Splitting text based on meaningful coherence rather than character count.
* **Advanced Retrieval**: Implementing metadata filtering and re-ranking for higher precision.



### 4. Prompt Management (`/04-prompt-management`)
* **Bedrock Prompt Management**: Deploying prompt variants and managing lifecycle versions (Live/Draft).
* **Prompt Engineering**: Examples of *Chain-of-Thought*, *Few-Shot*, and *System Prompting* techniques.

### 5. Efficiency & Performance (`/05-performance`)
* **Semantic Cache**: Implementing a vector cache to reduce latency and costs using Amazon Titan Embeddings.
* **Batch Inference**: Efficiently processing large datasets asynchronously.
* **Provisioned Throughput**: Invoking models using reserved capacity for high-demand applications.



### 6. Agentes & Tool Use (`/06-agents`)
* **Tool Use (Function Calling)**: Enabling models to interact with external APIs autonomously.
* **Agents for Amazon Bedrock**: Full agent configuration with Lambda Action Groups and session memory.

### 7. Model Evaluation (`/07-evaluation`)
* **Automated Evaluation**: Running evaluation jobs for metrics like Accuracy, Robustness, and Toxicity.
* **Human-in-the-loop**: Integrating with Amazon SageMaker Ground Truth for human-based scoring.

---

## 🛠️ Prerequisites

1.  **AWS Account** with model access granted in Amazon Bedrock (Nova, Claude, Titan).
2.  **Python 3.9+**.
3.  **AWS CLI** configured with appropriate IAM permissions.
4.  **Boto3 1.34.x+** (Ensure you have the latest version for Amazon Nova support).

---

## 🚀 Getting Started

1.  **Clone the repo**:
    ```bash
    git clone [https://github.com/your-user/aws-genai-pro-cookbook.git](https://github.com/your-user/aws-genai-pro-cookbook.git)
    cd aws-genai-pro-cookbook
    ```

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run an example**:
    ```bash
    python 01-invocation/converse_api_basic.py
    ```

---

## 🎓 Certification Resources
* [Official Exam Guide (AWS)](https://aws.amazon.com/certification/certified-generative-ai-developer-professional/)
* [Amazon Bedrock Documentation](https://docs.aws.amazon.com/bedrock/)
* [AWS Bedrock Samples GitHub](https://github.com/aws-samples/amazon-bedrock-samples)

---

## 📝 License
This project is licensed under the MIT License.
