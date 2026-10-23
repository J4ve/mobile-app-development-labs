# CCCS 106 Projects 
Application Development and Emerging Technologies 
Academic Year 2025-2026 

## Student Information
- **Name:** Jave Atanacio Bacsain
- **Student ID:** 231003016
- **Program:** Bachelor of Science in Computer Science
- **Section:** BSCS-3A

## Repository Structure 

### Week 1 Labs - Environment Setup and Python Basics
- `week1_labs/hello_world.py` - Basic Python introduction
- `week1_labs/basic_calculator.py` - Simple console calculator

### Week 2 Labs - Git and Flet GUI Development
- `week2_labs/hello_flet.py` - First Flet GUI application
- `week2_labs/personal_info_gui.py` - Enhanced personal information manager
- `week2_labs/enhanced_calculator.py` - GUI calculator (coming soon)

### Module 1 Final Project
- `module1_final/` - Final integrated project (TBD)

## Technologies Used
- **Python 3.8+** - Main programming language
- **Flet 0.28.3** - GUI framework for cross-platform applications
- **Git & GitHub** - Version control and collaboration
- **VS Code** - Integrated development environment

## Development Environment
- **Virtual Environment:** cccs106_env
- **Python Packages:** flet==0.28.3
- **Platform:** Windows 10/11

## Results
The Week 1 and Week 2 programs are marked completed in their lab reports, and each of the 5 added features in the Module 6 weather app has a screen recording.

| Lab | Result | Evidence |
|---|---|---|
| Week 1 | `hello_world.py` runs on Python 3.12.0. `basic_calculator.py` prints "Cannot divide by zero" for 1.0 / 0.0 and rejects text input. | [LAB1_REPORT.md](week1_labs/LAB1_REPORT.md), [screenshots](week1_labs/lab1_screenshots/) |
| Week 2 | `hello_flet.py` and `personal_info_gui.py` work. The form generates a student profile. | [LAB2_REPORT.md](week2_labs/LAB2_REPORT.md), [screenshots](week2_labs/lab2_screenshots/) |
| Module 6 | All 6 base features are checked off. Each of the 5 added features (search history, current location, 5-day forecast, offline cache, watchlist) has a screen recording. | [mod6_labs/README.md](mod6_labs/README.md), [recordings](mod6_labs/assets/gifs/) |

To test the weather service, add an OpenWeatherMap key to `mod6_labs/.env` (template in `.env.example`) and run `python test_weather_service.py` from `mod6_labs/`. It checks a valid city (London), an invalid city and an empty city name.

Week 3 (login app), Week 4 (contact book) and the sample APK build have code only, with no screenshots or lab reports.

## How to Run Applications

### Prerequisites
1. Python 3.8+ installed
2. Virtual environment activated: `cccs106_env\Scripts\activate`
3. Flet installed: `pip install flet==0.28.3`

### Running GUI Applications
```cmd
# Navigate to project directory
cd week2_labs

# Run applications
python hello_flet.py
python personal_info_gui.py
