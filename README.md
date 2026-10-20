# open-science-itc

CODECHECK metadata for checks conducted by "Open Science at ITC"

## Context

[Open Science at ITC](https://www.utwente.nl/en/service-portal/research-support/additional-information-per-facultyinstitute/geo-information-science-earth-observation-itc/open-science-itc) (OS@ITC) is a horizontal facility of the Faculty of Geo-Information Science and Earth Observation (ITC) at the University of Twente, the Netherlands.
It supports all ITC departments in moving towards Open Science, working together with research support groups such as LISA and CRIB, and aims to educate about Open Science practices to support their wider adoption within ITC ([Zenodo community](https://zenodo.org/communities/open_science_itc/about)).

In 2021, OS@ITC offered [CODECHECK](https://codecheck.org.uk/) as a service to ITC researchers ([archived service page](https://web.archive.org/web/20220926223457/https://www.itc.nl/research/open-science/codecheck/)).
Checks were conducted by Open Science Officer [Markus Konkol](https://orcid.org/0000-0001-6651-0976).
The service followed the CODECHECK philosophy of setting the bar for reproducible research low by asking _"Was the code reproducible once for someone else?"_:

> For a successful CODECHECK, at least one figure or table has to be repoducible using the source code and data. The more, the merrier. I check whether the code runs and generates the expected number of output files. The contents of those output files are checked visually and available for others to see. The validity of the code is not checked.

Any researcher or student affiliated with ITC could request a check, ideally before submitting a manuscript for peer review or as a preprint.
The codechecker ran the analysis, iterated with the authors on issues, proposed code improvements (e.g., as pull requests), and published a certificate on Zenodo in the [Open Science at ITC community](https://zenodo.org/communities/open_science_itc/).
The service was a "safe space": unsuccessful checks were not published.

## Certificates

The following three certificates were published.
Each subfolder is a CODECHECK bundle with a [`codecheck.yml`](https://codecheck.org.uk/spec/config/2.0/) (version 2.0) created retrospectively from the certificate and its Zenodo record, the certificate PDF (`codecheck/codecheck.pdf`), and the reproduced figures, extracted from the certificate PDF because the original outputs were not archived.

| Certificate | Checked work | Report | Check date | Register issue |
|---|---|---|---|---|
| [`2021-011`](2021-011/codecheck.yml) | Prikaziuk et al. (2021): Google Earth Engine Sentinel-3 OLCI Level-1 Dataset Deviates from the Original Data: Causes and Consequences. _Remote Sensing_ 13(6):1098. <https://doi.org/10.3390/rs13061098> | [10.5281/zenodo.5106408](https://doi.org/10.5281/zenodo.5106408) | 2021-07-15 | [#233](https://github.com/codecheckers/register/issues/233) |
| [`2021-012`](2021-012/codecheck.yml) | De la Paz Ruíz et al. (2021): Population census estimation for Spatial Microsimulation. Poster, IGISc 2021. <https://doi.org/10.5281/zenodo.14175899> | [10.5281/zenodo.5543112](https://doi.org/10.5281/zenodo.5543112) | 2021-10-01 | [#234](https://github.com/codecheckers/register/issues/234) |
| [`2021-013`](2021-013/codecheck.yml) | Harisena et al. (2021): When is variable importance estimation in species distribution modelling affected by spatial correlation? _Ecography_ 44(5):778-788. <https://doi.org/10.1111/ecog.05534> | [10.5281/zenodo.5574909](https://doi.org/10.5281/zenodo.5574909) | 2021-10-18 | [#235](https://github.com/codecheckers/register/issues/235) |

Notes on the metadata:

- Certificate identifiers are assigned in chronological order of the checks, continuing after the last 2021 identifier in the register (`2021-010`).
- The codechecker's forks for `2021-011` and `2021-012` no longer exist on GitHub; archived snapshots are linked in `repository`.

## License

- **CODECHECK material** (certificate PDFs and reproduced figures in each `codecheck/` directory) is published under the license stated in the `LICENSE` file of the respective certificate folder, i.e., the license of the certificate on Zenodo (all three: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
- **Metadata** (the `codecheck.yml` files) and all other content of this repository are published under [CC0 1.0 Universal](LICENSE), matching the license of this GitHub repository.

## Register entries

Lines for [`register.csv`](https://github.com/codecheckers/register/blob/master/register.csv) (columns `Certificate,Repository,Type,Venue,Issue,Wikidata`); the `Wikidata` column is left empty for the CODECHECK editor to fill during publication:

```csv
2021-011,github::codecheckers/open-science-itc|2021-011,institution,Open Science at ITC,233,
2021-012,github::codecheckers/open-science-itc|2021-012,institution,Open Science at ITC,234,
2021-013,github::codecheckers/open-science-itc|2021-013,institution,Open Science at ITC,235,
```

Line for [`venues.csv`](https://github.com/codecheckers/register/blob/master/venues.csv) (columns `name,longname,label,logo_url,website_url,policy_url,publisher,contact_name,contact_email,description,identifiers,wikidata,fediverse,hashtags`):

```csv
Open Science at ITC,"Open Science at ITC (OS@ITC), Faculty of Geo-Information Science and Earth Observation, University of Twente",institution,https://codecheck.org.uk/img/itc-logo@2x.png,https://www.utwente.nl/en/service-portal/research-support/additional-information-per-facultyinstitute/geo-information-science-earth-observation-itc/open-science-itc,https://web.archive.org/web/20220926223457/https://www.itc.nl/research/open-science/codecheck/,,Markus Konkol,m.konkol@utwente.nl,"Open Science at ITC (OS@ITC) is a horizontal facility of the Faculty of Geo-Information Science and Earth Observation (ITC) at the University of Twente, supporting all ITC departments in adopting Open Science practices. In 2021, it offered CODECHECK as a service to ITC researchers, with checks conducted by the faculty's Open Science Officer before or after submission of a manuscript. Certificates are published in the Open Science at ITC community on Zenodo.","Wikidata (ITC)|fa-database|Q644820|https://www.wikidata.org/wiki/Q644820;ROR (University of Twente)|fa-university|006hf6230|https://ror.org/006hf6230",Q644820,,
```
