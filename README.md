# 📚 SQL Study Repository

- Required Software
    - IDE
        - Beekeeper Studio Community Edition
        - TablePlus

- Shortcut
    - Run Current: Ctrl + Enter

- Tip
    1. Annotate when writing the code.
        - In SQL, annotations are marked with --.
        - If you want to leave comments in multiple lines, you can use /* */.
    2. You should use a semicolon when finishing SQL queries.
    3. SQL is not case sensitive.

### DDL, Data Definition Language

- CREATE TABLE TableName ();
- DROP TABLE TableName;
- INSERT INTO TableName VALUES ();
    - Always remember the sequence of columns, and know every value in each column.
    - If you want to enter values in specific rows, use it as below.
        - INSERT INTO TableName (RowNames) VALUES (RowNameValues);
        ```SQL
        CREATE TABLE movies (
            title TEXT,
            released INTEGER,
            overview TEXT,
            rating REAL,
            director TEXT,
            for_kids INTEGER -- If you want to express True or False in SQLite, set the data type to INTEGER and express it as 0 or 1 instead.
            -- poster_image BLOB
        ) STRICT; -- STRICT displays an error if the data type is not correct.

        INSERT INTO movies
            (title, rating, released)
        VALUES
            ('MovieTitle 1', 1, 2001), ('MovieTitle 2', 2, 2002);
        ```
        
