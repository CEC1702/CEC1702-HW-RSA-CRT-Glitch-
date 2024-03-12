# Fault-Injection Attack on Cryptographic Accelerator of CEC1702 Microcontroller
Project structure: 
- scripts.zip
  - CEC1702_BIGI_GLITCHING.ipynb - used for performing attacks on modular reduction
  - CEC1702_RSA_GLITCHING.ipynb  - used for performing attacks on RSA-CRT (HW or SW)
  - NOTE: Used within the ChipWhisperer v5.5 environment

- implementations.zip
  - MOD-REDUCTION - used for testing Modular Reduction only
  - RSA-CRT - implementation of RSA-CRT in HW (MikroC API calls) and SW
  - NOTE: RSA-CRT implementation has three folders depending on which key is used (all three keys should have been accessible just through preprocessor macros, I know...)
  - NOTE: Projects can be opened in MikroC IDE by opening *.mcpar files

- binaries.zip
  - all binaries used for attack, generated from implementations using MikroC IDE
  - loaded to CEC1702 Flash memory using USB-SPI converter and Flash programmer

- results
  - glitching results of various runs (SW, HW RSA-CRT, multiple MCUs)
  - Python Notebook for data analysis and graph creation  
