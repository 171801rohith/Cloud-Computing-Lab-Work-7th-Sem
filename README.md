# Cloud Computing Lab Manual (2022 Scheme)

Welcome to the **Cloud Computing Lab** repository! It provides a comprehensive set of 11 practical lab experiments exploring leading cloud platforms, virtualization environments, cloud simulation tools, Apex programming, and serverless architectures.

Each experiment is organized in its own dedicated directory, complete with step-by-step instructions, source code, configuration files, output screenshots, and verified results.

---

## Table of Experiments

| Exp # | Experiment Title | Tech Stack / Platform | Link | Screenshots |
|:---:|---|---|:---:|:---:|
| **01** | **Virtualization Setup**<br>Set up VirtualBox/VMware Workstation running a Linux or Windows OS | VirtualBox, Linux / Windows | [View Experiment](./01_VirtualBox) | 6 Images |
| **02** | **Virtual Machine C Compiler**<br>Configure a C compiler inside a virtual machine and execute a basic program | Linux (Ubuntu), GCC, VirtualBox | [View Experiment](./02_C_Compiler) | 5 Images |
| **03** | **AWS EC2 Instance**<br>Launch an EC2 instance on AWS (Amazon Web Services) | AWS EC2, Linux AMI, SSH | [View Experiment](./03_AWS_EC2) | 8 Images |
| **04** | **Salesforce Apex Application**<br>Build a basic application using the Apex programming language | Salesforce Developer Console, Apex | [View Experiment](./04_Salesforce_Apex) | Apex Code |
| **05** | **Salesforce Mailing Service**<br>Set up an email mailing service using the Apex programming language | Salesforce Developer Console, Apex | [View Experiment](./05_Salesforce_Mailing) | 3 Images |
| **06** | **CloudSim Simulation**<br>Model a cloud environment using CloudSim and execute a custom scheduling algorithm | Java, CloudSim API, Eclipse | [View Experiment](./06_CloudSim_Simulation) | Console Logs |
| **09** | **Google App Engine**<br>Deploy and launch web applications using the Google App Engine Launcher | Google App Engine, Python, `app.yaml` | [View Experiment](./09_Google_App_Engine) | 5 Images |

---

## Repository Structure

```
CLOUD_LAB/
├── README.md                              # Universal Repository Guide
├── 01_VirtualBox/                         # Exp 1: VirtualBox & OS Installation
├── 02_C_Compiler/                         # Exp 2: VM C Compiler Setup & Execution
├── 03_AWS_EC2/                            # Exp 3: AWS EC2 Instance Creation
├── 04_Salesforce_Apex/                    # Exp 4: Salesforce Apex Application
├── 05_Salesforce_Mailing/                 # Exp 5: Salesforce Mailing Service
├── 06_CloudSim_Simulation/                # Exp 6: CloudSim Simulation & Scheduling
└── 09_Google_App_Engine/                  # Exp 9: Google App Engine Web App
```

---

## Summary of Technologies & Platforms Used
- **Cloud Providers**: Amazon Web Services (AWS EC2, S3, CloudFront), Microsoft Azure (Blob Storage), Salesforce Cloud, Google App Engine (GAE).
- **Virtualization & Simulation**: Oracle VM VirtualBox, CloudSim Simulation Toolkit.
- **Languages & Frameworks**: C (`gcc`), Python (`Pillow`, `azure-storage-blob`), Java (CloudSim), Apex (Salesforce), YAML, JSON.
- **Web Servers & CDNs**: Apache HTTP Server (`httpd`), AWS CloudFront CDN.

---

## Getting Started

To get started with an experiment:
1. Open the desired experiment directory (e.g., `cd 03_AWS_EC2`).
2. Refer to the local `README.md` for the full aim, step-by-step procedure, source code, configuration guides, and visual walkthroughs.
3. Find all corresponding screenshots within each experiment's `images/` folder.
