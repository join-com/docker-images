FROM apache/airflow:2.7.2

# hadolint ignore=DL3013,DL3042,SC1091
RUN pip install --no-cache-dir \
      apache-airflow-providers-dbt-cloud==3.4.0 \
      gspread==5.12.0 \
      oauth2client==4.1.3 \
      google-ads>=18.1.0 \
      segment-analytics-python==2.2.0 \
      analytics-python==1.4.0 \
      grequests==0.7.0 \
      simple_salesforce==1.12.5
