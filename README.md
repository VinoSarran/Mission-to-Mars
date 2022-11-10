# Mission-to-Mars

## Deliverable 2:
   <br>
Questions: 
   <br>
How many months exist on Mars?  <br>
- Mars has 12 months   (Code: MAX month)<br>
 
 <br>
How many Martian (and not Earth) days worth of data exist in the scraped dataset? <br>
- 1867 days worth of observations (Code: count unique Sol)<br>
 
 <br>
Which month, on average, has the lowest temperature? The highest?       <br>
- COLDEST: Month 3, WARMEST: Month 8 
 <br>
 
 <br>
Which month, on average, has the lowest atmospheric pressure? The highest?       <br>
- LOWEST: Month 6, HIGHEST: Month 9 
 <br>
 
 <br>
How many terrestrial days exist in a Martian year? A visual estimate within 25% was made. <br>
- Used coldest temp cycle to estimate how many Earth Days it takes to hit those extreme low temps.  From graph, you see low temps appear about every 2 earth years.  722 Earth days are between the coldest Mars Month 3 in Mars Year 1 (2014-01-10) vs Month 3 in Mars Year 2 (2016-01-02).    

<br>Code: mars_df_days.groupby('month')['terrestrial_date'].apply(lambda x: x.max() - x.min()) <br>
