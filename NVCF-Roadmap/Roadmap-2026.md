# NVCF Open Source Roadmap

Welcome to the **NVIDIA Cloud Functions Open Source Roadmap** — a high-level overview of our current priorities, ongoing initiatives, and upcoming features. This page highlights the major themes, features, and improvements we're planning across upcoming development cycles.

The roadmap is organized by **quarters** (Q1, Q2, etc.) to give a snapshot of development focus and progress throughout the year.

As development evolves, we'll keep this roadmap up to date. Community feedback plays a big part in shaping what we build, so feel free to contribute ideas, open discussions, or share suggestions.

---

## Q1 2026 (January – March)

**Open Source NVIDIA Cloud Functions Components**  
Open source release of core building blocks for self-hosted deployments. Components include:

- **NVCF Go (Kaizen Go Framework)** — Go framework used by control-plane services.
- **byoo-otel-collector (BYOO OTel Collector)** — BYO Observability OpenTelemetry Collector.
- **NATS Auth Callout** — NATS client authentication and authorization service.
- **Container Cache** — Accelerates Function deployment by caching deployed containers.
- **Proxy Cache** — Proxy layer that caches S3 objects, NGC assets, and HuggingFace models via DNS-based MITM.
- **NVCF Invocation Service** - REST based stateless function invocation service
- **NVCF Autoscaler Service** — Prediction/Forecast based instance autoscaling service.
- **NVCA Operator & NVCA** - NVCF Cluster Agent performs the registration of the cluster and deployment orchestration in-cluster.
- **NVCF Rate Limiter** — Per‑function rate‑limiting service that throttles requests to a function.
- **NVCF gRPC Proxy** — Stateful function invocation service used for bi‑directional communication and state management.
- **NVCF ReVal / Helm ReVal** — Helm chart validation service that renders Helm charts with dynamic data.


---