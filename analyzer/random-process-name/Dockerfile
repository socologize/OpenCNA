FROM python:2.7.14

WORKDIR /csv_processing
COPY src/requirements.txt .
RUN pip install -r ./requirements.txt

COPY src .
COPY models .

ENTRYPOINT ["python", "-W", "ignore", "check_string_is_random.py"]
