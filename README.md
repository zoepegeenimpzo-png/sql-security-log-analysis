# sql-security-log-analysis

## Project Overview
This project demonstrates the use of SQL queries to investigate authentication logs and support security-related decision-making.

By applying conditional filters and pattern matching, I identified suspicious login activity and supported targeted system updates.

---

## Objectives
- Identify failed login attempts after business hours
- Retrieve login activity on specific dates
- Detect login attempts from unexpected geographic locations
- Filter employee records to support security patching


---

## Techniques Used
- SELECT statements
- WHERE clause filtering
- AND / OR / NOT operators
- LIKE pattern matching
- Date and time filtering

---

## Example Query

```sql
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00'
AND success = FALSE;
