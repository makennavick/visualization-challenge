## Pymaceuticals mice study challenge

#### Background
- Pymaceuticals Inc. studied mice with squamos cell carcinoma (skin cancer) 
- 45 days measuring their tumor growth/development when put on various drug regimens
- [View study data here](data)

#### Goal 
- How does Capomulin compare to other drug treatments?

#### Results
- See [stats_summary.csv](analysis/stats_summary.csv) for stats on each drug's effect on tumor volume, along with a few of the key visuals in the [analysis](analysis) folder
- Capomulin excelled in performance compared to every other treatment plan - Ramicane is its only competitor. Do not put your pet mouse on Propiva.
- Tumor size varies according to mouse weight (i.e. smaller mouse = smaller tumor)

### Sources
- Bootcamp starter code & previous class activities


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