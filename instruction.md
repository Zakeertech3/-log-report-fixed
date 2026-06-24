An Apache-style access log is at /app/access.log. Parse it and write a JSON summary report to /app/report.json.

The report must be a single JSON object with exactly these three keys:

- total_requests: the total number of non-empty log lines
- unique_ips: the number of distinct client IP addresses (the first field of each line)
- top_path: the request path that appears most frequently across all requests

Success criteria:

1. /app/report.json exists and contains a single valid JSON object.
2. total_requests equals the number of non-empty lines in the access log.
3. unique_ips equals the count of distinct client IP addresses.
4. top_path equals the most frequently requested path.
