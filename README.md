# robot-art

### Physical AI LEGO Quality Inspection & Sorting Robot

Our system combines **SmolVLA** and **ACT (Action Chunking with Transformers)** to learn robot movements from a human-operated leader arm. Using **Physical AI**, we collect real-world demonstration data by guiding the robot through LEGO inspection and sorting tasks.

The robot learns to **identify LEGO blocks, determine whether each piece is perfect or defective, and autonomously pick and place it onto the corresponding plate**. We use an **NVIDIA H100 GPU** for imitation-learning training, enabling the model to learn manipulation policies from the collected demonstrations.

To make the system easier to understand and troubleshoot, we also built a **debugging and visualization tool on Rerun.io**, allowing us to replay demonstrations, inspect robot actions, and analyze model behavior step by step.

**Pipeline:**
**Human Leader Arm → Physical AI Data Collection → SmolVLA + ACT → H100 Imitation Training → Robot Pick & Place → Perfect / Defective Plate → Rerun.io Debug & Replay**
