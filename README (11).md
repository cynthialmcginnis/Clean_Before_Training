# Clean Before You Train

An interactive exercise in preparing data for a machine learning model. No code and no spreadsheet.

You are handed a dataset of about 200 records and asked to train a model on it. Some of the bad data stops the model. Most of it does not. You find both kinds, choose how to fix them, and see what each choice does to the people the model will be used on.

**Try it:** https://YOUR-USERNAME.github.io/clean-before-you-train/

## How it works

1. **Pick a dataset.** Clinic appointments, a military family survey, store transactions, or aircraft maintenance records.
2. **Train on the data as delivered.** The model stops three times, on three kinds of problem: words where numbers belong, numbers typed with their units, and an outcome column spelled six ways. Fix each one and train again.
   You can download the dataset as a CSV file to sort and filter it in a spreadsheet.
3. **Check the result.** The model ran without a warning. It scores well on the data it learned from and badly on new records. A data dictionary and a column summary hold the clues.
4. **Decide how to clean.** Seven problems, each with more than one fix: unscaled numbers, blank cells, impossible and extreme values, categories stored as numbers, repeated records, a column that is filled in after the outcome is known, and records from before a policy change. Train again and compare up to 20 runs.
5. **Hand off.** Choose the run you can defend and save a cleaning log as a PDF or as text.

## What it teaches

- A model that runs is not a model that works. The errors that stop a model are the easy ones.
- Every cleaning choice costs something. Deleting rows with blanks can remove most of one group.
- An outlier can be a typing error or the most important record in the file.
- One overall score hides how a model does for each group.
- A model can score very well on its own data because a column gave the answer away. That column will be empty when the model is used.

## Running it

It is one file, `index.html`. There is nothing to install and no server. The page makes no network requests. Progress is saved in your own browser.

The model is a real five-nearest-neighbors classifier that runs in the browser. Every score is computed from your choices and tested on 400 held-back records.

## Notes

Every organization and every record is fictional. The data was generated for this exercise and describes no real person or group.

## Author

Cynthia McGinnis

&copy; 2026 Cynthia McGinnis. All rights reserved.
