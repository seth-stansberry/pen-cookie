Reproducible Pen Test Reporting
====================

A boilerplate for creating reproducible and consistent note taking structure to put together pen test reports. This project was designed after frustrations with KeepNote and wanting to create a template to keep my reporting more organized through constant note taking.

Credit
------
> Credit for the original template this was designed around [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science). The philosophy of [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science): *A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.*


> Inspiration for this goes to [James Hall](https://411hall.github.io/OSCP-Preparation/) after seeing his template and being impressed. 


Contributing
------------
Pull requests and forks are welcome. This project was designed entirely for my own use for OSCP self study and reporting for CTFs, however anyone else getting milage out of this would be a bonus.

Requirements
------------
Install `cookiecutter` command line: `pip install cookiecutter`    

Usage
-----
1) ### To start a new pen test project:

`cookiecutter gh:seth-stansberry/pen-cookie`

2) ### Complete report.
Use vim, nano, or similar.

3) ### To Display the newly crafted book/report as a webpage:
`gitbook serve https://github.com/GitbookIO/gitbook`

Project Structure
-----------------

```
.
├── bin                    <- Your compiled payloads, scripts can be stored here (not tracked by git)
├── config		           <- Configuration files, e.g., yaml for custom scripts or export values for metasploit if needed
├── cookiecutter.json
├── LICENSE
├── README.md
├── reports                <- Reporting structure based on a 5 step process outlined below. Setup as Gitbook.
│   ├── part1_enumeration  <- Inital footprinting with tools like nmap, dirb, and nikto.
│   ├── part2_exploitation <- Document whatever exploit, CVE, or feature was used to exploit host.
│   ├── part3_post_exploit <- List of enumerated services, applications, scheduled tasks, ec.
│   ├── part4_privesc      <- Privesc vulnerability, exploit code, and proof.
│   ├── part5_lootA	       <- Hashes, passwords, and flags- oh my!
│   └── SUMMARY.md	       <- A kind of table of contents.
├── report.yaml
└── VERSION

```

License
-------
This project is licensed under the terms of the [BSD License](/LICENSE)
