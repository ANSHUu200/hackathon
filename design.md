# AI Cloud Deployment Advisor — Design

## System Overview

The system behaves as an AI decision layer placed before deployment.

Input → Interpretation → Decision → Explanation

Instead of calculating cost after deployment, the system prevents bad deployment decisions.

---

## Components

### 1. Input Layer
Receives workload configuration from user dashboard.

### 2. Analysis Layer
Classifies workload type using reasoning:
- API service
- Batch processing
- Burst traffic
- Long running compute

### 3. Cost Engine
Calculates pricing across:
- AWS
- Azure
- GCP

Generates daily, monthly, yearly cost projections.

### 4. Decision Engine
Selects optimal provider and configuration.

### 5. Optimization Engine
Suggests:
- Memory right-sizing
- Region selection
- Service type change

### 6. Explanation Generator
Provides human-readable reasoning.

---

## Why This Is Buildable in Hackathon

• Uses static pricing dataset  
• Heuristic AI reasoning (no training required)  
• Modular REST architecture  
• Works without real cloud credentials
