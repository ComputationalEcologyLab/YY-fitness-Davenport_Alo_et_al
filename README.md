Data and code for "Fitness regulates non-native species recovery in a simulated trojan Myy brook trout application". Article DOI: 10.1111/EVA.70335

These data will allow to reproduce results obtained in the paper. There are 2 directories. One contains the data and the second one is the SRC directory which contains the appropriate CDMetaPOP version to run the simulations. Make sure to use this version otherwise the input files will not work.

Also make sure to have Python 3.8+ along with the NumPy and SciPy packages installed. If additional help is needed and/or you prefer to use the R package CDMetaPOP companion cdmetapopR follow the instructions given on the CDMetaPOP tutorial webpage: <https://computationalecologylab.github.io/cdmetapop_web/run_cdmetapop.html>

## Running the Simulations 

These instructions are for use in a command-line terminal — **Terminal** on macOS/Linux, or **Command Prompt / PowerShell** on Windows.

1.  Clone the repository and move into it:

``` bash
   git clone https://github.com/ComputationalEcologyLab/YY-fitness-Davenport_Alo_et_al.git
   cd YY-fitness-Davenport_Alo_et_al
```

2.  Change into the `src/` directory, where `CDMetaPOP.py` lives:

``` bash
   cd src
```

3.  Run the python simulation, pointing to the appropriate data folder, runVars file, and desired output name. For example, to run the baseline simulation:

``` bash
   python CDMetaPOP.py ../data/ID/baseline RunVars_LHS_71.csv test_baseline
```

> **Note:** paths are relative to `src/`, so use `../data/...` once you're inside that directory. Adjust the folder (`ID/baseline`), runVars file, and output name to match the scenario you want to run.
