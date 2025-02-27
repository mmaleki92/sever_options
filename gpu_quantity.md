# HPE DL380 Gen10 GPU Installation Parts List

To install 2× Tesla P40 and 1× Tesla T4 GPUs in your HPE DL380 Gen10 server, you'll need the following specific parts:

## Required Parts List with Part Numbers

| Component | Part Number | Quantity | Description | Purpose |
|-----------|-------------|----------|-------------|---------|
| **Tesla P40** | Q0V79A or P4R09A | 2 | NVIDIA Tesla P40 24GB PCIe GPU | Deep learning training |
| **Tesla T4** | Q1K38A | 1 | NVIDIA Tesla T4 16GB PCIe GPU | Inference workloads |
| **GPU Enablement Kit** | 826703-B21 | 1 | HPE DL380 Gen10 GPU Enablement Kit | Required for GPU installation |
| **High Performance Fan Kit** | 826706-B21 | 1 | HPE DL380 Gen10 High Perf Fan Kit | Enhanced cooling for GPUs |
| **GPU Power Cable** | 873558-B21 | 3 | HPE GPU Cable Kit | Power connection for GPUs |

## Server Base Requirements

purchasing these required components:

| Component | Part Number | Quantity | Notes |
|-----------|-------------|----------|-------|
| **Dual Power Supplies** | 865414-B21 | 2 | 800W Platinum Hot-Plug (minimum) |
| **PCIe Riser** | 826975-B21 | 1 | PCIe Riser Kit (if not included) |


## Single-Width GPU Memory Comparison

All the single-width GPUs available for your server have professional-grade memory:

| GPU Model | Form Factor | Memory Capacity | Use Case |
|-----------|-------------|----------------|----------|
| Tesla P40 | Single-width | **24GB GDDR5** | AI training, batch processing |
| Tesla T4 | Single-width | **16GB GDDR6** | Inference, small model training |
| Tesla P4 | Single-width | **8GB GDDR5** | Entry-level inference |
| Tesla V100S | Single-width | **32GB HBM2** | High-end training (not in your list) |

## Required Installation Parts

| Component | Part Number | Quantity | Purpose |
|-----------|-------------|----------|---------|
| GPU Enablement Kit | 826703-B21 | 1 | Required for GPU installation |
| High Performance Fan Kit | 826706-B21 | 1 | Enhanced cooling for GPUs |
| GPU Power Cables | 873558-B21 | 3 | Power connections (1 per GPU) |

## Final Configuration Notes

1. **Power Calculation**:
   - 2× Tesla P40: 500W (250W each)
   - 1× Tesla T4: 70W
   - System base: ~300W
   - Total: ~870W (well within dual 800W PSUs)

2. **Performance Profile**:
   - Deep learning training: 2× P40 with 48GB combined memory
   - Inference workloads: 1× T4 with 16GB memory
   - Maximum batch size for transformer models: Up to 24GB per GPU

3. **Assembly Sequence**:
   - Install GPU Enablement Kit first
   - Replace standard fans with high-performance fans
   - Install largest GPUs (P40s) first, then smaller GPUs (T4)
   - Connect all power cables before powering on

This configuration gives you excellent capacity for both training and inference workloads, with sufficient memory on each GPU for most AI applications.