1. **`mdb-export`**:

   - `mdb-export` is used to export data from an MDB file to various formats, such as CSV or SQL.

   - **Basic Syntax**:

     ```bash
     mdb-export [options] <mdb-file> <table-name>
     ```

     - `[options]`: Additional options for customizing the export.
     - `<mdb-file>`: The path to the MDB file you want to export from.
     - `<table-name>`: The name of the table from which you want to export data.

   - **Example Usage**:

     To export data from a table named "employees" in an MDB file called "sample.mdb" to a CSV file, you can use the following command:

     ```bash
     mdb-export sample.mdb employees > employees.csv
     ```

2. **`mdb-sql`**:

   - `mdb-sql` is used to interact with an MDB file using SQL queries. It allows you to query the data within the MDB file as if it were a traditional relational database.

   - **Basic Syntax**:

     ```bash
     mdb-sql [options] <mdb-file>
     ```

     - `[options]`: Additional options for customizing the SQL interaction.
     - `<mdb-file>`: The path to the MDB file you want to query.

   - **Example Usage**:

     To open an interactive SQL session with an MDB file called "sample.mdb," you can use the following command:

     ```bash
     mdb-sql sample.mdb
     ```

     Once in the interactive SQL session, you can execute SQL queries against the database.

3. **`mdb-tables`**:

   - `mdb-tables` is used to list the names of tables in an MDB file.

   - **Basic Syntax**:

     ```bash
     mdb-tables [options] <mdb-file>
     ```

     - `[options]`: Additional options for customizing the table listing.
     - `<mdb-file>`: The path to the MDB file for which you want to list the tables.

   - **Example Usage**:

     To list the names of tables in an MDB file called "sample.mdb," you can use the following command:

     ```bash
     mdb-tables sample.mdb
     ```

     This command will output the names of the tables in the MDB file, one per line.

These commands provide essential functionality for working with MDB files on non-Windows systems. You can use them to export data, run SQL queries, and list tables within Microsoft Access databases.