# Data_Cleaning_Assignment2
•	Named the empty column:
o	1st column has a unique value, but the heading is missing. So named it “Unique ID”.
•	Created Query 14 and Response 14:
o	Query 14 was created by combining the 2nd questions from Query 8 and Query 9 (i.e., the two questions you wanted to split). You concatenated both questions into one column for clarity.
o	Response 14 was created similarly by combining the corresponding Response 8 and Response 9.
•	Synced Missing Values:
o	when Query 3 or Response 3 were NULL or blank, the corresponding Query 12 and Response 12 were also set to NULL to maintain data integrity and avoid inconsistencies.
•	Converted Duration (Seconds to Minutes):
o	Duration values from seconds into minutes to make the data easier to interpret by creating a calculated field (i.e., dividing the seconds by 60).
•	Text Cleaning: 
o	In Query 7, the phrasing of a question was corrected by replacing incorrect parts of the string.
•	Response 13 Cleaning:
o	Handled NULL values in Response 13 by ensuring that if Query 13 had a value, Response 13 would show "N/A" when it was missing. This process was done with a calculated field, ensuring it retained the original values if they already existed.
