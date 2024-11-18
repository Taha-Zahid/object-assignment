# Object Detection Using Xubuntu in a Virtual Environment

This project demonstrates real-time object detection using a lightweight virtual environment powered by Xubuntu. The goal is to set up and execute an object detection script efficiently on constrained resources.

---

## Features
- Real-time object detection using OpenCV.
- Lightweight virtual machine setup with Xubuntu for stability and resource efficiency.
- Supports detection of various objects like cars, bikes, pedestrians, and buses.

---

## Prerequisites
Before starting, ensure you have the following:
1. **QEMU**: For running the virtual machine.
2. **Xubuntu ISO**: [Xubuntu 18.04](https://xubuntu.org/release/18-04/) (amd64).
3. **Python3 and OpenCV**: Installed within the Xubuntu virtual machine.

---

## Step-by-Step Instructions

### Step 1: Boot the Virtual Machine
Use the command below to boot the Xubuntu virtual machine:

```bash
qemu-system-x86_64 -M q35 -m 4096 -cdrom xubuntu-18.04.5-desktop-amd64.iso -boot order=d -smp 2 -vga virtio -display gtk

## Step 2: Clone the Repository
After booting the virtual machine, open the terminal and clone the GitHub repository:

```bash
git clone https://github.com/Taha-Zahid/object-assignment.git
cd object-assignment

## Step 3: Update the System and Install Dependencies
Ensure the virtual machine’s system is updated and install necessary packages:

sudo apt-get update
sudo apt-get install python3-opencv

## Step 4: Run the Object Detection Script
Execute the object detection script with the following command:

python3 object_detect.py



