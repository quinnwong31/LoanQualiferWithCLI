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

- **Path** - XXX
- **CSV** - XXX
- **Fire** - This library is used to accept command-line arguments. Please see [Python Fire Guide](https://google.github.io/python-fire/guide/) for more information.
- **Questionary** - This library is used to provide user dialogs for the CLI. Please see [Questionary Documentation](https://pypi.org/project/questionary/) for more information. You can access the [Questionary Source Code here](https://github.com/tmbo/questionary).

---

## Installation Guide

`Path` and `CSV` libraries are already installed with Python 3.7.

You will need to install `Fire` and `Questionary`. In order to use the Loan Qualifier application, you must install the following libraries first:

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

![Screenshot of Qualifying Loans application]()

### Saving Qualifying Loans

The applicant has an option to save qualifying loans to a CSV file which they can then view in Excel or any application
that handles CSV files.

If there are no qualifying loans, then the applicant will be notified and the application will exit.

If there are qualifying loans, the applicant can choose whether or not they want to save the file to CSV.

If the applicant chooses to save the loans, then they will be prompted for a file path to save the file.

---

## Contributors

This sample application was authored by:

- Quinn Wong (quinn.wong@gmail.com)
- LinkedIn: https://www.linkedin.com/in/quinnwong/

---

## License

When you share a project on a repository, especially a public one, it's important to choose the right license to specify what others can and can't with your source code and files. Use this section to include the license you want to use.
