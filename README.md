# Hi, I'm Tim Kong

**R&D Engineer** with a background in robotics startups and the semiconductor industry, currently pursuing a **Master's in Computer Science (Machine Learning specialization)** at Georgia Tech.

I specialize in:
- Reinforcement Learning & Generative AI
- Computer Vision, Activity Recognition, Multi-Agent Systems
- Full-stack tools and simulation for ML evaluation

**[timkongg.github.io](https://timkongg.github.io/)** – My full portfolio

---

## Highlight Projects

### Distributed Diffusion Inference Pipeline on Azure 

A distributed, event-driven, microservices-style image generation platform built on Azure. Users submit a draft hand-drawn image through the web frontend. Afterwards, the ML pipeline will be scheduled and fanned out across a GPU-backed inference cluster to produce 4 output drawings. Each output drawing is generated with a predefined prompt.

#### Architecture

![Architecture](https://github.com/user-attachments/assets/cf48ba4f-80f8-459c-bfe8-2066aedf0505)

- Web Services
  - Nextjs FE and Fastify API Server to serve the web frontend UI for user interactions
- Event Bus
  - Azure event hubs as the interface between Web services and ML services
- ML Services
  - Spark streaming job scheduler to trigger inference upon job submission event
  - Ray inference cluster orchestrating the GPU workers to perform the inference tasks
- Storage
  - PostgreSQL database to store user, job, and task records
  - Azure blob storage to store the input and output images, and the pretrained models
  - ML Flow to store the model parameters and inference script
 
#### Example Input and Outputs

|           Input           |             Output 1             |             Output 2             |             Output 3             |             Output 4             |
| :-----------------------: | :------------------------------: | :------------------------------: | :------------------------------: | :------------------------------: |
| ![Input](https://github.com/user-attachments/assets/e7b47968-cc08-4459-8dfe-25726967246b) | ![Output 0](https://github.com/user-attachments/assets/54bb3088-5d52-4ef1-9c6e-55eb0d86d6af) | ![Output 1](https://github.com/user-attachments/assets/8140b98c-1658-4cd6-816e-21b382812db8) | ![Output 2](https://github.com/user-attachments/assets/a73b06b1-e037-44b7-8c7f-c5e46dbbfb85) | ![Output 3](https://github.com/user-attachments/assets/bc3cec57-dabb-4e8b-be36-62d64286535b) |


### Multi-Agent RL in Overcooked-AI using CTDE MAPPO

![counter_circuit_o_1order-ezgif com-speed](https://github.com/user-attachments/assets/5bf1530e-0903-460a-835d-0d39f6ee623d)

- Trained agents using **MAPPO with Centralized Training and Decentralized Execution (CTDE)**.
- Designed reward shaping on subgoals and advantage sharing to foster collaboration.
- Achieved **7–11 soups per episode** with emergent asymmetric behaviors across agents.

---


### Lunar Lander Continuous Control with SAC

![lunarlander](https://github.com/user-attachments/assets/e59449db-3993-49bc-86c3-ca8f3cc85119)

- Applied **Soft Actor-Critic** to solve LunarLanderContinuous-v3 in Gym.
- Conducted hyperparameter sweeps on entropy, learning rate, and target update rate.
- Observed learning phases: crash → hover → stable landings (> 200 reward).

---

### MeshQuest: Benchmarking and Fine-Tuning Generative 3D Models

![MeshQuest](https://timkongg.github.io/images/meshquest.png)

- Benchmarked **Hunyuan3D, OpenLRM, One-2-3-45, Pixel2Mesh** on 16 stylized low-poly assets.
- Fine-tuned **OpenLRM** on 734 asset dataset with **DINOv2**, **triplane NeRF**, and **TV regularization**.
- Performed **human perceptual survey** and geometric analysis (CD/HD) to quantify improvements.

---

## Contact

📧 [hkong43@gatech.edu](mailto:hkong43@gatech.edu)  
🌐 [Portfolio](https://timkongg.github.io)  
📍 Vancouver, BC  
💼 [LinkedIn](https://www.linkedin.com/in/timkongcae)  
💻 [GitHub](https://github.com/timkongg)

---

