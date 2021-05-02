FROM python:3.7.6
ENV PYTHONUNBUFFERED 1
WORKDIR /user/src/app

COPY requirements.txt .

COPY . .
#RUN mv wait-for /bin/wait-for
RUN python -m pip install --upgrade pip
#RUN pip install --no-cache-dir -r requirements.txt
RUN pip install -r requirements.txt
RUN rm requirements.txt

#EXPOSE 8000

CMD ["gunicorn", "core.wsgi", "0:8000"]


