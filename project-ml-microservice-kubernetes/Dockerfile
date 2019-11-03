FROM python:3.7.3-stretch

## Step 1:
# Create a working directory
WORKDIR /opt/project

## Step 2:
# Copy source code to working directory
COPY . app.py /opt/project/

## Step 3:
# Install packages from requirements.txt
# hadolint ignore=DL3013
COPY requirements.txt /opt/project
RUN pip3 install --upgrade pip
RUN pip3 install -r /opt/project/requirements.txt


## Step 4:
EXPOSE 80

## Step 5:
# Run app.py at container launch
#RUN python /opt/project/app.py
CMD ["python", "app.py"]

