# datafun-02-automation
DataFun 02 — Automation Project (Brendon McNulty)

Automate basic project housekeeping tasks using Python. This script demonstrates repetition, branching, list comprehensions (as required), logging, and the standard main() + conditional execution pattern.

Repository Contents

brendon_project_setup.py — main script for this module (functions 1–5 and main()).

utils_brendon.py — Module 1 utilities (imports here to display your byline/tagline).

requirements.txt — packages needed for the project (install into .venv).

.gitignore — standard ignore rules.

project.log — log file created by the script (kept in the repo per class examples).

Setup

Create/activate a local virtual environment in the project root.

Install required packages:

python -m pip install --upgrade -r requirements.txt --timeout 100

How to Run

Execute the module directly to call main():

python brendon_project_setup.py


The script logs progress to the terminal and to project.log.

What the Script Does (Overview)

main() demonstrates five functions:

create_folders_for_range(start_year, end_year)
Creates year-named folders for an inclusive range (e.g., 2020, 2021, 2022, 2023).

create_folders_from_list(folder_list)
Creates one folder per list item (e.g., data-csv, data-excel, data-json).

create_prefixed_folders_using_list_comprehension(folder_list, prefix)
Uses a list comprehension to transform names and create prefixed folders
(e.g., output-csv, output-excel, output-json).

create_folders_periodically(duration_seconds)
Creates a small series of folders over time (e.g., periodic-1, periodic-2, periodic-3), pausing between each.

create_standardized_folders(folder_list, to_lowercase=True, remove_spaces=True)
Standardizes names (lowercase / remove spaces) and creates region folders
(e.g., northamerica, southamerica, europe, asia, africa, oceania, middleeast).

The script also imports your Module 1 utilities and logs your byline/tagline at the start of main().

Notes

Logging is handled with loguru; output is written to project.log.

List comprehensions are used where required.

The if __name__ == "__main__": main() guard is included so functions can be imported without running the script.