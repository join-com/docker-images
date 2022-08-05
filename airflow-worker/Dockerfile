FROM bitnami/airflow-worker:2.3.3

USER root
# hadolint ignore=DL3013,DL3042,SC1091
RUN . /opt/bitnami/airflow/venv/bin/activate && pip install --no-cache-dir gspread==5.4.0 oauth2client==4.1.3 requests==2.28.1 google-cloud-bigquery==3.2.0 google-api-python-client==2.52.0 google-auth-oauthlib==0.5.2 segment-analytics-python==2.2.0 apache-airflow-providers-dbt-cloud==2.0.1

USER 1001
