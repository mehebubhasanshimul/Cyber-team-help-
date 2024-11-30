# Cyber-team-help-
Hacking help service providers 

<?php

// Initialize cURL session
$ch = curl_init();

// Set cURL options
curl_setopt($ch, CURLOPT_URL, "http://fabrilife.com/sendOTP");
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
curl_setopt($ch, CURLOPT_POST, true);
curl_setopt($ch, CURLOPT_POSTFIELDS, "phone=01576219310&email=webhosttcs%40gmail.com");

// Set HTTP headers
$headers = [
    "Host: fabrilife.com",
    "Connection: keep-alive",
    "Content-Length: 46",
    "Accept: */*",
    "X-Requested-With: XMLHttpRequest",
    "X-CSRF-TOKEN: uP5CBcHx3JdnqlEXFT5wPf87WT1zTThegYFsdZ19",
    "User-Agent: Mozilla/5.0 (Linux; Android 10; K) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Mobile Safari/537.36",
    "Content-Type: application/x-www-form-urlencoded; charset=UTF-8",
    "Origin: http://fabrilife.com",
    "Referer: http://fabrilife.com/register",
    "Accept-Encoding: gzip, deflate",
    "Accept-Language: en-US,en;q=0.9",
    "Cookie: geolife=eyJpdiI6InQwXC9IQ3I5OTFlQVV3STNDRVA0UHd3PT0iLCJ2YWx1ZSI6Ik5JKzQwbjd0ZkJwVGNIaUtOYll0Rm01MllhVGdKa2xEWUx5aGx0dWdvVjk0NERGdlRXTWtLMkg2NHRuMERBcnNEREZmcE9rRjlSQ1ZNMVZcL0c0ckh2WjlNUzRnczlDMWJUXC9Td0pzUUQ5dXhaTjhNYjJuR3MxWlBZYkNSd25HblFFUlZoa1pOaHZpdVVMUHFhcW9sb3dLbldxcUlObHlJemdZSXB0aHBBQVFvPSIsIm1hYyI6IjNiYWEwOWM4MzZiMjE4NmYyNTUxMDFhNjgxZmM3YzQ2NjY4NzEzMGI3NzFkZjFiYTk3ZDk5NjhiMTRlNzJkMjYifQ%3D%3D; app_modal_times=1; XSRF-TOKEN=eyJpdiI6Im1QRjZCa3ptSUtmS3hHelZlZlZHaWc9PSIsInZhbHVlIjoidEtoSWJqd1FyaXhyelcyV1BDN05IQkpDNXJFQkZucFRrRHUxcmFCTWxKOEZPQUhwc2NtODlDSTE0Y3g4OTFvcCIsIm1hYyI6ImRhODQ0NTdkZTI2MGU5NzM3ZmU0NzZlNDIwNjZhOTU4Mzg0MmIwNTI2OTk2ZDQzNDM2ODM1MjAzZDAxNzRkODEifQ%3D%3D; fabrilife=eyJpdiI6IitGbnd5ck9LTGFDZkFreFwvRWMrT0hnPT0iLCJ2YWx1ZSI6IlU2bDJlaDY0S0ZPNEI2clBaR2VQYmZcL2I0cnd0UVBtV25nWWVDd0JMSGduY2toaUt1OGdtMUpESHBZdXVUMnBTMWwzUERLNnBLTjBWUjk0dzlCVUxGQWhEWDg5Y3h4Um5XeGJicXlGTDJYQjJweWJTRHlNVEhUaXptbU96OEZjWSIsIm1hYyI6IjE0MDMzYmVlYjVhZWU3MDQzMmViNzdmZmMwZjViMDE3Zjk0ZjBjZWNlY2E3ZWU4OTkyMTlmZWVkZWM4NTExOGQifQ%3D%3D"
];

// Add headers to the request
curl_setopt($ch, CURLOPT_HTTPHEADER, $headers);

// Execute the cURL request and capture the response
$response = curl_exec($ch);

// Check for errors
if (curl_errno($ch)) {
    echo "Error: " . curl_error($ch);
} else {
    // Process the response (optional)
    echo $response;
}

// Close cURL session
curl_close($ch);
?>