# AI-Based Timetable Generation System (NEP 2020 Aligned)

An intelligent and responsive web-based timetable generation system designed to automatically create conflict-free academic timetables using a Constraint Satisfaction Problem (CSP) approach. The project supports teacher-wise scheduling, classroom allocation, batch filtering, CSV import, Excel/PDF export, and teacher workload analytics.

This system is especially useful for colleges and universities following the flexible and multidisciplinary structure encouraged by **NEP 2020**, where departments, batches, labs, and teachers need efficient timetable planning.

---

## Project Overview

The **AI-Based Timetable Generation System** is a frontend-based application built using **React.js**, **HTML**, **CSS**, and **JavaScript**. It helps generate academic timetables by considering important constraints such as:

- Teacher availability conflict
- Classroom conflict
- Batch conflict
- Lab subject double-slot allocation
- Department-wise filtering
- Batch-wise filtering
- Teacher-wise timetable view

The application uses a **CSP-based backtracking algorithm with forward checking and MRV heuristic** to generate optimized timetables. If CSP scheduling fails, the system also provides a fallback timetable generation method.

---

## Features

### Smart Timetable Generation

The system uses CSP scheduling to assign subjects into available days and slots while avoiding conflicts between teachers, classrooms, and batches.

### NEP 2020 Aligned Structure

The project supports flexible timetable planning for different departments, batches, teachers, classrooms, and lab sessions, making it suitable for multidisciplinary academic systems.

### Add Subjects Manually

Users can manually add subject details such as:

- Subject name
- Teacher name
- Classroom
- Batch
- Department
- Day
- Slot

### CSV Import

Users can import timetable or subject data using a `.csv` file. The system reads the CSV file and converts it into timetable entries.

### Generate from CSV

After importing CSV data, users can directly generate the timetable from the uploaded file.

### Export Timetable

The generated timetable can be exported in:

- Excel format
- PDF format

The project uses XLSX for Excel export and jsPDF/html2canvas for PDF generation.

### Teacher Analytics

The system provides analytics such as:

- Total teachers
- Total rooms used
- Total classes
- Workload by teacher
- Busiest day of each teacher
- Rooms assigned to each teacher
- Batches handled by each teacher
- Departments handled by each teacher

### Filters

The timetable can be filtered by:

- Department
- Batch
- Teacher

This makes it easier to view specific schedules.

### Recess Slot

Users can select a recess/break slot dynamically from the available time slots.

### Local Storage Support

The system stores subjects, imported data, timetable, and settings in browser local storage, so data is not lost after refreshing the page.

### Responsive User Interface

The interface is fully responsive and works on desktop, tablet, and mobile screens.

---

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Core logic |
| React.js | Frontend UI components |
| Babel | Running JSX in browser |
| XLSX.js | Export timetable to Excel |
| jsPDF | Export timetable to PDF |
| html2canvas | Convert timetable view into image for PDF |
| LocalStorage | Save data in browser |
