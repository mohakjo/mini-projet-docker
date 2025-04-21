FROM python:3.8-buster
LABEL maintainer="Mohamed DIOUME"
COPY requirements.txt student_age.py /
run apt update -y && apt install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
run pip3 install -r /requirements.txt
volume ["/data"]
EXPOSE 5000
CMD [ "python3", "./student_age.py" ]

