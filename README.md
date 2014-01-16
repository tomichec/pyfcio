## pyfcio: Command line weather forecasts from forecast.io ##

### Install and config ###

* download the executable `fcst.py` 
* create a forecast.io account [here](https://developer.forecast.io/register) to get a forecast.io id
* create the file `.pyfcio.conf` in your home directory with the following options (adjusted to your location):

```
[Settings]
forecastioId: yOUr_foRecAST_dOt_Io_Id
lat: 50.7166
lon: -3.5333
rainheader: Probability of precipitation for Exeter, Devon, UK
```



### Usage ###

Currently, only the option `rain` is implemented. So the command 

```
fcst.py rain
```

will produce output similar to

```


      Probability of precipitation for Exeter, Devon, UK

      -------------------------------------------------------------
1.0  :                                                             :
     |                                                             |
     |                                                             |
     |                                                             |
0.75 :         **                                                  :
     |           *                                                 |
     |        *   *                                                |
     |                                                             |
0.5  :       *     *                                               :
     |                                                             |
     |      *                                                      |
     |              *                                              |
0.25 :               *                                             :
     |                                                       ******|
     |     *          **                                *****      |
     |    *             ********                   *****           |
0.0  :****                      *******************                :
      ---------------|--------------|--------------|---------------
                    15             30             45              
                             lead time [min]
     t_0 = 09:37                                  (www.forecast.io)


```


