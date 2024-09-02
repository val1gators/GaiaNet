# GaiaNet
To set up a validator node for GaiaNet, follow these steps:


1. **System Requirements**:
   - **Operating System**: Ubuntu 20.04+ or macOS (with Apple Silicon).
   - **Hardware**: At least 16 GB of RAM (32 GB recommended). If using a GPU, ensure it’s compatible with CUDA 12 SDK, with a minimum of 8 GB VRAM.
   - **Cloud Setup**: For cloud deployment, an Nvidia T4 GPU instance on Azure/AWS is recommended.

2. **Install GaiaNet Node**:
   - First, download and run the installation script:
     ```bash
     curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
     ```
   - After installation, set up the environment using the command provided by the installation script (likely starts with `source`).

3. **Initialize the Node**:
   - Run the initialization command:
     ```bash
     gaianet init
     ```
   - This command will download necessary model files and configurations (e.g., LLM files), so it might take some time.

4. **Start the Node**:
   - To start your node, use:
     ```bash
     gaianet start
     ```
   - Upon successful startup, a public URL will be displayed where you can access your node.

5. **Node Management**:
   - To stop the node:
     ```bash
     gaianet stop
     ```
   - For further customization, such as using different models or joining the GaiaNet protocol, refer to the detailed node operator guide.
