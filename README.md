# ViGNN-OTFS
Official PyTorch implementation of ViGNN-OTFS for graph-based automatic modulation classification in high-mobility OTFS systems.

## Overview

ViGNN-OTFS models the received delay-Doppler (DD) domain signal using non-overlapping patches and represents their spatial relationships through a **fixed directed K-nearest neighbor (K-NN) graph**.

Unlike dynamic feature-space graph construction, the proposed graph topology is determined by the spatial coordinates of the DD-domain patches. Therefore, the graph can be constructed once and reused during both training and inference.

The architecture employs **MRConv-based Grapher modules** for spatial feature aggregation and **feed-forward networks (FFNs)** for node-wise feature refinement.

## Key Features

- Automatic modulation classification for OTFS systems
- DD-domain patch-based signal representation
- Fixed spatial K-NN graph construction
- MRConv-based graph feature aggregation
- Absolute positional encoding
- Computationally efficient static graph topology
- Evaluation under high-mobility wireless channels
- Support for different OTFS frame dimensions and SNR conditions
