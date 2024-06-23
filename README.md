# Taipei City Dashboard

This project is a part of the 2024 Taipei Urban Spring Dashboard Hackathon, a government competition aimed at co-developing a dashboard with the government to promote joint concern between the government and citizens about Taipei City. Our theme for this competition is the Traffic Dashboard. Our team, "真的是Go了！" received an Honorable Mention.

## Ownership

The ownership of this dashboard belongs to the [Taipei Urban Intelligence Center (TUIC)](https://tuic.gov.taipei/en).

## Demo
<p align="center">
  <img src="https://www.lhu.edu.tw/psmart/ex/2019%E6%B5%B7%E5%A0%B1.jpg" />
</p>

Check out our demo video below:

[![Demo Video](https://img.youtube.com/vi/YOUR_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)

## Installation Steps

1. **Download the project**:
   [Download Link](https://github.com/JarrenPoh/Taipei-City-Dashboard/archive/refs/heads/main.zip)

2. **Navigate to the Docker directory**:
   ```sh
   cd docker

3. **Create the Docker network**:
   ```sh
   docker network create --driver=bridge --subnet=192.168.128.0/24 --gateway=192.168.128.1 br_dashboard

4. **Start the database services**:
   ```sh
   docker-compose -f docker-compose-db.yaml up -d

5. **Initialize the dashboard**:
   ```sh
   docker-compose -f docker-compose-init.yaml up -d
---
Note : To access the "Utility Features" section, you need to log in to the dashboard.
- Click on the "Log In" button at the top right corner.
- Shift-click the icon.
- Use the following credentials:
    - Username: admin@gmail.com
    - Password: admin1234
- Next, configure the Geocoding API Key in GCP.
    - Generate Geocoding API Key From [Google Cloud Platform (GCP)](https://cloud.google.com/?hl=zh_tw)
    - Replace the YOUR_API_KEY in report.vue with your Geocoding API Key.



## Contact Information

For any questions, please contact the backend developer of "真的是Go了！" below.
Email: jarren@wwwx.red
