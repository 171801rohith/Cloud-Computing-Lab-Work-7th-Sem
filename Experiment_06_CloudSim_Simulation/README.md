# Experiment 6: Simulate Cloud Scenario using CloudSim and Custom Scheduling Algorithm

## Aim
To simulate a cloud computing environment using CloudSim and execute a scheduling algorithm not natively included in CloudSim.


## Procedure

6. Simulate a cloud scenario using CloudSim and run a custom scheduling algorithm.
To configure and use CloudSim within Eclipse:

### Step 1: Download CloudSim installation package from
https://code.google.com/p/cloudsim/downloads/list and extract the archive.

### Step 2: Open Eclipse IDE.

### Step 3: Create a new Java Project: Navigate to **File** > **New** > **Java Project**.

### Step 4: Import the extracted CloudSim project and dependencies into the newly created Java Project.

### Step 5: Initialize the CloudSim package using the initialization method:
```java
CloudSim.init(num_user, calendar, trace_flag)
```

### Step 6: Create the Datacenter component. In CloudSim, datacenters serve as resource providers. To create a Datacenter, define a `DatacenterCharacteristics` object to store properties such as architecture, OS, host machine list, allocation policy (time-shared or space-shared), time zone, and pricing:
```java
Datacenter data center 9883 = new Datacenter(name, characteristics, new Vm Allocation Policy Simple(host List)
```

### Step 7: Instantiate the Datacenter Broker:
```java
DatacenterBroker broker = createBroker();
```

### Step 8: Configure and create the Virtual Machine (VM) by specifying the VM ID, owner ID (broker ID), processing speed (MIPS), number of PEs (CPUs), RAM, bandwidth, storage size, virtual machine monitor (VMM), and cloudlet scheduling policy:
```java
Vm vm = new Vm(vmid, brokerId, mips, pesNumber, ram, bw, size, vmm, new
```
CloudletSchedulerTimeShared())

### Step 9: Submit the VM list to the broker:
```java
broker.submitVmList(vmlist);
```

### Step 10: Create a cloudlet task with specified length, file size, output size, and utilization model:
```java
Cloudlet cloudlet = new Cloudlet(id, length, pesNumber, fileSize, outputSize, utilizationModel, utilizationMode
```

### Step 11: Submit the cloudlet list to the broker:
```java
broker.submitCloudletList(cloudletList);
```

### Step 12: Start the simulation:
```java
CloudSim.startSimulation();
```

### Sample Output from the Existing Example:
```text
Starting CloudSimExample1...
Initialising...
Starting CloudSim version 3.0
Datacenter_0 is starting...
Broker is starting...
Entities started.
0.0: Broker: Cloud Resource List received with 1 resource(s)
0.0: Broker: Trying to Create VM #0 in Datacenter_0
0.1: Broker: VM #0 has been created in Datacenter #2, Host #0
0.1: Broker: Sending cloudlet 0 to VM #0
400.1: Broker: Cloudlet 0 received
400.1: Broker: All Cloudlets executed. Finishing...
400.1: Broker: Destroying VM #0
Broker is shutting down...
Simulation: No more future events
CloudInformationService: Notify all CloudSim entities for shutting down.
Datacenter_0 is shutting down...
Broker is shutting down...
Simulation completed.
Simulation completed.
```

### Output Results Table:
```text
Cloudlet ID    STATUS     Data center ID    VM ID    Time    Start Time    Finish Time
0              SUCCESS    2                 0        400     0.1           400.1
*****Datacenter: Datacenter_0*****
User id    Debt
3          35.6
CloudSimExample1 finished!
```

## Results

The experiment for 'Simulate Cloud Scenario using CloudSim and Custom Scheduling Algorithm' was successfully implemented, configured, and verified.