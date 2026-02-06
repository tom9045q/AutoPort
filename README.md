# AutoPort - Automated Incident Report Generator

A Python GUI tool that automates incident report generation for security operations, cutting report creation time in half.

## The Problem

Security officers at healthcare facilities deal with 100+ incidents every month. Each one needs detailed documentation for hospital leadership, law enforcement, and legal compliance (reports have to be court-admissible).

Writing these reports manually was eating up huge amounts of time, creating inconsistencies between different officers' reports, and keeping the security team stuck at desks instead of doing actual security work.

## What AutoPort Does

AutoPort is a simple GUI that:
- Auto-fills standardized incident report templates
- Validates entries so nothing gets submitted incomplete
- Cuts report time from 45 minutes down to 5 minutes (89% faster)

## Built With

- Python 3.x for the core logic
- tkinter for the GUI
- Standard Python libraries for file handling and validation
- Runs on Windows 10/11

## Features

- Easy-to-use interface - I tested it with officers across different age groups and experience levels. Everyone picked it up without issues.
- Auto-fill templates - Enter your incident details once, and it populates the whole report
- Validation - Won't let you submit if required fields are missing or formatted wrong
- Export ready - Generates reports that are ready to submit immediately
- Actually in use - This isn't just a side project sitting on GitHub. It's deployed and used every day by our security team.

## Setup

Clone it:
git clone https://github.com/yourusername/autoport.git

Go to the folder:
cd autoport

Install what you need:
pip install selenium

You'll also need the dev version of Microsoft Edge installed.

## How to Use It

1. Fire up the application
2. Fill out the incident form:
   - When it happened
   - Where it happened
   - Who was involved
   - What happened
   - What you did about it
3. Hit "Generate Report"
4. Double-check it and export

## Real Impact

- Time saved: 89% reduction (45 min to 5 min per report)
- Volume: Handles 100+ incidents monthly
- Accuracy: No more typos or missed fields from manual entry

## What's Next

I'm thinking about adding:
- A database backend to track incidents over time and spot trends
- Direct PDF export
- Multi-user access with different permission levels
- Hooks into the hospital's existing incident management system
- Automatic routing so reports go to the right people

## Want to Contribute?

This started as a portfolio project, but I'm open to feedback. If you've got ideas or spot bugs, feel free to open an issue or PR.

## Contact

Thomas Marvin  
thomasmarvin123@gmail.com  
GitHub: https://github.com/yourusername/autoport
