## AVD

The Advanced Analytics Workspace (AAW) runs in the cloud and it's main interface is called Kubeflow. In order to access the AAW, please launch your AVD using the **Remote Desktop** icon on your personal computer.

![AVD Icon](../images/avd-icon.png)

Once your AVD has started, you can launch the AAW by opening the icon on your desktop. You can also access the AAW by following this link: [https://kubeflow.aaw.cloud.statcan.ca/](https://kubeflow.aaw.cloud.statcan.ca/).

![AAW Icon](../images/aaw-icon-on-desktop.png)

### Login with Your Statistics Canada Account

You'll need to login using your Statistics Canada account.

![Statistics Canada Account](../images/log-in-with-stats-account.png)

# Using the AAW through the Kubeflow Interface

## Kubeflow Central Dashboard

When you first log in to the AAW, you will see the Kubeflow Central Dashboard. This contains links to recently used Notebook Servers and documentation.

![Kubeflow Central Dashboard](../images/kubeflow-main-ui.PNG)

## Kubeflow Central Dashboard Sidebar

The sidebar on the left has 

- **Home**: The Kubeflow Central Dashboard.
- **Notebooks**: Manage your notebook servers.
- **Metrics**: Grafana, the AAW's observability platform.
- **Github**: The official Kubeflow Github repository.
- **Documentation**: The official Kubeflow documentation.

As a user of the Advanced Analytics Workspace, you'll only need to use **Home** and **Notebooks**.

![Kubeflow Central Dashboard Sidebar](../images/kubeflow-sidebar.png)

## Namespace Selection

When you are on the Kubeflow Central Dashboard, in the upper left corner you will find the **Select namespace** dropdown menu. If the menu says "Select namespace" then you need to select a namespace before you can view, edit or launch any of your notebook servers. 

![Selecting a Namespace](../images/select-a-namespace-1.png)

### Select the namespace from the namespace dropdown menu.

When you select the menu, a dropdown list will appear with all the namespaces you belong to. Please select the appropriate namespace before moving forward.

![Selecting a Namespace](../images/select-a-namespace-2.png)

### If you see the name of a namespace, you are ready to use the AAW.

Once a namespace has been selected, the name of the namespace will replace "Select namespace". If no namespaces appear in the menu, please contact us on [Jira](https://jirab.statcan.ca/projects/BTIS/issues).

![Selecting a Namespace](../images/select-a-namespace-3.png)

# Creating a new Notebook Server

## Click **Notebooks** from the sidebar on the left.

Once you click **Notebooks** from the Central Dashboard Sidebar, you will be brought to the Notebooks management section of Kubeflow where you can **Create**, **Start**, **Stop** and **Delete** your notebook servers and storage.

![Kubeflow Notebook Servers](../images/kubeflow-sidebar-notebooks-selected.png)

**Note**:  only one set of notebook servers can be viewed at a time. If you have more than one namespace. You may need to select the appropriate namespace from the **Select namespace** dropdown menu in the upper left-hand corner to see the notebook servers belonging to that particular namespace. 

## Click **"+ New Notebook"**

To create a new notebook server, press the **"+ New Notebook"** button in the upper right-hand corner.

![+ New Notebook](../images/new-notebook.png)

# Configure the Notebook Server

## Name your notebook server

The first thing you'll have to do is to name your Notebook Server. You must start the name with a lowercase letter and no spaces.

![Selecting a Namespace](../images/name-your-server.png)

## Select the notebook server type.

![Select Your Server Type](../images/make-a-new-sas-server.png)

The SAS image will be most appropriate for most users. If you don't need access to SAS, then the JupyterLab image is a lighter alternative. The RStudio image only has RStudio so if you only ever want to use RStudio that image may suite your needs well. The Ubuntu image is a more advanced desktop image for special desktop applications.

### JupyterLab

If you don't need access to SAS, then the JupyterLab image is a lighter alternative. The JupyterLab image contains environments for working with R, Python and Julia. 

#### Features

The JupterLab Notebook Server has the following features:

- Python
- R
- Julia
- Pluto
- OpenM++
- VS Code

#### Screenshot

Interactive sessions can be started by clicking on any of the icons in the Launcher as seen in the screenshot below.

![JupyterLab](../images/fullscreen-jupyter.png)

### RStudio

#### Features

The RStudio image only has RStudio so if you only ever want to use RStudio that image may suite your needs well. We include some packages by default:

- Tidyverse
- Tidymodels
- Caret
- Quarto

#### Screenshot

![JupyterLab](../images/fullscreen-rstudio.png)

### Ubuntu

The Ubuntu image is a more advanced desktop image for special desktop applications.

#### Screenshot

![JupyterLab](../images/fullscreen-ubuntu.png)

### SAS

The SAS image will be most appropriate for most users.

#### Screenshot

Interactive sessions can be started by clicking on any of the icons in the Launcher as seen in the screenshot below.

![JupyterLab](../images/fullscreen-sas.png)

## Select Protected B if you need it

Select Protected B if you need it. Your notebook server will not have access to the internet if you do this.

![Selecting a Namespace](../images/protected-b.png)

Once your notebook server has been named and you have selected the type of notebook server you can press **LAUNCH**.

![Selecting a Namespace](../images/launch.png)
