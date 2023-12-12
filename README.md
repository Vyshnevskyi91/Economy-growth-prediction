# Patents-per-year-prediction

![](https://media.licdn.com/dms/image/C5612AQFArFPF_T06WA/article-cover_image-shrink_600_2000/0/1620524567333?e=2147483647&v=beta&t=8s-vdd5oJeOyz5SO1lct0m4qo53J7GDCOLUN5mQuTN4)

"source": [
    "# Sort the DataFrame based on the top 5 countries for 2022\n",
    "df_combined_sorted_gdp = df_combined.loc[top_5_countries_2022].sort_values(by=\"2022_patent\", ascending=False)\n",
    "\n",
    "# Plotting\n",
    "plt.figure(figsize=(20, 6))\n",
    "\n",
    "# Plot the DataFrame using Seaborn's lineplot\n",
    "sns.lineplot(data=df_combined_sorted_gdp.transpose()[43:], markers=True)\n",
    "\n",
    "# Set custom x-axis tick labels from 1980 to 2022\n",
    "years = list(range(1980, 2023))\n",
    "plt.xticks(range(len(years)), years, rotation=90)\n",
    "\n",
    "plt.xlabel('Year')\n",
    "plt.ylabel('Meaning')\n",
    "\n",
    "\n",
    "plt.show()"
   ]
