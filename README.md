# YoutubeData
Youtube Data Harvesting using MongoDB , Postgre SQL and Streamlit

# Importing Packages
from googleapiclient.discovery import build               Importing build for the google api connection
import pymongo                                            Importing MongoDB
import certifi                                            for creating SSL certificates
import psycopg2                                           for manipulating data to SQL
import pandas as pd                                       for creating a dataframe
import streamlit as st                                    for showing the output in streamlit
ca = certifi.where()

# API key Function

def Api_connect():
    api_key = "AIzaSyCosw7zu6NnBMBDfing20ocBFd2IvMc8uM"                            Here, with the help of API key obtained from the google developer console
    api_service_name = "youtube"                                                   we are establishing a connection with the youtube.  
    api_version = "v3"

    youtube = build(api_service_name,api_version,developerKey=api_key)
    
    return youtube

youtube = Api_connect()
