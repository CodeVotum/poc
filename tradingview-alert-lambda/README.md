# **SMA Crossover Strategy with AWS Lambda Integration (POC)**

This folder contains a **Proof of Concept (POC)** for integrating a TradingView Pine Script strategy with **AWS Lambda**. The POC demonstrates how trading signals generated from a Simple Moving Average (SMA) Crossover strategy can be automated and processed using serverless infrastructure.

---

## **Overview**

### **Pine Script Strategy**
- Implements an SMA crossover strategy:
    - **Buy Signal**: Triggered when the short SMA crosses above the long SMA.
    - **Sell Signal**: Triggered when the short SMA crosses below the long SMA.
- Utilizes TradingView's **webhook alerts** to send signals in real time as JSON payloads.

### **AWS Lambda Integration**
- Webhook alerts are sent to an **AWS API Gateway** endpoint.
- The API Gateway triggers an **AWS Lambda** function that:
    - Processes the trading signals.
---
