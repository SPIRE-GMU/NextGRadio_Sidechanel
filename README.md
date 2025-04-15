# NextGRadio_Sidechanel

## README: 5G Side Channel Fingerprinting

### Overview

This directory contains all code, data, and documentation from our Open Air Interface (OAI) 5G network experiment.

## Folder Structure
### Inside `Code`:
- CW_Code.ipynb: Jupyter Notebook that defines and executes data collection.

### Inside `Final5GDataCollection`:
Two main folders for the two UEs that were tested: PHONE and RADIO

Inside the PHONE Folder:
Each represents a scenario we tested the network with using our phone.

- **Graphs/** - Contains plots comparing different network activities and their performance.
- **Idle/** - The phone is connected but is performing no activites.
- **News/** - Data from accessing online news websites.
- **Radio/** - Traces collected from streaming online broadcast radio stations.
- **Social_Media/** - Data and plots related to social media usage.
- **Youtube/** - Traces collected from YouTube streaming activities.
- **Retail/** - Traces collected from online retailers.

Inside the RADIO Folder:
- **Downlink/** - Traces collected from a downlink connection between the base station and UE
- **Uplink/** - Traces collected from a uplink connection between the base station and UE
    - **5M** - iPerf test with 5M bandwidth size
    - **10M** - iPerf test with 10M bandwidth size
    - **15M** - iPerf test with 15M bandwidth size
- **Idle/** - UE is connected but performing no activities.

### Inside Each Scenario Directory
Each folder contains:
- **`.npy` files** - These are numpy arrays storing raw network traces. They will be labeled `CollectionX` (e.g., `Collection1`, `Collection2`, etc.).
- Folders may have `.npy` files labeled `testX`. These are trace samples to test the ML model for accurate classification.
- Each `.npy` file has **200 traces**. We have aimed to collect at least **1000 traces** for each scenario. Test files have 50 traces each.

