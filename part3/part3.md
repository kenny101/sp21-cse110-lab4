1. The bug was due to num1 and num2 being strings which resulted in string concatenation instead of numerical addition.
2. I fixed the bug by modifying line 9 to let result = parseFloat(num1) + parseFloat(num2); which parses the strings to an float. This is to make sure that even decimals work for our inputs. If it were a float input, we may encounter NaN. If any anycase we don't expect float inputs then we could use parseInt() instead.
3. citylots.json
4. 11.15MB
5. part2.js
6. 79.35ms
7. User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36
8. Server: Apache
9. Last-Modified: Tue, 26 Jan 2021 22:14:13 GMT
10. Content-Type: application/json
11. The "onClick={fetchData()}" method in <button onClick={fetchData()}>Fetch Data</button>