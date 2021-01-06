FROM python:3.7
LABEL io.openshift.expose-service="8080:http" \
      io.k8s.display-name="flask-app" \
      io.k8s.description="Base flask application" \
      io.openshift.tags="flask, python"
EXPOSE 8080
RUN pip install flask
COPY . /app
WORKDIR /app
CMD python main.py
