# Apply Filters to SQL Queries

## Project Description

As a cybersecurity professional, I investigated potential security incidents involving employee login attempts and workstation activity. Using SQL queries and filters, I analyzed login records and employee data to identify suspicious activity and support security investigations.

## Retrieve After-Hours Failed Login Attempts

### Query

```sql
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00'
AND success = 0;
```

### Explanation

This query returns all failed login attempts that occurred after 6:00 PM. The `AND` operator combines two conditions: the login attempt must have occurred after business hours and must have failed.

---

## Retrieve Login Attempts on Specific Dates

### Query

```sql
SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-08'
OR login_date = '2022-05-09';
```

### Explanation

This query retrieves all login attempts that occurred on either of the specified dates. The `OR` operator allows records matching either condition to be returned.

---

## Retrieve Login Attempts Outside Mexico

### Query

```sql
SELECT *
FROM log_in_attempts
WHERE NOT country LIKE 'MEX%';
```

### Explanation

This query returns login attempts originating outside Mexico. The `LIKE` operator searches for values beginning with "MEX", while `NOT` excludes those records.

---

## Retrieve Employees in Marketing

### Query

```sql
SELECT *
FROM employees
WHERE department = 'Marketing'
AND office LIKE 'East%';
```

### Explanation

This query identifies Marketing employees located in offices within the East building. The `LIKE` operator filters office locations that begin with "East".

---

## Retrieve Employees in Finance or Sales

### Query

```sql
SELECT *
FROM employees
WHERE department = 'Finance'
OR department = 'Sales';
```

### Explanation

This query returns employees who belong to either the Finance or Sales department.

---

## Retrieve Employees Not in Information Technology

### Query

```sql
SELECT *
FROM employees
WHERE NOT department = 'Information Technology';
```

### Explanation

This query identifies all employees who are not members of the Information Technology department by using the `NOT` operator.

---

## Summary

This project demonstrates the use of SQL filtering techniques to investigate security events and manage employee information. I applied operators such as `AND`, `OR`, `NOT`, and `LIKE` to retrieve relevant records, filter data by dates and times, and support cybersecurity investigations.
