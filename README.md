# OpenFAST-DLC-sampler-Automator
 This project facilitates the execution and management of OpenFAST simulations by   dynamically updating input files, running simulations, and organizing outputs for Design Load Cases.

*Originally developed during the [Optimus 295-20 wind turbine project](https://github.com/WindEnergyEngineering/Optimus-295-20/tree/master/OpenFAST/Optimus-295-20) at Flensburg University of Applied Sciences.
--------------------------------------------------------------------------------
# Features

  - Automatically updates and configures OpenFAST input files:
    - Updates wind files (.bts)
    - Dynamically manages HydroDyn configuration files.
    - Edits the .fst file for hydrodynamic inputs.
  - Automates the execution of OpenFAST simulations using a batch file
  - Organizes simulation outputs by wind speed and seed for easy post-processing.
   
-----------------------------------------------------------------------------------------------
# Installation
1. Clone the Repository:
   git clone https://github.com/Araz-m/OpenFast_Automating-DLC-Simulations_Optimus_295_20_Hochschule-Flensburg.git
cd OpenFast_Automating-DLC-Simulations_Optimus_295_20_Hochschule-Flensburg

   
2. Install Dependencies: Ensure you have Python 3.x installed. Then install the required Python packages:
   pip install -r requirements.txt
   
4. Verify OpenFAST Installation:

- Confirm that OpenFAST is installed on your machine.
- Place the start_OpenFAST_v3-41.bat file in the appropriate directory, and update its path in the script if necessary.
   
# Usage

1. Prepare Input Files:

  - Organize wind files (.bts) in the Wind directory.
  - Place HydroDyn configuration files (.dat) in the Wave directory.
  
2. Run the Script: Execute the automation script:
   python project.py
   # I recommend to run the code in VScode because in contrast with cmd it can be scrolled for furthure checks
   
4. Outputs:

- Simulation outputs will be organized in the Outputs/DLC12 directory.
- Files are renamed using the format OPT-MP-V<WindSpeed>_S<Seed> for easier identification.
--------------------------------------------------------------------------------------
# Project Structure
📂 OpenFast_Automating-DLC-Simulations_Optimus_295_20_Hochschule-Flensburg
├── 📁 DLC12             # Main Directory
│  └── 📂 Outputs           # Outputs are generated here
│     └── 📂 DLC12         # Organized simulation results
│  └── project.py           # Main script for automation
│  └── test_project.py      # Test script for custom functions
├── 📁 Wind              # Contains .bts wind files
├── 📁 Wave              # Contains HydroDyn input files
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation

----------------------------------------------------------------------------
# Contributing
 Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Commit your changes (git commit -m "Add new feature").
4. Push to your branch (git push origin feature-branch).
5. Open a pull request.
--------------------------------------------------------------------------------

A detailed *pdf manual* will be added as a guide
--------------------------------------------------------------------------
