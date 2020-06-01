# Use the official lightweight Python image.
# https://hub.docker.com/_/python
FROM python:3.7-slim

# Copy local code to the container image.
ENV APP_HOME /app

# define work directory
WORKDIR $APP_HOME

# copy code to work direction
COPY . ./
# install production dependencies
RUN pip install -r requirements.txt

# Expose application port to container
EXPOSE 5000

# run execuation command 
ENTRYPOINT ["flask", "run", "--host", "0.0.0.0"]