## Pymaceuticals mice study challenge

Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. **The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.**

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

Files

sources -
- ai to help merge properly; it wasn't working correclty
- bootcamp starter code & previous class activities


<!-- NOTES TO SELF: 
# plt.boxplot(final_tumor_vols, flierprops={'marker': 'o', 'markerfacecolor': 'red', 'markersize': 10})
# plt.ylabel('Final Tumor Volume (mm3)')
# plt.xticks(range(1,5), labels=drug_names)
# plt.show() -->


<!-- 
# IGNORE THIS CELL
# (note to self)
# another way of plotting this, but it didn't work as well w/ the linear regression
# # Generate a scatter plot of mouse weight vs. the average observed tumor volume for the entire Capomulin regimen
# capomulin_mice = clean_df.loc[clean_df['Drug Regimen'] == 'Capomulin']
# avg_vol = capomulin_mice[['Mouse ID', 'Tumor Volume (mm3)', 'Weight (g)']].groupby('Mouse ID')['Tumor Volume (mm3)'].mean().tolist()
# avg_weight = capomulin_mice[['Mouse ID', 'Tumor Volume (mm3)', 'Weight (g)']].groupby('Mouse ID')['Weight (g)'].mean().tolist()
# plt.scatter(x=avg_weight, y=avg_vol)
# plt.ylabel('Avg Tumor Vol (mm3)')
# plt.title('Mouse Weight vs. Avg Tumor Volume (For Mice on Capomulin Treatment)')
# plt.show() -->