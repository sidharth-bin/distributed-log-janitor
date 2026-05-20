# 🧹 Distributed Log Janitor & Stream Optimizer

A production-grade, zero-dependency data optimization engine engineered to intercept, filter, and condense uncompressed application log arrays within distributed microservice topologies. 

This utility dynamically strips repetitive infrastructure telemetry noise (e.g., polling check-ins, debugging outputs) before long-term storage ingestion, directly cutting enterprise cloud logging bills without omitting mission-critical runtime system alerts.

---

## 💡 System Blueprint: The Three Ws

### 1. WHEN to use this tool?
*   **High-Volume Ingress Refactoring:** When applications produce gigabytes of chatty infrastructure telemetry lines that threaten to inflate logging budgets.
*   **Pre-Archive Maintenance Tasks:** Run this optimization loop before transferring raw application logs into cold storage solutions (like AWS S3 Glacier or Google Cloud Storage).
*   **Container Sidecar Operations:** Deploy this process as an isolated, lightweight helper inside container nodes to sanitize stream data cleanly before shipping logs to centralized analysis arrays.

### 2. WHERE does it run?
*   **Universal Platforms:** Built with strict zero-dependency runtime rules, this module operates perfectly on minimal container hosts, standalone Linux cloud instances, or native continuous build workers.

### 3. WHY use this over other solutions?
*   **Zero Architectural Overhead:** It implements low-overhead stream evaluations without requiring extensive third-party logging agent configurations or high CPU runtimes.

---

## ✨ Architectural Differentiators

*   **Isolated String Analysis Filters:** Employs precise block arrays that prevent data drops by isolating noise signatures without touching active application exception messages.
*   **Real-Time Data Metric Pipelines:** Compiles clear performance statistics to provide immediate operational visibility into data reduction and infrastructure savings.

---

## 📋 Prerequisites

*   **Runtime Footprint:** Standard Python 3.8 or higher system execution space.
*   **Dependencies:** None. Built cleanly with core platform utilities (`os`, `sys`, `json`, `time`) to ensure instant operability across diverse server topologies.

---

## 🔧 Tailoring to Your Infrastructure

To adapt the processing engine to catch custom internal tracing keywords, append your unique patterns inside the initializer block:

```python
# Modify or add target phrases within janitor.py to fit unique pipeline data structures
self.noise_signatures = ["DEBUG", "HEARTBEAT", "CUSTOM_NOISE_KEYWORD"]
