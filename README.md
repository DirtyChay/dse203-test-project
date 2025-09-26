# NDP Demo Workspace

1. **Launch JupyterHub**. We will start by launching JupyterHub. You can do this, either by clicking on the JupyterHub button at the bottom of this module, or through any other JupyterHub button within NDP

2. **Reserve Resources**. Once you're in JupyterHub, reserve with the following specifications (this is the default setup):
- Region: Any
- Zone: Any
- GPUs: 0
- Cores: 1
- RAM: 16GB
- GPU Type: Any
- Pre-built Image: Minimal NDP Starter JupyterLab
- Architecture: amd64

3. **Launch your server**. Once you specify the resources as indicated, click on Start Server and wait to be redirected to JupyterLab (this may take a few minutes).

4. **Set your storage**. Once in JupyterLab, click on the File Browser button (left sidebar) to navigate to a storage folder for your work. You could have 2 folders:

- *your-group-name-Shared-Storage*: This is a shared folder for your group. Space is limited to 5GB, so use this folder to store files that are shared among team members, especially frequently used files. Do not use it to work on modules or notebooks at the same time, or you will run into an overwrite conflict.
- *User_Persistent_Storage*: This is an individual storage folder. Use this folder to store files you're working on individually.

Each group member needs to save their work in their User_Persistent_Storage. To do this, please select the user persistent storage folder (double click). Click on the NDP button to get back to the NDP Widget and confirm your selection by looking at the Current Folder window.

**NOTE**: Any file that is not saved in these folders will be lost once you stop your server. Therefore, if you want your files to persist across sessions, you must place them inside one of your storage directories.

5. **Select Workspace**. In the NDP Widget, select the Data Challenge Onboarding Module from the dropdown list of workspaces.

6. **Clone repository**. Look at the Current Folder window and confirm that your current folder is your user persistent storage folder. Go to the Clone Repository section (below Select Workspace) and clone the repository into your selected storage folder by clicking the Clone Repository button. When cloning, keep the default settings (Include submodules checked, and Download the repository unchecked). The repository will take a few seconds to clone.

7. **Install Requirements**. Click on File Browser and navigate to the eh-onboarding directory within the cloned repository. Click again the NDP button and confirm that you are inside the eh-onboarding directory by looking at the Current Folder window. Install the dependencies by clicking the Install requirements.txt button (below Clone Repository). Upon successful installation, you will see a confirmation pop-up and a log file with the installed libraries will be generated automatically. In the case that your .log file is not automatically generated, click the Install requirements.txt button one more time. Sometimes, libraries are installed, but the file is not generated at first.

**NOTE**: Installing libraries will be effective for your current JupyterHub session. However, once you stop your server, your libraries will be lost. Therefore, each time you come back to work on a particular module, you need to reinstall the libraries.

8. **Add selected files**. Select the weather-station-measurements dataset from the Add Selected Files list. Select San Diego Weather Sample from the list of resources, check Create Dataset Folder and click on Add resources to current folder to download the dataset to your persistent storage. It will take a few seconds to download.

9. **Add a dataset to this workspace**. Go to the datasets section of this module, and click on Edit. Type the term lidar in the search bar, and add one dataset of your choice by clicking on +Add. Return to JupyterHub, and click on the refresh arrow next to Select Workspace, then select this module again and look at the datasets list to verify the addition of your dataset. We won't be using this dataset, but this exercise will help you gain experience using this feature.

10. **Complete the onboarding.ipynb notebook**. Click on File Browser to navigate back to the eh-onboarding directory. Open the onboarding.ipynb notebook and complete it, following the instructions and code within the notebook.

11. **Make your own solution**. Once you complete the onboarding.ipynb notebook, create a new notebook (File → New → Notebook), and work on a new model to improve upon our current benchmark. You can experiment with different model types, adjust hyperparameters, or engineer new features to enhance performance.

12. **Stop Your Server**. When you have finished your work, stop your server by navigating to File → Hub Control Panel → Stop Server.


FINAL NOTE:  If you return to this module at some point, you will only need to complete steps 2, 3, 4, and 7 of the setup because your files will be stored in your shared folder, so you will not need to clone the repository or download the data files again.
