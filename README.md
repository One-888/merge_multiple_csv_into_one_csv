# merge_multiple_csv_into_one_csv
Python


    os.chdir(r"S:\MIS\SAP consumption data\result")

    selected_columns = [
        "Account Number",
        "Premise",
        "Service Address",
        "Meter Number",
        "Doc Amount in $",
        "Usage in TGals",
        "Billing Date",
        "Due Date",
        "Rate Category",
    ]

    merge_to_csv(
        selected_columns=selected_columns,
        file_name=f"Jan*.csv",
        top_rows=10_000_000,
        output_file="_output",
    )
