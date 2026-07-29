# Downloadable Mermaid Diagrams

This folder contains standalone Mermaid source files for the Enterprise RAG project. Each diagram has a clear title and a recommended export filename, so downloaded images are named for interview or recruiter use.

## Export Requirements

Install Mermaid CLI once:

```bash
npm install -g @mermaid-js/mermaid-cli
```

Export one diagram:

```bash
mmdc -i docs/diagrams/01_system_design_architecture.mmd -o docs/diagrams/images/system-design-architecture.png
```

Export as SVG instead of PNG:

```bash
mmdc -i docs/diagrams/01_system_design_architecture.mmd -o docs/diagrams/images/system-design-architecture.svg
```

## Diagram Catalog

| Diagram | Mermaid Source | Recommended Image Name |
|---|---|---|
| System Design Architecture | `01_system_design_architecture.mmd` | `system-design-architecture.png` |
| Code Flow Architecture | `02_code_flow_architecture.mmd` | `code-flow-architecture.png` |
| Request Lifecycle | `03_request_lifecycle.mmd` | `request-lifecycle.png` |
| LangGraph State Machine | `04_langgraph_state_machine.mmd` | `langgraph-state-machine.png` |
| RAG Retrieval Architecture | `05_rag_retrieval_architecture.mmd` | `rag-retrieval-architecture.png` |
| Text2SQL Approval Architecture | `06_text2sql_approval_architecture.mmd` | `text2sql-approval-architecture.png` |
| Security Architecture | `07_security_architecture.mmd` | `security-architecture.png` |
| Cache Architecture | `08_cache_architecture.mmd` | `cache-architecture.png` |
| Evaluation Architecture | `09_evaluation_architecture.mmd` | `evaluation-architecture.png` |
| Deployment Architecture | `10_deployment_architecture.mmd` | `deployment-architecture.png` |
| Document Ingestion Architecture | `11_document_ingestion_architecture.mmd` | `document-ingestion-architecture.png` |

## Export All Diagrams

PowerShell:

```powershell
New-Item -ItemType Directory -Force docs/diagrams/images | Out-Null
mmdc -i docs/diagrams/01_system_design_architecture.mmd -o docs/diagrams/images/system-design-architecture.png
mmdc -i docs/diagrams/02_code_flow_architecture.mmd -o docs/diagrams/images/code-flow-architecture.png
mmdc -i docs/diagrams/03_request_lifecycle.mmd -o docs/diagrams/images/request-lifecycle.png
mmdc -i docs/diagrams/04_langgraph_state_machine.mmd -o docs/diagrams/images/langgraph-state-machine.png
mmdc -i docs/diagrams/05_rag_retrieval_architecture.mmd -o docs/diagrams/images/rag-retrieval-architecture.png
mmdc -i docs/diagrams/06_text2sql_approval_architecture.mmd -o docs/diagrams/images/text2sql-approval-architecture.png
mmdc -i docs/diagrams/07_security_architecture.mmd -o docs/diagrams/images/security-architecture.png
mmdc -i docs/diagrams/08_cache_architecture.mmd -o docs/diagrams/images/cache-architecture.png
mmdc -i docs/diagrams/09_evaluation_architecture.mmd -o docs/diagrams/images/evaluation-architecture.png
mmdc -i docs/diagrams/10_deployment_architecture.mmd -o docs/diagrams/images/deployment-architecture.png
mmdc -i docs/diagrams/11_document_ingestion_architecture.mmd -o docs/diagrams/images/document-ingestion-architecture.png
```

Mermaid Live Editor:

1. Open `https://mermaid.live`.
2. Open a `.mmd` file from this folder.
3. Copy the Mermaid source into the editor.
4. Choose `Actions` -> `Download PNG` or `Download SVG`.
5. Rename the downloaded file using the recommended image name from the table.
