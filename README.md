# HR Analytics Dashboard

A comprehensive HR Analytics solution built with Power BI to analyze employee attrition, workforce demographics, performance metrics, and organizational insights. This project helps HR professionals and management make data-driven decisions to improve employee retention and optimize workforce management.

## 📊 Project Overview

This Power BI dashboard provides deep insights into human resources metrics, focusing on employee attrition patterns, demographic analysis, performance tracking, and satisfaction levels across the organization. The analytics enable HR teams to identify risk factors, understand employee behavior, and implement targeted retention strategies.

## 🎯 Business Objectives

- 📉 **Monitor Attrition Rate** - Track and analyze employee turnover (16.08% overall attrition)
- 👥 **Workforce Demographics** - Understand employee composition by age, gender, department, and role
- 💼 **Performance Analysis** - Evaluate performance ratings and identify high performers
- 😊 **Employee Satisfaction** - Measure job satisfaction, work-life balance, and environment satisfaction
- 💰 **Compensation Insights** - Analyze salary distribution and its impact on retention
- 🎯 **Identify Risk Factors** - Pinpoint departments, roles, and segments with high attrition
- 📈 **Trend Analysis** - Understand patterns in tenure, promotions, and career progression

## 📁 Project Structure

```
HR-Analytics/
├── HR_Analytics.pbix          # Power BI dashboard with interactive visualizations
├── HR_Analytics.csv           # Employee dataset (1,480 records)
└── README.md                  # Project documentation
```

## 📈 Dataset Overview

### Dataset Statistics
- **Total Employees**: 1,480 records
- **Total Attributes**: 38 comprehensive HR metrics
- **Overall Attrition Rate**: 16.08% (238 employees left)
- **Active Employees**: 1,242 (83.92%)

### Key Metrics Included

#### 1. **Employee Identification**
- `EmpID` - Unique employee identifier
- `EmployeeNumber` - Employee number
- `EmployeeCount` - Count flag

#### 2. **Demographics**
- `Age` - Employee age (18-60 years)
- `AgeGroup` - Age brackets (18-25, 26-35, 36-45, 46-55, 55+)
- `Gender` - Male (60.06%) / Female (39.94%)
- `MaritalStatus` - Married, Single, Divorced
- `DistanceFromHome` - Commute distance in miles

#### 3. **Employment Information**
- `Department` - Research & Development (65.3%), Sales (30.4%), HR (4.3%)
- `JobRole` - 9 different roles (Sales Executive, Research Scientist, etc.)
- `JobLevel` - Career level (1-5)
- `BusinessTravel` - Travel frequency (Rarely, Frequently, Non-Travel)
- `OverTime` - Overtime work (Yes/No)

#### 4. **Experience & Tenure**
- `TotalWorkingYears` - Total career experience
- `YearsAtCompany` - Tenure at current company
- `YearsInCurrentRole` - Time in current position
- `YearsSinceLastPromotion` - Years since last promotion
- `YearsWithCurrManager` - Reporting relationship duration
- `NumCompaniesWorked` - Previous employers

#### 5. **Education**
- `Education` - Education level (1-5 scale)
- `EducationField` - Degree field (Life Sciences, Medical, Marketing, Technical, HR, Other)

#### 6. **Compensation**
- `MonthlyIncome` - Monthly salary
- `SalarySlab` - Salary brackets:
  - Upto 5k (50.9%)
  - 5k-10k (30.0%)
  - 10k-15k (10.1%)
  - 15k+ (9.0%)
- `HourlyRate` - Hourly pay rate
- `DailyRate` - Daily compensation
- `MonthlyRate` - Monthly rate
- `PercentSalaryHike` - Recent salary increase percentage
- `StockOptionLevel` - Stock options (0-3)

#### 7. **Performance & Satisfaction**
- `PerformanceRating` - Performance score (3-4 scale)
  - Rating 3: 84.66%
  - Rating 4: 15.34%
- `JobSatisfaction` - Job satisfaction level (1-4)
- `EnvironmentSatisfaction` - Workplace satisfaction (1-4)
- `RelationshipSatisfaction` - Manager relationship satisfaction (1-4)
- `WorkLifeBalance` - Work-life balance rating (1-4)

#### 8. **Engagement**
- `JobInvolvement` - Job involvement level (1-4)
- `TrainingTimesLastYear` - Training sessions attended

#### 9. **Target Variable**
- `Attrition` - Employee departure status (Yes/No)

## 🔍 Key Insights & Findings

### Attrition Analysis

#### Overall Attrition
- **Total Attrition Rate**: 16.08% (238 out of 1,480 employees)
- **Active Workforce**: 83.92% (1,242 employees)

#### Attrition by Department
| Department | Attrition Rate |
|------------|----------------|
| Sales | 20.67% (Highest) |
| Human Resources | 19.05% |
| Research & Development | 13.75% (Lowest) |

#### Attrition by Job Role (Top 5 Highest)
| Job Role | Attrition Rate |
|----------|----------------|
| Sales Representative | 39.29% ⚠️ |
| Laboratory Technician | 23.75% |
| Human Resources | 23.08% |
| Sales Executive | 17.63% |
| Research Scientist | 16.04% |

**Critical Finding**: Sales Representatives have the highest attrition rate at nearly 40%, indicating a need for immediate retention strategies in this role.

### Workforce Demographics

#### Age Distribution
- **26-35 years**: 41.28% (Largest segment)
- **36-45 years**: 31.82%
- **46-55 years**: 15.41%
- **18-25 years**: 8.31%
- **55+ years**: 3.18%

#### Gender Distribution
- **Male**: 60.06% (889 employees)
- **Female**: 39.94% (591 employees)

#### Marital Status
- **Married**: 45.88% (679 employees)
- **Single**: 31.96% (473 employees)
- **Divorced**: 22.16% (328 employees)

### Compensation Analysis

#### Salary Distribution
- **Upto 5k**: 50.88% (753 employees) - Entry to mid-level
- **5k-10k**: 30.00% (444 employees) - Mid-level
- **10k-15k**: 10.14% (150 employees) - Senior level
- **15k+**: 8.99% (133 employees) - Executive level

**Insight**: Majority of employees (80.88%) earn below 10k monthly, suggesting opportunities for competitive compensation strategies.

### Work Patterns

#### Business Travel
- **Travel Rarely**: 70.41% (1,042 employees)
- **Travel Frequently**: 18.85% (279 employees)
- **Non-Travel**: 10.20% (151 employees)

#### Overtime Work
- **No Overtime**: 71.76% (1,062 employees)
- **Overtime**: 28.24% (418 employees)

**Finding**: Over 28% of employees work overtime, which may correlate with work-life balance and attrition.

### Performance & Satisfaction

#### Performance Distribution
- **Rating 3** (Good): 84.66% (1,253 employees)
- **Rating 4** (Excellent): 15.34% (227 employees)

#### Work-Life Balance
- **Level 3** (Good): 60.74% (899 employees)
- **Level 2** (Fair): 23.38% (346 employees)
- **Level 4** (Excellent): 10.41% (154 employees)
- **Level 1** (Poor): 5.47% (81 employees)

### Education Background

#### Education Fields
- **Life Sciences**: 41.01% (607 employees)
- **Medical**: 31.76% (470 employees)
- **Marketing**: 10.88% (161 employees)
- **Technical Degree**: 8.92% (132 employees)
- **Other**: 5.61% (83 employees)
- **Human Resources**: 1.82% (27 employees)

## 📊 Power BI Dashboard Features

### Key Visualizations

#### 1. **Executive Summary KPIs**
- Total Employee Count
- Attrition Rate (%)
- Average Age
- Average Monthly Income
- Average Years at Company
- Active vs Attrited Employees

#### 2. **Attrition Analysis**
- Attrition by Department (Bar Chart)
- Attrition by Job Role (Horizontal Bar)
- Attrition by Age Group (Column Chart)
- Attrition by Salary Slab (Stacked Bar)
- Attrition by Gender (Pie/Donut Chart)
- Attrition Trend by Tenure (Line Chart)

#### 3. **Demographic Insights**
- Age Group Distribution (Histogram)
- Gender Distribution (Pie Chart)
- Marital Status Breakdown (Donut Chart)
- Department Headcount (Tree Map)
- Job Role Distribution (Stacked Column)

#### 4. **Compensation Analysis**
- Salary Distribution by Department (Box Plot)
- Salary Slab Analysis (Stacked Bar)
- Salary Hike Distribution (Histogram)
- Income vs Attrition (Scatter Plot)

#### 5. **Performance Metrics**
- Performance Rating Distribution (Gauge)
- Job Satisfaction Levels (Stacked Bar)
- Work-Life Balance Scores (Column Chart)
- Environment Satisfaction (Heat Map)

#### 6. **Experience & Tenure**
- Years at Company Distribution (Area Chart)
- Years Since Last Promotion (Column Chart)
- Total Working Years Analysis (Line Chart)
- Tenure vs Attrition Correlation

### Interactive Elements

**Slicers & Filters**:
- Department
- Job Role
- Age Group
- Gender
- Salary Slab
- Attrition Status
- Marital Status
- Overtime (Yes/No)
- Business Travel Frequency

**Drill-Through Capabilities**:
- Employee-level details
- Department deep dive
- Role-specific analysis

**Cross-Filtering**:
- Dynamic interaction across all visuals
- Multi-select filters for complex analysis

## 🛠️ Tools & Technologies

| Component | Technology |
|-----------|-----------|
| **Data Source** | CSV (1,480 records) |
| **ETL & Cleaning** | Power Query |
| **Data Modeling** | Power BI Data Model |
| **Calculations** | DAX (Data Analysis Expressions) |
| **Visualization** | Power BI Desktop |
| **Analytics** | Statistical Analysis, Correlation |

## 💡 Business Recommendations

Based on the analysis, key recommendations include:

### 1. **Address Sales Representative Attrition (39.29%)**
- Immediate intervention required
- Review compensation and incentive structure
- Improve career progression opportunities
- Enhance work-life balance initiatives

### 2. **Focus on Sales Department (20.67% attrition)**
- Department-wide retention program
- Competitive salary benchmarking
- Professional development opportunities
- Mentorship programs

### 3. **Compensation Strategy**
- Review salary competitiveness for lower slabs (50% earn <5k)
- Implement performance-based incentives
- Regular market salary surveys
- Transparent promotion criteria

### 4. **Work-Life Balance Improvements**
- Reduce overtime requirements (28% currently work OT)
- Flexible work arrangements
- Wellness programs
- Mental health support

### 5. **Career Development**
- Structured promotion timelines
- Skills development programs
- Clear career paths for each role
- Regular performance reviews

### 6. **Early Tenure Retention**
- Enhanced onboarding programs
- First-year check-ins
- Mentorship for new hires
- Clear expectations setting

## 🚀 Getting Started

### Prerequisites
- Power BI Desktop (latest version)
- Microsoft Excel (optional, for CSV viewing)

### Installation

1. **Clone the Repository**
```bash
git clone https://github.com/AdityaSingh7764/HR-Analytics.git
cd HR-Analytics
```

2. **Open Power BI Dashboard**
- Launch Power BI Desktop
- Open `HR_Analytics.pbix`
- Data source is embedded in the file

3. **Explore the Dashboard**
- Navigate through different report pages
- Use slicers to filter data
- Hover over visuals for detailed tooltips
- Click on charts for cross-filtering

### Updating Data

To refresh with new data:
1. Open Power BI file
2. Go to Home → Transform Data
3. Update the CSV file path
4. Click Close & Apply
5. Save the updated report

## 📊 DAX Measures Examples

```dax
// Total Employees
Total Employees = COUNT('HR_Analytics'[EmpID])

// Attrition Count
Attrition Count = 
    CALCULATE(
        COUNT('HR_Analytics'[EmpID]),
        'HR_Analytics'[Attrition] = "Yes"
    )

// Attrition Rate
Attrition Rate = 
    DIVIDE(
        [Attrition Count],
        [Total Employees],
        0
    )

// Average Monthly Income
Avg Monthly Income = AVERAGE('HR_Analytics'[MonthlyIncome])

// Active Employees
Active Employees = 
    CALCULATE(
        COUNT('HR_Analytics'[EmpID]),
        'HR_Analytics'[Attrition] = "No"
    )

// Attrition by Department
Dept Attrition Rate = 
    DIVIDE(
        CALCULATE([Attrition Count]),
        CALCULATE([Total Employees]),
        0
    )

// Average Tenure
Avg Tenure = AVERAGE('HR_Analytics'[YearsAtCompany])

// High Performer Count
High Performers = 
    CALCULATE(
        COUNT('HR_Analytics'[EmpID]),
        'HR_Analytics'[PerformanceRating] = 4
    )
```

## 🎓 Use Cases

This dashboard is valuable for:

### HR Professionals
- ✅ Monitor attrition trends
- ✅ Identify retention risks
- ✅ Plan recruitment strategies
- ✅ Optimize compensation packages

### Management
- ✅ Workforce planning
- ✅ Budget allocation
- ✅ Performance management
- ✅ Strategic decision-making

### Department Heads
- ✅ Team composition analysis
- ✅ Talent retention
- ✅ Performance tracking
- ✅ Resource planning

### Analysts
- ✅ Predictive modeling
- ✅ Trend analysis
- ✅ Correlation studies
- ✅ Benchmarking

## 🔄 Potential Enhancements

- **Predictive Analytics**: Machine learning model to predict attrition risk
- **Sentiment Analysis**: Employee feedback text analysis
- **Real-time Updates**: Connect to live HR database
- **Mobile Optimization**: Power BI Mobile app configuration
- **Advanced Segmentation**: Clustering analysis for employee personas
- **Exit Interview Integration**: Qualitative data incorporation
- **Benchmarking**: Industry comparison metrics
- **Automated Alerts**: Email notifications for critical metrics

## 🤝 Contributing

Contributions are welcome! To contribute:
1. Fork the repository
2. Create a feature branch
3. Make your enhancements
4. Submit a pull request

Suggestions for improvement:
- Additional DAX measures
- New visualizations
- Enhanced data model
- Documentation improvements

## 📧 Contact

**Aditya Singh**
- GitHub: [@AdityaSingh7764](https://github.com/AdityaSingh7764)

## 📄 License

This project is available for educational and analytical purposes.

---

## 📚 Key Learnings

This project demonstrates:
- ✅ HR analytics best practices
- ✅ Power BI dashboard design
- ✅ DAX calculations for HR metrics
- ✅ Data visualization techniques
- ✅ Attrition analysis methodologies
- ✅ Business intelligence storytelling
- ✅ Data-driven HR decision making

---

## 🔍 Technical Highlights

- **Dataset**: 1,480 employee records across 38 attributes
- **Attrition Rate**: 16.08% overall
- **Critical Finding**: Sales Representatives at 39.29% attrition
- **Departments Analyzed**: 3 (R&D, Sales, HR)
- **Job Roles**: 9 distinct positions
- **Salary Slabs**: 4 compensation tiers
- **Age Groups**: 5 demographic segments
- **Interactive Slicers**: 8+ filter options

---

⭐ **If you found this project helpful, please consider giving it a star!**

*Data-driven insights for human resources management and employee retention*
