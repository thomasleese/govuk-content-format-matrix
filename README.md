# GOV.UK Content Format Matrix

This repository contains tools and documentation for generating a GOV.UK Content Format Matrix.

![Example Content Format Matrix](images/screenshot.png)

## How to generate an up-to-date matrix?

### Generate CSV Dump

First you must generate a dump of your CSV file by running the following command on your development laptop:

```bash
$ ./generate-matrix
```

It should take about 5-10 minutes to complete.

### Importing into Google Sheets

Open the [Content Format Matrix Template spreadsheet][matrix-template] and make a copy by clicking on the button shown below.

![Make a copy](images/make-a-copy.png)

Import the CSV file into Google Sheets by clicking on the import button. Make sure you select "Append rows to current sheet" when the following import window appears.

![Append rows to current sheet](images/import-append.png)

Now you have a basic version of the matrix available.

### Adding extra data

The backend column cannot currently be determined automatically, and therefore
must be filled out using developer knowledge or investigation. Use the following letters in that column to get the colours to appear:

- **H**: Full content history is stored.
- **M**: Date metadata is representative and correct.
- **X**: Date metadata is not correct or representative.
- **?**: Unknown.

[matrix-template]: https://docs.google.com/a/digital.cabinet-office.gov.uk/spreadsheets/d/1KHiXEVvISrmUN8ou_VuIGnQL4GPOJOa0xAu4eP0tleY/edit?usp=sharing
