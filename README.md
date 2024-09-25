# DSDV Routing Protocol in OMNeT++

## Project Overview

This repository contains the implementation of the **Destination-Sequenced Distance-Vector (DSDV)** routing protocol in OMNeT++. DSDV is a proactive routing protocol designed for Mobile Ad-hoc Networks (MANETs). It improves the distance-vector routing protocol by using sequence numbers to prevent routing loops and ensure reliable routing information.

### Features:
- Simulation of DSDV routing protocol in OMNeT++.
- Support for multi-hop wireless communication in MANET environments.
- Sequence numbers to guarantee loop-free routing.
- Performance evaluation in terms of network parameters like node mobility and traffic load.

## Prerequisites

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

## How to Run the Simulation

1. After building the project, open the OMNeT++ IDE.
2. **Right-click on the `omnetpp.ini` file** inside the DSDV project directory.
3. Select **Run as OMNeT++ Simulation**.
4. View the results and performance metrics in the simulation window.

## Simulation Parameters

- **Node Count**: Defines the number of nodes in the MANET.
- **Mobility Model**: Implements random waypoint mobility for MANET simulations.
- **Traffic Model**: Constant bit rate (CBR) or user-defined traffic.
- **Routing Tables**: Automatically updated based on DSDV logic.

