# Email Verifier
Email Verifier is a simple command-line program that verifies email domains for the presence of MX records, SPF records, and DMARC records.
## Prerequisites
Email Verifier is written in Go and requires Go 1.13 or later to build and run. You can download Go from the official [website.](https://golang.org/)
## Installation
To install Email Verifier, run the following command:
```
go get https://github.com/Supsource/Golang-Projects
```
and then change the directory to Email Verifier by the following command:
```
cd email-verifier
```
## Usage
Email Verifier reads domain names from standard input and prints the results to standard output in a comma-separated format. To use Email Verifier, simply pipe a list of domain names to the program:
```
cat domains.txt | email-verifier
```
Replace `domains.txt` with the path to a file containing a list of domain names, one per line.

Email Verifier will output the following columns:
1. Domain name
2. Whether the domain has MX records (true or false)
3. Whether the domain has SPF records (true or false)
4. The SPF record for the domain (if any)
5. Whether the domain has DMARC records (true or false)
6. The DMARC record for the domain (if any)

## Example
```sql
$ echo "google.com" | email-verifier
domain, hasMX, hasSPF, sprRecord, hasDMARC, dmarcRecord
google.com, true, true, v=spf1 include:_spf.google.com ~all, true, v=DMARC1; p=none; rua=mailto:dmarc-feedback@google.com
```
## Contributing
If you'd like to contribute to Email Verifier, please fork the repository, make your changes, and submit a pull request. We welcome bug reports, feature requests, and feedback.




