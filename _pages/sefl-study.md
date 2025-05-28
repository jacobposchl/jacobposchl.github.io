---
title: "Self-Study"
permalink: /self-study/
layout: single
---

# Personal Knowledge Log

Welcome to my weekly brain-dump:

## Week of June 2, 2025 – Understanding the Jacobian in PyTorch Autograd
- **Summary:** vector‐Jacobian products, geometric interpretation  
- **Visuals:** ![Jacobian hill model](/assets/images/jacobian.png)  
- **Code snippet:**
  ```python
  y = x.pow(2).sum()
  grad = torch.autograd.grad(y, x)
