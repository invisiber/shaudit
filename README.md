```bash
 ███████╗██╗  ██╗       █████╗ ██╗   ██╗██████╗ ██╗████████╗
 ██╔════╝██║  ██║      ██╔══██╗██║   ██║██╔══██╗██║╚══██╔══╝
 ███████╗███████║█████╗███████║██║   ██║██║  ██║██║   ██║   
 ╚════██║██╔══██║╚════╝██╔══██║██║   ██║██║  ██║██║   ██║   
 ███████║██║  ██║      ██║  ██║╚██████╔╝██████╔╝██║   ██║   
 ╚══════╝╚═╝  ╚═╝      ╚═╝  ╚═╝ ╚═════╝ ╚═════╝ ╚═╝   ╚═╝   
 Invisiber                       Security Header Audit Tool
```

## 📄 shaudit — Security Headers Audit Tool

**shaudit** is a lightweight CLI tool designed to help you audit HTTP security headers on any website. It checks whether common security headers like Content-Security-Policy, Strict-Transport-Security, and many others are properly implemented or missing.

The output is clean, colorful, and easy to read — perfect for quick assessments directly from your terminal. You can also save the results to a file for later review.

**shaudit** works fully offline and is safe to use in production environments, making it a great choice for:

- Pentesters who need quick insights during engagements
- Security engineers verifying HTTP configurations
- Anyone who wants to scan web headers without the hassle


## Installation

```cli
pip install shaudit
```

## Options

```cli
shaudit -s -u https://google.com -h
usage: [-h] [-u URL] [-s] [-nc] [-o [OUTPUT]] [-i]

Security Headers Audit Tool

options:
  -h, --help            show this help message and exit
  -u, --url URL         Input URL to Scan
  -s, --silent          Silent Output
  -nc, --nocolor        No Color
  -o, --output [OUTPUT]
                        Output file (default: sh-example.com)
  -i, --info            Information
                                              
```

## Usage


#### for help or any information:
```cli
shaudit -h
```

#### Basic Scan:
```cli
shaudit -u https://example.com
```

#### Run without color output:
```cli
shaudit -u https://example.com -nc
```

#### Run without logo/banner:
```cli
shaudit -u https://example.com -s
```

#### Save results to a file (default or custom name):
```cli
shaudit -u https://example.com/ -o
shaudit -u https://example.com -o example.txt
```

#### Show list of audited headers and extra info:
```cli
shaudit -i
```

## 📱 Connect with Me
GitHub: **@invisiber**\
PyPI: **shaudit**\
YouTube: **@invisiber**

## Contributing

Contributions, ideas, or issues are welcome!  
Feel free to open a pull request or submit an issue.

## License

MIT License

Copyright (c) 2025 @invisiber

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
