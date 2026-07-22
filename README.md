# Web Scraper

A simple Bash script for scraping publicly available email addresses and phone numbers from websites.

## Features

- Email scraping
- Phone number scraping
- ID scraping
- Cookie scraping
- Full scan mode
- Colored terminal output
- Timestamped logging
- Error logging
- Banner/help menu

## Requirements

- Bash
- curl
- grep
- host
- tee

## Installation

Clone the repository:

```bash
git clone https://github.com/vaiop10/web-scraper.git
cd web-scraper
```

Make the script executable:

```bash
chmod +x web-scraper
```

## Usage

```
./web-scraper <option> <target>
```

### Options

| Option | Description |
|---------|-------------|
| `-e` | Scrape email addresses |
| `-p` | Scrape phone numbers |
| `-i` | Scrape IDs |
| `-c` | Scrape cookies |
| `-full` | Perform both scans |
| `-h` | Show help/banner |


### Examples

Scrape emails

```bash
./web-scraper.sh -e https://example.com
```

Scrape phone numbers

```bash
./web-scraper.sh -p https://example.com
```

Run a full scan

```bash
./web-scraper.sh -full https://example.com
```

## Logging

Successful results are written to:

```
/var/log/web-scraper.log
```

Errors are written to:

```
/var/log/web-scraper-error.log
```

## Notes

- Only scrape websites that you have permission to test.
- The script searches publicly available HTML content.
- Results depend on the data exposed by the target website.

## License

MIT License

## Author

Vaiop10
