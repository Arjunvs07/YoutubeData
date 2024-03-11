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
