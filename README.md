# **IK_FK_ABB_IRB_4600_40_255_ROBOTICS-PROJECT**  

## **📌 Project Summary**  
This project focuses on **simulating and analyzing** the motion of the **ABB IRB 4600-40/255 robot** using **CoppeliaSim** and **Python**. It involves implementing:  
- **Forward Kinematics (FK)** to compute the robot’s end-effector position.  
- **Inverse Kinematics (IK)** to determine the required joint angles for a given position.  
- **Trajectory generation** using interpolation methods.  

The robot was successfully programmed to trace a **trajectory in the shape of "201147"**. The final drawing was achieved with **high accuracy**, demonstrating the effectiveness of the **FK and IK algorithms** along with the **interpolation method**.  

---

## **📌 ZeroMQ Remote API**  
The **ZeroMQ remote API** is one of the available methods for external applications to communicate with **CoppeliaSim**. It allows external programs (e.g., real robots or remote computers) to control the simulator.  

🔗 **[ZeroMQ Remote API Documentation](https://www.coppeliarobotics.com/helpFiles/en/zmqRemoteApiOverview.htm)**  

### **Features of ZeroMQ Remote API:**  
- Supports controlling the **simulation** and **CoppeliaSim itself** from an external application.  
- Provides access to all API functions available in a CoppeliaSim script (e.g., `sim.*`, `simIK.*`, `simOMPL.*`, etc.).  
- Allows multiple external applications to interact with **CoppeliaSim** either **synchronously** (step-by-step) or **asynchronously** (free-running).  
- Supports remote control of the simulator (e.g., loading a scene, starting, pausing, or stopping a simulation).  

### **🔧 Install the Client Package:**  
To use the **ZeroMQ remote API** with Python, install the required package:  
```bash
$ python3 -m pip install coppeliasim-zmqremoteapi-client
```
> **Note:** The **ZeroMQ** and **CBOR** dependencies will be installed automatically.  

---

## **📌 Key Components**  

### **1️⃣ Robot Model and DH Table**  
- The **Denavit-Hartenberg (DH) parameters** were recalculated based on the actual dimensions of the robot in **CoppeliaSim**.  

### **2️⃣ Kinematics Calculations**  
#### **🔹 Forward Kinematics (FK)**  
- Implemented FK to **compute the end-effector position** based on joint angles.  

#### **🔹 Inverse Kinematics (IK)**  
- Developed an **IK function** to compute **joint angles** for a given end-effector position.  

### **3️⃣ Trajectory Implementation**  
- Defined **task space points** for the robot.  
- Used **linear interpolation** to generate a smooth trajectory.  

### **4️⃣ Drawing Implementation**  
- Added a **drawing surface** in the simulation environment.  
- Attached a **pen to the robot** to draw predefined paths.  

---

## **📌 Results**  
✅ The robot successfully traced the required **"201147"** trajectory.  
✅ The final drawing was **highly accurate**, confirming the correctness of the **FK and IK algorithms** and the **interpolation method**.  

---

## **📌 Requirements**  
Ensure you have the following dependencies installed before running the project:  

✅ **CoppeliaSim**  
✅ **Python 3**  
✅ **NumPy & Matplotlib libraries**  
✅ **coppeliasim-zmqremoteapi-client** (for ZeroMQ API)  

---

## **📌 Usage**  
### **🔧 Running the Simulation:**  
1. **Open CoppeliaSim** and load the robot scene.  
2. Run the **ZeroMQ Remote API server** in CoppeliaSim.  
3. Observe the robot's motion and drawing output.  

---

## **📌 License**  
This project is for **educational purposes** and can be freely modified or shared.  

---
