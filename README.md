# AutoPort - Automated Incident Report Generator

I built this Python tool to automate security incident reports at my hospital job. It turned a 45-minute manual process into a 5-minute one-click operation.

## Why I Built This

Working security at a healthcare facility means documenting everything. Tours, badge requests, equipment checks, patrol routes - all of it needs to go into the hospital's web-based incident system. Every single shift.

The problem was that filling out the same web forms over and over was killing productivity. Officers were spending more time typing reports than actually doing security work. Plus, manually entering the same info repeatedly led to typos and inconsistent formatting.

I needed something faster.

## How It Works

AutoPort is a tkinter GUI with pre-configured buttons for common shift tasks. Click a button, and it uses Selenium WebDriver to automatically fill out and submit the hospital's incident report form in the browser.

For routine stuff like building tours or equipment checks, it's literally one click. For custom incidents, there's a dialog box where you can add details, and it handles the rest.

## What I Used

- Python 3.x
- tkinter for the GUI
- Selenium WebDriver with Edge
- Hospital's existing web-based incident management system

## The Buttons

The interface has buttons for tasks I do every shift:
- Building tours (NDH Tour, Area Tour, Lights Out)
- ED post assignments
- Equipment checks (boiler, radios, keys)
- Special requests (OB badge access)
- Foot patrols with custom route tracking
- General custom reports

Each button auto-fills the incident type, location, timestamp, and description. The form validates everything before submission so nothing gets kicked back.

## Setting It Up

Clone the repo:
git clone https://github.com/yourusername/autoport.git

Install Selenium:
pip install selenium

Download Microsoft Edge WebDriver and update the driver path in the code to wherever you put it.

Note: This is configured for my hospital's specific incident system. You'd need to modify the form field IDs and values for a different setup.

## Running It

Just run the script:
python autoport.py

The GUI pops up with all the preset buttons. Click what you need, confirm if it asks for extra details, and it submits the report automatically.

## What It Actually Does

When you click a button, the script:
1. Launches Edge in the background
2. Navigates to the incident report page
3. Auto-fills date, time, facility, incident type, and description
4. Submits the form
5. Confirms submission

For foot patrols, there's a popup where you can add each location you checked. It builds the route description automatically.

## Real Results

Before AutoPort, filling out these reports took 30-45 minutes per shift depending on how busy it was. Now it's under 5 minutes total.

The security team processes over 100 incidents monthly. That time savings adds up, and officers can actually focus on security instead of paperwork.

Also eliminated the inconsistency problem. Every report follows the same format now, which matters for legal documentation.

## What I Might Add Later

- SQLite database to track submission history
- Export logs to PDF for backup records
- Configuration file instead of hardcoded paths
- Multi-facility support if other sites want to use it
- Better error logging for troubleshooting

## Notes

This is customized for Nuvance Health's incident system. The form field IDs, facility codes, and incident types are specific to their setup. If you want to adapt this for another system, you'll need to inspect their web forms and update the Selenium selectors.

## Contact

Thomas Marvin
thomasmarvin123@gmail.com
GitHub: https://github.com/yourusername/autoport
