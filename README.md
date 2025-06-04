# stac-harvester-configurations

This repository contains the configurations for harvesting STAC catalogues. Configurations require a URL, a schedule, a source folder and a target folder. Some examples are provided below.


Example configuration for a STAC catalogue

```json
{
  "url": "https://api.stac.ceda.ac.uk/",
  "path": "ceda-harvester/public",
  "source": "ceda-harvester/public",
  "target": "catalogs/public",
  "schedule": "57 16 * * *"
}
```

Example configuration for a STAC collection

```json
{
    "url": "https://api.stac.ceda.ac.uk/collections/sentinel1_ard",
    "path": "supported-datasets/ceda-stac-catalogue/sentinel1_ard",
    "source": "ceda-harvester/public",
    "target": "catalogs/public",
    "schedule": "6 9 * * *"
}
```

Example configuration for Git

```json
{
  "url": "https://github.com/<organisation>/example-repo",
  "path": "public/example-repo",
  "source": "example-repo",
  "target": "catalogs/public/catalogs",
  "schedule": "40 14 * * *"
}
```

