# 🧪 Testing & Validation Guide

This document outlines the testing methodology used to verify the integrity, security, and self-healing capabilities of this DevSecOps/GitOps pipeline.

## 1. Local Image Validation
Verify the container builds and runs locally before pushing.
```bash
docker build -t telemetry-backend:test ./app
docker run -p 8080:3000 telemetry-backend:test