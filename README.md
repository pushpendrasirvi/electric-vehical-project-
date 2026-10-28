# EV Market Analysis — College Project Package

## What is included
- `data/ev_market_train.csv`: supplied training dataset (200,000 rows, 37 columns)
- `data/ev_market_test.csv`: supplied test dataset (100,000 rows, same fields)
- `sql/`: MySQL schema/import guidance and analysis queries
- `tableau/tableau_build_guide.md`: seven distinct visualization types, calculated fields, dashboard/story plan
- `flask_app/`: responsive Flask site with dashboard/story embedding slots
- `documentation/Project_Report.docx` and `.pdf`: editable and printable report
- `testing/`: checklist and results template; fill actual observed performance after running it

## Data caution
The provided EV dataset appears synthetic/educational. All results must be described as analysis of the supplied dataset, not verified real-world EV industry statistics. `model_year` is model year, not a confirmed sales-time field. `manufacturing_country` is not the sales market.

## Start here
1. Read `documentation/Project_Report.pdf`.
2. Use MySQL Workbench to create the table using `sql/schema_and_import.sql`; clean duplicate IDs and document null handling before import.
3. Run `sql/analysis_queries.sql` after loading data.
4. Follow the Tableau guide to build nine distinct chart types and the dashboard/story.
5. Run Flask: `cd flask_app`, create/activate a virtual environment, `pip install -r requirements.txt`, set published Tableau URLs, then `python app.py`.

Flask is a local development demo. Tableau embedding requires a published/accessible view URL and the right sharing settings. No fabricated performance measurements are included.

## Training data audit (raw training CSV)
- Rows: 200,000; columns: 37
- Unique categories: 15; battery types: 5; manufacturers: 200
- Missing cells: 18,996; repeated vehicle IDs beyond first occurrence: 1
- Mean range: 324.5 km; mean battery capacity: 78.2 kWh; mean rating: 4.09/5

## Graph previews
Nine PNG previews are in `visualizations/`. Recreate the nine charts in Tableau for the native workbook requirement; the PNGs are visual previews, not a `.twb`/`.twbx` workbook.
