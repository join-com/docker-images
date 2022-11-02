FROM apache/airflow:2.4.2

# hadolint ignore=DL3013,DL3042,SC1091
RUN pip install --no-cache-dir \
      apache-airflow-providers-dbt-cloud==2.2.0 \
      gspread==5.6.2 \
      oauth2client==4.1.3 \
      requests==2.28.1 \
      google-cloud-bigquery==3.3.5 \
      google-api-python-client==1.12.11 \
      google-auth-oauthlib==0.5.3 \
      segment-analytics-python==2.2.0 \
      analytics-python==1.4.0 \
      google-ads==18.1.0
