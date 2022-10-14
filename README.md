# YoutubeDataAnalysis
First Project Hands on
<br>
Data to be used 
https://www.kaggle.com/datasets/datasnaek/youtube-new

#Create a bucket in s3 bucket - de-youtube-raw-eu-central-1-dev

#Replace It With Your Bucket Name

#using command
s3 mb s3:///de-youtube-raw-eu-central-1-dev

# To copy all JSON Reference data to same location:
aws s3 cp . s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics_reference_data/ --recursive --exclude "*" --include "*.json" <br>

# To copy all data files to its own location, following Hive-style patterns:
aws s3 cp CAvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=ca/ <br>
aws s3 cp DEvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=de/ <br>
aws s3 cp FRvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=fr/ <br>
aws s3 cp GBvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=gb/ <br>
aws s3 cp INvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=in/ <br>
aws s3 cp JPvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=jp/ <br>
aws s3 cp KRvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=kr/ <br>
aws s3 cp MXvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=mx/ <br>
aws s3 cp RUvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=ru/ <br>
aws s3 cp USvideos.csv s3://de-youtube-raw-eu-central-1-dev/youtube/raw_statistics/region=us/ <br>

