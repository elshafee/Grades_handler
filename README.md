# 📊 Horus University Grades Tool

A professional-grade web application for managing, converting, and validating student grades for Horus University. Developed by ESSIC.

---

## 🎯 Overview

The Horus Grades Tool is a comprehensive solution designed to streamline grade management workflows in educational institutions. It provides two main functionalities:

1. **Grade Converter** - Transform grades between different bylaw standards and formats
2. **Grade Checker** - Validate and compare grade files for consistency and accuracy

This tool eliminates manual errors and saves significant time when processing student records across multiple grading systems.

---

## ✨ Features

### 🔄 Grade Converter
- **Multi-Format Support**: Handle three distinct grading bylaws
  - **Bylaw 2025**: Modern grading system with Midterm, Final Term, Class Work, and Experimental/Oral components
  - **Bylaw 2018**: Traditional system including Quiz, Midterm, Final Term, Activity, Oral, and Course Work
  - **Online Mode**: Direct Microsoft Forms integration for remote assessments
  
- **Flexible Exports**: Select which grade components to export
- **Automatic Email Domain Configuration**: Append institution-specific email domains (default: @horus.edu.eg)
- **Batch Processing**: Generate multiple output files in a single conversion
- **Drag-and-Drop Upload**: Intuitive file handling

### ✅ Grade Checker
- **Multi-File Validation**: Compare original grades against converted output files
- **Detailed Discrepancy Reports**: 
  - Matching grades (✓)
  - Value differences (⚠)
  - Missing student records (●)
  - Extra/unexpected entries (+)
- **Flexible Comparison Modes**:
  - Standard mode for traditional grading systems
  - Online mode for Microsoft Forms exports
- **Column-Smart Matching**: Intelligently identifies and matches grade columns
- **Comprehensive Analytics**: Summary statistics and per-file reports

### 🎨 User Experience
- **Modern, Intuitive Interface**: Clean design with professional styling
- **Real-Time Feedback**: Progress indicators and detailed logging
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Visual Status Indicators**: Color-coded summaries (success, warning, error)
- **Download Management**: Individual or batch download options

---

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Excel files (.xlsx or .xls format)
- No installation required

### Usage

#### Converting Grades
1. Navigate to the **Converter** tab
2. Upload your Excel grades file
3. Select the appropriate bylaw standard
4. Configure email domain (if needed)
5. Choose which grade components to export
6. Click "Convert & Generate Files"
7. Download the generated files

#### Checking Grades
1. Navigate to the **Checker** tab
2. Upload the original grades file
3. Upload one or more converted output files
4. Select the output file type (Standard or Online)
5. Configure the email domain
6. Click "Compare Files"
7. Review the detailed comparison report

---

## 📋 File Format Requirements

### Input Files
- **Format**: Excel (.xlsx or .xls)
- **Required Column**: "Code" (student ID)
- **Optional Columns**: "Student Name" or "Name"
- **Grade Columns**: Depending on selected bylaw

### Output Files
Standard output contains the following columns:
- ID
- Start time
- Completion time
- Email
- Name
- Total points
- Quiz feedback
- Question
- Points - Question
- Feedback - Question

---

## 🛠 Technical Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Spreadsheet Processing**: [XLSX.js](https://sheetjs.com/)
- **Font Family**: Inter (UI), IBM Plex Mono (Code)
- **Styling**: Custom CSS with CSS variables for theming
- **Architecture**: Single-page application (SPA) with modular JavaScript

---

## 🎓 Bylaw Standards

### Bylaw 2025
Modern grading structure optimized for comprehensive assessment:
- **Components**: Midterm, Final Term, Class Work, Exp./Oral, Note
- **Use Case**: Current academic year evaluations

### Bylaw 2018
Traditional grading methodology:
- **Components**: Quiz, Midterm, Final Term, Activity, Oral, Course Work, Note
- **Use Case**: Legacy system compatibility, historical records

### Online Mode
Specialized format for remote assessment:
- **Source**: Microsoft Forms exports
- **Components**: Email, Total Points
- **Use Case**: Distance learning, exam portals

---

## 📊 Key Functions

### Grade Processing
- Automatic numeric normalization (removes .0 from whole numbers)
- Email domain auto-appending for online mode
- Invalid row filtering
- Column header detection and matching

### Validation Engine
- Numeric equality comparison (tolerance: 0.001)
- Case-insensitive string matching
- Fuzzy column name matching for robust detection
- Comprehensive discrepancy classification

---

## 💾 Supported File Operations

- **Upload**: Drag-and-drop or click-to-browse
- **Download**: Individual files or batch download with 300ms intervals
- **Multiple File Handling**: Process multiple output files simultaneously
- **Clear/Remove**: Delete uploaded files from the interface

---

## 🔐 Privacy & Security

- All processing happens **in-browser** using JavaScript
- No files are uploaded to external servers
- No data is stored or logged
- Your information remains completely private

---

## 🐛 Troubleshooting

### Common Issues

**"Could not find 'Code' column"**
- Ensure your input file contains a column labeled "Code"
- Check for typos in column headers
- Verify the header row is within the first 10 rows

**"No valid rows found"**
- Verify that the Code column contains numeric student IDs
- Check for blank or corrupted rows
- Ensure data rows follow the header row

**"Column mismatch in Checker"**
- Ensure the input and output files use the same bylaw standard
- Verify column names are spelled correctly
- Try manual column selection in Online mode

**Browser Compatibility**
- Use a modern browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Clear browser cache if experiencing UI glitches

---

## 📝 License

This project is licensed under the **Apache License 2.0**. See the LICENSE file for details.

---

## 👥 Credits

**Developed by**: Ahmad K. Elshafee @ ESSIC  
**Institution**: Horus University  
**Version**: 1.0.0

---

## 📮 Support & Feedback

For issues, questions, or feature requests, please create an issue in the repository.

---

## 🗺️ Roadmap

- [ ] Direct database integration
- [ ] Scheduled batch processing
- [ ] Advanced analytics dashboard
- [ ] User authentication & role management
- [ ] Grade curve analysis
- [ ] Custom bylaw builder
- [ ] API for third-party integrations

---

**Made with ❤️ for academic excellence**
