
# CareerLens

A predictive analytics platform for personalized career navigation that bridges the gap between academic preparation and workforce readiness.

## Table of Contents
- [Description](#description)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Roadmap](#roadmap)
- [Database Structure](#database-structure)
- [Contributing](#contributing)
- [Team](#team)
- [License](#license)

## Description

CareerLens functions as an employment analytics application which enables students together with career advisors to base their career decisions on data sets. The predictive algorithms on the platform compare student information including academic records and skills with their preferences to discover perfect career choices. Additionally, the system offers market analytics tools to career advisors.

Therefore, the application deals with this issue by providing the user with, industry reports, professional profiles, salary data, and information about job market trends that are consolidated into one database and that contain recommendations specifically for the user.

## Expected Project Structure

```
careerlens/
├── data/
│   ├── career_prediction/
│   ├── salary_prediction/
│   └── job_skills_mapping/
├── src/
│   ├── database/
│   │   ├── schema.py
│   │   └── data_validation.py
│   ├── algorithms/
│   │   ├── prediction_models.py
│   │   ├── skill_matching.py
│   │   └── salary_estimation.py
│   ├── ui/
│   │   ├── student_interface/
│   │   └── advisor_interface/
│   └── main.py
├── tests/
│   ├── test_database.py
│   ├── test_algorithms.py
│   └── test_ui.py
├── requirements.txt
├── docs/
│   ├── project_charter.md
│   └── roadmap.md
└── README.md
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Durgasowmyasri/Carrer-lens.git
cd career-lens
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up the database:
```bash
python src/database/schema.py
```

5. Load initial data:
```bash
python src/database/data_validation.py
```

## Usage

### For Students

To launch the student interface:
```bash
python src/main.py --mode student
```

This will open the CareerLens student dashboard where you can:
1. Complete your profile and skills assessment
2. View your recommended career paths
3. Explore job matches based on your profile
4. Identify skill gaps and find resources to improve them
5. Connect with your assigned career advisor

### For Career Advisors

To launch the advisor interface:
```bash
python src/main.py --mode advisor
```

The advisor dashboard provides:
1. Job market trends and analytics
2. Salary benchmarking tools
3. Skills demand visualization
4. Student management and guidance tools
5. Customizable filters for data exploration

## Features

### Student Interface
- **Profile completion tracking**: Visual indicator of profile completeness
- **Career path visualization**: Four-step journey (Assessment → Matching → Development → Application)
- **Skills analysis dashboard**: Identification of strengths and improvement areas
- **Personalized job matches**: Recommendations with match percentage scores
- **Advisor connection**: Direct access to assigned career counselor

### Advisor Interface
- **Interactive market filters**: Customize data views by industry, location, experience level
- **Job market trend visualization**: Visual representation of demand across different roles
- **Salary distribution analysis**: Compensation trends by experience level
- **In-demand skills tracking**: Detailed breakdown with growth trends and salary impact
- **Student management tools**: Track and guide multiple students

### Core Technology
- **Career Role Suggestion Engine**: Analyzes academic performance and skills
- **Skills-Role Matching System**: Maps user skills to relevant job roles
- **Salary Prediction Module**: Provides expected salary ranges based on profile

## Roadmap

Our development timeline spans from January 2025 to June 2025:

1. **Project Kick-Off** (January 2025)
   - Team formation
   - Initial requirements gathering
   - Project charter creation

2. **Database Design & Implementation** (February 2025)
   - Schema diagrams
   - SQLite3 tables implementation
   - Data source integration

3. **Core Algorithm Development** (March 2025)
   - Prediction models
   - Skill matching logic
   - Salary estimation algorithms

4. **User Interface Design** (April 2025)
   - UI wireframes
   - Student interface implementation
   - Advisor interface implementation

5. **Testing & Refinement** (May 2025)
   - User testing
   - Bug fixing
   - Performance optimization

6. **Platform Launch** (June 2025)
   - Deployment
   - User onboarding
   - Post-launch monitoring

## Database Structure

The CareerLens application uses SQLite3 with three primary tables:

1. **Career_Prediction**: Contains student academic performance metrics, skills assessments, and career preferences that drive the role suggestion engine.

2. **Salary_Prediction**: Stores salary data across various job titles, experience levels, education backgrounds, and locations to power the compensation forecasting module.

3. **Job_Skills_Mapping**: Maintains relationships between job roles and required skills, enabling the system to perform skill gap analysis and matching to employment opportunities.

## Contributing

We welcome contributions to the CareerLens project! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

For major changes, please open an issue first to discuss what you would like to change.

## Team

This is  being developed by Group 15:

- **Mounika Dadi** - Project Sponsor
- **Durga Sowmya Sri Madineni** - Project Manager
- **Vishnu Vardham Naidu Madhineni** - Team Member
- **Anjali Mailavarapu** - Customer
- **Akash Cherukuri** - Subject Matter Expert

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


Advisor Dashboard

 ![image](https://github.com/user-attachments/assets/e22b5121-f25a-416d-b0dc-666db20ab1c9)

Student Dashboard

![image](https://github.com/user-attachments/assets/ac6a716c-c231-4da2-a166-325f9db6791c)

 
