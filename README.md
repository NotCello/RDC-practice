# Robot Dynamics & Control - Practice Repository

This repository contains practical exercises and implementations for the **Robot Dynamics & Control** course (2025) taught by Roberto Cannata, Pedro Luis Figueroa Saire and Simone Borelli at the University of Genoa.

## 📚 Course Overview

The course focuses on practical implementation of robot dynamics and control algorithms using MATLAB/Simulink and Simscape Multibody. The exercises progress from basic simulation tools to advanced robotic control systems.

## 🗂️ Repository Structure

### Session 2: Serial Robot Modeling and Statics
**Files:** `GC/`
- **Serial Robot Construction**: Step-by-step 2R robot building
  - Base link design with rigid transforms
  - Joint implementation (revolute joints)
  - Link subsystem creation
- **Denavit-Hartenberg Convention**: Frame placement for kinematic chains
- **Gravity Compensation**: Static force analysis and torque computation
  - Virtual work principle application
  - Jacobian-based force/torque mapping
  - Transform sensing for pose information

**Key Learning Objectives:**
- Build complete serial robot models in Simscape
- Understand kinematic conventions (DH parameters)
- Implement gravity compensation algorithms
- Master coordinate frame transformations

### Session 3: Newton-Euler Recursive Dynamics
**Files:** `NE/`
- **Newton-Euler Algorithm**: Complete recursive implementation
  - Forward recursion: velocities and accelerations
  - Backward recursion: forces and torques
- **1R Robot Dynamics**: Detailed step-by-step analysis
  - Angular velocity and acceleration computation
  - Center of mass dynamics
  - Joint force and torque calculation
- **Closed-Form Models**: Analytical solutions for verification
- **Trajectory Generation**: Open-loop motion planning

**Key Learning Objectives:**
- Implement recursive dynamics algorithms
- Understand multibody force propagation
- Derive closed-form dynamic equations
- Generate and test robot trajectories

### Session 4: Dynamic Robot Control
**Files:** `PD & TORQUE/`
- **MATLAB Robotics Toolbox Integration**: Commercial robot models
- **PD Control for Regulation**: Position holding with gravity compensation
- **Computed Torque Control**: Trajectory tracking with full dynamics
  - Mass matrix computation
  - Coriolis and centrifugal terms
  - Gravity torque calculation
- **Control System Validation**: Error analysis and performance evaluation

**Key Learning Objectives:**
- Integrate commercial robot models
- Implement advanced control strategies
- Master dynamic model-based control
- Evaluate control system performance

## 🔧 Technical Requirements

### Software Dependencies
- **MATLAB/Simulink** (2020b or later recommended)
- **Simscape Multibody Toolbox**
- **Robotics System Toolbox**
- **Robot Library Data** (for commercial robot models)

### Hardware Requirements
- Standard computer capable of running MATLAB
- Sufficient RAM for multibody simulations (8GB+ recommended)

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/NotCello/RDC-practice.git
   cd RDC-practice
   ```

2. **Setup MATLAB environment:**
   - Add repository folders to MATLAB path
   - Ensure all required toolboxes are installed
   - Install Robot Library Data for commercial robot models

3. **Run exercises in order:**
   - Start with Session 1 basic examples
   - Progress through each session sequentially
   - Use provided templates and hints

## 📝 Exercise Guidelines

### Implementation Strategy
- **Modular Design**: Create reusable subsystems for robot components
- **Verification**: Always compare results with closed-form solutions when possible
- **Documentation**: Comment your models extensively
- **Testing**: Validate each component before integration

### Common Patterns
- Use PS-Simulink converters for signal interfacing
- Implement proper coordinate frame management
- Apply consistent naming conventions
- Create subsystems for complex robot structures

## 🎯 Key Algorithms Implemented

### Static Analysis
- **Jacobian Computation**: Both analytical and geometric approaches
- **Gravity Compensation**: Force-torque mapping using virtual work
- **Transform Management**: DH convention and frame relationships

### Dynamic Analysis
- **Newton-Euler Recursion**: Complete forward/backward algorithm
- **Closed-Form Dynamics**: Analytical equation derivation
- **Mass Matrix Methods**: Systematic dynamic parameter identification

### Control Systems
- **PID Control**: Basic tracking and regulation
- **Gravity Compensation**: Feedforward torque computation
- **Computed Torque**: Model-based trajectory tracking
- **Error Analysis**: Performance evaluation methods

## 📊 Robot Models Included

### Basic Models
- **1R Robot (Simple Pendulum)**: Fundamental dynamics understanding
- **2R Planar Robot**: Coupled multi-body dynamics
- **3R Planar Robot**: Extended kinematic chains

### Advanced Models
- **2R Non-Planar Robot**: 3D spatial dynamics
- **3R Non-Planar Robot**: Complex multi-body interactions
- **Commercial Robots**: UR10 and other industrial manipulators

## 🔍 Validation and Testing

### Model Verification
- Compare recursive algorithms with closed-form solutions
- Validate gravity compensation with static equilibrium tests
- Check trajectory tracking performance with error metrics

### Control Performance
- Steady-state error analysis
- Transient response evaluation
- Stability margin assessment
- Robustness testing with parameter variations

## 📚 Further Exercises

The repository includes additional challenges for exam preparation:
- **Model Variations**: Different link lengths, masses, and configurations
- **Advanced Control**: Impedance control and environment interaction
- **Custom Structures**: Design and implement novel robot configurations

## 🎓 Exam Preparation

### Recommended Approach
1. Complete all session exercises successfully
2. Implement variations on basic structures
3. Practice recursive algorithm implementation
4. Master both toolbox and custom implementations
5. Prepare working models in advance

### Key Skills to Master
- Serial robot modeling from scratch
- Gravity compensation implementation
- Newton-Euler recursive dynamics
- PD and computed torque control
- Model validation and testing

## 📖 References

- Course lecture slides and materials
- MATLAB Robotics System Toolbox documentation
- Simscape Multibody user guides
- Classic robotics textbooks (Craig, Spong, etc.)

## 👥 Contributors

- **Course Instructors**: Pedro Luis Figueroa Saire, Simone Borelli
- **Institution**: University of Genoa
- **Contact**: name.surname@edu.unige.it

## 📄 License

This repository contains educational materials for academic use. Please respect university policies regarding code sharing and collaboration.

---

**Note**: This repository is designed for educational purposes. All implementations should be thoroughly tested and validated before any practical application.
