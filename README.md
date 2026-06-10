# API Load Testing Project

## Overview
This repository contains the performance engineering strategy used to validate API scalability, stability, resilience, and recovery capabilities.

## Test Scenarios

### 1. Baseline Load Test
- Goal: Validate support for 3 million requests/day
- Target: P95 <= 2 seconds
- Error Rate <= 0.5%

### 2. Performance Step Test
- Load progression: 100, 200, 400, 600, 800, 1000 req/s
- Goal: Identify performance degradation threshold

### 3. Stress Test
- Goal: Determine breaking point
- Monitor:
  - CPU > 90%
  - Heap > 80%
  - HTTP 5xx
  - Timeouts

### 4. Recovery Test
- Goal: Validate application recovery after stress
- Target: Return to P95 <= 2 seconds

## Monitoring
- Grafana
- Kibana
- Elasticsearch
- Kafka

## Tools
- Apache JMeter
- Grafana
- Kibana

## Deliverables
- JTL Results
- Performance Metrics
- Throughput Charts
- Error Analysis
- Executive Report
