# DataVisualization-Lab-3
Marks and Section: these come from students_marks.csv.
Load it with csv.DictReader.
Convert the five marks (Math, Stats, Python, Databases, English) with int().
Add Average as the sum divided by 5, rounded to 2 decimals.
City and Hostel: these come from students_info.json.
Load it with json.load.
Read the city as s["Contact"]["City"], because it is nested inside Contact.
Hostel is already true/false.
FeeStatus: this comes from the fees table in university.db.
Read RollNo, DueDate and PaidOn using SQLAlchemy and text().
If PaidOn is None, the status is “Unpaid”.
If PaidOn is after DueDate, the status is “Late”.
Otherwise, the status is “On time”.
Compare the dates with datetime.strptime(..., "%Y-%m-%d").
Joining: RollNo appears in all three sources.
Build dictionaries keyed by RollNo, such as info_by_roll[roll] and fees[roll].
Loop over the students and combine the fields into one dictionary each.
Saving and printing:
Write the list with json.dump(full, f, indent=2).
Print len(full), which should be 25.
Print full[0], the first record.
