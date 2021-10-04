# data_wrangling_examples
Example notebooks demonstrating how to use Python packages to wrangle common atmospheric datasets. At this point, one such notebook is available: Working with GRIB2 Data, which demonstrates how to use xarray (with the eccodes/cfgrib backend) to read in and perform basic operations with GRIB2-formatted data. This example also demonstrates how to access data from the Amazon Web Services s3 Global Ensemble Forecast System datastore; the process of reading in GRIB2 data is simpler if you are working with local data and/or just a single file.

Package versions used in creating these examples:
<ul>
  <li><b>xarray</b>: 0.19.0 (with a <i>dask</i> dependency due to the use of open_mfdataset)</li>
  <li><b>eccodes</b>: 2.23.0</li>
  <li><b>cfgrib</b>: 0.9.8.5 (should also work with 0.9.9.1 but probably not with 0.9.9.0 due to a cfgrib bug)</li>
  <li><b>fsspec</b>: 2021.9.0 (used to access public AWS S3 data)</li>
  <li><b>Python</b>: 3.7.10 (should also work with newer versions)</li>
</ul>
