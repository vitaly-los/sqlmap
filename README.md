# sqlmap


If you need to save some time, you can increase the number of threads used. Do note that this might affect the results for time-based related test.

> python sqlmap -u "https://target.com/index.php?name=abc" --threads=10

Batch is using the default option instead of waiting for the user’s input.

> python sqlmap -u "https://target.com/index.php?name=abc" --batch

You could also increase the risk and level value for sqlmap to test for more payloads.

> python sqlmap -u "https://target.com/index.php?name=abc" --risk=3 --level=5
