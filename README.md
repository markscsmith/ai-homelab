# ai-homelab
Repo for configuring hosts for basic AI development, including libraries for development and GPU drivers.

## Initial Target Platforms
- Ubuntu 22.04 LTS
    - CPU
        - AMD 5950X
        - AMD 5800X
        - ARM?
    - GPU
        - NVidia 3090
        - AMD 7900XTX
        - AMD 6900XT


- macOS 14
    - M1 Max (16" MBP)
    - M2 (13" MBA)
    - M1 (13" MBA)
    - Intel i9 (16" MBP)

(based on available test hardware)

## Initial Target Libraries
- PyTorch
- TensorFlow
- stable_baselines3
- OpenAI Gym
- OpenCV?
- Others for LLM / Diffusion?


## Assumptions about base target environment:
- Ubuntu 22.04 LTS
    - ssh keys are in place
    - sudo is available
    - apt is available
    - internet is available
    - user is in sudoers group
    - GPU is installed in motherboard
    - GPU has available drivers
    - system has booted succesfully WITHOUT proprietary drivers installed

- macOS 14
    - ssh keys are in place
    - xcode command line tools are installed
    - sudo is available

## Assumptions about base source environment (if building over ssh):
- Bash or ZSH shell environment
- ssh keys are in place
- ansible is available on the source machine
- internet is available on the source and destination machines
- connectivity to target hosts is available


# TODO:
"now install build-essentials and the dependencies for the amdgpu pro drivers" causes copilot to create an infinite loop suggesting the same packages over and over. Hm.