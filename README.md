# New-client-sign-up-tracking-list-
This query is designed to provide a list of new client sign-ups with additional details, such as category and booking status, and allows for tracking and analysis of new clients.



- **Title**: This query is titled "New Client Sign-Up Tracking List" to describe its purpose.

- **Step 1**: A common table expression (CTE) named `time_frame_week` is defined to calculate a time frame. It captures the date 3 days before the current date and time.

- **Step 2**: The main query retrieves data related to new client sign-ups.

- **Step 3**: The `CASE` expression maps `category_id` values to their corresponding categories, making the data more user-friendly.

- **Step 4**: Another `CASE` expression is used to determine if any bookings were made for each client. The count of bookings is also calculated.

- **Step 5**: Tables are joined to obtain the required data from multiple sources.

- **Step 6**: Filters are applied to select clients who joined on or after April 1, 2021. There's also a commented-out filter for a week frame that can be uncommented and adjusted as needed.

- **Step 7**: The results are grouped by specific columns for aggregation. The column numbers (1 to 7) are used to refer to the selected columns in the GROUP BY clause.

- **Step 8**: The results are ordered in descending order based on the "Date Joined" column.
