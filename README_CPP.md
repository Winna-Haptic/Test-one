# Basketball Haptic Training System - C++ Version

**Standard C++ implementation for Visual Studio Code development**

## 🎯 What This Is

This is the **standard C++ version** of the basketball haptic training system, designed to work with Visual Studio Code and standard C++ compilers. Perfect for:

- ✅ **Development & Testing** - Test algorithms without hardware
- ✅ **Visual Studio Code** - Your preferred IDE
- ✅ **Standard C++** - No special frameworks needed
- ✅ **Cross-platform** - Works on Windows, Mac, Linux
- ✅ **Easy Debugging** - Standard debugging tools

## 📁 C++ Project Structure

```
├── src/                    # C++ source code
│   ├── main.cpp           # Main program (START HERE)
│   ├── sensors.h          # Sensor definitions
│   ├── haptic.h           # Haptic feedback control
│   └── data_logger.h      # Data logging & analysis
├── Makefile               # Build configuration
└── README_CPP.md          # This file
```

## 🚀 Quick Start

### 1. Open in Visual Studio Code
```bash
# Open the project folder in VS Code
code /path/to/your/project
```

### 2. Build & Run
```bash
# Build the project
make

# Run the program
make run

# Or build and run in one step
./basketball_trainer
```

### 3. Development Workflow
```bash
# Clean build files
make clean

# Debug build
make debug

# Format code
make format
```

## 🔧 Requirements

- **C++ Compiler** (g++ recommended)
- **Make** (for building)
- **Visual Studio Code** (your IDE)

**That's it!** No special libraries or frameworks needed.

## 💻 How It Works

### **Simulation Mode**
The C++ version simulates hardware components:
- **Sensors** - Generates realistic motion data
- **Haptic feedback** - Prints feedback messages
- **I2C communication** - Simulated with function calls
- **Timing** - Uses standard C++ chrono library

### **Real Hardware Integration**
When you're ready for hardware:
1. Keep the C++ logic
2. Replace simulation functions with actual sensor code
3. Add ESP32-specific libraries
4. Deploy to ESP32

## 🎯 Key Features

### ✅ **Complete Basketball Logic**
- Shot detection algorithms
- Form analysis calculations  
- Calibration system
- Performance tracking

### ✅ **Professional C++ Code**
- Standard C++17
- Clean class structure
- Proper memory management
- Cross-platform compatible

### ✅ **Easy Testing**
- No hardware required
- Instant compilation
- Standard debugging
- Unit test ready

## 🔄 Development Process

### **Phase 1: Algorithm Development**
1. **Develop in C++** - Test logic without hardware
2. **Perfect algorithms** - Shot detection, form analysis
3. **Debug easily** - Standard C++ debugging tools

### **Phase 2: Hardware Integration**
1. **Keep C++ structure** - Don't rewrite everything
2. **Replace simulation** - Add real sensor code
3. **Deploy to ESP32** - Use existing logic

## 📊 Program Flow

```cpp
main() 
├── setup()                 // Initialize systems
└── loop()                  // Main program loop
    ├── checkButtons()      // User input
    ├── handleStandby()     // Standby mode
    ├── handleCalibration() // Learning mode
    ├── handleTraining()    // Active training
    └── handleDataReview()  // Performance analysis
```

## 🎮 System States

- **STANDBY** - Ready, monitoring sensors
- **CALIBRATION** - Learning optimal form (10 shots)
- **TRAINING** - Active feedback during practice
- **DATA_REVIEW** - Show performance statistics

## 🔧 Customization

### **Adjust Thresholds**
```cpp
const double ELBOW_ANGLE_TOLERANCE = 5.0;  // degrees
const double WRIST_ANGLE_TOLERANCE = 3.0;  // degrees
const double SHOT_DURATION_MIN = 1.2;      // seconds
```

### **Modify Feedback**
```cpp
void provideHapticFeedback(const FreeThrowData& shotData) {
    // Customize feedback logic here
    if (elbowError > threshold) {
        // Strong feedback for elbow correction
    }
}
```

## 🚀 Next Steps

### **For Development:**
1. **Run the C++ version** - Test algorithms
2. **Modify parameters** - Tune for basketball
3. **Add features** - Enhance as needed

### **For Production:**
1. **Convert to Arduino** - Use the firmware/ folder files
2. **Deploy to ESP32** - Upload to hardware
3. **Test with sensors** - Real-world validation

## 💡 Why This Approach?

- **✅ Faster development** - No hardware needed
- **✅ Better debugging** - Standard tools
- **✅ Team collaboration** - Everyone can run it
- **✅ Algorithm focus** - Perfect the logic first
- **✅ Professional code** - Industry standard C++

## 🎯 Perfect for Startup Development

This C++ version lets you:
- **Develop algorithms quickly**
- **Test without hardware**  
- **Debug with standard tools**
- **Collaborate easily**
- **Prepare for production**

**Start here, perfect the algorithms, then deploy to hardware!**
