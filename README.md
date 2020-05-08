# Description
This repository contains the dataset for the paper:

- J. C. S. Santos, A. Peruma, M. Mirakhorli, M. Galstery, J. V. Vidal and A. Sejfia, "Understanding Software Vulnerabilities Related to Architectural Security Tactics: An Empirical Investigation of Chromium, PHP and Thunderbird," 2017 IEEE International Conference on Software Architecture (ICSA), Gothenburg, 2017, pp. 69-78.

```
@inproceedings{7930201, 
  author={J. C. S. {Santos} and A. {Peruma} and M. {Mirakhorli} and M. {Galster} and J. V. {Vidal} and A. {Sejfia}}, 
  title={Understanding Software Vulnerabilities Related to Architectural Security Tactics: An Empirical Investigation of Chromium, PHP and Thunderbird}, 
  year={2017}, 
  volume={}, 
  number={}, 
  booktitle={2017 IEEE International Conference on Software Architecture (ICSA)},   
  pages={69-78},
}
```
## Datasets
The data collected for each case study can be accessed in the CSV files:

- `chromium-datasets.csv`
- `php-datasets.csv`
- `thunderbird-datasets.csv`

These csv files have the following columns:

- `cve_id`: The unique identifier of the vulnerability in the National Vulnerability Database;
- `date_of_report`: The time when the Vulnerability was first reported;
- `cve_type`: Indicates whether the vulnerability (CVE) is TACTICAL or NON-TACTICAL.
- `root_cause`: In case of tactical vulnerabilities, this field indicates the root cause (given as an id to the CWE dictionary);
- `total_impacted_files`: Number of files that were affected (i.e., changed/added/removed) to fix the vulnerability;
- `code_churn`: Number of lines changed in the patch released to fix the vulnerability;
- `bugtrack_url`: The URL to the bug entry in the Issue Tracker of the project related to that vulnerability or a URL to a place that reports the vulnerability (example: a mailing list, such as http://marc.info/)
- `commit_url`: The URL(s) to the Web page that contains the committed code to the patch that fixed the issue;
