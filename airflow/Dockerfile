FROM apache/airflow:2.6.0

# hadolint ignore=DL3013,DL3042,SC1091
RUN pip install --no-cache-dir \
      apache-airflow-providers-dbt-cloud==2.3.1 \
      gspread==5.8.0 \
      oauth2client==4.1.3 \
      segment-analytics-python==2.2.0 \
      analytics-python==1.4.0 \
      simple_salesforce==1.12.3
