## AODV, GPSR and DSDV Routing Protocol in OMNeT++

## Project Overview
# Routing Protocols for MANETs in OMNeT++

This repository contains the implementation of three routing protocols for Mobile Ad-hoc Networks (MANETs) in OMNeT++: **Destination-Sequenced Distance-Vector (DSDV)**, **Ad hoc On-Demand Distance Vector (AODV)**, and **Greedy Perimeter Stateless Routing (GPSR)**.

## Project Overview

- **DSDV**: A proactive routing protocol that maintains up-to-date routing information by periodically exchanging routing tables. It uses sequence numbers to prevent routing loops and ensure reliable routing.

- **AODV**: An on-demand routing protocol that establishes routes only when needed, minimizing overhead in dynamic networks.

- **GPSR**: A geographic routing protocol that uses location information to forward packets efficiently, utilizing greedy forwarding and perimeter routing.

## Key Features

- **Proactive Routing (DSDV)**: Always available routes with periodic updates.
- **On-Demand Routing (AODV)**: Reduces control overhead by creating routes as needed.
- **Geographic Forwarding (GPSR)**: Efficient packet delivery based on location information.


You need to install the following tools to run this project:

- **OMNeT++ 6.x**: A discrete event simulation environment for communication networks. [Download OMNeT++](https://omnetpp.org/download/)
- **INET Framework**: The INET framework provides protocol models for OMNeT++. [Download INET Framework](https://inet.omnetpp.org/)

## Installation and Setup

Follow these steps to set up the project on your system:

### Set up OMNeT++:

1. **Install OMNeT++**:
   - Follow the instructions to install OMNeT++ from the official website: [OMNeT++ Installation Guide](https://doc.omnetpp.org/omnetpp/manual/#sec:installing-omnetpp).
   
2. **Install the INET framework**:
   - Clone the INET framework and compile it in OMNeT++:
     ```bash
     git clone https://github.com/inet-framework/inet.git
     cd inet
     make
     ```
   - To get additional files to add MANET protocols few additionals will be added or you can check out [here](https://inet.omnetpp.org/docs/showcases/routing/manet/doc/)

### Add the DSDV project to OMNeT++ IDE:

1. **Open OMNeT++ IDE**.
2. **Import this cloned repository (DSDV)** as an existing project:
   - Go to **File > Import > General > Existing Projects into Workspace** and select the DSDV project directory.
3. **Ensure the INET framework is also imported and built**.
   - Import INET the same way and make sure it's built before running simulations.

### Build the project:

1. **Right-click on the DSDV project** in the OMNeT++ IDE.
2. Select **Build Project**.
3. **Check out for [Part 2](https://github.com/Nicsetty/iNet-add-on) to get additional configured files for iNet framework :)**

## How to Run the Simulation

1. After building the project, open the OMNeT++ IDE.
2. **Right-click on the `omnetpp.ini` file** inside the DSDV project directory.
3. Select **Run as OMNeT++ Simulation**.
4. View the results and performance metrics in the simulation window.


## Sample simulation image
![dsdvv output](https://github.com/user-attachments/assets/5b383db4-7021-4b6d-9a70-9e2665e540d4)

