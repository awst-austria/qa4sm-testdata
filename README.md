# QA4SM integration test data

This repository contains (integration) test data for the qa4sm webservice software <https://github.com/awst-austria/qa4sm>.

The goal is to have example data from the same geographic region for each dataset supported by qa4sm in this repository - in order to do realistic integration testing.

To limit the size of the repository, the region selected is Hawaii: Since soil moisture values are only computable over land, the product files for Pacific islands are much smaller than the ones over continents. (It also allows the developers to dream of a tropical holiday destination while they hack away in rainy Europe.)

Reference data sets (GLDAS, ERA, ISMN, ...) are processed in the period 2017-01 to 2018-12.
Satellite dataset (CCI, SMOS, C3S, SMAP, ASCAT, ...) are for the available period at the time
the testdata was generated.

CGLS SSM and SWI data are only available for Europe at the moment. In order to use existing test data together with CGLS, synthetic test data for
CGLS SSM and SWI in Hawaii were generated.

More comprehensive information about the datasets is [available here](https://qa4sm.eu/datasets/).

## ISMN Testdata

Note that we use the same test files for all ISMN versions. Files are symlinked from `ISMN_TESTDATA_HAWAII` into the respective version directories.

## ESA CCI SM Testdata

Note that neither the ACTIVE nor the PASSIVE CCI SM datasets are available for Hawaii. We therefore use copies of the `COMBINED` data for testing.
