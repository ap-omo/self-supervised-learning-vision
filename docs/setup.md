# Setup/Environment

## Hardware:
- Laptop with a dedicated GPU (crucial for keeping compute times in machine learning low enough to write, execute and debug code in adequate time)
  - CPU - AMD Ryzen 7-8845HS, GPU - Laptop Nvidia RTX 4060 (8GB VRAM), RAM - 16GB DDR5
 
## Software:
- Latest version of Windows 10 Home installed
- WSL2 (Windows Subsystem for Linux) enabled and fully set up
  - Full documentation on WSL2 usage here: https://learn.microsoft.com/en-us/windows/wsl/install
- Latest version of VSCode (Visual Studio Code) installed and ran through WSL2
  - The Jupyter Notebook extension was an integral addition within VSCode due to its ability to run code in separate blocks, simplifying the visualisation and debugging of specific bits of code
- Python and the necessary libraries were installed in the WSL2 environment (e.g. TensorFlow/Keras, matplotlib, numpy etc.)
  - Python 3.12 was used specifically because it was the Latest version supported by TensorFlow 2.20.0
  - Many other prerequisites come with the use of TensorFlow (for example specific versions of Nvidia CudNN and CUDA libraries, see below for more)
  - Full documentation of TensorFlow installation (using pip) here: https://www.tensorflow.org/install/pip#windows-wsl2
 
## Other notes:
- The project was ran within a named virtual environment inside WSL2 (fresh python installation, libraries etc.) which I highly recommend
  - Running projects in separate, fresh environments is usually regarded as good practice due to potential conflicts with previous installations
  - I suspect this solved a lot of the issues I had starting out (other versions of python installations or libraries interfering with each other) while also preventing many issues too
 - WSL2 was used due to native Windows only supported by an outdated version of TensorFlow (which was much more inferior in terms of performance and reliability)
   - Installation on native Windows did not go smoothly and caused the first major hiccup of the project too where I was sent back to square one
 - The CPU-only version of TensorFlow is compatible with native Windows but with a project that requires the computing power of a decent GPU it could not be a suitable alternative
 - Google CoLab would be a viable subsitution for someone who doesn't have access to a machine with a dedicated GPU
   - People working on datasets that require a much larger scale of compute power would also benefit greatly from this service
   - I was not able to run my models on datasets like CelebA in a timely manner for example, CoLab would make short work of such datasets depending on the plan provided
