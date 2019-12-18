### ALL TEST DATA

#importing required libraries
from sklearn.preprocessing import MinMaxScaler
from keras.models import Sequential
from keras.layers import Dense, Dropout, LSTM
import pandas as pd

train_df=pd.read_excel('C:/Users/Ritu/Documents/IUB/Social Media Mining/Final/Train/hcltech_train.xlsx')
test_df=pd.read_excel('C:/Users/Ritu/Documents/IUB/Social Media Mining/Final/Test/hcltech_test.xlsx')
train_df.drop('year', axis=1, inplace=True)
train_df.drop('month', axis=1, inplace=True)
train_df.drop('qtr_start_date', axis=1, inplace=True)
train_df.drop('qtr_end_date', axis=1, inplace=True)
train_df.drop('Net Sales/Income from operations', axis=1, inplace=True)
train_df.drop('Total Income From Operations', axis=1, inplace=True)
train_df.drop('P/L Before Other Inc. , Int., Excpt. Items & Tax', axis=1, inplace=True)
print(train_df)

