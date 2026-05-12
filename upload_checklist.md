# GitHub Upload Checklist

Before uploading to GitHub, add these files:

## Required

- `README.md`
- Power BI file in `powerbi/`
- Dashboard screenshot in `images/`

## Recommended

- Dataset in `data/`, only if you are allowed to share it
- Cleaning steps in `docs/cleaning_steps.md`
- DAX measures in `docs/dax_measures.md`

## File Names To Use

```text
powerbi/Super_Store_Sales_Dashboard.pbix
images/dashboard_overview.png
data/super_store_sales_dataset.csv
```

## Important Legal Note

If your dataset came from Kaggle or another website, check the dataset license before uploading the raw CSV.

Your current dashboard was created from a YouTube tutorial:

```text
https://www.youtube.com/watch?v=fZn83JRt4Nk
```

If the video description does not clearly mention dataset license or sharing permission, avoid uploading the raw dataset. Also remember that a `.pbix` file can contain the dataset inside it.

Safe option:

- Upload screenshots
- Upload README and documentation
- Add the dataset source link
- Do not upload the raw dataset if the license is unclear

If you still want to upload the `.pbix`, mention clearly that it was created from a tutorial and is for educational/portfolio use.

## GitHub Steps

1. Create a new repository named `Super-Store-Sales-Dashboard`.
2. Upload the contents of this folder.
3. Add a clear repository description:

```text
Power BI dashboard project analyzing Super Store sales, profit, categories, ship modes, and regional performance.
```

4. Commit the files.
5. Open the repository and check that the README preview looks correct.
