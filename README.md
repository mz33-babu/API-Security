# API Reconnaissance Techniques and Tools
## Active Reconnaissance:
### Nmap:
A versatile port scanner that can be used to scan for open ports, fingerprint services, and detect potential vulnerabilities. To scan for APIs, you can use the following command:

```css
nmap -sV <target IP> -p 80,443 --script http-api*
```
# Amass: 
A reconnaissance tool that helps in discovering subdomains and IP addresses associated with a target domain. It also has the ability to identify potential API endpoints. To scan for APIs, you can use the following command:

```css
amass intel -d <target domain> -api
```
# Kiterunner: 
A tool that helps in discovering hidden API endpoints by performing brute force testing on common paths and parameters. To scan for APIs, you can use the following command:

```css
kiterunner -t <target URL> -p <port> -w <wordlist>
```
# Directory Buster: 
A tool used to discover hidden directories and files on a web server. It can be used to find hidden API endpoints by brute forcing common directories. To scan for APIs, you can use the following command:

```css
dirb <target URL> -p <port> -o <output file>
```
# Devtools: 
A browser extension that can be used to inspect and analyze API requests/responses in real-time. It allows you to capture and modify requests, and view the corresponding responses. You can use this tool to identify APIs and test their functionality.

# Passive Reconnaissance:
Git Dorking: A technique used to search for sensitive information in GitHub repositories by using advanced search operators. To search for API keys and secrets, you can use the following search query:

```css
"api_key" OR "api_secret" site:github.com
```
# Google Dorking: 
Similar to Git Dorking, it involves using advanced search operators to find sensitive information indexed by Google. To search for APIs, you can use the following search query:

```css
site:<target domain> inurl:/api/
```
# Shodan: 
A search engine that helps in discovering Internet-connected devices and services. It can be used to find APIs exposed on the Internet by using search filters. To search for APIs, you can use the following search query:

```css
http.component:"api" http.title:"API" 
```
# Trufflehog: 
A tool used to search for sensitive information in source code repositories. It can be used to search for API keys and secrets. To scan for APIs, you can use the following command:

```css
trufflehog --regex --entropy=False <target repository>
```
# Wayback Machine: 
An Internet archive that stores snapshots of websites at different points in time. It can be used to discover past versions of API endpoints and identify changes made over time. To search for APIs, you can enter the target domain and look for API endpoints in the archived pages.
