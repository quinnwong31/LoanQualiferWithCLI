# Loan Qualifier Application

## Description

The Loan Qualifier application allows a loan applicant to determine whether or not they qualify for a loan
based on today's daily loan rates. The Loan Qualifer application determines this by asking the
applicant the following questions:

1. Enter a file path to the daily rate sheet.
2. Credit score
3. Current montly debt
4. Monthly income
5. Desired loan amount
6. Home value

Based on this information, the application calculates the following:

- **Debt-to-Income Ratio (DTI)**
- **Loan-to-Value (LTV)**

The application then checks to see if there are any lenders that has a qualifying loan based on the DTI and the LTV specified.

Finally, the applicant has an option to save qualifying loans to a CSV file which they can then view in Excel or any application
that handles CSV files.

---

## Technologies

This application uses Python 3.7 or above.

The following libraries are used:

- **pathlib** - This library is used to determine the path to the daily_rate_sheet.csv and the path to save the qualifying_loans.csv to. Please see [pathlib documentation](https://docs.python.org/3/library/pathlib.html) for more information.
- **csv** - This library is used to read and write csv files. Please see [csv documentation](https://docs.python.org/3/library/csv.html) for more information.
- **fire** - This library is used to accept command-line arguments. Please see [Python Fire Guide](https://google.github.io/python-fire/guide/) for more information.
- **questionary** - This library is used to provide user dialogs for the CLI. Please see [Questionary Documentation](https://pypi.org/project/questionary/) for more information. You can access the [Questionary Source Code here](https://github.com/tmbo/questionary).
- **tabulate** - This library is used to display the qualifying loans in the CLI. Please see [Tabulate Documentation](https://pypi.org/project/tabulate/) for more information.

---

## Installation Guide

The `pathlib` and `csv` libraries are already installed with Python 3.7.

In order to use the Loan Qualifier application, you will need to install `fire`, `questionary` and `tabulate`. Below are the instructions for installing each required library.

**Fire**

To install Fire, do the following steps:

1. Launch the terminal.
2. Enter the following:

```
pip install fire
```

**Questionary**

To install Questionary, do the following steps:

1. Launch the terminal.
2. Enter the following:

```
pip install questionary
```

**Tabulate**

To install Tabulate, do the following steps:

1. Launch the terminal.
2. Enter the following:

```
pip install tabulate
```

---

## Usage

### Launching the Loan Qualifer Application

To use the Loan Qualifier application, you must launch the terminal and enter in the following:

```
python app.python
```

The Loan Qualifier application will then begin a series of questions to determine which loans that you qualify for.

### Determining Qualifying Loans

The Loan Qualifier application will walk the applicant through several questions that it uses to determine the DTI and LTV. Based on the applicant's DTI and LTV, the applicant will be matched with any loans that they qualify for.

Below is a screenshot of questions that the applicant will be asked:

![Screenshot of Qualifying Loans Questions](/images/loan_qualifier_questions.jpg)

### Saving Qualifying Loans

The applicant has an option to save qualifying loans to a CSV file which they can then view in Excel or any application
that handles CSV files.

If there are no qualifying loans, then the applicant will be notified and the application will exit.

If there are qualifying loans, the applicant can choose whether or not they want to save the file to CSV.

If the applicant chooses to save the loans, then they will be prompted for a file path to save the file.

Below is a screenshot of the application requesting if the applicant wants to save the qualifying loans to CSV.

![Screenshot of Qualifying Loans Save Feature](/images/loan_qualifier_save.jpg)

---

## Contributors

This sample application was authored by:

- Quinn Wong (quinn.wong@gmail.com)
- LinkedIn: https://www.linkedin.com/in/quinnwong/

---

## License

The MIT License (MIT)

Copyright (c) 2022 Quinn Wong

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
