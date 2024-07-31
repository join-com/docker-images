FROM apache/airflow:2.9.3

# hadolint ignore=DL3013,DL3042,SC1091
RUN pip install --no-cache-dir \
      gspread>=5.12.0 \
      oauth2client>=4.1.3 \
      google-ads>=22.1.0 \
      segment-analytics-python==2.2.0 \
      analytics-python==1.4.0 \
      grequests==0.7.0 \
      simple_salesforce>=1.12.5
