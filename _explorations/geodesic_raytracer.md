---
layout: post
title: "Real-time ray tracing rendering accretion disk of a Schwarzschild black hole"
description: >
  Real-time ray tracing rendering accretion disk of a Schwarzschild black hole 
  with relativistic Doppler effect and intensity boosting effect, implemented in CUDA and OpenGL (C++).
thumbnail: assets/img/geodesic_raytracer.png
date: 2026-04-01
related_posts: false
---

Real-time rendered accretion disk of a Schwarzschild black hole with relativistic Doppler effect and intensity boosting effect, implemented in CUDA and OpenGL (C++). Each pixel traces a null geodesic through the Schwarzschild metric using a 4th-order Runge-Kutta integrator, producing an accretion disk with animated texture. Part of the accretion disk red/blue shifts out of visible light band. The [photon ring](https://en.wikipedia.org/wiki/Photon_sphere) is visible at 1.5 radius of the event horizon. Benchmarked on an NVIDIA® GeForce RTX 4060 Ti: `1280×720` resolution at `30 FPS`. \[[GitHub repository](https://github.com/dachengx/geodesic-raytracer)\] \[[Derivation of geodesic equation](https://www.overleaf.com/read/yvtnzvtqjppk#843385)\]

---

<figure>
  <div style="position: relative; width: 100%; padding-bottom: 56.25%; height: 0;">
    <iframe src="https://drive.google.com/file/d/1PU-lZFQq_QndPTaHMRtiicFkKxLC80Vv/preview"
            style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"
            frameborder="0" allow="autoplay" allowfullscreen></iframe>
  </div>
</figure>
