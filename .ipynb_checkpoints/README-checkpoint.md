# ProjectCode
Project Code 

Change these lines :

```py
fulldata = pd.read_csv("/Users/apsharma/IST718 Dropbox/IST 718 Project/Taxi Data/2015-01_100k.csv")
weatherdata = pd.read_excel("/Users/apsharma/IST718 Dropbox/IST 718 Project/Weather Data/2015_weather.xlsx")
holidaysdata = pd.read_excel("/Users/apsharma/IST718 Dropbox/IST 718 Project/Holiday Data/holidays.xlsx")
```

into these lines :

```py
fulldata = pd.read_csv(os.environ.get("TAXI_DATA"))
weatherdata = pd.read_excel(os.environ.get("WEATHER_DATA"))
holidaysdata = pd.read_excel(os.environ.get("HOLIDAY_DATA"))
```

### Setup the environment variables for Data Path

Append these lines into this file `~/.bash_profile` 
CAUTION: Do not overwrite bash profile, just add these lines to it !

The contents of this file should look like this :

```bash
export TAXI_DATA="/Users/apsharma/IST718 Dropbox/IST 718 Project/Taxi Data/2015-01_100k.csv"
export WEATHER_DATA="/Users/apsharma/IST718 Dropbox/IST 718 Project/Weather Data/2015_weather.xlsx"
export HOLIDAY_DATA="/Users/apsharma/IST718 Dropbox/IST 718 Project/Holiday Data/holidays.xlsx"
```

### How to launch the anaconda navigator

open command line and run anaconda-navigator from there.

```bash
$ anaconda-navigator
```

