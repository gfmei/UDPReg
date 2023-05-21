## Unsupervised Deep Probabilistic Approach for Partial Point Cloud Registration

The repository offers the official implementation of our paper in PyTorch.

:t-rex:News(March 4, 2023)!  **Our paper is accepted by CVPR2023!** **We will release our all code soon!!!**

### Abstract
Deep point cloud registration methods face challenges to partial overlaps and rely on labeled data.To address these issues, we propose UDPReg, an unsupervised deep probabilistic registration framework for point clouds with partial overlaps. Specifically, we first adopt a network to learn posterior probability distributions of Gaussian mixture models (GMMs) from point clouds. To handle partial point cloud registration, we apply the Sinkhorn algorithm to predict the distribution-level correspondences under the constraint of the mixing weights of GMMs. To enable unsupervised learning, we design three distribution consistency-based losses: self-consistency, cross-consistency, and local contrastive. The self-consistency loss is formulated by encouraging GMMs in Euclidean and feature spaces to share identical posterior distributions. The cross-consistency loss derives from the fact that the points of two partially overlapping point clouds  belonging to the same clusters share the cluster centroids. The cross-consistency loss allows the network to flexibly learn a transformation-invariant posterior distribution of two aligned point clouds. 
The local contrastive loss facilitates the network to extract discriminative local features. Our UDPReg achieves state-of-the-art performance on the 3DMatch/3DLoMatch and ModelNet/ModelLoNet benchmarks.

### Citation

If you take use of our code or feel our paper is useful for you, please cite our papers:

```
@article{mei2023unsupervised,
    author    = {Guofeng Mei and Hao Tang and Xiaoshui Huang and Weijie Wang and Juan Liu and Jian Zhang and Luc Van Gool and Qiang Wu},
    title     = {Unsupervised Deep Probabilistic Approach for Partial Point Cloud Registration},
    journal   = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    year      = {2023}
}
```

If you have any questions, please contact me without hesitation (gfmeiwhu@outlook.com or liu_juan@bit.edu.cn).
