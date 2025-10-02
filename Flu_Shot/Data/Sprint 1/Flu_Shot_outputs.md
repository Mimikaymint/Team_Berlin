    ['FLU_SHOT.ipynb',
     'Observations&Questions.md',
     'dataset_profile.html',
     'training_set_labels.csv',
     'submission_format.csv',
     'README.md',
     'training_set_features.csv',
     'Labels.md',
     'test_set_features.csv',
     'sprint_1.md']



    /usr/local/bin/python3


    (26707, 38)
    Dataset shape: (26707, 38)
    respondent_id                    int64
    h1n1_concern                   float64
    h1n1_knowledge                 float64
    behavioral_antiviral_meds      float64
    behavioral_avoidance           float64
    behavioral_face_mask           float64
    behavioral_wash_hands          float64
    behavioral_large_gatherings    float64
    behavioral_outside_home        float64
    behavioral_touch_face          float64
    doctor_recc_h1n1               float64
    doctor_recc_seasonal           float64
    chronic_med_condition          float64
    child_under_6_months           float64
    health_worker                  float64
    health_insurance               float64
    opinion_h1n1_vacc_effective    float64
    opinion_h1n1_risk              float64
    opinion_h1n1_sick_from_vacc    float64
    opinion_seas_vacc_effective    float64
    opinion_seas_risk              float64
    opinion_seas_sick_from_vacc    float64
    age_group                       object
    education                       object
    race                            object
    sex                             object
    income_poverty                  object
    marital_status                  object
    rent_or_own                     object
    employment_status               object
    hhs_geo_region                  object
    census_msa                      object
    household_adults               float64
    household_children             float64
    employment_industry             object
    employment_occupation           object
    h1n1_vaccine                     int64
    seasonal_vaccine                 int64
    dtype: object


    True
    respondent_id                      0
    h1n1_concern                      92
    h1n1_knowledge                   116
    behavioral_antiviral_meds         71
    behavioral_avoidance             208
    behavioral_face_mask              19
    behavioral_wash_hands             42
    behavioral_large_gatherings       87
    behavioral_outside_home           82
    behavioral_touch_face            128
    doctor_recc_h1n1                2160
    doctor_recc_seasonal            2160
    chronic_med_condition            971
    child_under_6_months             820
    health_worker                    804
    health_insurance               12274
    opinion_h1n1_vacc_effective      391
    opinion_h1n1_risk                388
    opinion_h1n1_sick_from_vacc      395
    opinion_seas_vacc_effective      462
    opinion_seas_risk                514
    opinion_seas_sick_from_vacc      537
    age_group                          0
    education                       1407
    race                               0
    sex                                0
    income_poverty                  4423
    marital_status                  1408
    rent_or_own                     2042
    employment_status               1463
    hhs_geo_region                     0
    census_msa                         0
    household_adults                 249
    household_children               249
    employment_industry            13330
    employment_occupation          13470
    h1n1_vaccine                       0
    seasonal_vaccine                   0
    dtype: int64



    
![png](output_6_1.png)
    



    
![png](output_7_0.png)
    



                                                 |          | [  0%]   00:00 -> (? left)


    Report dataset_profile.html was generated! NOTEBOOK/COLAB USERS: the web browser MAY not pop up, regardless, the report IS saved in your notebook/colab files.


    Summary statistics for numerical features:



<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>count</th>
      <th>mean</th>
      <th>std</th>
      <th>min</th>
      <th>25%</th>
      <th>50%</th>
      <th>75%</th>
      <th>max</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>respondent_id</th>
      <td>26707.0</td>
      <td>13353.000000</td>
      <td>7709.791156</td>
      <td>0.0</td>
      <td>6676.5</td>
      <td>13353.0</td>
      <td>20029.5</td>
      <td>26706.0</td>
    </tr>
    <tr>
      <th>h1n1_concern</th>
      <td>26615.0</td>
      <td>1.618486</td>
      <td>0.910311</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>2.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>h1n1_knowledge</th>
      <td>26591.0</td>
      <td>1.262532</td>
      <td>0.618149</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>behavioral_antiviral_meds</th>
      <td>26636.0</td>
      <td>0.048844</td>
      <td>0.215545</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_avoidance</th>
      <td>26499.0</td>
      <td>0.725612</td>
      <td>0.446214</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_face_mask</th>
      <td>26688.0</td>
      <td>0.068982</td>
      <td>0.253429</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_wash_hands</th>
      <td>26665.0</td>
      <td>0.825614</td>
      <td>0.379448</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_large_gatherings</th>
      <td>26620.0</td>
      <td>0.358640</td>
      <td>0.479610</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_outside_home</th>
      <td>26625.0</td>
      <td>0.337315</td>
      <td>0.472802</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>behavioral_touch_face</th>
      <td>26579.0</td>
      <td>0.677264</td>
      <td>0.467531</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>doctor_recc_h1n1</th>
      <td>24547.0</td>
      <td>0.220312</td>
      <td>0.414466</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>doctor_recc_seasonal</th>
      <td>24547.0</td>
      <td>0.329735</td>
      <td>0.470126</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>chronic_med_condition</th>
      <td>25736.0</td>
      <td>0.283261</td>
      <td>0.450591</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>child_under_6_months</th>
      <td>25887.0</td>
      <td>0.082590</td>
      <td>0.275266</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>health_worker</th>
      <td>25903.0</td>
      <td>0.111918</td>
      <td>0.315271</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>health_insurance</th>
      <td>14433.0</td>
      <td>0.879720</td>
      <td>0.325300</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>opinion_h1n1_vacc_effective</th>
      <td>26316.0</td>
      <td>3.850623</td>
      <td>1.007436</td>
      <td>1.0</td>
      <td>3.0</td>
      <td>4.0</td>
      <td>5.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>opinion_h1n1_risk</th>
      <td>26319.0</td>
      <td>2.342566</td>
      <td>1.285539</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>opinion_h1n1_sick_from_vacc</th>
      <td>26312.0</td>
      <td>2.357670</td>
      <td>1.362766</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>opinion_seas_vacc_effective</th>
      <td>26245.0</td>
      <td>4.025986</td>
      <td>1.086565</td>
      <td>1.0</td>
      <td>4.0</td>
      <td>4.0</td>
      <td>5.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>opinion_seas_risk</th>
      <td>26193.0</td>
      <td>2.719162</td>
      <td>1.385055</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>opinion_seas_sick_from_vacc</th>
      <td>26170.0</td>
      <td>2.118112</td>
      <td>1.332950</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>household_adults</th>
      <td>26458.0</td>
      <td>0.886499</td>
      <td>0.753422</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>household_children</th>
      <td>26458.0</td>
      <td>0.534583</td>
      <td>0.928173</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>h1n1_vaccine</th>
      <td>26707.0</td>
      <td>0.212454</td>
      <td>0.409052</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>seasonal_vaccine</th>
      <td>26707.0</td>
      <td>0.465608</td>
      <td>0.498825</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>0.0</td>
      <td>1.0</td>
      <td>1.0</td>
    </tr>
  </tbody>
</table>
</div>


    
    Summary statistics for categorical features:



<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>count</th>
      <th>unique</th>
      <th>top</th>
      <th>freq</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>age_group</th>
      <td>26707</td>
      <td>5</td>
      <td>65+ Years</td>
      <td>6843</td>
    </tr>
    <tr>
      <th>education</th>
      <td>25300</td>
      <td>4</td>
      <td>College Graduate</td>
      <td>10097</td>
    </tr>
    <tr>
      <th>race</th>
      <td>26707</td>
      <td>4</td>
      <td>White</td>
      <td>21222</td>
    </tr>
    <tr>
      <th>sex</th>
      <td>26707</td>
      <td>2</td>
      <td>Female</td>
      <td>15858</td>
    </tr>
    <tr>
      <th>income_poverty</th>
      <td>22284</td>
      <td>3</td>
      <td>&lt;= $75,000, Above Poverty</td>
      <td>12777</td>
    </tr>
    <tr>
      <th>marital_status</th>
      <td>25299</td>
      <td>2</td>
      <td>Married</td>
      <td>13555</td>
    </tr>
    <tr>
      <th>rent_or_own</th>
      <td>24665</td>
      <td>2</td>
      <td>Own</td>
      <td>18736</td>
    </tr>
    <tr>
      <th>employment_status</th>
      <td>25244</td>
      <td>3</td>
      <td>Employed</td>
      <td>13560</td>
    </tr>
    <tr>
      <th>hhs_geo_region</th>
      <td>26707</td>
      <td>10</td>
      <td>lzgpxyit</td>
      <td>4297</td>
    </tr>
    <tr>
      <th>census_msa</th>
      <td>26707</td>
      <td>3</td>
      <td>MSA, Not Principle  City</td>
      <td>11645</td>
    </tr>
    <tr>
      <th>employment_industry</th>
      <td>13377</td>
      <td>21</td>
      <td>fcxhlnwr</td>
      <td>2468</td>
    </tr>
    <tr>
      <th>employment_occupation</th>
      <td>13237</td>
      <td>23</td>
      <td>xtkaffoo</td>
      <td>1778</td>
    </tr>
  </tbody>
</table>
</div>


    h1n1_vaccine
    0    78.754634
    1    21.245366
    Name: proportion, dtype: float64
       Class  Count  Percentage
    0      0  21033   78.754634
    1      1   5674   21.245366


    seasonal_vaccine
    0    53.439173
    1    46.560827
    Name: proportion, dtype: float64
       Class  Count  Percentage
    0      0  14272   53.439173
    1      1  12435   46.560827



    
![png](output_13_0.png)
    



    
![png](output_13_1.png)
    


    Markdown file created with outputs only!

