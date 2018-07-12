religion	<$10k	$10-20k	$20-30k	$30-40k	$40-50k	$50-75k
Agnostic	27	34	60	81	76	137
Atheist	12	27	37	52	35	70
Buddhist	27	21	30	34	33	58
Catholic	418	617	732	670	638	1116
Dont know/refused	15	14	15	11	10	35
Evangelical Prot	575	869	1064	982	881	1486
Hindu	1	9	7	9	11	34
Historically Black Prot	228	244	236	238	197	223
Jehovahs Witness	20	27	24	24	21	30
Jewish	19	19	25	25	30	95

## Objective for this Data set is tidy up by moving the the column $10k "income" to row and create another column of "freq"
import pandas as pd 
import datetime
df=pd.read_csv("pew-raw.csv")
df

## pd.melt allows you to unpivot data, or changing from wide format to long format file. 

formatted_df =pd.melt(df,["religion"],var_name ="income", value_name = "freq"  )

formatted_df = formatted_df.sort_values (by=[" religion"])

formatted_df.head(10)

 religion   income  freq
 Agnostic    <$10k    27
 Agnostic  $30-40k    81
 Agnostic  $40-50k    76
 Agnostic  $50-75k   137
 Agnostic  $10-20k    34
 Agnostic  $20-30k    60
  Atheist  $40-50k    35
  Atheist  $20-30k    37
  Atheist  $10-20k    27
  Atheist  $30-40k    52
