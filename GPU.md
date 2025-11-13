# 🎮 GPU Instances on Akamai Cloud

Akamai Cloud offers powerful GPU instances equipped with NVIDIA GPUs to accelerate your AI, machine learning, and compute-intensive workloads. This page provides detailed information about available GPU types, specifications, and use cases.

## GPU Types

Akamai Cloud currently offers three types of NVIDIA GPUs:

- **NVIDIA RTX Pro 6000 Blackwell** - High-performance GPU for demanding AI, scientific, and design workloads
- **NVIDIA RTX 4000 Ada** - Optimized for lightweight AI inference and media workloads
- **NVIDIA Quadro RTX 6000** - Designed for deep learning and data science price-performance


## GPU Specifications


### NVIDIA RTX Pro 6000 Blackwell

The RTX Pro 6000 Blackwell GPU is a high-performance GPU designed for demanding AI, scientific, and design workloads, featuring:

- **GPU Memory (VRAM)**: 96 GB GDDR7 with ECC
- **CUDA Cores**: 24,064 (Parallel-Processing)
- **Tensor Cores**: 5th-generation Tensor Cores
- **RT Cores**: 4th-generation RT Cores
- **Memory Technology**: GDDR7 with Error Correction Code (ECC)

**Best for**: Large-scale AI model training, scientific computing, professional design workloads, high-performance computing

### NVIDIA RTX 4000 Ada

The RTX 4000 Ada GPU is built for media workloads and AI inference, featuring:

- **GPU Memory (VRAM)**: 20 GB GDDR6
- **CUDA Cores**: 6,144 (Parallel-Processing)
- **Tensor Cores**: 192 (Transcoding)
- **RT Cores**: 48 (Ray Tracing)
- **FP32 Performance**: 26.7 TFLOPS
- **Media Encoding**: 2x encoding, 2x decoding, and 1x AV1 encode/decode engines per card
- **Performance**: Up to 25x faster media encoding performance

**Best for**: Lightweight AI inference, media encoding/decoding, video processing

### NVIDIA Quadro RTX 6000

The Quadro RTX 6000 GPU is optimized for deep learning and data science workloads:

- **GPU Memory (VRAM)**: 24 GB GDDR6
- **CUDA Cores**: 4,608 (Parallel-Processing)
- **Tensor Cores**: 576 (Transcoding)
- **RT Cores**: 72 (Ray Tracing)
- **FP32 Performance**: 16.3 TFLOPS

**Best for**: Deep learning model training, data science, complex AI workloads


For performance benchmarks and analysis, see the [Benchmarking NVIDIA RTX Pro 6000 Blackwell](https://www.akamai.com/blog/cloud/benchmarking-nvidia-rtx-pro-6000-blackwell-akamai-cloud) blog post.

For more detailed specifications, refer to the [GPU Compute Instances Documentation](https://techdocs.akamai.com/cloud-computing/docs/gpu-compute-instances#gpu-specifications).

## GPU Use Cases

GPUs are designed to process large blocks of data in parallel, making them excellent for compute-intensive tasks that require thousands of simultaneous threads. Common use cases include:

### Machine Learning and AI

- Building prediction algorithms and recommendation systems
- Training and deploying deep learning models
- AI inference workloads with low latency requirements
- Natural language processing (NLP) tasks
- Computer vision applications

### Big Data Analysis

- Analyzing and extracting insights from large and complex data sets
- Parallel data processing and transformation
- Real-time analytics and stream processing

### Video Encoding and Media Processing

- Converting video files to different formats efficiently
- Real-time video transcoding and streaming
- Media encoding/decoding workloads
- Content delivery optimization

### General Purpose Computing (GPGPU)

- Writing code in C, C++, Python, or other supported languages to utilize GPU power
- CUDA-accelerated applications
- Parallel computing tasks

### Graphics Processing

- Ray tracing and 3D rendering
- Graphics simulations and visualizations
- CAD and design applications
- Scientific visualization

For more information on GPU use cases, refer to the [GPU Compute Instances Documentation](https://techdocs.akamai.com/cloud-computing/docs/gpu-compute-instances#gpu-use-cases).

## Key Features

- **Dedicated GPU Resources**: 100% allocated GPU and CPU resources for predictable performance
- **On-Demand Deployment**: Deploy GPUs when needed, starting at $0.52 per hour
- **Predictable Pricing**: Low, transparent pricing without contracts or hidden costs
- **Low Egress Costs**: Save up to 90% on egress with Akamai Cloud ($0.005 per GB in most regions)
- **Flexible Management**: Manage infrastructure with UI, API, CLI, and developer tool integrations
- **Full Documentation**: Access comprehensive documentation and support for NVIDIA CUDA toolkit installation

## Performance Benchmarks

### NVIDIA RTX Pro 6000 Blackwell Performance

According to benchmarking on Akamai Cloud, the NVIDIA RTX Pro 6000 Blackwell delivers exceptional performance for AI inference workloads:

- **Inference Throughput**: Up to **1.63× higher inference throughput** compared to the NVIDIA H100
- **Performance Metrics**: Achieves **24,240 transactions per second (TPS)** per server at 100 concurrent requests
- **FP4 Precision Mode**: Offers exceptional throughput at reduced power and cost, making it ideal for distributed environments
- **Multimodal Capabilities**: Supports concurrent and multimodal workloads including text, vision, and speech processing on a single unit, reducing the need for specialized accelerators and minimizing data movement across the network

The RTX Pro 6000 Blackwell is particularly well-suited for high-performance AI inference workloads where throughput and efficiency are critical. Its large 96 GB memory capacity and advanced architecture make it ideal for running large language models and complex AI applications.

For detailed benchmarking results and analysis, see the [Benchmarking NVIDIA RTX Pro 6000 Blackwell](https://www.akamai.com/blog/cloud/benchmarking-nvidia-rtx-pro-6000-blackwell-akamai-cloud) blog post.

### Media Workloads: VPUs vs GPUs

For media encoding workloads, Akamai Cloud also offers NETINT Video Processing Units (VPUs) as an alternative to GPUs. According to recent benchmarking:

- **Energy Efficiency**: VPUs demonstrated **4.7x higher energy efficiency** compared to GPUs in demanding media workloads
- **Performance**: VPUs outperformed GPUs in some high-resolution scenarios (e.g., 19 simultaneous 1080p jobs vs 16 for GPUs)
- **Power Consumption**: VPUs use significantly less power (7-13 watts vs 51-82 watts for GPUs)
- **Cost Savings**: For 1,000 year-long 1080p streams, VPUs can reduce annual energy consumption from 32 MWh to 5.5 MWh—approximately **80% energy savings** and around 12.6 tonnes of CO₂ emissions reduction per year

VPUs are particularly well-suited for video encoding, transcoding, and media processing workloads where energy efficiency is a priority. GPUs remain excellent for AI inference, machine learning, and other parallel computing tasks.

For detailed benchmarking results and VMAF quality scores, see the [Benchmarking VPUs and GPUs for Media Workloads](https://www.linode.com/blog/compute/benchmarking-vpus-and-gpus-for-media-workloads/) blog post.

## Resources

- **[Akamai Cloud GPU Product Page](https://www.linode.com/products/gpu/)** - Overview of GPU offerings and pricing
- **[GPU Compute Instances Documentation](https://techdocs.akamai.com/cloud-computing/docs/gpu-compute-instances)** - Comprehensive technical documentation
- **[Benchmarking VPUs and GPUs for Media Workloads](https://www.linode.com/blog/compute/benchmarking-vpus-and-gpus-for-media-workloads/)** - Performance comparison and energy efficiency analysis
- **[Benchmarking NVIDIA RTX Pro 6000 Blackwell](https://www.akamai.com/blog/cloud/benchmarking-nvidia-rtx-pro-6000-blackwell-akamai-cloud)** - Performance benchmarks and analysis

## Getting Started

1. Review the [GPU Compute Instances Documentation](https://techdocs.akamai.com/cloud-computing/docs/gpu-compute-instances) for setup instructions
2. Choose the appropriate GPU type based on your workload requirements
3. Deploy a GPU instance through the Linode Cloud Manager
4. Install the NVIDIA CUDA toolkit to begin development

For questions or support, visit the [Linode Community](https://www.linode.com/community/questions/) or [Documentation](https://www.linode.com/docs/).

