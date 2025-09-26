---
title: "Archiving Cookbook FAQ"
keywords: archiving, guidance, cookbook, tools, FAQ
tags: [guidelines, archiving, data, NCEI, tools, FAQ]
toc: false
summary: Frequently asking questions on the NCEI Archiving Process
editor_options: 
  markdown: 
    wrap: sentence
---

## General Questions

#### Real time vs delayed mode?

NCEI would like all of the data, both delayed QA/QC data and real-time data.

#### Directory structure?

NCEI prefers the files to be organized by platform, with each platform being its own directory.
See the example below:

![](./faq-1-0.png)

````{=html}
<!--   Preferred directory structure

```
    .
    ├── PR1
    │   ├── DSG_PR1.accelerometer2.realtime.nc
    │   ├── DSG_PR1.diagnostics.realtime.nc
    │   ├── DSG_PR1.doppler.realtime.zcell36.nc
    │   ├── DSG_PR1.met.pr.realtime.nc
    │   ├── DSG_PR1.sbe37.realtime.1m.nc
    │   ├── DSG_PR1.waves.mstrain.v1.realtime.nc
    │   └── DSG_PR1.waves.triaxys.realtime.nc
    ├── PR2
    │   ├── DSG_PR2.accelerometer2.realtime.nc
    │   ├── DSG_PR2.diagnostics.realtime.nc
    │   ├── DSG_PR2.doppler.realtime.zcell36.nc
    │   ├── DSG_PR2.met.pr.realtime.nc
    │   ├── DSG_PR2.sbe37.realtime.1m.nc
    │   ├── DSG_PR2.waves.mstrain.v1.realtime.nc
    │   ├── DSG_PR2.waves.triaxys.realtime.nc
    ├── PR3
    │   ├── DSG_PR3.accelerometer2.realtime.nc
    │   ├── DSG_PR3.diagnostics.realtime.nc
    │   ├── DSG_PR3.doppler.realtime.zcell36.nc
    │   ├── DSG_PR3.met.pr.realtime.nc
    │   ├── DSG_PR3.sbe37.realtime.1m.nc
    │   └── DSG_PR3.waves.mstrain.v1.realtime.nc
    ├── VI1
    │   ├── DSG_VI1.accelerometer2.realtime.nc
    │   ├── DSG_VI1.diagnostics.realtime.nc
    │   ├── DSG_VI1.doppler.realtime.zcell40.nc
    │   ├── DSG_VI1.met.pr.realtime.nc
    │   ├── DSG_VI1.sbe37.realtime.1m.nc
    │   ├── DSG_VI1.waves.mstrain.v1.realtime.nc
    │   └── DSG_VI1.waves.triaxys.realtime.nc
    └── VIA
        ├── DSG_VIA.diagnostics.cbibs.realtime.nc
        ├── DSG_VIA.doppler.cbibs.realtime.nc
        ├── DSG_VIA.met.cbibs.realtime.nc
        ├── DSG_VIA.waves.cbibs.realtime.nc
        └── DSG_VIA.wqm.cbibs.realtime.nc

``` -->
````

#### What should we put in the archive section of the certification?

In order to be certified, a RICE must provide a Standard Operating Procedure (to be no more than 2 pages) that identifies (in general terms) their process for archiving data, identifies aggregated data sets to be archived, provides a timeline for completion of the necessary agreement with NCEI or other appropriate national data archive center.
An approved agreement with NCEI must be in red prior to being approved as a certified RICE.
The approved agreement with NCEI will be in one of the following formats (**2** and **3** can be obtained from the ATRAC system):

1.  Submission Information Form (deprecated);

2.  Request to Archive; or

3.  Data Submission Agreement.

Below are examples of the various archive states the archival of RICE data could be in.
NCEI has provided their recommendation of what information to include in the certification, in some cases, specific text to include.

1.  **If the region does not have an agreement with NCEI** include the following information:

    a.  List of parameters/observations being collected.

    b.  Processing steps/quality control including final format.

    c.  Timing of data submissions and approximate sizes.

    d.  Development of data documentation (metadata).

    e.  Data disposition (path to archive center).

    f.  Data affiliations, including both institutions and individual persons whose names will be associated with the data set in some way, e.g., where did it come from, where does it go, etc.

2.  **If the region is under negotiations with NCEI to archive the data.**

    a.  Include the information requested above and the current Request to Archive documentation from the ATRAC system.

    b.  Provide an estimated date as to when the RICE expects to be archiving their data.

3.  **If the region has an approved Request to Archive, but NCEI has not implemented the archive procedure yet.**

    1.  Include the approved Request to Archive.

    2.  Add the following text to the certification (replacing *RICE* with your region name): *RICE **has completed the required documentation for the** (description of data files) **data files in the NCEI ATRAC system. The Request to Archive (attached here) has been approved and NCEI is developing the archival process. We expect the automated archival of** RICE (description of data files) **to be operational by the end of** (give a date when we can expect the data to be archived, for example the calendar year (January 2017))*.

4.  **If the region has an already existing agreement with NCEI and will be making adjustments to that process after the certification is submitted.**

    a.  Include the current agreement to the certification documentation.

    b.  Include a statement that details how the current framework is being renegotiated with NCEI and the documentation will be updated to reflect any changes.

5.  **If the region has established an agreement with NCEI and are actively archiving data.**

    a.  Include the approved Request to Archive document exported from the ATRAC system.

    b.  Include the Submission Agreement document exported from the ATRAC system.

    c.  Add the following text to the certification (replacing *RICE* with your region name): *RICE **already archives** (description of data) **through NCEI and this process is documented in the accompanying Request to Archive and Submission Agreement Form updated** (date of last update to submission agreement form)*.

------------------------------------------------------------------------

## Data File Questions

#### What do you recommend for file naming conventions?

NCEI's [Data Submissions Format Guidance](https://www.ncei.noaa.gov/archive#v-pills-preferred) and [Archiving Guidelines](https://www.ncei.noaa.gov/archive/atrac/guidelines.html) web pages provides advice on file naming.
For example, the following pattern used to construct file names would be acceptable:

<organization><platform><start date>-<end date>.nc, where

-   <organization> is an abbreviation or code for the organization that collected the data (no spaces and no special characters included),

-   <platform> is an abbreviation or code for the platform which collected the data (no spaces and no special characters included), and

-   <start date> and <end date> are the first and last dates, respectively, that data was collected, and are formatted "YYYMMDD," where

    -   YYYY is the four-digit year,

    -   MM is the two-digit month, and

    -   DD is the two-digit day, and

-   .nc is the file extension indicating the type of file (in this example, the file format is NetCDF).

#### Who do we list as the creator_name in the netCDF file?

The person generating the files.

#### What do we list in the projects attribute?

Any associated projects that are affiliated with the data in that file.


```{=html}
<!-- #### What should we list in the institution global attribute?

Our recommendation is to populate the institution global attribute with the associated institution that collected the data. This could be a list of institutions which collected the data:

<pre><b>    institution: GLOS,U-GLOS, University of Michigan Marine Hydrodynamics Laboratories </b></pre>

Or, one institution:

<pre><b>    institution: University of South Florida(USF) Coastal Ocean Monitoring and Prediction System </b></pre> -->
```
