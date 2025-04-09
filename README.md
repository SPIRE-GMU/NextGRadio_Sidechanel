# NextGRadio_Sidechanel

README: 5G Side Channel Fingerprinting

Overview

This directory contains all code, data, and documentation from our Open Air Interface (OAI) 5G network 
experiment.

Folder Structure:

Inside dataCollection/Phone:

Each represents a scenario we tested the network with using our phone.

App_Downloads/Contains trace data and plots related to application downloads over the 5G network.

Blogs/Data related to browsing and accessing blog sites.

Comparison_Plots/Contains plots comparing different network activities and their performance.

Netflix/Network traces from streaming activities on Netflix.

News_Sites/Data from accessing online news websites.

Radio_Station/Traces collected from streaming online radio stations.

Social_Media/Data and plots related to social media usage.

UE_Connected_No_Activity/Baseline network traces from a connected User Equipment (UE) with no active data transfer.

Upload/Data related to file uploads over the network.

Youtube/Traces collected from YouTube streaming activities.

Retail_Sites/Traces collected from online retailers.

Inside Each Application Directory

Each folder contains:

.npy files: These are numpy arrays storing raw network traces. They will be labeled CollectionX (e.g. Collection1, Collection2 etc)

collectionX_plots/: Plots generated from data collection runs. These are charts to visualize the traces.

zoomedX_plots/: Zoomed-in versions of the main plots to highlight key patterns.

Some folders may have .npy files labeled testX. These are trace samples to test the ML model for accurate classification.

Each .npy file has 200 traces. We have aimed to collect at least 1000 traces for each scenario.



