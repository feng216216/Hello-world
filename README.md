import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
mauinfis_filepath=pd.read_csv(r"C:\fengmuschietti\Desktop\mauinuifoodinse.csv")
mauinfis_data=pd.read_csv(mauinfis_filepath, index_col="month")
mauinfis_data
plt.figure(figsize=(10,6))
plt.titel("Maui Nui Number of People in SNAP")
sns.barplot(x=mauinfis_data.index, y=mauinfis_data['Maui Nui'])
plt.ylabel("Number of People(in SNAP)")
plt.xlabel("Month from 7/20/20 to 4/2021")
