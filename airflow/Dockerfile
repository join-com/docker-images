FROM apache/airflow:2.5.3

# hadolint ignore=DL3013,DL3042,SC1091
RUN pip install --no-cache-dir \
      apache-airflow-providers-dbt-cloud==2.3.1 \
      gspread==5.7.2 \
      oauth2client==4.1.3 \
      requests==2.28.1 \
      google-cloud-bigquery==2.34.4 \
      google-api-python-client==1.12.11 \
      google-auth-oauthlib==0.7.0 \
      segment-analytics-python==2.2.0 \
      analytics-python==1.4.0 \
      google-ads==18.0.0 \
      simple_salesforce==1.12.3

ENV PIP_USER=false

#python venv setup
RUN python3 -m venv /opt/airflow/join

RUN /opt/airflow/join/bin/pip install --no-cache-dir \
      gspread==5.8.0 \
      oauth2client==4.1.3 \
      requests==2.29.0 \
      google-cloud-bigquery==3.10.0 \
      google-api-python-client==2.86.0 \
      segment-analytics-python==2.2.2 \
      google-ads==21.0.0 \
      simple_salesforce==1.12.3 \
      apache-airflow==2.5.3 \
      apache-airflow-providers-google==10.0.0

ENV PIP_USER=true
