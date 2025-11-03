---
title: "Distributed Raytracer"
excerpt: "Static raytracing with parallel memory and computation<br/><img src='/images/render.jpg'>"
collection: projects
---

Networked ray tracing system implemented in Rust that splits rendering across cooperating servers. The first server type comprises of an orchestrator that discovers workers via UDP multicast, partitions the scene into spatial bounding volumes, and coordinates renders. Other server types include object servers that store and serve scene geometry and ray servers that compute rays/pixels in parallel. Clients connect to the orchestrator over WebSocket to submit scenes and start renders. Nodes communicate with compact binary messages (bincode) and TCP for low-overhead RPC. The project uses asynchronous Rust (tokio, tokio-tungstenite, futures) and safe concurrency primitives (Arc, channels) to maximize throughput, and outputs standard PPM images.

[Github Link](https://github.com/notrandomath/distributed-raytracer)
