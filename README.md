# YoutubeData
Youtube Data Harvesting using MongoDB , Postgre SQL and Streamlit


from googleapiclient.discovery import build              Importing build for the google api connection
import pymongo                                            Importing MongoDB
import certifi                                             
import psycopg2
import pandas as pd
import streamlit as st
ca = certifi.where()
