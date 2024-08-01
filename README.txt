This tool cleans your Geography information from text or long format names  to ISO 2-letter codes (i.e. United States of America -> US or America -> US).

Step 1. Drop your file into this folder.

Step 2. Change the csv_to_fix variable to the correct filename.

Step 3. Run the code. When you reach the 5th cell, there should be a file called "ambig.csv" that is created. Here, the tool has done most of the work cleaning obvious names, but in every dataset, there are ambiguous terms. Your job is to look at this file and make those changes.

Step 4. Go into ambig.csv. 

Input string        | Mapped name| Mapped code | Quarantine?
korea dem ppl s rep, North Korea,      KP,    

Input string: What the dataset had
Mapped name: The computer's best guess
Mapped code: Code corresponding to best guess
Quarantine?: Put any letter (i.e. 'x') to indicate that this nation state needs further investigating. Quarantined rows will be dropped.

You can either changed the Mapped name & Mapped code if you know the answer, or quarantine it with an 'x', if you want to get rid of/later deal with unknown data rows.

Step 5. Run the rest of the code. It will return a zip file packaged with all versions, corrected and original, so that you can keep track of your changes. 