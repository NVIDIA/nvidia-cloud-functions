# NVCF Open Source Roadmap

Welcome to the **NVIDIA Cloud Functions Open Source Roadmap** — a high-level overview of our current priorities, ongoing initiatives, and upcoming features. This page highlights the major themes, features, and improvements we're planning across upcoming development cycles.

The roadmap is organized by **quarters** (Q1, Q2, etc.) to give a snapshot of development focus and progress throughout the year.

As development evolves, we'll keep this roadmap up to date. Community feedback plays a big part in shaping what we build, so feel free to contribute ideas, open discussions, or share suggestions.

## Overview

The following outlines the **themes** driving each quarter's roadmap — the strategic focus areas that shape our priorities and feature work.

**Q1 2026 (January – March)**  
Themes: Advanced Scheduling, Self-Hosted MVP, Open Source NVIDIA Cloud Functions Components — Phase 1

**Q2 2026 (April – June)**  
Themes: Self-hosted Multi-cluster, Self-hosted Tasks, High Performance Storage

---

## Q1 2026 (January – March)

**1. Helm Functions**  
Enable secure deployment and management of Helm charts as functions.

**2. Optional Helm Function restriction**  
Enable customizable, cluster-specific security policies and custom Kubernetes API allowances for validating Helm charts prior to deployment.

**3. Support Dynamo Operator**  
Enable Dynamo operator deployment in NVIDIA Cloud Functions clusters.

**4. Support KAI Scheduler**  
Support NVIDIA KAI Scheduler in NVIDIA Cloud Functions Cluster allowing workloads to use the scheduler, maximizing cluster resource utilization through advanced GPU bin-packing and network topology-aware scheduling.

**5. Degraded Function State**  
Provide accurate visibility into workload health by exposing a "Degraded" status for functions that are actively failing health checks.

**6. Autoscaler in Self-Hosted platform**  
Adds autoscaler support so self-hosted customers can scale function replicas up and down.

**7. Autoscaling Customizalibility**  
Provide customers with comprehensive control over their autoscaling logic by allowing them to configure custom scale-up and scale-down thresholds, adjust auto-shutoff times, and select specific system or user-provided metrics to drive scaling actions

**8. Decouple Control Plane/GPU Cluster Configuration**  
Enables a single control plane to register and manage multiple GPU clusters. Operators can add, remove, or update GPU clusters without reconfiguring or redeploying the control plane, keeping control plane settings separate from GPU cluster settings.

**9. FluentBit support for BYOO [Beta]**  
Enhances Bring Your Own Observability (BYOO) by automatically extracting and routing container stdout and stderr logs to designated telemetry endpoint, eliminating the need for developers to manually export OTLP logs from their applications

**10. Open Source NVIDIA Cloud Functions Components — Phase 1**  
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

## Q2 2026 (April – June)

**1. Support Multi-Cluster Installation Path**  
Supports a multi-cluster installation path by integrating the decoupled control plane and GPU cluster model into Helmfile.

**2. NVCF Tasks**  
Brings Tasks support to self-hosted platform. Enables the task workflows and capabilities for self-hosted deployments.

**3. Support user-defined CPU and memory in instance types**  
Allows users to define CPU and memory for instance types instead of relying only on predefined shapes.

**4. Automated function profiling via NSight**  
Enables automated function profiling using Nsight tooling. Helps developers analyze and optimize NVCF function performance.

**5. Support High Performance Multi-Node Storage**  
Enables integration with high-performance multi-node file systems so customers can bring their own storage.

---
