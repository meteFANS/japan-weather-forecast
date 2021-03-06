# Japan Weather Data
*From the Japanese Meteorological Agency (scraper + data)* 🌞🌧️🌈🌩️❄️

## Get started

```bash
git clone git@github.com:philipperemy/japan-weather-forecast.git && cd japan-weather-forecast
pip install -r requirements.txt
cd scraper && python scraper.py # data will be located in ../output
```

## Data format

Examples are provided [here](output).

```json
{
  "station": "WAKKANAIWMO Station ID:47401",
  "view": "Monthly total of sunshine duration",
  "data": {
    "Jan": {
      "1938": "59.2",
      "1939": "45.9",
      "1940": "59.5",
      "1941": "44.1",
      "1942": "36.3",
      "1943": "37.7",
      "1944": "29.3",
      "1945": "29.2",
      [...]
      "2012": "1377.4",
      "2013": "1384.1",
      "2014": "1640.6",
      "2015": "1437.5",
      "2016": "1401.1",
      "2017": "1502.0",
      "2018": "1471.0",
      "2019": "316.9 ]"
    }
  }
}
```

```
        Jan    Feb    Mar    Apr    May    Jun    Jul    Aug    Sep    Oct    Nov    Dec  Annual
1938   42.6   47.2   30.9   76.3   56.8   56.6   31.7   83.8  440.6  134.9   85.8   85.4  1172.6
1939   38.0   26.7   20.6   88.3   53.9   94.2  182.6   69.6  103.8   78.0  125.3  141.3  1022.3
1940   98.5   48.5  167.6  106.4   73.5   93.3   72.0  227.8   65.2   85.5  125.5  179.6  1343.4
1941   83.1   83.8   96.1   48.5   84.2   68.3  112.3   29.0  172.4  248.6   79.1  134.2  1239.6
1942   59.0   70.6  104.5  104.9  111.2   45.6  143.8  160.3  126.5   89.0  235.6  122.7  1373.7
1943  118.1   73.0   27.1   49.8   46.6   57.8   93.6  173.4   63.5  153.7  185.9  113.7  1156.2
1944   47.5   68.1   40.6   22.0   23.0  109.6   52.9  115.3  242.2   91.6  122.8  115.4  1051.0
1945   42.4   28.5   34.9   56.1  121.0   39.6   47.2   86.1   60.3  129.2  117.6  173.1   936.0
1946   86.3   80.2   61.2   81.1   77.2  110.4   50.6   48.9  226.0  198.2   80.0   97.3  1197.4
[...]
2013  124.0   49.0   69.5   78.0   52.0   29.0   23.5  116.0  110.0  106.5  194.5   93.5  1045.5
2014  105.0   44.0   20.0   34.5   62.0  144.5   44.0  275.5  256.5   58.5  103.5  143.0  1291.0
2015   55.5   48.5  105.5   40.0   82.0  132.0  205.5   20.5  103.5  182.5   62.5  110.0  1148.0
2016  118.5  115.5   40.0   82.5   41.5  146.0  154.0  112.0  316.0  132.5  129.5   34.5  1422.5
2017   47.5   37.5   43.0   68.5   33.0   86.5   97.0   70.0  115.0  104.0  177.5  153.0  1032.5
2018  122.0   75.0   95.5   32.0  102.0  114.0  121.5   94.0   56.0  160.0   70.0   72.0  1114.0
2019   56.0   46.5   35.5    NaN    NaN    NaN    NaN    NaN    NaN    NaN    NaN    NaN     NaN
```
