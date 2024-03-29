# Regression



=== "Table"

    | Model                                    | Dataset       |        MAE |       RMSE |            R2 |   Memory in Mb |   Time in s |
    |:-----------------------------------------|:--------------|-----------:|-----------:|--------------:|---------------:|------------:|
    | Adaptive Model Rules                     | ChickWeights  |  24.1943   |  37.2166   |    0.725319   |    0.046977    |    5.25855  |
    | Adaptive Model Rules                     | TrumpApproval |   1.39847  |   2.43336  |   -1.02372    |    0.114429    |    9.38293  |
    | Adaptive Random Forest                   | ChickWeights  |  26.1016   |  40.8094   |    0.669725   |    1.19043     |   56.006    |
    | Adaptive Random Forest                   | TrumpApproval |   0.800378 |   2.11495  |   -0.528761   |    1.28462     |   87.4457   |
    | Aggregated Mondrian Forest               | ChickWeights  |  25.6742   |  41.7123   |    0.65479    |    8.21412     |  127.415    |
    | Aggregated Mondrian Forest               | TrumpApproval |   0.268533 |   0.349421 |    0.958184   |   16.9323      |  186.034    |
    | Bagging                                  | ChickWeights  |  23.1143   |  36.6311   |    0.733893   |    0.628034    |   38.0203   |
    | Bagging                                  | TrumpApproval |   0.908203 |   2.23718  |   -0.710572   |    1.31579     |   82.0689   |
    | Exponentially Weighted Average           | ChickWeights  | 121.818    | 141.004    |   -2.94294    |    3.09241     |   55.8851   |
    | Exponentially Weighted Average           | TrumpApproval |  40.7546   |  40.7905   | -567.663      |    5.27613     |  141.452    |
    | Hoeffding Adaptive Tree                  | ChickWeights  |  23.3739   |  37.6579   |    0.718766   |    0.0947332   |    7.99029  |
    | Hoeffding Adaptive Tree                  | TrumpApproval |   0.921313 |   2.23942  |   -0.713986   |    0.138225    |   16.7576   |
    | Hoeffding Tree                           | ChickWeights  |  23.1619   |  36.7336   |    0.732402   |    0.0440512   |    6.29305  |
    | Hoeffding Tree                           | TrumpApproval |   0.956103 |   2.24987  |   -0.730022   |    0.148639    |   11.7656   |
    | Linear Regression                        | ChickWeights  |  23.7587   |  37.0377   |    0.727954   |    0.00421047  |    3.21471  |
    | Linear Regression                        | TrumpApproval |   1.31455  |   3.91198  |   -4.23035    |    0.00497341  |   11.5379   |
    | Linear Regression with l1 regularization | ChickWeights  |  23.7577   |  37.078    |    0.727361   |    0.00444126  |    9.7485   |
    | Linear Regression with l1 regularization | TrumpApproval |   1.15377  |   3.82872  |   -4.01007    |    0.0052042   |   13.3595   |
    | Linear Regression with l2 regularization | ChickWeights  |  25.2738   |  38.5885   |    0.704694   |    0.00423336  |    1.22128  |
    | Linear Regression with l2 regularization | TrumpApproval |   1.87151  |   4.13052  |   -4.83107    |    0.0049963   |    4.15677  |
    | Passive-Aggressive Regressor, mode 1     | ChickWeights  |  24.3423   |  37.596    |    0.71969    |    0.00345898  |    1.10187  |
    | Passive-Aggressive Regressor, mode 1     | TrumpApproval |   4.98403  |   6.97667  |  -15.6354     |    0.00443554  |    2.99338  |
    | Passive-Aggressive Regressor, mode 2     | ChickWeights  | 100.624    | 143.066    |   -3.05911    |    0.00345898  |    1.16798  |
    | Passive-Aggressive Regressor, mode 2     | TrumpApproval |  31.0933   |  34.6257   | -408.765      |    0.00443554  |    4.72475  |
    | River MLP                                | ChickWeights  |  51.4078   |  80.9203   |   -0.298584   |    0.0123129   |   28.2295   |
    | River MLP                                | TrumpApproval |   1.58058  |   5.03392  |   -7.66066    |    0.0133505   |   32.2432   |
    | Stochastic Gradient Tree                 | ChickWeights  |  68.7588   |  80.358    |   -0.280601   |    1.12059     |   22.3803   |
    | Stochastic Gradient Tree                 | TrumpApproval |   9.42975  |  17.9379   | -108.972      |    3.08244     |   52.4507   |
    | Streaming Random Patches                 | ChickWeights  |  23.7097   |  38.4416   |    0.706938   |    0.355182    |   93.4014   |
    | Streaming Random Patches                 | TrumpApproval |   0.656697 |   1.98434  |   -0.345761   |    1.06461     |  134.903    |
    | [baseline] Mean predictor                | ChickWeights  |  50.2509   |  71.1144   |   -0.00292947 |    0.000490189 |    0.302835 |
    | [baseline] Mean predictor                | TrumpApproval |   1.56755  |   2.20286  |   -0.658483   |    0.000490189 |    1.08177  |
    | k-Nearest Neighbors                      | ChickWeights  |  24.8406   |  39.2016   |    0.695236   |    2.88522     |   40.0878   |
    | k-Nearest Neighbors                      | TrumpApproval |   0.641679 |   1.59417  |    0.131425   |    5.03263     |  123.301    |

=== "Chart"

    *Try reloading the page if something is buggy*

    ```vegalite
    {
      "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
      "data": {
        "values": [
          {
            "step": 11,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 30.432219699626994,
            "RMSE": 31.267456151778337,
            "R2": -1257.4692714745631,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.000963
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 20.75760844034268,
            "RMSE": 23.632210645041404,
            "R2": -590.4769976066937,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.002374
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 14.555240079240876,
            "RMSE": 19.34929493332969,
            "R2": -259.0232069515881,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.004113
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 11.14363365913676,
            "RMSE": 16.767243978820222,
            "R2": -220.3452424437857,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.006175
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 10.841164000616114,
            "RMSE": 17.714902804136145,
            "R2": -60.2608923989398,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.008581
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 10.32598508406065,
            "RMSE": 16.527353468164844,
            "R2": -21.985729074745297,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.01133
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 9.718401993814265,
            "RMSE": 15.52109639018614,
            "R2": -12.587024696233003,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.014424
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 8.767755200283737,
            "RMSE": 14.552446235427842,
            "R2": -9.829280875288257,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.017858
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.977130626229444,
            "RMSE": 13.740429605807138,
            "R2": -7.074807888709797,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0216349999999999
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.506893871110683,
            "RMSE": 13.098273311725844,
            "R2": -4.124041411671393,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0257519999999999
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.252833276832352,
            "RMSE": 12.607637144454216,
            "R2": -2.6562249812820733,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0302089999999999
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.896359231575217,
            "RMSE": 12.121970224209305,
            "R2": -1.7624336939368233,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0350039999999999
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.581914741629191,
            "RMSE": 11.688367143429067,
            "R2": -1.080274127204615,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0401389999999999
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.347682986169337,
            "RMSE": 11.314945909537578,
            "R2": -0.6567859420078188,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0456129999999999
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.47676439389405,
            "RMSE": 11.21748999353191,
            "R2": -0.3089959076061037,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0514269999999999
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.552290709218319,
            "RMSE": 11.100632967129414,
            "R2": -0.0335718949744832,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0575809999999999
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.503097179992549,
            "RMSE": 10.915357728148932,
            "R2": 0.1817591258850298,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0640729999999999
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.420443618722296,
            "RMSE": 10.727647067877951,
            "R2": 0.3713230272376924,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.070904
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 6.54715053669462,
            "RMSE": 10.814712106795348,
            "R2": 0.4732913339801876,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0780719999999999
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.075852889975692,
            "RMSE": 11.488147441481184,
            "R2": 0.479648982578291,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0855759999999999
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.197265349840174,
            "RMSE": 11.527376107146,
            "R2": 0.5518657524511614,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.0934159999999999
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.359957454348683,
            "RMSE": 11.71365363090123,
            "R2": 0.6276606533313056,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.1015909999999999
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 7.389343614466645,
            "RMSE": 11.70410418267156,
            "R2": 0.6771453727427903,
            "Memory in Mb": 0.0041303634643554,
            "Time in s": 0.1101019999999999
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 8.007684680730522,
            "RMSE": 12.681713023454453,
            "R2": 0.6536838584261326,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.1189499999999999
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 8.456356064016727,
            "RMSE": 13.562457362384484,
            "R2": 0.6514630282957669,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.128137
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 8.682222588679535,
            "RMSE": 13.91372755183948,
            "R2": 0.6822857451181047,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.137663
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 8.656490376145301,
            "RMSE": 13.862729792291397,
            "R2": 0.7264657185265005,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.147527
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 9.17087534181789,
            "RMSE": 14.586626878398466,
            "R2": 0.730278281446047,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.157738
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 10.253235573939358,
            "RMSE": 17.040182474587255,
            "R2": 0.6659707835095393,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.270641
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 10.67218268870669,
            "RMSE": 17.597898989920818,
            "R2": 0.6951262006904333,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.38498
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 10.865878827617594,
            "RMSE": 17.684075493652397,
            "R2": 0.7243197409220903,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.500381
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 11.014541487264225,
            "RMSE": 17.788847456042067,
            "R2": 0.7464163188501894,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.6168239999999999
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 11.893125923244742,
            "RMSE": 19.14640328452056,
            "R2": 0.7147396000186461,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.7343709999999999
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 12.40252640363099,
            "RMSE": 20.24468752454989,
            "R2": 0.7068188127948265,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.8529599999999999
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 12.78041264925886,
            "RMSE": 20.84297745742841,
            "R2": 0.7250508110390363,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 0.972583
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 12.908163646252072,
            "RMSE": 20.82655299121286,
            "R2": 0.7440434321899679,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.093238
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 13.78624220521945,
            "RMSE": 22.297725224665918,
            "R2": 0.7272822586077066,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.214927
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 14.56231380927385,
            "RMSE": 23.732773749874315,
            "R2": 0.7099846963904786,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.3375199999999998
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 15.109717404902195,
            "RMSE": 24.64206848989837,
            "R2": 0.7221580232945248,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.4604629999999998
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 15.287005413554732,
            "RMSE": 24.72152256024044,
            "R2": 0.7401560140604169,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.583729
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 15.806865735774078,
            "RMSE": 25.331119330890413,
            "R2": 0.7387809061287051,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.707315
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 16.912347710111163,
            "RMSE": 27.450327347193877,
            "R2": 0.7118740092210123,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.831218
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 17.68786801080465,
            "RMSE": 28.74804692307192,
            "R2": 0.7209603573249957,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 1.955435
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 18.02230431978895,
            "RMSE": 29.040370094251127,
            "R2": 0.7308604085348502,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.079964
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 18.47643461729765,
            "RMSE": 29.56562239854821,
            "R2": 0.7375811559076941,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.204806
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 19.368862660258834,
            "RMSE": 31.016595939650863,
            "R2": 0.7195863076124669,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.32996
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 20.093492725340727,
            "RMSE": 32.00802507821089,
            "R2": 0.7181912437784894,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.455434
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 20.883641447975457,
            "RMSE": 33.20140091570763,
            "R2": 0.727385103943677,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.581219
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 21.055940734584823,
            "RMSE": 33.19901872731025,
            "R2": 0.7386798629639011,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.707313
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 22.04665839885113,
            "RMSE": 34.818142407426606,
            "R2": 0.7214274205964286,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.833717
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 22.75015079068996,
            "RMSE": 35.737018888500465,
            "R2": 0.7193638350430389,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 2.960429
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 23.60149518688988,
            "RMSE": 36.92142939550449,
            "R2": 0.722919218201958,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 3.087448
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "ChickWeights",
            "MAE": 23.75865667886776,
            "RMSE": 37.03767126301035,
            "R2": 0.7279537206511313,
            "Memory in Mb": 0.0042104721069335,
            "Time in s": 3.2147080000000003
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 20.71537559933632,
            "RMSE": 24.27612097298636,
            "R2": -1381.3340079163324,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.003774
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 12.956746822999646,
            "RMSE": 17.85530816845139,
            "R2": -127.17403450091604,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.008234
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 10.540337295823328,
            "RMSE": 15.264267507077204,
            "R2": -125.28803290438402,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.013346
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 8.92648259034571,
            "RMSE": 13.436420463778148,
            "R2": -97.15695382305036,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.019104
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 7.5495393499287236,
            "RMSE": 12.076339439187349,
            "R2": -48.75014684916543,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.025552
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 6.571266653106965,
            "RMSE": 11.058195411086311,
            "R2": -34.38851346579008,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.032651
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 5.868178209177549,
            "RMSE": 10.265658199354172,
            "R2": -30.51567288629301,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.040397
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 5.226493262391851,
            "RMSE": 9.609365926739027,
            "R2": -23.352843972650145,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.048786
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 4.806672346419344,
            "RMSE": 9.079121174210671,
            "R2": -18.092824435696784,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.057857
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 4.400421129740624,
            "RMSE": 8.617551092451054,
            "R2": -16.252012396913173,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.06766
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 4.083414123099576,
            "RMSE": 8.223437931584808,
            "R2": -15.946617088642816,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.0781589999999999
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 3.82353438841577,
            "RMSE": 7.87966547036827,
            "R2": -14.67643164713968,
            "Memory in Mb": 0.0048131942749023,
            "Time in s": 0.0893539999999999
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 3.573342996804622,
            "RMSE": 7.572887494545769,
            "R2": -13.674649599158814,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.1012429999999999
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 3.399764262602937,
            "RMSE": 7.307305033384193,
            "R2": -13.305426773388604,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.1138299999999999
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 3.2435269592384794,
            "RMSE": 7.069212717011484,
            "R2": -12.166742621467945,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.2177469999999999
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 3.1105754847518408,
            "RMSE": 6.854541649824586,
            "R2": -11.99216513034567,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.416803
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.9569354047226284,
            "RMSE": 6.651479799277566,
            "R2": -11.928129373171446,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.618037
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.8537856094930785,
            "RMSE": 6.474036710445056,
            "R2": -11.348131391644102,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 0.8214119999999999
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.750449728962714,
            "RMSE": 6.305826559379086,
            "R2": -11.120053648606476,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 1.026924
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.663414115575528,
            "RMSE": 6.151161672136967,
            "R2": -10.85874486639798,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 1.234147
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.556259025339157,
            "RMSE": 6.003825249623929,
            "R2": -10.671335514866264,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 1.4420449999999998
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.471571610669061,
            "RMSE": 5.868919367302693,
            "R2": -9.950915405915524,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 1.6506019999999997
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.379680763039582,
            "RMSE": 5.740715994508566,
            "R2": -8.935993501779443,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 1.860033
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.293542327214648,
            "RMSE": 5.620383847029998,
            "R2": -8.304713733239236,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 2.070158
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.2170719472274363,
            "RMSE": 5.50775327209046,
            "R2": -7.748060324415055,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 2.280968
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.1605380581247338,
            "RMSE": 5.403051906918496,
            "R2": -7.433320998258445,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 2.492507
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.093930365363914,
            "RMSE": 5.302901387269021,
            "R2": -7.093810234661742,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 2.70473
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 2.0590245226095627,
            "RMSE": 5.213512799867119,
            "R2": -7.009651494197669,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 2.917634
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.9976476082662875,
            "RMSE": 5.1231852511763165,
            "R2": -6.925804791819894,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 3.1312199999999994
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.950641059884997,
            "RMSE": 5.038426259116397,
            "R2": -6.58092298894084,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 3.3455269999999997
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.9139787950639096,
            "RMSE": 4.959092402037442,
            "R2": -6.2321238970256,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 3.560656999999999
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.8644177203659007,
            "RMSE": 4.8815607080230725,
            "R2": -5.87676544995844,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 3.776474999999999
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.8242147858959743,
            "RMSE": 4.808190620674182,
            "R2": -5.62363098938706,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 3.992974
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.7745110240786572,
            "RMSE": 4.737042423784333,
            "R2": -5.530654039159668,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 4.267744
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.73663030353679,
            "RMSE": 4.669916427921507,
            "R2": -5.51357997146441,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 4.544746
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.692679144669073,
            "RMSE": 4.604703216269991,
            "R2": -5.472066122280332,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 4.823995
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.6517738073879171,
            "RMSE": 4.542197076044804,
            "R2": -5.293761488897717,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 5.105493
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.6176019850850996,
            "RMSE": 4.482676429973872,
            "R2": -5.196305855003581,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 5.389141
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.5865007641193465,
            "RMSE": 4.425455260516019,
            "R2": -5.066178353973196,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 5.673523
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.5595678531598225,
            "RMSE": 4.370690133148669,
            "R2": -4.970481738375755,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 5.9679660000000005
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.535948345073891,
            "RMSE": 4.318357063182573,
            "R2": -4.892367885242343,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 6.2645230000000005
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.509480285222116,
            "RMSE": 4.267276732370252,
            "R2": -4.807214337073276,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 6.563154000000001
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.4815681878661566,
            "RMSE": 4.217864876321593,
            "R2": -4.663732871777943,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 6.863868000000001
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.452683177817048,
            "RMSE": 4.169823323470254,
            "R2": -4.507942651608292,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 7.276079000000001
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.425504815240136,
            "RMSE": 4.123417367951589,
            "R2": -4.4087270270070205,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 7.880966000000001
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.401135420694234,
            "RMSE": 4.078757160785335,
            "R2": -4.379153600942964,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 8.488067000000001
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.3798894262867003,
            "RMSE": 4.035722473386745,
            "R2": -4.310917809364017,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 9.096757
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.3578157698337674,
            "RMSE": 3.993911445090692,
            "R2": -4.255827563021541,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 9.706153
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.334955498529068,
            "RMSE": 3.953168904153961,
            "R2": -4.249147855442176,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 10.316233
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.3157385915327031,
            "RMSE": 3.913934448961732,
            "R2": -4.232086679588724,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 10.926998
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Linear Regression",
            "dataset": "TrumpApproval",
            "MAE": 1.3145482000473083,
            "RMSE": 3.911980916488244,
            "R2": -4.230354806784151,
            "Memory in Mb": 0.0049734115600585,
            "Time in s": 11.537908000000002
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 30.519429760441792,
            "RMSE": 31.341724959881887,
            "R2": -1263.4547929656037,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.001889
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 20.93274945698016,
            "RMSE": 23.730069634788823,
            "R2": -595.3856524245364,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.005264
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 14.671976905269483,
            "RMSE": 19.432784890847977,
            "R2": -261.2719879213097,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.0454959999999999
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.206218788565426,
            "RMSE": 16.83704009498573,
            "R2": -222.1918420065333,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.086209
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.7873677371092,
            "RMSE": 17.69725945175844,
            "R2": -60.138926246201024,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.127302
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.358479420064798,
            "RMSE": 16.54420972880916,
            "R2": -22.032639310332936,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.168766
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.753598876381378,
            "RMSE": 15.536347024393615,
            "R2": -12.613738343052718,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.2106009999999999
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.774706713989955,
            "RMSE": 14.560860647391404,
            "R2": -9.841807755380492,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.252804
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.976543403311107,
            "RMSE": 13.74760854733656,
            "R2": -7.083247758311314,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.295373
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.528406770561816,
            "RMSE": 13.11078583789324,
            "R2": -4.133835882207287,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.338308
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.271666718491515,
            "RMSE": 12.6229442838289,
            "R2": -2.665108536473531,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.38161
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.91845605456336,
            "RMSE": 12.134014714075713,
            "R2": -1.767925975098496,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.425278
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.610383809165891,
            "RMSE": 11.700505099139123,
            "R2": -1.084596952740374,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.469311
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.3485668448406924,
            "RMSE": 11.31852948419668,
            "R2": -0.6578355548574832,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.51371
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.473998962981321,
            "RMSE": 11.222073845492618,
            "R2": -0.3100659276219817,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.558476
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.543521830550948,
            "RMSE": 11.096254270292285,
            "R2": -0.0327566612108853,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.603607
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.493894355635018,
            "RMSE": 10.908553918682982,
            "R2": 0.1827788670738018,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.649102
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.432058292739276,
            "RMSE": 10.739983052449066,
            "R2": 0.3698763337697944,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.6949599999999999
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 6.530905166315106,
            "RMSE": 10.805387069826963,
            "R2": 0.4741992564876139,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.74118
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.049069109840064,
            "RMSE": 11.46222613381468,
            "R2": 0.4819945238144716,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.7877609999999999
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.185364391622807,
            "RMSE": 11.520615160379734,
            "R2": 0.5523912707049028,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.834703
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.384443509591489,
            "RMSE": 11.759466507882768,
            "R2": 0.6247424700583044,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.882006
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.370825288025247,
            "RMSE": 11.706644644448966,
            "R2": 0.6770052015955412,
            "Memory in Mb": 0.0043611526489257,
            "Time in s": 0.929669
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 7.997212264968545,
            "RMSE": 12.688148058774216,
            "R2": 0.6533323093865229,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 0.977694
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.45564901988644,
            "RMSE": 13.583827871673952,
            "R2": 0.6503637760490552,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.026082
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.687395226209604,
            "RMSE": 13.953064893865328,
            "R2": 0.6804867014487179,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.074833
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.660171229881424,
            "RMSE": 13.910099225377923,
            "R2": 0.7245931722706233,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.1239519999999998
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.16625719191718,
            "RMSE": 14.612234985526298,
            "R2": 0.7293304097140514,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.1734349999999998
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.250950211093048,
            "RMSE": 17.0718306278326,
            "R2": 0.664728869016383,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.2232849999999995
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.679670450254022,
            "RMSE": 17.65395670255975,
            "R2": 0.6931807697512926,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.3407639999999996
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.873729384474112,
            "RMSE": 17.73873175202587,
            "R2": 0.7226130148559202,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 1.6983979999999996
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.018541118771262,
            "RMSE": 17.831871437600412,
            "R2": 0.745188204067577,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 2.057199
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.899574150448762,
            "RMSE": 19.1903382176024,
            "R2": 0.7134289333715201,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 2.417118
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.408282768986876,
            "RMSE": 20.289550367060546,
            "R2": 0.7055179762102581,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 2.778154
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.788104615245372,
            "RMSE": 20.897902847676004,
            "R2": 0.7235998101431352,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 3.140457
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.90822201416442,
            "RMSE": 20.86950621812891,
            "R2": 0.7429865604297317,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 3.503137
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 13.78564736405168,
            "RMSE": 22.33392717480972,
            "R2": 0.726395986248676,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 3.866169
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 14.562464823979756,
            "RMSE": 23.77146138634261,
            "R2": 0.709038397249883,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 4.229544
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 15.115712915071189,
            "RMSE": 24.692790084324347,
            "R2": 0.7210130632693055,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 4.59326
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 15.290646451171162,
            "RMSE": 24.766775019882367,
            "R2": 0.7392038606135755,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 4.957315
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 15.806610158983217,
            "RMSE": 25.37056359629737,
            "R2": 0.7379667599208486,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 5.321708999999999
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 16.91167446753811,
            "RMSE": 27.489289014578038,
            "R2": 0.711055524573946,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 5.686440999999999
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 17.69453441784174,
            "RMSE": 28.803034656505247,
            "R2": 0.7198918720890418,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 6.051508999999999
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 18.02591429387984,
            "RMSE": 29.08166628667707,
            "R2": 0.7300944167213836,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 6.416912999999999
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 18.47687089345869,
            "RMSE": 29.604201733284565,
            "R2": 0.7368958634072684,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 6.782651999999999
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 19.37032815671457,
            "RMSE": 31.058772984483277,
            "R2": 0.7188231637639817,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 7.148725999999999
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 20.096649322747314,
            "RMSE": 32.051830787895724,
            "R2": 0.717419357352562,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 7.515149999999999
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 20.88685610593147,
            "RMSE": 33.24610520798377,
            "R2": 0.7266504806846955,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 7.882236999999999
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 21.052957054073875,
            "RMSE": 33.24035912136826,
            "R2": 0.7380286507287471,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 8.25334
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 22.046178761536364,
            "RMSE": 34.86098206113683,
            "R2": 0.7207414968982613,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 8.62558
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 22.751953045975853,
            "RMSE": 35.78242297978339,
            "R2": 0.7186502822700677,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 8.998921
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 23.603432973098663,
            "RMSE": 36.96472548228527,
            "R2": 0.7222689970347711,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 9.373355
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "ChickWeights",
            "MAE": 23.757667537133976,
            "RMSE": 37.07802525541943,
            "R2": 0.7273605875689941,
            "Memory in Mb": 0.0044412612915039,
            "Time in s": 9.748496
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 20.96628233331211,
            "RMSE": 24.387937149248955,
            "R2": -1394.0974368768457,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.003367
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 12.95809265443779,
            "RMSE": 17.886947111698607,
            "R2": -127.62867621055317,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.060679
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 10.43403375286247,
            "RMSE": 15.198987179765494,
            "R2": -124.2101566950438,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.118829
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 8.76952679896777,
            "RMSE": 13.348146279436204,
            "R2": -95.8714533526398,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.177742
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 7.318348711169017,
            "RMSE": 11.969856517585775,
            "R2": -47.87667264392048,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.237441
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 6.2853039116310185,
            "RMSE": 10.94189036106609,
            "R2": -33.648027646243705,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.297866
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 5.5208355911538485,
            "RMSE": 10.138862242229528,
            "R2": -29.74195117722151,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.359017
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.9080595636493145,
            "RMSE": 9.487746704217276,
            "R2": -22.740310036230184,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.420891
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.437342628193194,
            "RMSE": 8.948953859899,
            "R2": -17.549281500204398,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.483487
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.020740144728086,
            "RMSE": 8.490404067975657,
            "R2": -15.746680942149272,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.546844
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.702540763677515,
            "RMSE": 8.09713522450445,
            "R2": -15.430052960036054,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.610978
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.449057445346116,
            "RMSE": 7.755193128790045,
            "R2": -14.185073150160106,
            "Memory in Mb": 0.0050439834594726,
            "Time in s": 0.675884
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.201640426877581,
            "RMSE": 7.451485247160068,
            "R2": -13.20791735379428,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 0.741568
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.9861522146348123,
            "RMSE": 7.180696949733205,
            "R2": -12.814002869999907,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 0.808037
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.8260389726991693,
            "RMSE": 6.939608203297966,
            "R2": -11.688379207589731,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 0.926618
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.694730270614988,
            "RMSE": 6.722171113188908,
            "R2": -11.495217468089896,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 1.215588
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.572442774284147,
            "RMSE": 6.524300196624447,
            "R2": -11.438471282384336,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 1.5070640000000002
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.4832798669216825,
            "RMSE": 6.345294903725613,
            "R2": -10.86190793294698,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 1.8008990000000002
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.371542642654472,
            "RMSE": 6.177015076243767,
            "R2": -10.629949316856385,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 2.0970690000000003
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.263251524870982,
            "RMSE": 6.020874949010495,
            "R2": -10.36170885736068,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 2.4016
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.166901825777709,
            "RMSE": 5.8760767656227735,
            "R2": -10.179937857653265,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 2.706944
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.102550908901192,
            "RMSE": 5.743886676480224,
            "R2": -9.489284487381322,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 3.013076
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.036030402550628,
            "RMSE": 5.61908468135586,
            "R2": -8.519416508014515,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 3.319991
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.965717807967496,
            "RMSE": 5.50138701729293,
            "R2": -7.914879120336785,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 3.627685
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.8948913466896105,
            "RMSE": 5.390446783732167,
            "R2": -7.379388774419297,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 3.93618
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.8304411336225568,
            "RMSE": 5.286008256480869,
            "R2": -7.071904701569496,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 4.245555
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.7733791235095338,
            "RMSE": 5.187623645241403,
            "R2": -6.74573862520947,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 4.555757000000001
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.7328732375480085,
            "RMSE": 5.096231477200102,
            "R2": -6.653340289034931,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 4.866786000000001
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.6922671720641331,
            "RMSE": 5.009032279128942,
            "R2": -6.5765398617523605,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 5.1996410000000015
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.6600221636451291,
            "RMSE": 4.9270067527590165,
            "R2": -6.249341959517198,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 5.545038000000002
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.6169171465584515,
            "RMSE": 4.847662648980224,
            "R2": -5.910766757861972,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 5.892753000000002
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.5787668849144931,
            "RMSE": 4.771995268006674,
            "R2": -5.5715350899413965,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 6.242777000000002
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.535700232104731,
            "RMSE": 4.69925054984221,
            "R2": -5.326885534626132,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 6.599796000000002
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.5003699975160405,
            "RMSE": 4.630081239411466,
            "R2": -5.239062722957792,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 6.957619000000002
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.4782734303433982,
            "RMSE": 4.565354365023557,
            "R2": -5.225160013321354,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 7.316272000000002
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.4563696019956498,
            "RMSE": 4.503833132228122,
            "R2": -5.19161922746511,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 7.675697000000002
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.4392280778003554,
            "RMSE": 4.445645440595998,
            "R2": -5.02903742417401,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 8.035893000000002
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.4073407178561264,
            "RMSE": 4.387021097703184,
            "R2": -4.9346827726614455,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 8.396854000000001
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.3782504190107006,
            "RMSE": 4.330701361336262,
            "R2": -4.809192109617374,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 8.758623000000002
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.3571814777264213,
            "RMSE": 4.277370073659861,
            "R2": -4.718248073230613,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 9.121240000000002
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.3328025450945626,
            "RMSE": 4.2253925636382,
            "R2": -4.641399853721709,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 9.484674000000002
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.311715211433691,
            "RMSE": 4.175582527272098,
            "R2": -4.560327645533724,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 9.848922000000002
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.2897432923325247,
            "RMSE": 4.127236925138345,
            "R2": -4.422957957045758,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 10.213983000000002
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.2672991203860131,
            "RMSE": 4.080383024210964,
            "R2": -4.274192362897992,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 10.579853000000002
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.2421842209255052,
            "RMSE": 4.03488734209176,
            "R2": -4.178968845613636,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 10.965988
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.220808929344255,
            "RMSE": 3.991045752926761,
            "R2": -4.15028972045945,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 11.354575
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.2057181063421545,
            "RMSE": 3.9494511154557617,
            "R2": -4.0862825167589865,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 11.745471
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.188437369603739,
            "RMSE": 3.9086583836793856,
            "R2": -4.0338431039290805,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 12.138778
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.1710173649101312,
            "RMSE": 3.869039281342956,
            "R2": -4.028105053503917,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 12.545048
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.1544521877618488,
            "RMSE": 3.830602085194232,
            "R2": -4.011663649294047,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 12.952187
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Linear Regression with l1 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.1537672749321948,
            "RMSE": 3.8287168981917103,
            "R2": -4.010074752320696,
            "Memory in Mb": 0.0052042007446289,
            "Time in s": 13.359495
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 30.6062254572366,
            "RMSE": 31.39938120772091,
            "R2": -1268.1112549740517,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.000711
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 21.412737763681047,
            "RMSE": 23.97862157826266,
            "R2": -607.9443275975191,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.001889
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 15.119104680903606,
            "RMSE": 19.655410372524667,
            "R2": -267.315679768846,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.003406
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.691588950452092,
            "RMSE": 17.042779535378298,
            "R2": -227.6797328948204,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.00525
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.128477598777668,
            "RMSE": 17.570968714531574,
            "R2": -59.26944361385635,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.007421
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.75565671610116,
            "RMSE": 16.483156797846284,
            "R2": -21.862958739409084,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.009919
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.454334080303978,
            "RMSE": 15.644372833730271,
            "R2": -12.803711937026078,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.012745
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.893519322025275,
            "RMSE": 14.807378680481822,
            "R2": -10.212022929829027,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.015896
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.219705201317108,
            "RMSE": 14.0445461378022,
            "R2": -7.436202462041329,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.019372
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.828389618716818,
            "RMSE": 13.455080798744472,
            "R2": -4.4070097733575375,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.023173
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.61456960864212,
            "RMSE": 13.037583740326507,
            "R2": -2.909846715773841,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.027299
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.52880743945525,
            "RMSE": 12.69008098915324,
            "R2": -2.0274307958032884,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.031782
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.39143583855712,
            "RMSE": 12.35961426350804,
            "R2": -1.3260696348061909,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.036638
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.12180315101294,
            "RMSE": 12.009375103170282,
            "R2": -0.866389387173786,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.0418749999999999
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.136940986261356,
            "RMSE": 11.920551719153746,
            "R2": -0.4782218583187949,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.0474919999999999
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.284290032332207,
            "RMSE": 11.93362687305613,
            "R2": -0.1945108920445761,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.0534829999999999
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.390309464431912,
            "RMSE": 11.903488345267943,
            "R2": 0.0269083954035856,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.0598469999999999
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.350219958465262,
            "RMSE": 11.791481226840991,
            "R2": 0.2404518209934976,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.06659
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.499019855105985,
            "RMSE": 11.958125495095471,
            "R2": 0.3560283448388185,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.073713
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 8.90272187978296,
            "RMSE": 12.527163169679886,
            "R2": 0.3812690011074207,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.081218
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.171291167504233,
            "RMSE": 12.73748746029564,
            "R2": 0.4528394877125938,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.08971
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.37629466014084,
            "RMSE": 13.047657656056804,
            "R2": 0.538024139715424,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.099295
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.440817816219347,
            "RMSE": 13.0964165059942,
            "R2": 0.5957634168273553,
            "Memory in Mb": 0.0041532516479492,
            "Time in s": 0.110134
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 9.906487060964151,
            "RMSE": 13.855497684527965,
            "R2": 0.5866088718530376,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.1222419999999999
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.387009537918406,
            "RMSE": 14.786939232799543,
            "R2": 0.5856869069436603,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.1355289999999999
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.701469010841246,
            "RMSE": 15.270898285463774,
            "R2": 0.6172820078624095,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.1498919999999999
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 10.689852199892528,
            "RMSE": 15.284847538688991,
            "R2": 0.6674656839655615,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.1772019999999999
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 11.168487287417785,
            "RMSE": 16.008183102465477,
            "R2": 0.6751444757196481,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.2058519999999999
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.085867087734242,
            "RMSE": 18.170753499240718,
            "R2": 0.6201764868699093,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.2348879999999999
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.672501856506583,
            "RMSE": 19.05837058612535,
            "R2": 0.6424226539377311,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.2642819999999999
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 12.822446828447037,
            "RMSE": 19.13937756684808,
            "R2": 0.6770787925994421,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.2940279999999999
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 13.055746883990931,
            "RMSE": 19.31213644577825,
            "R2": 0.7011272480618885,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.3241269999999999
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 13.79008745873622,
            "RMSE": 20.396105048894267,
            "R2": 0.6762859401979866,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.3545779999999999
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 14.293199062265238,
            "RMSE": 21.539399675842866,
            "R2": 0.6681199603719434,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.3853799999999999
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 14.740320816630271,
            "RMSE": 22.31102616496048,
            "R2": 0.6849554171717112,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.4261629999999999
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 14.862968645899144,
            "RMSE": 22.29409698811668,
            "R2": 0.7067005430463744,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.467315
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 15.699705023283965,
            "RMSE": 23.67314903355933,
            "R2": 0.6925996644733732,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.508826
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 16.38213993729544,
            "RMSE": 25.048095107979137,
            "R2": 0.6769473375050636,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.55069
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 16.967894830794286,
            "RMSE": 26.15320189056989,
            "R2": 0.6870368010887093,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.592905
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 17.10728249235129,
            "RMSE": 26.204092785638924,
            "R2": 0.7080553660644732,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.6354690000000001
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 17.603016925007317,
            "RMSE": 26.772391386711117,
            "R2": 0.7082099437723521,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.6783830000000001
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 18.614531201761597,
            "RMSE": 28.786744962703725,
            "R2": 0.6831362914484524,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.7216460000000001
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 19.48829335200544,
            "RMSE": 30.38515335394973,
            "R2": 0.6882746780375071,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.7652570000000001
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 19.755002868307955,
            "RMSE": 30.52390276571354,
            "R2": 0.7026599444855313,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.8092140000000001
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 20.22217092676305,
            "RMSE": 31.08727194033441,
            "R2": 0.7098743070293987,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.8535240000000001
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 21.03670858216615,
            "RMSE": 32.44431034253017,
            "R2": 0.6931769059461363,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.898204
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 21.78200415465676,
            "RMSE": 33.496021791915204,
            "R2": 0.6913806254796178,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.943264
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 22.56258004106143,
            "RMSE": 34.768391171729405,
            "R2": 0.7010449079513538,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 0.988697
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 22.68725373887437,
            "RMSE": 34.77075336357408,
            "R2": 0.7133508993505916,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 1.0345
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 23.627725892037507,
            "RMSE": 36.32441604878253,
            "R2": 0.6968033114915981,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 1.080674
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 24.34737619246692,
            "RMSE": 37.30920796407717,
            "R2": 0.6941284720923248,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 1.127216
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 25.18573737545828,
            "RMSE": 38.51358935872805,
            "R2": 0.698506895988072,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 1.174127
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "ChickWeights",
            "MAE": 25.27380465992389,
            "RMSE": 38.58852748240754,
            "R2": 0.7046942807227952,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 1.2212839999999998
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 20.994354275814885,
            "RMSE": 24.339467027537435,
            "R2": -1388.5575385664913,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.002841
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 12.808927193108108,
            "RMSE": 17.83271591943186,
            "R2": -126.84988353201342,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.006663
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 10.864002308096952,
            "RMSE": 15.320672400398038,
            "R2": -126.22308256175272,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.011298
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 8.882777304938948,
            "RMSE": 13.38981065066765,
            "R2": -96.4771385394691,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.01675
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 7.231639558854497,
            "RMSE": 11.98203471414171,
            "R2": -47.97617801736401,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.023066
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 6.334108393931037,
            "RMSE": 10.98237795329033,
            "R2": -33.904913895880355,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.030179
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 5.563493982833803,
            "RMSE": 10.178707085968126,
            "R2": -29.98405233271513,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.038033
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 5.002122045077101,
            "RMSE": 9.533278572445496,
            "R2": -22.968717144675637,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.048318
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.587842803317817,
            "RMSE": 9.003737317880292,
            "R2": -17.777085610739057,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.072946
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.458683971614509,
            "RMSE": 8.652080760634158,
            "R2": -16.390543570087573,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.099467
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 4.239995800771734,
            "RMSE": 8.280452519944822,
            "R2": -16.182419642449048,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.129303
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.943592784264584,
            "RMSE": 7.932077353220182,
            "R2": -14.885669934585447,
            "Memory in Mb": 0.004836082458496,
            "Time in s": 0.159907
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.7846302486799286,
            "RMSE": 7.646201644169009,
            "R2": -13.96015951270874,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.191262
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.6468171672887713,
            "RMSE": 7.389977926170562,
            "R2": -13.630953412847402,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.2233629999999999
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.526112368086922,
            "RMSE": 7.1621871014808685,
            "R2": -12.51535851099468,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.2587739999999999
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.5074300839639245,
            "RMSE": 6.985469271455791,
            "R2": -12.493228210862725,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.2965239999999999
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.434140699763514,
            "RMSE": 6.814822943627961,
            "R2": -12.570888751300782,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.3365219999999999
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.42722001559718,
            "RMSE": 6.678288393486038,
            "R2": -12.13957341395007,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.3787709999999999
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.332029752839207,
            "RMSE": 6.516115548498917,
            "R2": -11.941900403072644,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.4232519999999999
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.217390968362987,
            "RMSE": 6.356555790563252,
            "R2": -11.66392028459017,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.4696459999999999
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.100825681509746,
            "RMSE": 6.206562691759863,
            "R2": -11.47288048490914,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.516851
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 3.0187726323631243,
            "RMSE": 6.072312098448126,
            "R2": -10.723095644711892,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.5652379999999999
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.947022825868371,
            "RMSE": 5.94849802587685,
            "R2": -9.668265577306911,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.6161209999999999
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.867282537241402,
            "RMSE": 5.828292237410032,
            "R2": -9.005843404687633,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.6743809999999999
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.8281006485905213,
            "RMSE": 5.729646774374514,
            "R2": -8.467133754251039,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.7334769999999999
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.759113137285707,
            "RMSE": 5.623931694381955,
            "R2": -8.136932704030892,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.79343
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.7113951403332286,
            "RMSE": 5.52770300084093,
            "R2": -7.794584318722522,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.8541829999999999
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.646739535451309,
            "RMSE": 5.432090595521053,
            "R2": -7.695343452205655,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 0.94202
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.5972398336076634,
            "RMSE": 5.343168086286508,
            "R2": -7.621065103502998,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.0306859999999998
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.533455116608919,
            "RMSE": 5.255265792942869,
            "R2": -7.247487071141652,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.1202
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.497138699914293,
            "RMSE": 5.178243230235351,
            "R2": -6.88544757519055,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.210495
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.4712145738198297,
            "RMSE": 5.107804033669319,
            "R2": -6.528964961790648,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.30153
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.429247896498525,
            "RMSE": 5.0347117637840935,
            "R2": -6.262430681498119,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.3932969999999998
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.398090124502612,
            "RMSE": 4.967521902410674,
            "R2": -6.18160824182094,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.4857959999999997
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.360396901712673,
            "RMSE": 4.90286744871834,
            "R2": -6.1796262474179136,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.5790619999999995
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.3150393936015323,
            "RMSE": 4.836721469702358,
            "R2": -6.140716883970916,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.6730619999999998
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.267679208737699,
            "RMSE": 4.77254376860168,
            "R2": -5.948293801048677,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.7677929999999995
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.2434173929652075,
            "RMSE": 4.715867112708654,
            "R2": -5.857742612566196,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.863279
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.199009654391343,
            "RMSE": 4.656030786420359,
            "R2": -5.714767077599112,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 1.959541
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.159659681172017,
            "RMSE": 4.59898830049537,
            "R2": -5.610494506343661,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.056608
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.1249482408574707,
            "RMSE": 4.545176313025559,
            "R2": -5.527610390446187,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.175652
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.094058354623314,
            "RMSE": 4.493551443258636,
            "R2": -5.439404045425388,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.37025
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.062104039794744,
            "RMSE": 4.442864622918497,
            "R2": -5.284107374622643,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.565666
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.030706594140141,
            "RMSE": 4.393695684791879,
            "R2": -5.115247638705276,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.761867
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 2.003263565299311,
            "RMSE": 4.347049681772325,
            "R2": -5.011317673951863,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 2.958847
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.9706878923964863,
            "RMSE": 4.300488305941944,
            "R2": -4.979898179552831,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 3.156658
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.949819924248383,
            "RMSE": 4.257394252920471,
            "R2": -4.91037086709413,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 3.355253
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.9258186229947107,
            "RMSE": 4.214725843085415,
            "R2": -4.85305905428677,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 3.554625
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.900426010360992,
            "RMSE": 4.173138113177231,
            "R2": -4.849565137575967,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 3.754774
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.872733130377695,
            "RMSE": 4.13253797119814,
            "R2": -4.832859832721421,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 3.955698
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Linear Regression with l2 regularization",
            "dataset": "TrumpApproval",
            "MAE": 1.871510887330926,
            "RMSE": 4.130524228438989,
            "R2": -4.8310671605777085,
            "Memory in Mb": 0.0049962997436523,
            "Time in s": 4.156775
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 26.624124996337724,
            "RMSE": 28.77138517975663,
            "R2": -1064.5628215382144,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.000572
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 16.0510878175865,
            "RMSE": 20.931739283093208,
            "R2": -463.0233071270199,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.001645
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 12.49930786476168,
            "RMSE": 17.564629142555763,
            "R2": -213.26922094451623,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.003059
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 10.378514545021682,
            "RMSE": 15.405121473747096,
            "R2": -185.84310618709696,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.004809
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 10.844108697295251,
            "RMSE": 17.128215293517524,
            "R2": -56.27037115396167,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.006892
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 9.889488781892217,
            "RMSE": 15.88743125142584,
            "R2": -20.24022051627188,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.009306
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 9.103343480706034,
            "RMSE": 14.91594241381016,
            "R2": -11.548186613409534,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.012052
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 8.288900850158633,
            "RMSE": 14.011374344891149,
            "R2": -9.0389683228034,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.015129
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.736865157066078,
            "RMSE": 13.281093172283262,
            "R2": -6.543957317046456,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.018712
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.618125386224052,
            "RMSE": 12.858171267844924,
            "R2": -3.9379074608874927,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.022717
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.580936033253089,
            "RMSE": 12.51524762994286,
            "R2": -2.6028352541816,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.027127
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.191573127926202,
            "RMSE": 12.024287681643044,
            "R2": -1.7180920054032294,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.031928
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.001452140019149,
            "RMSE": 11.63905100750295,
            "R2": -1.062756769701151,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0371139999999999
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 6.959260067984971,
            "RMSE": 11.397763679955697,
            "R2": -0.6811278108981134,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0426889999999999
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.036161429677985,
            "RMSE": 11.359538570018056,
            "R2": -0.3423577921849861,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0486539999999999
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.141200516910354,
            "RMSE": 11.407680550849577,
            "R2": -0.0915406328349714,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0550109999999999
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.061965626679777,
            "RMSE": 11.211626858308708,
            "R2": 0.1367382583661435,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0617539999999999
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 6.988600359846859,
            "RMSE": 11.023879576943443,
            "R2": 0.3361231572252737,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0688849999999999
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.115468527113427,
            "RMSE": 11.18859440458875,
            "R2": 0.4362434515233688,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0763959999999999
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.571784360381598,
            "RMSE": 11.99879894105818,
            "R2": 0.4323613497222297,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0842879999999999
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.610536559977233,
            "RMSE": 11.962244483436113,
            "R2": 0.5174164020157423,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.0937539999999999
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.753677752144043,
            "RMSE": 12.109970858596688,
            "R2": 0.6020391290764042,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.1045109999999999
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 7.763402728464486,
            "RMSE": 12.046916639776326,
            "R2": 0.6579556132088519,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.123112
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 8.37232599699494,
            "RMSE": 12.9382814211091,
            "R2": 0.6395292100633578,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.147917
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 8.870502401884236,
            "RMSE": 14.03783628218945,
            "R2": 0.6266016212673495,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.173118
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 9.125553299295866,
            "RMSE": 14.312481045438886,
            "R2": 0.6638140497188074,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.198688
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 9.11642729851449,
            "RMSE": 14.234872044017685,
            "R2": 0.7115826499817814,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.225283
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 9.63053955101658,
            "RMSE": 15.01159987060024,
            "R2": 0.7143329631149452,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.252265
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 10.671899739762464,
            "RMSE": 17.42953249336733,
            "R2": 0.650531972004655,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.279616
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 11.1135598398273,
            "RMSE": 17.980470366868552,
            "R2": 0.6817264420663893,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.307329
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 11.368994570730054,
            "RMSE": 18.183536514460908,
            "R2": 0.7085274545262112,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.335405
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 11.47998520043724,
            "RMSE": 18.216810890558104,
            "R2": 0.7340681346165732,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.363842
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 12.490995837872443,
            "RMSE": 19.84181186896939,
            "R2": 0.693641639088806,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.392636
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 12.988870134156189,
            "RMSE": 20.81926805033374,
            "R2": 0.6899406322869175,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4217869999999999
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 13.420579982415202,
            "RMSE": 21.48960215237335,
            "R2": 0.7077263415053474,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4512919999999999
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 13.424816444492956,
            "RMSE": 21.37796604773129,
            "R2": 0.7303103668220552,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.481151
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 14.284688005634004,
            "RMSE": 22.70157511582256,
            "R2": 0.7173140296578691,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.514769
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 15.038658536726118,
            "RMSE": 24.042516108283174,
            "R2": 0.7023651722582169,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.548784
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 15.59029009825774,
            "RMSE": 24.916858152232297,
            "R2": 0.7159269075042054,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.583167
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 15.812702077031824,
            "RMSE": 25.07250049330081,
            "R2": 0.7327254930224041,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.617914
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 16.346042839206106,
            "RMSE": 25.68091484988461,
            "R2": 0.7315167856134144,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.653021
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 17.370765923434053,
            "RMSE": 27.689388199834635,
            "R2": 0.7068336630361484,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.688487
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 18.264179516209435,
            "RMSE": 29.30099868065636,
            "R2": 0.7101227966068765,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.724309
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 18.63502154656571,
            "RMSE": 29.559619400414903,
            "R2": 0.7211497930314269,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.760485
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 19.145243718121584,
            "RMSE": 30.130361606680754,
            "R2": 0.7274603750306702,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.7970149999999999
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 19.98075812634153,
            "RMSE": 31.43770898148617,
            "R2": 0.7119202509985216,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.8338999999999999
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 20.7046141289421,
            "RMSE": 32.42665929478992,
            "R2": 0.7107714616434232,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.8711439999999999
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 21.54126059149082,
            "RMSE": 33.75343345950398,
            "R2": 0.7182443212146572,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.908739
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 21.73603745751772,
            "RMSE": 33.829762552174344,
            "R2": 0.7286559632490104,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.946687
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 22.674609740448528,
            "RMSE": 35.33904665998618,
            "R2": 0.7130297805712756,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.984985
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 23.350956760305525,
            "RMSE": 36.24046007710213,
            "R2": 0.7114012814424304,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.023633
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 24.20743030595361,
            "RMSE": 37.47019278346573,
            "R2": 0.7146215025224946,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.06263
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "ChickWeights",
            "MAE": 24.342328163686027,
            "RMSE": 37.59599019491026,
            "R2": 0.7196900586014492,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.101865
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 20.806898309502586,
            "RMSE": 26.56763494383828,
            "R2": -1654.6182189603317,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.003003
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 14.866074912822512,
            "RMSE": 20.957300378156614,
            "R2": -175.5777711351631,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.009504
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 11.772648582583251,
            "RMSE": 17.555009093750932,
            "R2": -166.03688377592212,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.016813
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 10.372925375947808,
            "RMSE": 15.758572852966298,
            "R2": -134.01675577859288,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.02489
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 9.950999863257042,
            "RMSE": 14.807263848606526,
            "R2": -73.79513907078027,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.033777
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 9.131163180965077,
            "RMSE": 13.743973626529105,
            "R2": -53.66614209724606,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.043434
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 8.532294463666167,
            "RMSE": 12.93588512414824,
            "R2": -49.04322437944699,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.05944
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 8.33219708929472,
            "RMSE": 12.40854626547306,
            "R2": -39.60710527883104,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.077842
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 8.281092452540433,
            "RMSE": 12.043698542516514,
            "R2": -32.597139849683785,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0986229999999999
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 7.889313429527772,
            "RMSE": 11.548268653424005,
            "R2": -29.98173855178904,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.121857
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 7.555718436766954,
            "RMSE": 11.115454500430198,
            "R2": -29.96211572526289,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.149384
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 7.300584612865839,
            "RMSE": 10.768588372618428,
            "R2": -28.278525817685868,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.177703
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 7.073956995660685,
            "RMSE": 10.455941089275187,
            "R2": -26.97505735848669,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.206834
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.879100927439736,
            "RMSE": 10.179149173565092,
            "R2": -26.75935065850941,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.236782
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.698392466938299,
            "RMSE": 9.935855831167723,
            "R2": -25.01038668400382,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.26759
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.496977203333427,
            "RMSE": 9.674599820332077,
            "R2": -24.881575653507443,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.299212
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.319501534649956,
            "RMSE": 9.433800456219284,
            "R2": -25.005937123592886,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3316429999999999
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.189316591643737,
            "RMSE": 9.224778235838508,
            "R2": -24.070488458586468,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3648849999999999
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 6.05373584315195,
            "RMSE": 9.02603667348878,
            "R2": -23.83217081250324,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3989449999999999
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.893196935767096,
            "RMSE": 8.831009888188627,
            "R2": -23.44247524737401,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.4338649999999999
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.787168115685009,
            "RMSE": 8.669033337133486,
            "R2": -23.33356914323267,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.4696089999999999
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.789860410241021,
            "RMSE": 8.633597516354541,
            "R2": -22.69832962851382,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.5061589999999999
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.751464501173282,
            "RMSE": 8.532971696368575,
            "R2": -20.952287666855003,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.5516559999999999
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.758413491181221,
            "RMSE": 8.476961067588123,
            "R2": -20.166616413985547,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.599555
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.682950272504451,
            "RMSE": 8.3510488559106,
            "R2": -19.11151854181045,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.6519079999999999
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.627995468360723,
            "RMSE": 8.245754355787446,
            "R2": -18.64179334000355,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.705132
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.546541731300828,
            "RMSE": 8.130789587119862,
            "R2": -18.02792190581397,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.7591289999999999
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.474658569482086,
            "RMSE": 8.019262742277965,
            "R2": -17.95054121046633,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.813877
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.409420416004319,
            "RMSE": 7.920158789530457,
            "R2": -17.94222667017848,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.869386
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.394854582323811,
            "RMSE": 7.870548110777217,
            "R2": -17.498743363524373,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.941553
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.360408122735632,
            "RMSE": 7.801849933723111,
            "R2": -16.900148820132806,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.016153
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.332182524169608,
            "RMSE": 7.745335706289596,
            "R2": -16.312002846243146,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.093294
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.286484086266954,
            "RMSE": 7.672164501241343,
            "R2": -15.864310422998043,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.1728
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.240017672508232,
            "RMSE": 7.591734569529257,
            "R2": -15.77351804027652,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.259908
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.203631741702394,
            "RMSE": 7.526058935068808,
            "R2": -15.917522479350382,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.347915
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.198551833398676,
            "RMSE": 7.481861117849272,
            "R2": -16.086729414362967,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.436748
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.200051628353664,
            "RMSE": 7.443314903444159,
            "R2": -15.900950117878589,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.526395
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.146415466772512,
            "RMSE": 7.367313347205083,
            "R2": -15.73695108767244,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.61685
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.164438314106662,
            "RMSE": 7.352756459959702,
            "R2": -15.745558187055655,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.708114
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.199091748701669,
            "RMSE": 7.381485816300255,
            "R2": -16.029304780133675,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.8001699999999998
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.184244405270293,
            "RMSE": 7.343677512392477,
            "R2": -16.040406471643664,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.892982
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.162940711797175,
            "RMSE": 7.295196877254559,
            "R2": -15.972283354719572,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.986541
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.146772746928229,
            "RMSE": 7.251973114148485,
            "R2": -15.742866229030533,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.080851
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.141562534384022,
            "RMSE": 7.225910341165371,
            "R2": -15.54014218136778,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.175912
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.113671043317916,
            "RMSE": 7.181653170625269,
            "R2": -15.40700562565575,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.271722
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.082725756932772,
            "RMSE": 7.134180367835326,
            "R2": -15.456838882747109,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.368328
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.049460198345376,
            "RMSE": 7.092641752853287,
            "R2": -15.403746251323405,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.491683
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 5.012955702794688,
            "RMSE": 7.041188655025779,
            "R2": -15.335641983730405,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.616037
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 4.992587411597517,
            "RMSE": 7.002009756347646,
            "R2": -15.46809971530338,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.74122
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 4.986581819477306,
            "RMSE": 6.97972894589718,
            "R2": -15.638912943338369,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.867218
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 1",
            "dataset": "TrumpApproval",
            "MAE": 4.984033991902679,
            "RMSE": 6.9766666383395455,
            "R2": -15.63541499061877,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.993378
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 39.19936706045659,
            "RMSE": 55.118879370280126,
            "R2": -3909.733983269086,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.001533
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 31.495026158423794,
            "RMSE": 43.23165104261441,
            "R2": -1978.396532834284,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.004589
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 30.680053698816124,
            "RMSE": 39.98506660332775,
            "R2": -1109.3949268723327,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.008788
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 29.375885022911746,
            "RMSE": 37.29886968855784,
            "R2": -1094.3128086885838,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.014141
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 31.707444751978134,
            "RMSE": 40.753235251415205,
            "R2": -323.21264874535376,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.020635
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 31.96097441162184,
            "RMSE": 40.14945868859866,
            "R2": -134.64726490280094,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.028271
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 32.25989567011213,
            "RMSE": 39.82501544894248,
            "R2": -88.45229320906665,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.041195
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 32.76307262878121,
            "RMSE": 39.802536485586,
            "R2": -80.01195436020778,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.054526
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 32.66411513705659,
            "RMSE": 39.325402336106926,
            "R2": -65.1420916497486,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.068227
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 34.19940912800194,
            "RMSE": 40.704130728492046,
            "R2": -48.48362457590105,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.082293
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 34.629161705635866,
            "RMSE": 40.92880988729008,
            "R2": -37.53219439908784,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.096719
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 35.29035427006805,
            "RMSE": 41.59178542812187,
            "R2": -31.520750879588867,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.111503
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 36.23638449140802,
            "RMSE": 42.62018794050648,
            "R2": -26.65945376164948,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.126644
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 36.72501013289919,
            "RMSE": 42.91835139661213,
            "R2": -22.83677510551845,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.142141
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 36.731745662210095,
            "RMSE": 42.91744223234227,
            "R2": -18.16084111691443,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.157996
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 37.94402632003076,
            "RMSE": 44.39720610255875,
            "R2": -15.5331835318136,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.174208
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 38.69858083339784,
            "RMSE": 45.06856008203835,
            "R2": -12.949305609255877,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.190776
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 40.18624064352699,
            "RMSE": 46.68267333461602,
            "R2": -10.905017439998025,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.2077
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 40.85432327682653,
            "RMSE": 47.463811090322665,
            "R2": -9.145320047375163,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.224978
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 41.36451127701117,
            "RMSE": 48.41262940233051,
            "R2": -8.240888884363313,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.24261
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 42.17342712408468,
            "RMSE": 49.46918668675267,
            "R2": -7.253093192412523,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.260594
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 43.81461612103895,
            "RMSE": 51.73551020684679,
            "R2": -6.2632609796369465,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.27893
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 44.90819615603068,
            "RMSE": 53.07334253773936,
            "R2": -5.6387075541588505,
            "Memory in Mb": 0.0034055709838867,
            "Time in s": 0.297618
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 46.45334973048907,
            "RMSE": 55.82244674340302,
            "R2": -5.710187070138379,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.3166589999999999
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 48.05643802527038,
            "RMSE": 58.804796990371536,
            "R2": -5.552357606253864,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.3360539999999999
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 49.41721923566732,
            "RMSE": 60.72765972830183,
            "R2": -5.052332799264802,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.3558019999999999
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 51.23299901747073,
            "RMSE": 63.29154255446438,
            "R2": -4.701716347098143,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.3759049999999999
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 52.82583967659276,
            "RMSE": 65.36972550348784,
            "R2": -4.417008197806662,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.3963679999999999
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 54.851023886215806,
            "RMSE": 70.45860717413167,
            "R2": -4.71089374971376,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4171839999999999
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 56.58220488738844,
            "RMSE": 72.62689780553444,
            "R2": -4.192702597603254,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4383529999999999
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 58.456862484765374,
            "RMSE": 75.26810540469758,
            "R2": -3.994165343488624,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4598799999999999
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 59.98229295122657,
            "RMSE": 76.97767263775137,
            "R2": -3.748486775975887,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.4817619999999999
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 61.989108820835376,
            "RMSE": 80.62951920841103,
            "R2": -4.0588898392459045,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.503996
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 63.93796840595574,
            "RMSE": 84.48840832488506,
            "R2": -4.106322034628877,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.526584
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 65.15236861414519,
            "RMSE": 85.79755918852514,
            "R2": -3.6588935912158114,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.551564
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 66.90365663892747,
            "RMSE": 87.9249329113371,
            "R2": -3.562003118430529,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.5777180000000001
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 68.17917622540308,
            "RMSE": 89.58756462611774,
            "R2": -3.402382103640547,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.6050150000000001
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 70.80702754948452,
            "RMSE": 94.96753809429286,
            "R2": -3.643808228470034,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.6334650000000001
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 72.44730173566225,
            "RMSE": 97.09455233033468,
            "R2": -3.313534410167211,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.663057
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 74.29167351363806,
            "RMSE": 99.40774027870644,
            "R2": -3.201483315326532,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.693783
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 75.83174494284101,
            "RMSE": 101.77506329990584,
            "R2": -3.216760347648722,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.725638
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 78.5111288104629,
            "RMSE": 106.99570126481906,
            "R2": -3.3774383617967887,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.758621
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 81.63741116996734,
            "RMSE": 112.58139375423264,
            "R2": -3.2793958269429844,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.79391
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 82.66628549198501,
            "RMSE": 113.50934761838604,
            "R2": -3.1118432523868984,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.829617
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 84.40016304476833,
            "RMSE": 116.34990208847,
            "R2": -3.0639935553557365,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.865723
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 86.52132256561038,
            "RMSE": 120.30772815943004,
            "R2": -3.2188880650982723,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.902224
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 87.79244029751037,
            "RMSE": 121.63869088166206,
            "R2": -3.069866847809537,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.93912
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 90.43735682351402,
            "RMSE": 126.62066541565774,
            "R2": -2.9650251625135784,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 0.976398
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 91.59763342322412,
            "RMSE": 127.6295949640952,
            "R2": -2.862114672867245,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.014034
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 93.80067010965053,
            "RMSE": 131.39026699356185,
            "R2": -2.966921087845916,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.0520230000000002
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 96.52355815418714,
            "RMSE": 136.33091173427522,
            "R2": -3.0840934586689466,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.0903630000000002
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 99.60515399822415,
            "RMSE": 141.80943605664237,
            "R2": -3.0875177525301325,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.129055
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "ChickWeights",
            "MAE": 100.62422612381133,
            "RMSE": 143.06646930774232,
            "R2": -3.0591132110693486,
            "Memory in Mb": 0.0034589767456054,
            "Time in s": 1.167982
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 48.24517612267716,
            "RMSE": 65.52170729560882,
            "R2": -10068.892101934754,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0014
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 41.96170708962665,
            "RMSE": 54.398737007050464,
            "R2": -1188.715138210959,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0037089999999999
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 37.75687919715097,
            "RMSE": 48.78450375470138,
            "R2": -1288.953469480389,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0068
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 34.906129137913965,
            "RMSE": 44.99379649673769,
            "R2": -1099.675197364534,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.010662
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 33.91700787894482,
            "RMSE": 42.88559259598606,
            "R2": -626.4029768570122,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0153429999999999
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 33.25318798467783,
            "RMSE": 41.41783833748641,
            "R2": -495.442160460349,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0207979999999999
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 32.454169303664,
            "RMSE": 40.06534641626261,
            "R2": -479.0547686921885,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0270209999999999
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.456143135335843,
            "RMSE": 38.757475924320815,
            "R2": -395.1605214699538,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0340139999999999
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.609503890456164,
            "RMSE": 37.605439707525925,
            "R2": -326.55474603918685,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0417749999999999
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.18524212396377,
            "RMSE": 36.915721425331306,
            "R2": -315.5882175367347,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0503299999999999
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.065472528043387,
            "RMSE": 36.44442035805252,
            "R2": -331.8421153382835,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0596439999999999
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.78865598017145,
            "RMSE": 35.91292614465666,
            "R2": -324.6366197799479,
            "Memory in Mb": 0.0043020248413085,
            "Time in s": 0.0697149999999999
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.781114432924586,
            "RMSE": 35.79236523689611,
            "R2": -326.81251307944893,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.0853099999999999
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.53323842574737,
            "RMSE": 35.35890478021234,
            "R2": -333.95306350592915,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.1033029999999999
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.45783145374521,
            "RMSE": 35.09485674586195,
            "R2": -323.506345927368,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.1237949999999999
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.587592426740265,
            "RMSE": 34.99099947403571,
            "R2": -337.56135797788454,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.1466579999999999
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.592186767063264,
            "RMSE": 34.82748458593961,
            "R2": -353.4405109424598,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.178415
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.81187133621213,
            "RMSE": 34.87255971663822,
            "R2": -357.27671195740294,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.2110159999999999
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 29.96085998978186,
            "RMSE": 34.8837386376585,
            "R2": -369.9082961036221,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.2444429999999999
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.10861760053803,
            "RMSE": 34.89146879370085,
            "R2": -380.5600928496674,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.2787509999999999
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.237056214581205,
            "RMSE": 34.87113676993804,
            "R2": -392.72834237954817,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3138979999999999
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.396870134836657,
            "RMSE": 34.919939008119975,
            "R2": -386.68686883790514,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3498769999999999
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.5142090152444,
            "RMSE": 34.936230377424984,
            "R2": -366.9859696545672,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.3866269999999999
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.60304766371323,
            "RMSE": 34.90556469597589,
            "R2": -357.88920799289923,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.4241359999999999
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.723498435612367,
            "RMSE": 34.929338036322235,
            "R2": -350.83863344189655,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.462404
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.811640107301315,
            "RMSE": 34.91688659850233,
            "R2": -351.20164208687333,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.5014689999999999
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.90684609870959,
            "RMSE": 34.93305250730057,
            "R2": -350.23597283973027,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.541291
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.83222834631613,
            "RMSE": 34.80844611918478,
            "R2": -356.0442181025925,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.58187
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.81214247339674,
            "RMSE": 34.7464796172207,
            "R2": -363.5733105101423,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.629234
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.96266506693229,
            "RMSE": 34.82326914665847,
            "R2": -361.1357082485383,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.6774979999999999
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.066025409450507,
            "RMSE": 34.86865150113252,
            "R2": -356.54586556020155,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.743837
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.17687176552783,
            "RMSE": 34.929241693507976,
            "R2": -351.0830657253844,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.810979
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.17965741293356,
            "RMSE": 34.892251240403844,
            "R2": -347.8114699445998,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.87889
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.2564554130016,
            "RMSE": 34.924087575336145,
            "R2": -353.970503405387,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 0.947564
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.205643809070587,
            "RMSE": 34.8991435368638,
            "R2": -362.7735100050666,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.017054
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.176512353694505,
            "RMSE": 34.84497410939031,
            "R2": -369.6124031875757,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.087302
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.10578554229227,
            "RMSE": 34.74995813099662,
            "R2": -367.37224871607793,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.158309
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.047274834607855,
            "RMSE": 34.691812272848594,
            "R2": -370.11801689051305,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.23401
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.10380007346799,
            "RMSE": 34.703384372728905,
            "R2": -372.0292841604823,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.319073
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.08555480002386,
            "RMSE": 34.670374973731704,
            "R2": -374.68721566223496,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.406663
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.19885148971359,
            "RMSE": 34.750222550469864,
            "R2": -380.56447731408525,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.496625
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.25463715565584,
            "RMSE": 34.7657556157579,
            "R2": -384.4513633760299,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.5889890000000002
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.316317159155098,
            "RMSE": 34.79186578621207,
            "R2": -384.3655387384781,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 1.693075
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.241979864666277,
            "RMSE": 34.706915019978055,
            "R2": -380.5804591262153,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.065505
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.224226006229813,
            "RMSE": 34.673719949901624,
            "R2": -381.4558834892021,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.440347
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.14134426690263,
            "RMSE": 34.58836614994504,
            "R2": -385.8283921715467,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 2.817664
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.997921544748237,
            "RMSE": 34.45657797481166,
            "R2": -386.1428842704396,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 3.197344
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.060400411885407,
            "RMSE": 34.566740304864304,
            "R2": -392.6960879419034,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 3.57811
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 30.96911325529305,
            "RMSE": 34.515642414657464,
            "R2": -399.1566023636026,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 3.959721
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.09609109084082,
            "RMSE": 34.63142513356851,
            "R2": -408.6269881777103,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 4.342153
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Passive-Aggressive Regressor, mode 2",
            "dataset": "TrumpApproval",
            "MAE": 31.093334457100017,
            "RMSE": 34.62570772928248,
            "R2": -408.7651443035993,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 4.724752
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 4.6439393939393945,
            "RMSE": 12.708027567111456,
            "R2": -206.8805289598106,
            "Memory in Mb": 0.0208587646484375,
            "Time in s": 0.001745
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.7674242424242426,
            "RMSE": 9.021574170013263,
            "R2": -85.19732920009746,
            "Memory in Mb": 0.0300941467285156,
            "Time in s": 0.005817
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.3601010101010105,
            "RMSE": 7.4346315168437105,
            "R2": -37.38846247874159,
            "Memory in Mb": 0.0395355224609375,
            "Time in s": 0.012524
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 1.988257575757577,
            "RMSE": 6.459864921032004,
            "R2": -31.8544119108943,
            "Memory in Mb": 0.0488433837890625,
            "Time in s": 0.023287
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.201515151515152,
            "RMSE": 6.079045396219125,
            "R2": -6.214006750846093,
            "Memory in Mb": 0.0583724975585937,
            "Time in s": 0.035467
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.2709595959595963,
            "RMSE": 5.693634951086079,
            "R2": -1.7279153546475992,
            "Memory in Mb": 0.0685691833496093,
            "Time in s": 0.049542
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.6114718614718617,
            "RMSE": 5.706903555891601,
            "R2": -0.8368793810695487,
            "Memory in Mb": 0.0782623291015625,
            "Time in s": 0.068809
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.5236742424242427,
            "RMSE": 5.412016943708686,
            "R2": -0.4977726858852578,
            "Memory in Mb": 0.0879554748535156,
            "Time in s": 0.099298
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.4695286195286204,
            "RMSE": 5.169211114529652,
            "R2": -0.1428260058474422,
            "Memory in Mb": 0.0976486206054687,
            "Time in s": 0.132347
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 2.7553030303030317,
            "RMSE": 5.269495069058163,
            "R2": 0.1706792355598563,
            "Memory in Mb": 0.1073417663574218,
            "Time in s": 0.167959
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 3.1511019283746564,
            "RMSE": 5.580125306741311,
            "R2": 0.2837685080447375,
            "Memory in Mb": 0.117034912109375,
            "Time in s": 0.206371
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 3.315782828282829,
            "RMSE": 5.649452649212155,
            "R2": 0.3999904226030885,
            "Memory in Mb": 0.1272315979003906,
            "Time in s": 0.248032
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 3.6019813519813537,
            "RMSE": 5.868270501527574,
            "R2": 0.475635686274607,
            "Memory in Mb": 0.1369247436523437,
            "Time in s": 0.313422
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 3.745995670995673,
            "RMSE": 5.964828521670115,
            "R2": 0.5395766265984425,
            "Memory in Mb": 0.1466178894042968,
            "Time in s": 0.409887
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 4.050202020202021,
            "RMSE": 6.4542180762994805,
            "R2": 0.5666546129487657,
            "Memory in Mb": 0.15631103515625,
            "Time in s": 0.575073
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 4.420928030303032,
            "RMSE": 6.954884488253524,
            "R2": 0.5942812793055753,
            "Memory in Mb": 0.1660041809082031,
            "Time in s": 0.746583
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 4.757664884135474,
            "RMSE": 7.278917476631412,
            "R2": 0.6361362300357987,
            "Memory in Mb": 0.1756973266601562,
            "Time in s": 0.922657
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 5.192340067340069,
            "RMSE": 7.767087259749381,
            "R2": 0.6704396407154757,
            "Memory in Mb": 0.1858940124511718,
            "Time in s": 1.103506
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 5.571690590111645,
            "RMSE": 8.414476478500024,
            "R2": 0.6811438926382001,
            "Memory in Mb": 0.195587158203125,
            "Time in s": 1.289988
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 6.017651515151518,
            "RMSE": 9.535434778453542,
            "R2": 0.641509702161033,
            "Memory in Mb": 0.2052803039550781,
            "Time in s": 1.481758
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 6.514646464646468,
            "RMSE": 10.15268578355149,
            "R2": 0.652376522878304,
            "Memory in Mb": 0.2149734497070312,
            "Time in s": 1.688886
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 7.006955922865016,
            "RMSE": 10.883499074839364,
            "R2": 0.6785664047839641,
            "Memory in Mb": 0.2246665954589843,
            "Time in s": 1.905808
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 7.401119894598158,
            "RMSE": 11.259257694820905,
            "R2": 0.7012209269570091,
            "Memory in Mb": 0.2343597412109375,
            "Time in s": 2.129833
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 7.873800505050509,
            "RMSE": 12.237701558545494,
            "R2": 0.6775097363055258,
            "Memory in Mb": 0.2446098327636718,
            "Time in s": 2.3598440000000003
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 8.501393939393942,
            "RMSE": 13.456617650281162,
            "R2": 0.6568816796501455,
            "Memory in Mb": 0.254302978515625,
            "Time in s": 2.605392
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 8.999592074592076,
            "RMSE": 14.081405883193678,
            "R2": 0.6745818706784585,
            "Memory in Mb": 0.2639961242675781,
            "Time in s": 2.8696780000000004
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 9.403647586980924,
            "RMSE": 14.487230370517851,
            "R2": 0.7012657763253116,
            "Memory in Mb": 0.2736892700195312,
            "Time in s": 3.1592620000000005
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 9.82559523809524,
            "RMSE": 15.247017337775036,
            "R2": 0.7053028346163965,
            "Memory in Mb": 0.2833824157714844,
            "Time in s": 3.471445000000001
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 10.570794148380358,
            "RMSE": 17.082267622288043,
            "R2": 0.6643188025566307,
            "Memory in Mb": 0.2930755615234375,
            "Time in s": 3.895766000000001
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 11.342676767676773,
            "RMSE": 18.20491056057454,
            "R2": 0.6737311884314376,
            "Memory in Mb": 0.3032722473144531,
            "Time in s": 4.333389
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 11.75625610948192,
            "RMSE": 18.5968301788559,
            "R2": 0.6951271166039881,
            "Memory in Mb": 0.3129653930664062,
            "Time in s": 4.790776
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 12.16955492424243,
            "RMSE": 18.94133239132977,
            "R2": 0.7124941202708752,
            "Memory in Mb": 0.3226585388183594,
            "Time in s": 5.260338
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 12.609595959595964,
            "RMSE": 19.7022738973151,
            "R2": 0.6979354313341102,
            "Memory in Mb": 0.3323516845703125,
            "Time in s": 5.750168
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 13.251024955436726,
            "RMSE": 20.7851367099449,
            "R2": 0.6909564285254863,
            "Memory in Mb": 0.3420448303222656,
            "Time in s": 6.251716
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 13.78255411255412,
            "RMSE": 21.481025974379733,
            "R2": 0.7079595790244884,
            "Memory in Mb": 0.3522415161132812,
            "Time in s": 6.769761
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 14.010311447811455,
            "RMSE": 21.53574862211497,
            "R2": 0.7263147242326703,
            "Memory in Mb": 0.3619346618652344,
            "Time in s": 7.297159
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 14.576126126126132,
            "RMSE": 22.56379182999173,
            "R2": 0.720735043690873,
            "Memory in Mb": 0.3716278076171875,
            "Time in s": 7.841892
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 15.256658692185017,
            "RMSE": 23.708044463333223,
            "R2": 0.710588766956741,
            "Memory in Mb": 0.38134765625,
            "Time in s": 8.4256
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 15.863597513597522,
            "RMSE": 24.650993900023582,
            "R2": 0.7219567169230845,
            "Memory in Mb": 0.3910675048828125,
            "Time in s": 9.118776
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 16.15655303030304,
            "RMSE": 24.89490243600041,
            "R2": 0.7364984966983625,
            "Memory in Mb": 0.4007606506347656,
            "Time in s": 9.83444
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 16.474242424242437,
            "RMSE": 25.235361878916876,
            "R2": 0.7407521096740679,
            "Memory in Mb": 0.4109573364257812,
            "Time in s": 10.564263
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 17.206240981241,
            "RMSE": 26.51959634874256,
            "R2": 0.731081178462164,
            "Memory in Mb": 0.4206771850585937,
            "Time in s": 11.311639
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 18.061486962649766,
            "RMSE": 27.919441407022266,
            "R2": 0.7368140706560946,
            "Memory in Mb": 0.430450439453125,
            "Time in s": 12.077289
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 18.444800275482105,
            "RMSE": 28.396609389438456,
            "R2": 0.742660608098584,
            "Memory in Mb": 0.4401702880859375,
            "Time in s": 12.86575
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 18.85067340067341,
            "RMSE": 28.917019336286597,
            "R2": 0.7489686179689856,
            "Memory in Mb": 0.4499168395996094,
            "Time in s": 13.665871
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 19.39739789196312,
            "RMSE": 29.705616030262235,
            "R2": 0.7427898649120724,
            "Memory in Mb": 2.5872955322265625,
            "Time in s": 16.820609
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 20.115441650548043,
            "RMSE": 30.73530324863436,
            "R2": 0.7401565757784102,
            "Memory in Mb": 2.6296463012695312,
            "Time in s": 20.027458000000003
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 20.836142676767683,
            "RMSE": 31.98623382904741,
            "R2": 0.7469752640852343,
            "Memory in Mb": 2.6746597290039062,
            "Time in s": 23.267231
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 21.017594310451457,
            "RMSE": 32.125858524254696,
            "R2": 0.7553011842320496,
            "Memory in Mb": 2.717792510986328,
            "Time in s": 26.555547000000004
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 21.677242424242426,
            "RMSE": 32.83678407493398,
            "R2": 0.7522301799631583,
            "Memory in Mb": 2.769092559814453,
            "Time in s": 29.885669000000004
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 22.80977421271539,
            "RMSE": 35.198755082788004,
            "R2": 0.727753941720713,
            "Memory in Mb": 2.8112449645996094,
            "Time in s": 33.249092000000005
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 24.195600233100237,
            "RMSE": 38.25560047694445,
            "R2": 0.7025325582791198,
            "Memory in Mb": 2.857513427734375,
            "Time in s": 36.653026
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "ChickWeights",
            "MAE": 24.84062860438293,
            "RMSE": 39.201635479156685,
            "R2": 0.6952358931227007,
            "Memory in Mb": 2.885215759277344,
            "Time in s": 40.087818000000006
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 2.554585433333335,
            "RMSE": 9.794739803036965,
            "R2": -224.02989290855143,
            "Memory in Mb": 0.0335884094238281,
            "Time in s": 0.001545
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 1.7993247666666672,
            "RMSE": 6.973235588114817,
            "R2": -18.54942689237887,
            "Memory in Mb": 0.0554847717285156,
            "Time in s": 0.0054
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 1.366773144444445,
            "RMSE": 5.705236645726316,
            "R2": -16.642396889136542,
            "Memory in Mb": 0.0773544311523437,
            "Time in s": 0.012332
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 1.1277757833333335,
            "RMSE": 4.947712433075743,
            "R2": -12.30953248968821,
            "Memory in Mb": 0.0997543334960937,
            "Time in s": 0.028826
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 1.046201766666667,
            "RMSE": 4.439862929674892,
            "R2": -5.724544452799038,
            "Memory in Mb": 0.1216506958007812,
            "Time in s": 0.050318
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 1.000865705555556,
            "RMSE": 4.0744555355418335,
            "R2": -3.804331488196434,
            "Memory in Mb": 0.1435470581054687,
            "Time in s": 0.086896
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9447764619047624,
            "RMSE": 3.7809361134406254,
            "R2": -3.275153002458012,
            "Memory in Mb": 0.1659469604492187,
            "Time in s": 0.149837
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9352969166666673,
            "RMSE": 3.5531790499707645,
            "R2": -2.329617982408036,
            "Memory in Mb": 0.1878433227539062,
            "Time in s": 0.2304459999999999
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9445764925925928,
            "RMSE": 3.380979243961517,
            "R2": -1.647692611170827,
            "Memory in Mb": 0.2097396850585937,
            "Time in s": 0.432465
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9456943733333336,
            "RMSE": 3.232789339199984,
            "R2": -1.427877878808435,
            "Memory in Mb": 0.2321395874023437,
            "Time in s": 0.648003
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9124697575757575,
            "RMSE": 3.0919339165015143,
            "R2": -1.3957229068060464,
            "Memory in Mb": 0.2540359497070312,
            "Time in s": 0.888162
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9329223611111108,
            "RMSE": 2.985727855147271,
            "R2": -1.2507750530936188,
            "Memory in Mb": 0.2759323120117187,
            "Time in s": 1.171554
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.9025974717948716,
            "RMSE": 2.873740673763463,
            "R2": -1.11319648675526,
            "Memory in Mb": 0.2984657287597656,
            "Time in s": 1.484213
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.8654126523809523,
            "RMSE": 2.773524640439575,
            "R2": -1.0608690746642817,
            "Memory in Mb": 0.3203620910644531,
            "Time in s": 1.81098
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.8525042622222223,
            "RMSE": 2.688069339615046,
            "R2": -0.9037818439458584,
            "Memory in Mb": 0.3422584533691406,
            "Time in s": 2.170241
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.8265282395833334,
            "RMSE": 2.6077957497476296,
            "R2": -0.880493509713772,
            "Memory in Mb": 0.3646583557128906,
            "Time in s": 2.558101
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.8137511019607846,
            "RMSE": 2.539210136300266,
            "R2": -0.8840673465916704,
            "Memory in Mb": 0.3865547180175781,
            "Time in s": 3.13755
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.7887328240740744,
            "RMSE": 2.4696835584739105,
            "R2": -0.7969398815662787,
            "Memory in Mb": 0.4084510803222656,
            "Time in s": 3.744079
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.7710879228070179,
            "RMSE": 2.4087271831437693,
            "R2": -0.7684619785143365,
            "Memory in Mb": 0.4303474426269531,
            "Time in s": 4.380375
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.756179386666667,
            "RMSE": 2.351105641867075,
            "R2": -0.7324819925835522,
            "Memory in Mb": 0.4527473449707031,
            "Time in s": 5.04744
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.7300392539682541,
            "RMSE": 2.295700426816902,
            "R2": -0.7064552265553199,
            "Memory in Mb": 0.4746437072753906,
            "Time in s": 5.735437
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.7180258560606063,
            "RMSE": 2.24592493832078,
            "R2": -0.6037054809307543,
            "Memory in Mb": 0.4965400695800781,
            "Time in s": 6.669957
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.7103659666666668,
            "RMSE": 2.200554873752302,
            "R2": -0.4599688187191526,
            "Memory in Mb": 0.5189399719238281,
            "Time in s": 7.633919000000001
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6905233472222223,
            "RMSE": 2.1551860359584523,
            "R2": -0.3681716631920215,
            "Memory in Mb": 0.5408363342285156,
            "Time in s": 8.635162000000001
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6835753693333335,
            "RMSE": 2.11616682722306,
            "R2": -0.2914054626850582,
            "Memory in Mb": 2.70669937133789,
            "Time in s": 12.111573000000002
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6741869282051286,
            "RMSE": 2.077523623184556,
            "R2": -0.2468444979074313,
            "Memory in Mb": 2.7946739196777344,
            "Time in s": 15.640183000000002
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6635047197530868,
            "RMSE": 2.0412653603832838,
            "R2": -0.1992917531598592,
            "Memory in Mb": 2.8836631774902344,
            "Time in s": 19.224183000000004
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6666769047619049,
            "RMSE": 2.01181749557566,
            "R2": -0.1926963577893738,
            "Memory in Mb": 2.973125457763672,
            "Time in s": 22.863484000000003
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.662313208045977,
            "RMSE": 1.9804661409620816,
            "R2": -0.1843991731259868,
            "Memory in Mb": 3.06191635131836,
            "Time in s": 26.560120000000005
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6595208444444446,
            "RMSE": 1.9515625148224915,
            "R2": -0.1373580524839326,
            "Memory in Mb": 3.158283233642578,
            "Time in s": 30.31408200000001
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6603871010752689,
            "RMSE": 1.924909501402362,
            "R2": -0.0896376201735813,
            "Memory in Mb": 3.248737335205078,
            "Time in s": 34.12595900000001
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6518434010416667,
            "RMSE": 1.8967107462711992,
            "R2": -0.0381713320833934,
            "Memory in Mb": 3.341320037841797,
            "Time in s": 37.99311800000001
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6481796161616163,
            "RMSE": 1.873162681009878,
            "R2": -0.00527242303062,
            "Memory in Mb": 3.435527801513672,
            "Time in s": 41.91854100000001
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6594073715686274,
            "RMSE": 1.8574009428793896,
            "R2": -0.0040456355040212,
            "Memory in Mb": 3.5269508361816406,
            "Time in s": 45.90599500000001
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6619153695238096,
            "RMSE": 1.8376987056605067,
            "R2": -0.0086724321908719,
            "Memory in Mb": 3.615283966064453,
            "Time in s": 49.957909000000015
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6538050537037038,
            "RMSE": 1.8142062090777376,
            "R2": -0.0046457590045041,
            "Memory in Mb": 3.7059364318847656,
            "Time in s": 54.07172000000001
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6437102684684685,
            "RMSE": 1.7904191974020045,
            "R2": 0.0221149973980568,
            "Memory in Mb": 3.8005104064941406,
            "Time in s": 58.24412800000001
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6465423666666668,
            "RMSE": 1.7722456151874884,
            "R2": 0.0314860408387392,
            "Memory in Mb": 3.89126205444336,
            "Time in s": 62.47501600000001
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6423591829059828,
            "RMSE": 1.752432393946061,
            "R2": 0.0487781645727875,
            "Memory in Mb": 3.987659454345703,
            "Time in s": 66.76475200000002
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6415445258333332,
            "RMSE": 1.7335108155585357,
            "R2": 0.0607905571401552,
            "Memory in Mb": 4.087154388427734,
            "Time in s": 71.11932700000001
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.641812437398374,
            "RMSE": 1.7198679523833968,
            "R2": 0.0653630129096917,
            "Memory in Mb": 4.179523468017578,
            "Time in s": 75.53533700000001
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6391550126984127,
            "RMSE": 1.7023246638821516,
            "R2": 0.0758317950759702,
            "Memory in Mb": 4.276576995849609,
            "Time in s": 80.015814
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6397551612403103,
            "RMSE": 1.6865214638981003,
            "R2": 0.0944734629735503,
            "Memory in Mb": 4.372867584228516,
            "Time in s": 84.56990800000001
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6401663234848486,
            "RMSE": 1.6719359262678322,
            "R2": 0.1144902218209267,
            "Memory in Mb": 4.465221405029297,
            "Time in s": 89.18993400000001
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6373928251851855,
            "RMSE": 1.6559913256631793,
            "R2": 0.1276383063389357,
            "Memory in Mb": 4.558887481689453,
            "Time in s": 93.877546
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6333341724637681,
            "RMSE": 1.6410816825275083,
            "R2": 0.1291995533352813,
            "Memory in Mb": 4.652858734130859,
            "Time in s": 98.626246
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.637460545390071,
            "RMSE": 1.630772212254164,
            "R2": 0.1328113217779126,
            "Memory in Mb": 4.746517181396484,
            "Time in s": 103.437785
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6446958777777775,
            "RMSE": 1.6213030711335543,
            "R2": 0.1338907909289651,
            "Memory in Mb": 4.844425201416016,
            "Time in s": 108.312072
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.643768610068027,
            "RMSE": 1.6085965270907718,
            "R2": 0.1308548353743899,
            "Memory in Mb": 4.935100555419922,
            "Time in s": 113.251739
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6420156240666665,
            "RMSE": 1.59493855356346,
            "R2": 0.1311681221050482,
            "Memory in Mb": 5.030651092529297,
            "Time in s": 118.255967
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "k-Nearest Neighbors",
            "dataset": "TrumpApproval",
            "MAE": 0.6416785025641023,
            "RMSE": 1.5941707450098015,
            "R2": 0.1314249186277071,
            "Memory in Mb": 5.032634735107422,
            "Time in s": 123.301096
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 8.042756132756132,
            "RMSE": 17.336048579080593,
            "R2": -385.8634917094176,
            "Memory in Mb": 0.0162086486816406,
            "Time in s": 0.002632
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.456785613727984,
            "RMSE": 12.282422261556867,
            "R2": -158.770726389092,
            "Memory in Mb": 0.0177879333496093,
            "Time in s": 0.007319
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 3.4353973358733074,
            "RMSE": 10.07037651743448,
            "R2": -69.4325218162971,
            "Memory in Mb": 0.0230522155761718,
            "Time in s": 0.013907
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 2.736909422894262,
            "RMSE": 8.732393473100391,
            "R2": -59.03623058514604,
            "Memory in Mb": 0.0241050720214843,
            "Time in s": 0.0217009999999999
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 2.788577579622257,
            "RMSE": 8.074088551816661,
            "R2": -11.726025456653014,
            "Memory in Mb": 0.0309486389160156,
            "Time in s": 0.0303349999999999
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 3.395880085598137,
            "RMSE": 7.878422021930021,
            "R2": -4.223121571879303,
            "Memory in Mb": 0.0404243469238281,
            "Time in s": 0.040093
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 3.889526501621088,
            "RMSE": 7.800910386370324,
            "R2": -2.432180745921895,
            "Memory in Mb": 0.0467414855957031,
            "Time in s": 0.0511699999999999
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.072650698433535,
            "RMSE": 7.572197783925699,
            "R2": -1.9320509270116557,
            "Memory in Mb": 0.0525321960449218,
            "Time in s": 0.0635609999999999
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.410984939713907,
            "RMSE": 7.55185413515251,
            "R2": -1.439151418709002,
            "Memory in Mb": 0.0535850524902343,
            "Time in s": 0.0772419999999999
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.370948473977548,
            "RMSE": 7.327634340090197,
            "R2": -0.6036593212329582,
            "Memory in Mb": 0.0551643371582031,
            "Time in s": 0.0921019999999999
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.401973824893138,
            "RMSE": 7.197046558152955,
            "R2": -0.1914453698838978,
            "Memory in Mb": 0.0551643371582031,
            "Time in s": 0.1081669999999999
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.283071400630936,
            "RMSE": 6.979735895990854,
            "R2": 0.0841519683549982,
            "Memory in Mb": 0.0551643371582031,
            "Time in s": 0.1323959999999999
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.169649051526778,
            "RMSE": 6.77851615807502,
            "R2": 0.3003478880703081,
            "Memory in Mb": 0.0556907653808593,
            "Time in s": 0.1602449999999999
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.107721988217097,
            "RMSE": 6.620782354691122,
            "R2": 0.4327427443050297,
            "Memory in Mb": 0.0556907653808593,
            "Time in s": 0.1914819999999999
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.386134129138624,
            "RMSE": 6.8739888422895685,
            "R2": 0.5084535624523276,
            "Memory in Mb": 0.0556907653808593,
            "Time in s": 0.2319989999999999
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.592324836010107,
            "RMSE": 7.0395287886899816,
            "R2": 0.5843455987500039,
            "Memory in Mb": 0.0562171936035156,
            "Time in s": 0.273788
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.658423416973056,
            "RMSE": 7.057579140031887,
            "R2": 0.6579286220132116,
            "Memory in Mb": 0.0562171936035156,
            "Time in s": 0.316974
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.6782517314261085,
            "RMSE": 7.042640058036562,
            "R2": 0.7290497323677609,
            "Memory in Mb": 0.0562171936035156,
            "Time in s": 0.361531
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 4.896652959256127,
            "RMSE": 7.410861778989444,
            "R2": 0.7526693351807108,
            "Memory in Mb": 0.0217466354370117,
            "Time in s": 0.409543
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 5.507880191409123,
            "RMSE": 8.546476599974424,
            "R2": 0.7120144996082314,
            "Memory in Mb": 0.0280637741088867,
            "Time in s": 0.458317
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 5.703958017872014,
            "RMSE": 8.760797449465004,
            "R2": 0.7411581545051223,
            "Memory in Mb": 0.0333280563354492,
            "Time in s": 0.507954
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 5.934527728379076,
            "RMSE": 9.145062262320872,
            "R2": 0.7730513990797492,
            "Memory in Mb": 0.0380659103393554,
            "Time in s": 0.576578
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 6.025889093973978,
            "RMSE": 9.259481324724224,
            "R2": 0.7979290061199974,
            "Memory in Mb": 0.0417509078979492,
            "Time in s": 0.647861
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 6.701040765258382,
            "RMSE": 10.569442782845146,
            "R2": 0.7594412957229723,
            "Memory in Mb": 0.0418310165405273,
            "Time in s": 0.7217790000000001
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 7.201977905163474,
            "RMSE": 11.695812678726384,
            "R2": 0.740801257827299,
            "Memory in Mb": 0.0418310165405273,
            "Time in s": 0.7983520000000001
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 7.47608974362833,
            "RMSE": 12.176082777300053,
            "R2": 0.7566872347890514,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 0.889757
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 7.495029117947843,
            "RMSE": 12.186858586615225,
            "R2": 0.7886035011133373,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 0.982264
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 8.05089484284177,
            "RMSE": 13.06419009031293,
            "R2": 0.7836428997387894,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.075782
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 9.171875092169309,
            "RMSE": 15.802620207207104,
            "R2": 0.7127274179827436,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.170327
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 9.626867556328977,
            "RMSE": 16.443718231711543,
            "R2": 0.7338058453397931,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.26591
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 9.854283538219804,
            "RMSE": 16.574189924013226,
            "R2": 0.7578382368534643,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.362543
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 10.034558550660114,
            "RMSE": 16.72149964752778,
            "R2": 0.7759339138910493,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.460131
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 10.942839439265006,
            "RMSE": 18.18973374364872,
            "R2": 0.7425340708967089,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.65219
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 11.480189522121243,
            "RMSE": 19.36955258798825,
            "R2": 0.7316181626186655,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 1.847066
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 11.884428250077962,
            "RMSE": 20.018801475409063,
            "R2": 0.7463650656532205,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 2.044712
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 12.037067702603975,
            "RMSE": 20.02507161492445,
            "R2": 0.7633646392298079,
            "Memory in Mb": 0.0423574447631835,
            "Time in s": 2.245044
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 12.938689395183468,
            "RMSE": 21.571547182252875,
            "R2": 0.7447563988620904,
            "Memory in Mb": 0.0393133163452148,
            "Time in s": 2.459951
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 13.737065020554605,
            "RMSE": 23.070023559587742,
            "R2": 0.7259561921053947,
            "Memory in Mb": 0.039839744567871,
            "Time in s": 2.675857
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 14.305628841534729,
            "RMSE": 24.020997573013894,
            "R2": 0.7359868139097058,
            "Memory in Mb": 0.0408926010131835,
            "Time in s": 2.892761
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 14.503019064271443,
            "RMSE": 24.118168317988548,
            "R2": 0.7526847575357923,
            "Memory in Mb": 0.0414190292358398,
            "Time in s": 3.110678
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 15.042001004765991,
            "RMSE": 24.757154413851225,
            "R2": 0.7504844548860922,
            "Memory in Mb": 0.0429983139038085,
            "Time in s": 3.329579
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 16.165694044127083,
            "RMSE": 26.934291479182736,
            "R2": 0.7226050873941003,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 3.549505
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 16.958578383564387,
            "RMSE": 28.26726815061745,
            "R2": 0.7302155620528221,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 3.77047
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 17.309589456804158,
            "RMSE": 28.5754148947933,
            "R2": 0.7394096166099926,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 4.010874
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 17.77955786237919,
            "RMSE": 29.119281838039548,
            "R2": 0.7454446166142166,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 4.254034
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 18.687135400012505,
            "RMSE": 30.600738447390604,
            "R2": 0.7270552375925041,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 4.499866
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 19.426270300418786,
            "RMSE": 31.61383923822668,
            "R2": 0.7250895764829616,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 4.748399
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 20.230319490239392,
            "RMSE": 32.829508990096734,
            "R2": 0.7334580691909136,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 5.00325
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 20.415951878027045,
            "RMSE": 32.83473210597698,
            "R2": 0.7443832332812113,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 5.259172
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 21.41946931942451,
            "RMSE": 34.477948502753435,
            "R2": 0.726844465494657,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 5.516121
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 22.135259536350134,
            "RMSE": 35.412182207518484,
            "R2": 0.7244424125617825,
            "Memory in Mb": 0.0435247421264648,
            "Time in s": 5.774111
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 22.998428764364284,
            "RMSE": 36.61317436816486,
            "R2": 0.7275265693889857,
            "Memory in Mb": 0.044051170349121,
            "Time in s": 6.033148000000001
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "ChickWeights",
            "MAE": 23.16185046142029,
            "RMSE": 36.73359474841229,
            "R2": 0.7324023432169282,
            "Memory in Mb": 0.044051170349121,
            "Time in s": 6.293050000000001
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 4.834704431652337,
            "RMSE": 13.708514217962266,
            "R2": -439.7934984576362,
            "Memory in Mb": 0.0500869750976562,
            "Time in s": 0.001817
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 3.4692310697037447,
            "RMSE": 9.813795721313518,
            "R2": -37.72035957928713,
            "Memory in Mb": 0.0732498168945312,
            "Time in s": 0.005553
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.530247618203559,
            "RMSE": 8.024836796214231,
            "R2": -33.90460110966681,
            "Memory in Mb": 0.0858840942382812,
            "Time in s": 0.011369
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.1398752670733447,
            "RMSE": 6.982837000856316,
            "R2": -25.510487239912003,
            "Memory in Mb": 0.09588623046875,
            "Time in s": 0.023421
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.2521629689485394,
            "RMSE": 6.362737158647257,
            "R2": -12.810573390910957,
            "Memory in Mb": 0.1053619384765625,
            "Time in s": 0.037893
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.275331183116589,
            "RMSE": 5.895687482983747,
            "R2": -9.059182991303912,
            "Memory in Mb": 0.1095733642578125,
            "Time in s": 0.054815
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.181766409647037,
            "RMSE": 5.493495699082884,
            "R2": -8.025069637302263,
            "Memory in Mb": 0.1116790771484375,
            "Time in s": 0.074219
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.0635226048812747,
            "RMSE": 5.165876255053421,
            "R2": -6.037983110569301,
            "Memory in Mb": 0.1158905029296875,
            "Time in s": 0.098519
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.9951428730766116,
            "RMSE": 4.906287161641783,
            "R2": -4.575559841528811,
            "Memory in Mb": 0.1179962158203125,
            "Time in s": 0.130188
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.8700446037321656,
            "RMSE": 4.662539866408188,
            "R2": -4.050299616280768,
            "Memory in Mb": 0.015085220336914,
            "Time in s": 0.169487
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.7830718267282506,
            "RMSE": 4.458344141345012,
            "R2": -3.981078161152351,
            "Memory in Mb": 0.0312490463256835,
            "Time in s": 0.210179
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.714887283408722,
            "RMSE": 4.280191261764102,
            "R2": -3.625492757292576,
            "Memory in Mb": 0.0370397567749023,
            "Time in s": 0.273546
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.626899515259654,
            "RMSE": 4.116599014627653,
            "R2": -3.336325373761703,
            "Memory in Mb": 0.044569969177246,
            "Time in s": 0.338443
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.6037708656255951,
            "RMSE": 3.992199218884993,
            "R2": -3.269831686495559,
            "Memory in Mb": 0.0575590133666992,
            "Time in s": 0.405125
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.5808413297038584,
            "RMSE": 3.882244388071726,
            "R2": -2.971019208275212,
            "Memory in Mb": 0.0675611495971679,
            "Time in s": 0.4768960000000001
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.5112246352788372,
            "RMSE": 3.7620340381312185,
            "R2": -2.9135432145577016,
            "Memory in Mb": 0.0754575729370117,
            "Time in s": 0.5560110000000001
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.464954049061847,
            "RMSE": 3.6574443601858126,
            "R2": -2.908900292165721,
            "Memory in Mb": 0.0807218551635742,
            "Time in s": 0.6372390000000001
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.4845626481571883,
            "RMSE": 3.5832345434246853,
            "R2": -2.782695640732784,
            "Memory in Mb": 0.0886182785034179,
            "Time in s": 0.7206760000000001
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.451940332797817,
            "RMSE": 3.496542725118452,
            "R2": -2.72647470962537,
            "Memory in Mb": 0.0938825607299804,
            "Time in s": 0.8063740000000001
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.4093274160891025,
            "RMSE": 3.4133346926199284,
            "R2": -2.65159153540002,
            "Memory in Mb": 0.1012525558471679,
            "Time in s": 0.8943350000000001
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3677964737960675,
            "RMSE": 3.3343173536823296,
            "R2": -2.5997996751089016,
            "Memory in Mb": 0.1054639816284179,
            "Time in s": 1.079576
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.335717224673182,
            "RMSE": 3.2621145597551164,
            "R2": -2.3832380441779537,
            "Memory in Mb": 0.1112546920776367,
            "Time in s": 1.2716070000000002
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3223220949397412,
            "RMSE": 3.20054856097613,
            "R2": -2.088360697350681,
            "Memory in Mb": 0.1196775436401367,
            "Time in s": 1.466366
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.2961820395725512,
            "RMSE": 3.1370925842333546,
            "R2": -1.8988499404168715,
            "Memory in Mb": 0.1275739669799804,
            "Time in s": 1.663894
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.2652762767168435,
            "RMSE": 3.076750388249757,
            "R2": -1.7299037995212605,
            "Memory in Mb": 0.1323118209838867,
            "Time in s": 1.864298
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.2471740635308572,
            "RMSE": 3.022290137612829,
            "R2": -1.6387160551274738,
            "Memory in Mb": 0.1375761032104492,
            "Time in s": 2.070902
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.222508472081129,
            "RMSE": 2.968388528244746,
            "R2": -1.5361060189709668,
            "Memory in Mb": 0.1396818161010742,
            "Time in s": 2.286544
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.2073384071706728,
            "RMSE": 2.920065266046622,
            "R2": -1.5126838513129577,
            "Memory in Mb": 0.1444196701049804,
            "Time in s": 2.5053300000000003
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1845779132924192,
            "RMSE": 2.8723790540044147,
            "R2": -1.4914188956527816,
            "Memory in Mb": 0.1470518112182617,
            "Time in s": 2.7271330000000003
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1745692976588702,
            "RMSE": 2.8296294830278077,
            "R2": -1.3910651808347,
            "Memory in Mb": 0.1414899826049804,
            "Time in s": 2.96944
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1708259630571385,
            "RMSE": 2.7920061348512903,
            "R2": -1.2924200227078335,
            "Memory in Mb": 0.1441221237182617,
            "Time in s": 3.214893
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1599967464968943,
            "RMSE": 2.7528504813508814,
            "R2": -1.186915838733254,
            "Memory in Mb": 0.1462278366088867,
            "Time in s": 3.481443
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1455993461288598,
            "RMSE": 2.715465758170179,
            "R2": -1.112620243595547,
            "Memory in Mb": 0.0933332443237304,
            "Time in s": 3.768351
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1331386715536065,
            "RMSE": 2.679518493749607,
            "R2": -1.0895638535289454,
            "Memory in Mb": 0.1028089523315429,
            "Time in s": 4.057625
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1287919059851137,
            "RMSE": 2.648832972736431,
            "R2": -1.0956110522943685,
            "Memory in Mb": 0.1107053756713867,
            "Time in s": 4.349483
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1090542602054634,
            "RMSE": 2.6130484736329,
            "R2": -1.0841769561048746,
            "Memory in Mb": 0.1170225143432617,
            "Time in s": 4.655905000000001
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0919225542546631,
            "RMSE": 2.579731998640208,
            "R2": -1.0301471378292058,
            "Memory in Mb": 0.1207075119018554,
            "Time in s": 4.969391000000001
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0729346607841277,
            "RMSE": 2.546521266569091,
            "R2": -0.9996439724530696,
            "Memory in Mb": 0.1238660812377929,
            "Time in s": 5.409378000000001
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0548522699101792,
            "RMSE": 2.514796200212546,
            "R2": -0.958866579835745,
            "Memory in Mb": 0.1301832199096679,
            "Time in s": 5.856313000000001
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0458975693179249,
            "RMSE": 2.486381451783576,
            "R2": -0.9321678603320388,
            "Memory in Mb": 0.1405134201049804,
            "Time in s": 6.306401000000001
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.042667475968943,
            "RMSE": 2.463395040447954,
            "R2": -0.9174360179218256,
            "Memory in Mb": 0.1468305587768554,
            "Time in s": 6.759550000000001
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0338402028724885,
            "RMSE": 2.4371652901742165,
            "R2": -0.8942452584110789,
            "Memory in Mb": 0.1505155563354492,
            "Time in s": 7.215791000000001
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0182769822752689,
            "RMSE": 2.409744604248102,
            "R2": -0.8486703239118398,
            "Memory in Mb": 0.1520948410034179,
            "Time in s": 7.680462000000001
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.007294910176456,
            "RMSE": 2.3841216724611445,
            "R2": -0.8005738256179296,
            "Memory in Mb": 0.1552534103393554,
            "Time in s": 8.149683000000001
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9984699415812968,
            "RMSE": 2.359722022526475,
            "R2": -0.7713409518355698,
            "Memory in Mb": 0.1573591232299804,
            "Time in s": 8.622145000000002
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9848390746890626,
            "RMSE": 2.334975438117308,
            "R2": -0.7628805257854674,
            "Memory in Mb": 0.1254529953002929,
            "Time in s": 9.108636
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9804934467335736,
            "RMSE": 2.3136297350671566,
            "R2": -0.7454793227879806,
            "Memory in Mb": 0.1344251632690429,
            "Time in s": 9.599086
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9715993160407668,
            "RMSE": 2.291923159938466,
            "R2": -0.7307898991199615,
            "Memory in Mb": 0.1402158737182617,
            "Time in s": 10.092417
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.96479276321034,
            "RMSE": 2.271398262551761,
            "R2": -0.7329444574748756,
            "Memory in Mb": 0.1444272994995117,
            "Time in s": 10.588738
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.956776427041678,
            "RMSE": 2.250974677037298,
            "R2": -0.7305695321170174,
            "Memory in Mb": 0.1486387252807617,
            "Time in s": 11.174487
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Hoeffding Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9561028857812052,
            "RMSE": 2.249867758958838,
            "R2": -0.7300222157865335,
            "Memory in Mb": 0.1486387252807617,
            "Time in s": 11.765558
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 8.051220648038832,
            "RMSE": 17.336198122120386,
            "R2": -385.8701660091343,
            "Memory in Mb": 0.0229225158691406,
            "Time in s": 0.002862
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.498502947359929,
            "RMSE": 12.28528637536428,
            "R2": -158.84524831763767,
            "Memory in Mb": 0.0245628356933593,
            "Time in s": 0.008031
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 3.4668695042339137,
            "RMSE": 10.074636808082968,
            "R2": -69.49212762837747,
            "Memory in Mb": 0.0298271179199218,
            "Time in s": 0.0152
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 2.7637805804889557,
            "RMSE": 8.735764655686483,
            "R2": -59.08259408516962,
            "Memory in Mb": 0.0309410095214843,
            "Time in s": 0.027573
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 2.814517498310432,
            "RMSE": 8.074396776941786,
            "R2": -11.726997097138026,
            "Memory in Mb": 0.0377845764160156,
            "Time in s": 0.040817
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 3.396900059747575,
            "RMSE": 7.862006773633152,
            "R2": -4.201378762014764,
            "Memory in Mb": 0.0472602844238281,
            "Time in s": 0.055065
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 3.8844336568547537,
            "RMSE": 7.782255505653143,
            "R2": -2.415785129732385,
            "Memory in Mb": 0.0536384582519531,
            "Time in s": 0.070503
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.068768385552718,
            "RMSE": 7.555909217267645,
            "R2": -1.9194502155140076,
            "Memory in Mb": 0.0594291687011718,
            "Time in s": 0.087235
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.319029347030655,
            "RMSE": 7.489629607912237,
            "R2": -1.3991215781815165,
            "Memory in Mb": 0.0604820251464843,
            "Time in s": 0.105314
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.231978704025333,
            "RMSE": 7.230698639905546,
            "R2": -0.5615110336669555,
            "Memory in Mb": 0.0620613098144531,
            "Time in s": 0.124657
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.279767976439616,
            "RMSE": 7.114292598648662,
            "R2": -0.1642036472993016,
            "Memory in Mb": 0.0620613098144531,
            "Time in s": 0.145348
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.161677712403324,
            "RMSE": 6.8979209349412445,
            "R2": 0.1054968774084013,
            "Memory in Mb": 0.0620613098144531,
            "Time in s": 0.183683
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.036201943040193,
            "RMSE": 6.686446116179646,
            "R2": 0.3192250351622916,
            "Memory in Mb": 0.0241641998291015,
            "Time in s": 0.233347
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.002163310161137,
            "RMSE": 6.555243218534794,
            "R2": 0.4439177197734564,
            "Memory in Mb": 0.034926414489746,
            "Time in s": 0.283952
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.269310553181931,
            "RMSE": 6.794169336453219,
            "R2": 0.5198027804498322,
            "Memory in Mb": 0.041365623474121,
            "Time in s": 0.335528
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.394431170074558,
            "RMSE": 6.916563516446891,
            "R2": 0.5987399306940604,
            "Memory in Mb": 0.0471563339233398,
            "Time in s": 0.38817
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.429782113532627,
            "RMSE": 6.896434310822903,
            "R2": 0.6733712331422652,
            "Memory in Mb": 0.052016258239746,
            "Time in s": 0.441959
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.448580123995543,
            "RMSE": 6.86078369215091,
            "R2": 0.7428621234581485,
            "Memory in Mb": 0.0546483993530273,
            "Time in s": 0.496925
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 4.634718338792146,
            "RMSE": 7.17917659207716,
            "R2": 0.7678921596594357,
            "Memory in Mb": 0.0546483993530273,
            "Time in s": 0.5531490000000001
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 5.229854791420841,
            "RMSE": 8.435313620968111,
            "R2": 0.7194573631198581,
            "Memory in Mb": 0.0552968978881835,
            "Time in s": 0.6106500000000001
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 5.400637324787383,
            "RMSE": 8.615072190659467,
            "R2": 0.7496975788166091,
            "Memory in Mb": 0.0552968978881835,
            "Time in s": 0.6850710000000001
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 5.622607300541604,
            "RMSE": 8.982158345389516,
            "R2": 0.781064800957145,
            "Memory in Mb": 0.0552968978881835,
            "Time in s": 0.7630730000000001
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 5.728895576419993,
            "RMSE": 9.10264619767678,
            "R2": 0.8047163053551843,
            "Memory in Mb": 0.0552968978881835,
            "Time in s": 0.8439190000000001
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 6.468790531655633,
            "RMSE": 10.532848432020362,
            "R2": 0.7611041743489119,
            "Memory in Mb": 0.0553770065307617,
            "Time in s": 0.926058
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 6.961259791220884,
            "RMSE": 11.725202267966395,
            "R2": 0.7394969764024641,
            "Memory in Mb": 0.0553770065307617,
            "Time in s": 1.009526
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 7.243017687832032,
            "RMSE": 12.175095097400796,
            "R2": 0.7567267064951951,
            "Memory in Mb": 0.0539121627807617,
            "Time in s": 1.109836
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 7.333189926829036,
            "RMSE": 12.221129948725446,
            "R2": 0.7874128689691341,
            "Memory in Mb": 0.0544385910034179,
            "Time in s": 1.300493
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 7.907494608974745,
            "RMSE": 13.13418786953933,
            "R2": 0.7813182108747583,
            "Memory in Mb": 0.0545606613159179,
            "Time in s": 1.494565
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 9.086203691627809,
            "RMSE": 16.084282058543664,
            "R2": 0.7023956098414756,
            "Memory in Mb": 0.0561399459838867,
            "Time in s": 1.6919570000000002
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 9.398286710797228,
            "RMSE": 16.38837159928856,
            "R2": 0.7355947540985646,
            "Memory in Mb": 0.0561399459838867,
            "Time in s": 1.900794
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 9.688169379844998,
            "RMSE": 16.65705092991554,
            "R2": 0.7554108572015372,
            "Memory in Mb": 0.0561399459838867,
            "Time in s": 2.110987
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 9.856066264187849,
            "RMSE": 16.815734957180027,
            "R2": 0.7734013139584004,
            "Memory in Mb": 0.0561399459838867,
            "Time in s": 2.322457
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 10.788654210226415,
            "RMSE": 18.368645129880047,
            "R2": 0.7374443731514406,
            "Memory in Mb": 0.0561399459838867,
            "Time in s": 2.535213
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 11.535989444086796,
            "RMSE": 20.177763325541772,
            "R2": 0.7087539856658172,
            "Memory in Mb": 0.0658864974975586,
            "Time in s": 2.749718
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 11.949331836981814,
            "RMSE": 20.800028245688587,
            "R2": 0.7261827687212361,
            "Memory in Mb": 0.0713338851928711,
            "Time in s": 2.965855
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 11.958714190964644,
            "RMSE": 20.66064387908481,
            "R2": 0.748105206776327,
            "Memory in Mb": 0.0781774520874023,
            "Time in s": 3.183657
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 12.807531574997112,
            "RMSE": 22.01468171576837,
            "R2": 0.7341619793955468,
            "Memory in Mb": 0.0825719833374023,
            "Time in s": 3.418965
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 13.71794187476778,
            "RMSE": 23.73901232910809,
            "R2": 0.7098322050491193,
            "Memory in Mb": 0.0846776962280273,
            "Time in s": 3.659139
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 14.269314924317156,
            "RMSE": 24.65274813293709,
            "R2": 0.7219171428567855,
            "Memory in Mb": 0.0656805038452148,
            "Time in s": 3.912261
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 14.511771919641935,
            "RMSE": 24.834167752766053,
            "R2": 0.7377826277560943,
            "Memory in Mb": 0.0706624984741211,
            "Time in s": 4.16702
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 15.00667707818897,
            "RMSE": 25.401748915029017,
            "R2": 0.7373221851710817,
            "Memory in Mb": 0.0787420272827148,
            "Time in s": 4.423509
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 16.106263610815663,
            "RMSE": 27.4394567629727,
            "R2": 0.7121021651653525,
            "Memory in Mb": 0.0857076644897461,
            "Time in s": 4.681795
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 16.950411373417108,
            "RMSE": 28.951900473786843,
            "R2": 0.7169889638801871,
            "Memory in Mb": 0.0888662338256836,
            "Time in s": 4.941903
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 17.321905164714362,
            "RMSE": 29.29627092175635,
            "R2": 0.7260962478080234,
            "Memory in Mb": 0.0889272689819336,
            "Time in s": 5.203768
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 17.829552469069228,
            "RMSE": 29.855361574147427,
            "R2": 0.732412614196017,
            "Memory in Mb": 0.0889272689819336,
            "Time in s": 5.467412
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 18.715769054600838,
            "RMSE": 31.21095148117224,
            "R2": 0.7160610523989874,
            "Memory in Mb": 0.0895147323608398,
            "Time in s": 5.743327000000001
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 19.54236471467993,
            "RMSE": 32.39367117342827,
            "R2": 0.7113596352744775,
            "Memory in Mb": 0.0743856430053711,
            "Time in s": 6.026441000000001
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 20.379374275832948,
            "RMSE": 33.670378810622296,
            "R2": 0.7196292071862618,
            "Memory in Mb": 0.0787191390991211,
            "Time in s": 6.311317000000001
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 20.522458105265056,
            "RMSE": 33.639909372937744,
            "R2": 0.7316929916628531,
            "Memory in Mb": 0.0872030258178711,
            "Time in s": 6.597982000000001
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 21.5114661084191,
            "RMSE": 35.24478084224406,
            "R2": 0.714558707096332,
            "Memory in Mb": 0.0935201644897461,
            "Time in s": 6.886526000000001
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 22.293418976341684,
            "RMSE": 36.29050935662323,
            "R2": 0.7106036021726428,
            "Memory in Mb": 0.0934362411499023,
            "Time in s": 7.177067000000001
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 23.158877831353536,
            "RMSE": 37.47206255417766,
            "R2": 0.7145930209145848,
            "Memory in Mb": 0.0946111679077148,
            "Time in s": 7.581349000000001
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ChickWeights",
            "MAE": 23.37390218951093,
            "RMSE": 37.6579284312523,
            "R2": 0.7187656938003131,
            "Memory in Mb": 0.0947332382202148,
            "Time in s": 7.990285000000001
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 4.828377634536296,
            "RMSE": 13.70786256219322,
            "R2": -439.7515918302183,
            "Memory in Mb": 0.0568618774414062,
            "Time in s": 0.005477
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 3.453811275213839,
            "RMSE": 9.811073218407971,
            "R2": -37.69887927291551,
            "Memory in Mb": 0.0800857543945312,
            "Time in s": 0.014203
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.5116544078850294,
            "RMSE": 8.021960641037959,
            "R2": -33.879585508404254,
            "Memory in Mb": 0.0927200317382812,
            "Time in s": 0.025216
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.1224425015381523,
            "RMSE": 6.9797990571526345,
            "R2": -25.487425023640156,
            "Memory in Mb": 0.102783203125,
            "Time in s": 0.038581
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.246653919301699,
            "RMSE": 6.363694444016854,
            "R2": -12.814729355257526,
            "Memory in Mb": 0.1122589111328125,
            "Time in s": 0.054574
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.270681160376927,
            "RMSE": 5.896666779393501,
            "R2": -9.06252500695684,
            "Memory in Mb": 0.1164703369140625,
            "Time in s": 0.096737
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 2.162967815650222,
            "RMSE": 5.491011289549727,
            "R2": -8.016908386196121,
            "Memory in Mb": 0.1185760498046875,
            "Time in s": 0.145193
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.9648637778298337,
            "RMSE": 5.147547754256808,
            "R2": -5.988130255135697,
            "Memory in Mb": 0.048110008239746,
            "Time in s": 0.201618
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.86652787828915,
            "RMSE": 4.875884330950751,
            "R2": -4.506673701927233,
            "Memory in Mb": 0.0645513534545898,
            "Time in s": 0.259848
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.773434994745299,
            "RMSE": 4.638841370319518,
            "R2": -3.999091327975425,
            "Memory in Mb": 0.0751142501831054,
            "Time in s": 0.334681
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.6594682627798778,
            "RMSE": 4.42936028038101,
            "R2": -3.916524330360767,
            "Memory in Mb": 0.0809926986694336,
            "Time in s": 0.415547
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.5811297097344512,
            "RMSE": 4.24689633509078,
            "R2": -3.553810703437006,
            "Memory in Mb": 0.0831594467163086,
            "Time in s": 0.499019
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.4918706813368772,
            "RMSE": 4.083314206963185,
            "R2": -3.2664860479391056,
            "Memory in Mb": 0.0869779586791992,
            "Time in s": 0.584777
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.4582505621214346,
            "RMSE": 3.950619643811522,
            "R2": -3.181352514384196,
            "Memory in Mb": 0.0965147018432617,
            "Time in s": 0.672987
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.4293807431017047,
            "RMSE": 3.836527362327468,
            "R2": -2.8780450161882043,
            "Memory in Mb": 0.1050596237182617,
            "Time in s": 0.763791
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3766835460490845,
            "RMSE": 3.718390713103106,
            "R2": -2.8232679475596494,
            "Memory in Mb": 0.1113767623901367,
            "Time in s": 0.862886
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3285707966483495,
            "RMSE": 3.611463128557805,
            "R2": -2.8112330604866624,
            "Memory in Mb": 0.0969266891479492,
            "Time in s": 1.077289
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3305028688272291,
            "RMSE": 3.538102571280229,
            "R2": -2.688007239623816,
            "Memory in Mb": 0.1048231124877929,
            "Time in s": 1.294249
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.3086678355415842,
            "RMSE": 3.4529556765760527,
            "R2": -2.6341471363086995,
            "Memory in Mb": 0.1101484298706054,
            "Time in s": 1.513868
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.256053624567095,
            "RMSE": 3.3666460142322228,
            "R2": -2.552379472359031,
            "Memory in Mb": 0.1175184249877929,
            "Time in s": 1.736306
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.2254239545780012,
            "RMSE": 3.2887455105144454,
            "R2": -2.5020714662192383,
            "Memory in Mb": 0.1217298507690429,
            "Time in s": 1.978865
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.204020924712129,
            "RMSE": 3.2198773978896,
            "R2": -2.2961943419959137,
            "Memory in Mb": 0.1275205612182617,
            "Time in s": 2.244474
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1975328241312166,
            "RMSE": 3.1601130927415366,
            "R2": -2.010817456858815,
            "Memory in Mb": 0.1354780197143554,
            "Time in s": 2.513147
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.186148143661266,
            "RMSE": 3.1001176815841758,
            "R2": -1.8309188655239268,
            "Memory in Mb": 0.1433744430541992,
            "Time in s": 2.784897
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1667856894749518,
            "RMSE": 3.042966728214852,
            "R2": -1.6702825792738007,
            "Memory in Mb": 0.1362333297729492,
            "Time in s": 3.07197
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.153194144927427,
            "RMSE": 2.98944402729251,
            "R2": -1.5816728306403074,
            "Memory in Mb": 0.1415586471557617,
            "Time in s": 3.362254
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1356058423088553,
            "RMSE": 2.937036564746637,
            "R2": -1.4828164968540292,
            "Memory in Mb": 0.1436643600463867,
            "Time in s": 3.655648
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.125648357086568,
            "RMSE": 2.890393580385493,
            "R2": -1.4618789770567937,
            "Memory in Mb": 0.1484022140502929,
            "Time in s": 3.952243
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.1072323197222282,
            "RMSE": 2.84377722554966,
            "R2": -1.4420491211959612,
            "Memory in Mb": 0.1510343551635742,
            "Time in s": 4.252035
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0962221602561253,
            "RMSE": 2.8010574809052518,
            "R2": -1.343021715112041,
            "Memory in Mb": 0.1547193527221679,
            "Time in s": 4.557891000000001
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.095549207215165,
            "RMSE": 2.765029222449673,
            "R2": -1.2483344123018605,
            "Memory in Mb": 0.1578779220581054,
            "Time in s": 4.883158000000001
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.085957414095071,
            "RMSE": 2.726589883354214,
            "R2": -1.1453910301968575,
            "Memory in Mb": 0.1599836349487304,
            "Time in s": 5.354946000000001
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0751762466913892,
            "RMSE": 2.6908702968299423,
            "R2": -1.074523242859362,
            "Memory in Mb": 0.1636686325073242,
            "Time in s": 5.834119000000001
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0667684392102676,
            "RMSE": 2.656475453821568,
            "R2": -1.0537791659469915,
            "Memory in Mb": 0.1663007736206054,
            "Time in s": 6.316591000000001
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.066718890752265,
            "RMSE": 2.6278494556992995,
            "R2": -1.0625405514881172,
            "Memory in Mb": 0.1547193527221679,
            "Time in s": 6.8062700000000005
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0487756272096451,
            "RMSE": 2.5923957614441,
            "R2": -1.0513617944147002,
            "Memory in Mb": 0.1594572067260742,
            "Time in s": 7.299083
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0336933816342644,
            "RMSE": 2.5596915816453274,
            "R2": -0.9987276211091368,
            "Memory in Mb": 0.1632032394409179,
            "Time in s": 7.795134000000001
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0143808347523189,
            "RMSE": 2.5263993770636084,
            "R2": -0.968167584311768,
            "Memory in Mb": 0.1647825241088867,
            "Time in s": 8.298925
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0004245938094416,
            "RMSE": 2.495691505058861,
            "R2": -0.9292169429583496,
            "Memory in Mb": 0.1695814132690429,
            "Time in s": 8.809149000000001
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9976736219043986,
            "RMSE": 2.469777786083391,
            "R2": -0.9064485942635294,
            "Memory in Mb": 0.1616849899291992,
            "Time in s": 9.32665
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 1.0020392091388557,
            "RMSE": 2.450590646975973,
            "R2": -0.8975546778436754,
            "Memory in Mb": 0.1643171310424804,
            "Time in s": 9.853038000000002
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9936292081382508,
            "RMSE": 2.424886643827349,
            "R2": -0.8752066007627983,
            "Memory in Mb": 0.1680021286010742,
            "Time in s": 10.484318000000002
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9794930742877992,
            "RMSE": 2.3980423354299125,
            "R2": -0.8307587924463844,
            "Memory in Mb": 0.1701078414916992,
            "Time in s": 11.125036
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9694853941742788,
            "RMSE": 2.372794343098121,
            "R2": -0.7835048635250907,
            "Memory in Mb": 0.1727399826049804,
            "Time in s": 11.769143
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9594920424525858,
            "RMSE": 2.348266033222206,
            "R2": -0.7541836724323567,
            "Memory in Mb": 0.1115369796752929,
            "Time in s": 12.432199
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9482726802907966,
            "RMSE": 2.324135545417226,
            "R2": -0.7465505219679065,
            "Memory in Mb": 0.1163969039916992,
            "Time in s": 13.10541
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9455376055826032,
            "RMSE": 2.30345366329758,
            "R2": -0.7301587545146957,
            "Memory in Mb": 0.1223096847534179,
            "Time in s": 13.781537
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9379298129457146,
            "RMSE": 2.282181144273129,
            "R2": -0.7161074287562055,
            "Memory in Mb": 0.1296796798706054,
            "Time in s": 14.460614
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.930996996530802,
            "RMSE": 2.261860474984104,
            "R2": -0.7184214614837348,
            "Memory in Mb": 0.1349439620971679,
            "Time in s": 15.148323
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9214575102921838,
            "RMSE": 2.2404008018877137,
            "R2": -0.714349138962711,
            "Memory in Mb": 0.1382246017456054,
            "Time in s": 15.950631
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "TrumpApproval",
            "MAE": 0.9213134079227226,
            "RMSE": 2.239416179559339,
            "R2": -0.7139861919037982,
            "Memory in Mb": 0.1382246017456054,
            "Time in s": 16.757639
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 41.63636363636363,
            "RMSE": 41.64569169030137,
            "R2": -2231.5319148936137,
            "Memory in Mb": 0.0096149444580078,
            "Time in s": 0.001328
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 41.31818181818181,
            "RMSE": 41.32960638133835,
            "R2": -1808.0547045951903,
            "Memory in Mb": 0.0126094818115234,
            "Time in s": 0.003944
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 41.12121212121212,
            "RMSE": 41.13871582091424,
            "R2": -1174.393494897962,
            "Memory in Mb": 0.015787124633789,
            "Time in s": 0.007623
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 41.159090909090914,
            "RMSE": 41.17451771534076,
            "R2": -1333.7620984139928,
            "Memory in Mb": 0.0188732147216796,
            "Time in s": 0.012489
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 41.5090909090909,
            "RMSE": 41.57075020645253,
            "R2": -336.3506066081568,
            "Memory in Mb": 0.0218257904052734,
            "Time in s": 0.019505
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 42.681818181818166,
            "RMSE": 42.82080349691271,
            "R2": -153.29834830483878,
            "Memory in Mb": 0.0246181488037109,
            "Time in s": 0.027128
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 43.50649350649351,
            "RMSE": 43.70978671356627,
            "R2": -106.75487995129542,
            "Memory in Mb": 0.0275020599365234,
            "Time in s": 0.035372
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 44.21590909090909,
            "RMSE": 44.43649707984724,
            "R2": -99.97346126163,
            "Memory in Mb": 0.0300197601318359,
            "Time in s": 0.047911
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 45.05050505050505,
            "RMSE": 45.309262771858165,
            "R2": -86.8022342468144,
            "Memory in Mb": 0.0329036712646484,
            "Time in s": 0.072727
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 46.16363636363636,
            "RMSE": 46.52487115902242,
            "R2": -63.64797006437341,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.103163
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 47.21487603305785,
            "RMSE": 47.67304278378361,
            "R2": -51.27707184490422,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.146595
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 48.29545454545455,
            "RMSE": 48.843054157105485,
            "R2": -43.84882422437649,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.196283
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 49.44055944055945,
            "RMSE": 50.100318941519305,
            "R2": -37.220279564063546,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.258522
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 50.532467532467535,
            "RMSE": 51.29137544271156,
            "R2": -33.04474826644667,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.329566
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 51.690909090909095,
            "RMSE": 52.61253451297311,
            "R2": -27.795548438273773,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.40393
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 53.00568181818182,
            "RMSE": 54.11860921749895,
            "R2": -23.566226925646237,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.481694
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 54.41176470588235,
            "RMSE": 55.733754017636336,
            "R2": -20.33250305682894,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.681251
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 56.02525252525252,
            "RMSE": 57.635786091488654,
            "R2": -17.146924852486976,
            "Memory in Mb": 0.2696781158447265,
            "Time in s": 0.884966
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 55.16354936929098,
            "RMSE": 57.0482200725598,
            "R2": -13.656313160472004,
            "Memory in Mb": 0.6838865280151367,
            "Time in s": 1.131695
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 53.62203856749311,
            "RMSE": 56.03531795068661,
            "R2": -11.37998411824978,
            "Memory in Mb": 0.6869077682495117,
            "Time in s": 1.3969520000000002
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.77279286370195,
            "RMSE": 55.29408706815337,
            "R2": -9.311090357596036,
            "Memory in Mb": 0.6899290084838867,
            "Time in s": 1.6754760000000002
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.49661908339594,
            "RMSE": 55.0071045368674,
            "R2": -7.210918602421254,
            "Memory in Mb": 0.6929502487182617,
            "Time in s": 1.960024
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.25631812193077,
            "RMSE": 54.71344660515688,
            "R2": -6.055353919833875,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 2.270278
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 51.62511478420569,
            "RMSE": 54.312843786153664,
            "R2": -5.352168023774992,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 2.586688
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 51.4425344352617,
            "RMSE": 54.29364548356293,
            "R2": -4.585603291722447,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 2.915419
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 51.75651621106165,
            "RMSE": 54.635705044608144,
            "R2": -3.8989478253777694,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 3.266148
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.373839404142416,
            "RMSE": 55.25476711535166,
            "R2": -3.3456400671942,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 3.622985
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.87239275875638,
            "RMSE": 55.86677247417265,
            "R2": -2.9565197175813718,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 3.98691
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 52.69554478958866,
            "RMSE": 56.2770501442128,
            "R2": -2.6433309475704183,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 4.356941
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 53.85316804407712,
            "RMSE": 57.75044402630399,
            "R2": -2.2832890424968197,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 4.733992
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 54.90678041411178,
            "RMSE": 59.01114057562677,
            "R2": -2.0697921090482247,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 5.128946
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 56.00533746556472,
            "RMSE": 60.30224520856101,
            "R2": -1.9140207825503284,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 5.54848
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 55.99599298772852,
            "RMSE": 60.54917173074773,
            "R2": -1.852879941931207,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 6.172488
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 56.87222492302705,
            "RMSE": 61.81275171085535,
            "R2": -1.7331917323651345,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 6.808446
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 58.41786698150333,
            "RMSE": 63.95254893573906,
            "R2": -1.588502821427925,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 7.450193
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 59.7033976124885,
            "RMSE": 65.46926983257002,
            "R2": -1.5293357430909813,
            "Memory in Mb": 0.6947126388549805,
            "Time in s": 8.100657
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 60.057805647389294,
            "RMSE": 66.17359973042984,
            "R2": -1.4019380007417157,
            "Memory in Mb": 1.1097631454467771,
            "Time in s": 8.796904
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 59.7070864579051,
            "RMSE": 66.11592086962122,
            "R2": -1.2507954049688483,
            "Memory in Mb": 1.1127843856811523,
            "Time in s": 9.50192
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 60.122823673891816,
            "RMSE": 66.73609937588846,
            "R2": -1.0378169857688957,
            "Memory in Mb": 1.1158056259155271,
            "Time in s": 10.222461
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 60.39504675635191,
            "RMSE": 66.96100690444877,
            "R2": -0.906365593827489,
            "Memory in Mb": 1.1188268661499023,
            "Time in s": 10.951743
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 60.27126048587789,
            "RMSE": 66.93502892662679,
            "R2": -0.8239085862185902,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 11.696828
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 60.340686610373176,
            "RMSE": 67.43825007380137,
            "R2": -0.7390015352251049,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 12.465469
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 61.40703262301831,
            "RMSE": 69.11306667757516,
            "R2": -0.6127592621572406,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 13.248766
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 61.95796621360106,
            "RMSE": 69.71422620021941,
            "R2": -0.5510154280248158,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 14.047315
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 62.59018166487368,
            "RMSE": 70.55352405729404,
            "R2": -0.4943708535906215,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 14.854826
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 62.49664579133251,
            "RMSE": 70.88193125644693,
            "R2": -0.4644752452013045,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 15.674675
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 63.25224079915844,
            "RMSE": 71.92080214464903,
            "R2": -0.4228062717918979,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 16.51129
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 64.80783657170488,
            "RMSE": 74.3681944005728,
            "R2": -0.367764222300833,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 17.364023
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 65.59959781369417,
            "RMSE": 75.30113885843834,
            "R2": -0.3443906138479853,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 18.342072
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 65.79684627343133,
            "RMSE": 76.01328745307667,
            "R2": -0.3277190973108916,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 19.334776
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 66.6512855136148,
            "RMSE": 77.20436469287773,
            "R2": -0.3097569166669509,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 20.336346
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 68.11975592628174,
            "RMSE": 79.56492566870935,
            "R2": -0.2867456678376987,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 21.353617
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "ChickWeights",
            "MAE": 68.75877313437184,
            "RMSE": 80.35800679505147,
            "R2": -0.2806007657015741,
            "Memory in Mb": 1.120589256286621,
            "Time in s": 22.38029
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 43.8732195,
            "RMSE": 43.87807788634269,
            "R2": -4514.954899312423,
            "Memory in Mb": 0.0199413299560546,
            "Time in s": 0.002168
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 42.4932955,
            "RMSE": 42.52255283421693,
            "R2": -725.9491167623446,
            "Memory in Mb": 0.0317363739013671,
            "Time in s": 0.006794
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 42.2167785,
            "RMSE": 42.2386240157387,
            "R2": -966.0073736019044,
            "Memory in Mb": 0.0438976287841796,
            "Time in s": 0.018434
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 41.975705625,
            "RMSE": 41.99760868559829,
            "R2": -957.9655948743646,
            "Memory in Mb": 0.0562419891357421,
            "Time in s": 0.031286
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 41.37550450000001,
            "RMSE": 41.410913785433536,
            "R2": -583.9966399141301,
            "Memory in Mb": 0.5381031036376953,
            "Time in s": 0.048039
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 40.936110000000006,
            "RMSE": 40.97829382197767,
            "R2": -484.9611418859003,
            "Memory in Mb": 0.5386066436767578,
            "Time in s": 0.080711
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 40.6885472857143,
            "RMSE": 40.72961738075088,
            "R2": -495.1050461477588,
            "Memory in Mb": 0.5391101837158203,
            "Time in s": 0.166791
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 40.35105437500001,
            "RMSE": 40.39801158334292,
            "R2": -429.4078677932073,
            "Memory in Mb": 0.5393619537353516,
            "Time in s": 0.262676
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 40.00981655555555,
            "RMSE": 40.06373388340122,
            "R2": -370.7794659133543,
            "Memory in Mb": 0.5396137237548828,
            "Time in s": 0.43318
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 39.80633095,
            "RMSE": 39.860362966711,
            "R2": -368.1089073295326,
            "Memory in Mb": 0.5077581405639648,
            "Time in s": 0.638958
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 36.497516001377406,
            "RMSE": 38.01945344470104,
            "R2": -361.2329206514933,
            "Memory in Mb": 1.3602590560913086,
            "Time in s": 0.913553
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 33.64243104419191,
            "RMSE": 36.40668421494773,
            "R2": -333.65237138497804,
            "Memory in Mb": 1.360762596130371,
            "Time in s": 1.221179
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 31.222114965034955,
            "RMSE": 34.98371838354962,
            "R2": -312.16748668977897,
            "Memory in Mb": 1.3610143661499023,
            "Time in s": 1.570709
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 29.18205946861472,
            "RMSE": 33.71869814960704,
            "R2": -303.5986275675674,
            "Memory in Mb": 1.361769676208496,
            "Time in s": 1.939253
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 27.34275770505051,
            "RMSE": 32.57805191350732,
            "R2": -278.63174197976707,
            "Memory in Mb": 1.3620214462280271,
            "Time in s": 2.324555
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 25.81388747443183,
            "RMSE": 31.5521424826706,
            "R2": -274.2849072221064,
            "Memory in Mb": 1.3630285263061523,
            "Time in s": 2.877117
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 24.51835124153299,
            "RMSE": 30.62414457186519,
            "R2": -273.0482727941538,
            "Memory in Mb": 1.3640356063842771,
            "Time in s": 3.447
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 23.451930423400693,
            "RMSE": 29.78792492645533,
            "R2": -260.4155562259403,
            "Memory in Mb": 1.3660497665405271,
            "Time in s": 4.029196
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 22.46844053349284,
            "RMSE": 29.014219480552867,
            "R2": -255.5915105297988,
            "Memory in Mb": 1.3665533065795898,
            "Time in s": 4.629964999999999
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 21.59490700757577,
            "RMSE": 28.301677882839343,
            "R2": -250.0434007116766,
            "Memory in Mb": 0.510127067565918,
            "Time in s": 5.253793
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 20.62268781294523,
            "RMSE": 27.62086591367872,
            "R2": -246.0239415518119,
            "Memory in Mb": 1.3623762130737305,
            "Time in s": 5.968102
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 19.786863931462925,
            "RMSE": 26.990398924900397,
            "R2": -230.60756767519212,
            "Memory in Mb": 1.3643903732299805,
            "Time in s": 6.700306
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 19.05732899619648,
            "RMSE": 26.404670160589287,
            "R2": -209.2038511633616,
            "Memory in Mb": 1.3666563034057615,
            "Time in s": 7.451319000000001
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 18.376512097202227,
            "RMSE": 25.854792215140314,
            "R2": -195.90337768575387,
            "Memory in Mb": 1.3701810836791992,
            "Time in s": 8.221931000000001
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 17.755044410127518,
            "RMSE": 25.338820973360427,
            "R2": -184.1550753065148,
            "Memory in Mb": 1.3716917037963867,
            "Time in s": 9.124580000000002
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 17.16611419898163,
            "RMSE": 24.851444862058347,
            "R2": -177.4118263333629,
            "Memory in Mb": 1.3737058639526367,
            "Time in s": 10.044684000000002
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 16.628565596068775,
            "RMSE": 24.392285078947275,
            "R2": -170.25012213753183,
            "Memory in Mb": 1.3747129440307615,
            "Time in s": 10.981068000000002
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 16.091244232649693,
            "RMSE": 23.955027361350904,
            "R2": -168.10096043791202,
            "Memory in Mb": 1.3752164840698242,
            "Time in s": 11.990243000000005
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 15.590768135673304,
            "RMSE": 23.54051091957351,
            "R2": -166.33817208986073,
            "Memory in Mb": 1.3764753341674805,
            "Time in s": 13.016881000000003
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 15.168708628495342,
            "RMSE": 23.15108754841241,
            "R2": -159.05714501634571,
            "Memory in Mb": 0.5124959945678711,
            "Time in s": 14.090212000000005
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 14.742446374247312,
            "RMSE": 22.77953961802373,
            "R2": -151.59887848495535,
            "Memory in Mb": 3.064208030700684,
            "Time in s": 15.285325000000004
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 14.319364852585176,
            "RMSE": 22.42187566882095,
            "R2": -144.08105420081068,
            "Memory in Mb": 3.0679845809936523,
            "Time in s": 16.529242000000004
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 13.916412195872256,
            "RMSE": 22.080274918425697,
            "R2": -138.68241285181185,
            "Memory in Mb": 3.0712575912475586,
            "Time in s": 17.842975000000003
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 13.515604789075644,
            "RMSE": 21.753254558457893,
            "R2": -136.71797028279042,
            "Memory in Mb": 3.074782371520996,
            "Time in s": 19.280557
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 13.16391092204058,
            "RMSE": 21.44141764506316,
            "R2": -136.3120101768532,
            "Memory in Mb": 3.0773000717163086,
            "Time in s": 20.753146
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 12.828283113852926,
            "RMSE": 21.142484202016185,
            "R2": -135.44313416922282,
            "Memory in Mb": 3.078558921813965,
            "Time in s": 22.284495
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 12.50446646701278,
            "RMSE": 20.855361315179096,
            "R2": -131.6825380828392,
            "Memory in Mb": 3.0800695419311523,
            "Time in s": 23.930702
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 12.187542748969031,
            "RMSE": 20.57929219886472,
            "R2": -129.592708960364,
            "Memory in Mb": 3.0813283920288086,
            "Time in s": 25.608717
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 11.899403743710543,
            "RMSE": 20.31464229706916,
            "R2": -126.82553676745258,
            "Memory in Mb": 3.08359432220459,
            "Time in s": 27.347366
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 11.634366305883283,
            "RMSE": 20.06137952581079,
            "R2": -124.7856004590591,
            "Memory in Mb": 3.084601402282715,
            "Time in s": 29.130085
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 11.363415331478278,
            "RMSE": 19.815492221289517,
            "R2": -123.0687724200615,
            "Memory in Mb": 3.08560848236084,
            "Time in s": 30.98707
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 11.106640469158773,
            "RMSE": 19.57848368678801,
            "R2": -121.2430978899656,
            "Memory in Mb": 3.086615562438965,
            "Time in s": 32.880055
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 10.873909665943762,
            "RMSE": 19.35022618912736,
            "R2": -118.20364312373844,
            "Memory in Mb": 3.087119102478028,
            "Time in s": 34.808534
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 10.65545006969969,
            "RMSE": 19.130035299019603,
            "R2": -114.92727947355436,
            "Memory in Mb": 3.0873708724975586,
            "Time in s": 36.791638
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 10.439309697188907,
            "RMSE": 18.916827199314994,
            "R2": -112.83532852765144,
            "Memory in Mb": 3.08762264251709,
            "Time in s": 38.832751
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 10.21789524284777,
            "RMSE": 18.710158789526105,
            "R2": -112.19133803320568,
            "Memory in Mb": 3.087874412536621,
            "Time in s": 40.951802
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 10.012578535125469,
            "RMSE": 18.510293787577226,
            "R2": -110.72583714230213,
            "Memory in Mb": 3.077906608581543,
            "Time in s": 43.146806
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 9.811853150109153,
            "RMSE": 18.316579311485903,
            "R2": -109.54344305213982,
            "Memory in Mb": 3.0804243087768555,
            "Time in s": 45.38444
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 9.61909067795052,
            "RMSE": 18.12881604876013,
            "R2": -109.39183420714345,
            "Memory in Mb": 3.080927848815918,
            "Time in s": 47.662491
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 9.438738635632271,
            "RMSE": 17.946847607318464,
            "R2": -109.00797869183796,
            "Memory in Mb": 3.082438468933105,
            "Time in s": 50.039238
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Stochastic Gradient Tree",
            "dataset": "TrumpApproval",
            "MAE": 9.429746533156267,
            "RMSE": 17.937886241411594,
            "R2": -108.97151968967049,
            "Memory in Mb": 3.082438468933105,
            "Time in s": 52.450717
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 7.837563210503649,
            "RMSE": 16.830121687224917,
            "R2": -363.61289911513376,
            "Memory in Mb": 0.1506052017211914,
            "Time in s": 0.01357
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 4.3557641651310055,
            "RMSE": 11.925612892987612,
            "R2": -149.62275175212707,
            "Memory in Mb": 0.1761331558227539,
            "Time in s": 0.033876
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 3.3711466349197527,
            "RMSE": 9.780434627556833,
            "R2": -65.4351822307151,
            "Memory in Mb": 0.214268684387207,
            "Time in s": 0.065705
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 2.6922077728217837,
            "RMSE": 8.482083592242564,
            "R2": -55.643739991610765,
            "Memory in Mb": 0.2312593460083007,
            "Time in s": 0.110591
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 2.74736475641488,
            "RMSE": 7.825318026963682,
            "R2": -10.953904022002217,
            "Memory in Mb": 0.2869501113891601,
            "Time in s": 0.166016
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 2.8724679940162905,
            "RMSE": 7.312536888278379,
            "R2": -3.4997438549991955,
            "Memory in Mb": 0.3332719802856445,
            "Time in s": 0.243978
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 3.0470429271529937,
            "RMSE": 7.064245743713448,
            "R2": -1.8145642692685129,
            "Memory in Mb": 0.3119173049926758,
            "Time in s": 0.346862
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 2.9741223361578246,
            "RMSE": 6.690154558226259,
            "R2": -1.288758200280824,
            "Memory in Mb": 0.3463144302368164,
            "Time in s": 0.647937
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 3.5306191185317584,
            "RMSE": 6.892431773474538,
            "R2": -1.031779280787943,
            "Memory in Mb": 0.3914194107055664,
            "Time in s": 0.960086
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 3.8799314967396743,
            "RMSE": 6.981555605673833,
            "R2": -0.4557571678865852,
            "Memory in Mb": 0.4218912124633789,
            "Time in s": 1.292146
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 4.113667008668635,
            "RMSE": 7.033914104811044,
            "R2": -0.1380455127293207,
            "Memory in Mb": 0.4422159194946289,
            "Time in s": 1.662194
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 4.34164975929163,
            "RMSE": 7.058470289925444,
            "R2": 0.0633731167085442,
            "Memory in Mb": 0.4695367813110351,
            "Time in s": 2.044753
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 4.57586761829926,
            "RMSE": 7.15786747745719,
            "R2": 0.2198462773680444,
            "Memory in Mb": 0.5039682388305664,
            "Time in s": 2.459644
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 4.72768375743327,
            "RMSE": 7.245199860946492,
            "R2": 0.3206991207112422,
            "Memory in Mb": 0.5465364456176758,
            "Time in s": 2.897301
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 5.104360720447454,
            "RMSE": 7.731417459148682,
            "R2": 0.3781793296599212,
            "Memory in Mb": 0.5543031692504883,
            "Time in s": 3.478625
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 5.614563299993537,
            "RMSE": 8.384781892618234,
            "R2": 0.4103032354466553,
            "Memory in Mb": 0.577855110168457,
            "Time in s": 4.083596
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 6.030281219875818,
            "RMSE": 8.796345271037008,
            "R2": 0.4686144271207236,
            "Memory in Mb": 0.5973634719848633,
            "Time in s": 4.712472
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 6.128233569544692,
            "RMSE": 8.84845009665535,
            "R2": 0.572286448100142,
            "Memory in Mb": 0.6156282424926758,
            "Time in s": 5.362321
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 6.65587905711115,
            "RMSE": 9.6527323574251,
            "R2": 0.5803946009681837,
            "Memory in Mb": 0.637272834777832,
            "Time in s": 6.068711
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 7.106977341119842,
            "RMSE": 10.677274056234571,
            "R2": 0.550512947323095,
            "Memory in Mb": 0.6516351699829102,
            "Time in s": 6.792503
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 7.51605472684967,
            "RMSE": 11.121858780588036,
            "R2": 0.582840670024279,
            "Memory in Mb": 0.6455926895141602,
            "Time in s": 7.540065
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 7.8763674823035235,
            "RMSE": 11.54794620868086,
            "R2": 0.6381207504866175,
            "Memory in Mb": 0.654301643371582,
            "Time in s": 8.314509000000001
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 8.048654689630025,
            "RMSE": 11.785882981718466,
            "R2": 0.6726179175042853,
            "Memory in Mb": 0.6542215347290039,
            "Time in s": 9.228486
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 8.558470564817128,
            "RMSE": 12.694815113306078,
            "R2": 0.6529678969258632,
            "Memory in Mb": 0.7006998062133789,
            "Time in s": 10.165772
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 9.011287699636805,
            "RMSE": 13.865710758190522,
            "R2": 0.6357023625954032,
            "Memory in Mb": 0.7181978225708008,
            "Time in s": 11.12726
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 9.454493871269731,
            "RMSE": 14.39909947248495,
            "R2": 0.6597325750664246,
            "Memory in Mb": 0.7397470474243164,
            "Time in s": 12.112744
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 9.455634964453314,
            "RMSE": 14.370566123736594,
            "R2": 0.7060577585099084,
            "Memory in Mb": 0.6961946487426758,
            "Time in s": 13.208544
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 9.98259297559382,
            "RMSE": 15.278989711680778,
            "R2": 0.7040656028742478,
            "Memory in Mb": 0.7122316360473633,
            "Time in s": 14.327932
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 10.896304985778038,
            "RMSE": 17.680267148091307,
            "R2": 0.6404050215106214,
            "Memory in Mb": 0.7230386734008789,
            "Time in s": 15.472301
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 11.34830207391465,
            "RMSE": 18.238325787402868,
            "R2": 0.6725323523293205,
            "Memory in Mb": 0.7481813430786133,
            "Time in s": 16.699404
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 11.700671911575691,
            "RMSE": 18.698639858183288,
            "R2": 0.6917798823884449,
            "Memory in Mb": 0.750828742980957,
            "Time in s": 17.953966
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 12.012928806619971,
            "RMSE": 19.028065448277463,
            "R2": 0.7098550919958697,
            "Memory in Mb": 0.779423713684082,
            "Time in s": 19.24314
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 12.590729727774807,
            "RMSE": 20.061815233276363,
            "R2": 0.6868102538385266,
            "Memory in Mb": 0.8219194412231445,
            "Time in s": 20.584825
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 13.29572445199132,
            "RMSE": 21.688967498502105,
            "R2": 0.6634948622954009,
            "Memory in Mb": 0.8368387222290039,
            "Time in s": 21.949532
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 13.850252347511734,
            "RMSE": 22.377982941031117,
            "R2": 0.6830616430184708,
            "Memory in Mb": 0.8398981094360352,
            "Time in s": 23.337733
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 13.995508749414425,
            "RMSE": 22.434927630401365,
            "R2": 0.7029833246789492,
            "Memory in Mb": 0.8451242446899414,
            "Time in s": 24.808931
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 14.855647843034443,
            "RMSE": 23.972462409994428,
            "R2": 0.6847772413527866,
            "Memory in Mb": 0.8440675735473633,
            "Time in s": 26.305221
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 15.648428200057216,
            "RMSE": 25.832735423225586,
            "R2": 0.6563908585574095,
            "Memory in Mb": 0.8621377944946289,
            "Time in s": 27.821712
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 16.477960681723363,
            "RMSE": 27.01651731063008,
            "R2": 0.6660339910533338,
            "Memory in Mb": 0.8826723098754883,
            "Time in s": 29.421277
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 16.794784005292485,
            "RMSE": 27.277386650758192,
            "R2": 0.6836500576952018,
            "Memory in Mb": 0.8854074478149414,
            "Time in s": 31.044846
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 17.2443539228967,
            "RMSE": 27.815314781786785,
            "R2": 0.6850336806962379,
            "Memory in Mb": 0.915654182434082,
            "Time in s": 32.692345
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 18.21783864235053,
            "RMSE": 29.965283642676138,
            "R2": 0.6566601868655235,
            "Memory in Mb": 0.947678565979004,
            "Time in s": 34.453267999999994
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 19.154558799374207,
            "RMSE": 31.27949805899601,
            "R2": 0.6696542166515442,
            "Memory in Mb": 0.9631280899047852,
            "Time in s": 36.23863899999999
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 19.65302219917293,
            "RMSE": 31.71092492917292,
            "R2": 0.6790841892096586,
            "Memory in Mb": 0.979741096496582,
            "Time in s": 38.04845199999999
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 20.17748759588543,
            "RMSE": 32.35841629000369,
            "R2": 0.6856630158751376,
            "Memory in Mb": 1.0035409927368164,
            "Time in s": 39.89288999999999
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 20.994447812000203,
            "RMSE": 33.88452895368057,
            "R2": 0.6653322556738073,
            "Memory in Mb": 1.0402307510375977,
            "Time in s": 41.77183299999999
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 21.74940325928189,
            "RMSE": 34.92971521251369,
            "R2": 0.6643962418834424,
            "Memory in Mb": 1.0591440200805664,
            "Time in s": 43.68222899999999
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 22.71806819464153,
            "RMSE": 36.27208023143736,
            "R2": 0.6746268651566016,
            "Memory in Mb": 1.0802621841430664,
            "Time in s": 45.622796999999984
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 22.976084812890598,
            "RMSE": 36.32299861842887,
            "R2": 0.6871862958215178,
            "Memory in Mb": 1.1105661392211914,
            "Time in s": 47.62064799999998
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 23.812560792713985,
            "RMSE": 37.68037385984369,
            "R2": 0.6737446986071818,
            "Memory in Mb": 1.1564149856567385,
            "Time in s": 49.63871399999998
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 24.744158926088524,
            "RMSE": 38.95638961509032,
            "R2": 0.6665241448790927,
            "Memory in Mb": 1.171940803527832,
            "Time in s": 51.68634399999998
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 25.965548256363952,
            "RMSE": 40.779089345824126,
            "R2": 0.6619939776632806,
            "Memory in Mb": 1.1861085891723633,
            "Time in s": 53.83172099999997
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "ChickWeights",
            "MAE": 26.10164191353107,
            "RMSE": 40.80941552099692,
            "R2": 0.669724624616493,
            "Memory in Mb": 1.1904268264770508,
            "Time in s": 56.00600499999997
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 4.656196028844478,
            "RMSE": 13.301506400077992,
            "R2": -414.0076115498352,
            "Memory in Mb": 0.2015810012817382,
            "Time in s": 0.057323
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 3.307191630717303,
            "RMSE": 9.5148436405931,
            "R2": -35.39725790498291,
            "Memory in Mb": 0.2895097732543945,
            "Time in s": 0.159522
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 2.3916587233350866,
            "RMSE": 7.783560456255013,
            "R2": -31.83725667748105,
            "Memory in Mb": 0.3228082656860351,
            "Time in s": 0.43784
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 2.0172424359013847,
            "RMSE": 6.770328731809264,
            "R2": -23.92145608895444,
            "Memory in Mb": 0.3692712783813476,
            "Time in s": 0.749169
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 2.069330341220504,
            "RMSE": 6.141775226189047,
            "R2": -11.868015650386663,
            "Memory in Mb": 0.4076700210571289,
            "Time in s": 1.082433
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 2.013474643057227,
            "RMSE": 5.653544639730099,
            "R2": -8.249866206703038,
            "Memory in Mb": 0.4241609573364258,
            "Time in s": 1.485703
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.894365920134237,
            "RMSE": 5.255534318342925,
            "R2": -7.260127227254786,
            "Memory in Mb": 0.4439592361450195,
            "Time in s": 2.052392
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.942363436061872,
            "RMSE": 4.987168106592344,
            "R2": -5.559462264629689,
            "Memory in Mb": 0.4557695388793945,
            "Time in s": 2.6505280000000004
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.9639788846395132,
            "RMSE": 4.758402061618727,
            "R2": -4.244508869717663,
            "Memory in Mb": 0.4725847244262695,
            "Time in s": 3.3297560000000006
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.9045329443413328,
            "RMSE": 4.539431452034987,
            "R2": -3.787127034775958,
            "Memory in Mb": 0.5018167495727539,
            "Time in s": 4.037089000000001
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.7801675790175082,
            "RMSE": 4.332908187325825,
            "R2": -3.704734847036908,
            "Memory in Mb": 0.539036750793457,
            "Time in s": 4.871381000000001
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.7262455165213564,
            "RMSE": 4.162317120423255,
            "R2": -3.374233717467068,
            "Memory in Mb": 0.5583086013793945,
            "Time in s": 5.726343000000002
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.6726006855046047,
            "RMSE": 4.010034080286883,
            "R2": -3.11472540009772,
            "Memory in Mb": 0.586766242980957,
            "Time in s": 6.608691000000002
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.6001254820213158,
            "RMSE": 3.86938412403892,
            "R2": -3.01116046378164,
            "Memory in Mb": 0.6034517288208008,
            "Time in s": 7.537396000000002
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.5903246290151525,
            "RMSE": 3.758572865099384,
            "R2": -2.72204992570884,
            "Memory in Mb": 0.6344270706176758,
            "Time in s": 8.563678000000001
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.5306703522535514,
            "RMSE": 3.644833568467773,
            "R2": -2.673500446315358,
            "Memory in Mb": 0.6524057388305664,
            "Time in s": 9.653495
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.462120415173825,
            "RMSE": 3.538151879462345,
            "R2": -2.658070572544154,
            "Memory in Mb": 0.6771516799926758,
            "Time in s": 10.778313
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.4104873891633294,
            "RMSE": 3.442715407420023,
            "R2": -2.491830651593505,
            "Memory in Mb": 0.712040901184082,
            "Time in s": 12.006044
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.3577274631021343,
            "RMSE": 3.353553439657788,
            "R2": -2.42792224294701,
            "Memory in Mb": 0.7612085342407227,
            "Time in s": 13.264975000000002
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.328889471148693,
            "RMSE": 3.2750276755937477,
            "R2": -2.361664675892684,
            "Memory in Mb": 0.7830896377563477,
            "Time in s": 14.608014
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.2856838141339133,
            "RMSE": 3.198005596242657,
            "R2": -2.3114858734875385,
            "Memory in Mb": 0.8153314590454102,
            "Time in s": 15.987435
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.2502461578606217,
            "RMSE": 3.1277634460074983,
            "R2": -2.1102975482726696,
            "Memory in Mb": 0.8549776077270508,
            "Time in s": 17.476653000000002
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.2118787702501406,
            "RMSE": 3.0607885313580625,
            "R2": -1.824527619127544,
            "Memory in Mb": 0.8641138076782227,
            "Time in s": 19.005275
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.1755519926992437,
            "RMSE": 2.997482691409013,
            "R2": -1.6465763687209671,
            "Memory in Mb": 0.904881477355957,
            "Time in s": 20.582478
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.1542746800420942,
            "RMSE": 2.9412002898427465,
            "R2": -1.494663742459657,
            "Memory in Mb": 0.9429025650024414,
            "Time in s": 22.213321
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.1232655769227813,
            "RMSE": 2.885625631130148,
            "R2": -1.4054721071787497,
            "Memory in Mb": 0.9187402725219728,
            "Time in s": 23.93785
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.0927628011224122,
            "RMSE": 2.8324064719208977,
            "R2": -1.3090698562992058,
            "Memory in Mb": 0.9784936904907228,
            "Time in s": 25.72016
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.0798076211233285,
            "RMSE": 2.7860066009246958,
            "R2": -1.2872677886963872,
            "Memory in Mb": 0.8415918350219727,
            "Time in s": 27.559893
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.0533259806656756,
            "RMSE": 2.7386650773118006,
            "R2": -1.2648586320750757,
            "Memory in Mb": 0.926945686340332,
            "Time in s": 29.430927
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.0370277841126194,
            "RMSE": 2.695306817676886,
            "R2": -1.1694452334238137,
            "Memory in Mb": 1.0152063369750977,
            "Time in s": 31.394822
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.0220360797787769,
            "RMSE": 2.6548714349996483,
            "R2": -1.0727572654712625,
            "Memory in Mb": 0.9687509536743164,
            "Time in s": 33.420245
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 1.006223169156282,
            "RMSE": 2.615089153799328,
            "R2": -0.9735122270872276,
            "Memory in Mb": 0.8030519485473633,
            "Time in s": 35.538976
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.9862189251721106,
            "RMSE": 2.576116595691222,
            "R2": -0.901357605879683,
            "Memory in Mb": 0.7759256362915039,
            "Time in s": 37.763356
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.9658028732124052,
            "RMSE": 2.5385905860617046,
            "R2": -0.8755448750460146,
            "Memory in Mb": 0.8428354263305664,
            "Time in s": 40.028227
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.958070286753166,
            "RMSE": 2.506070409170758,
            "R2": -0.8758066430098239,
            "Memory in Mb": 0.9465646743774414,
            "Time in s": 42.353807
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.9436099236768006,
            "RMSE": 2.472715624364642,
            "R2": -0.8663281360281503,
            "Memory in Mb": 1.0379304885864258,
            "Time in s": 44.723793
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.9279645732871132,
            "RMSE": 2.440285299254925,
            "R2": -0.8166009677654511,
            "Memory in Mb": 1.1119890213012695,
            "Time in s": 47.149898
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.91590994704171,
            "RMSE": 2.410261116608071,
            "R2": -0.7913739428902633,
            "Memory in Mb": 1.1737489700317385,
            "Time in s": 49.62861
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8968362370347621,
            "RMSE": 2.379411736746614,
            "R2": -0.7536320120768303,
            "Memory in Mb": 1.261582374572754,
            "Time in s": 52.179919
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8878342141912964,
            "RMSE": 2.351392140243472,
            "R2": -0.7280625702741705,
            "Memory in Mb": 1.3552255630493164,
            "Time in s": 54.784302
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8775558321142263,
            "RMSE": 2.3237456817971016,
            "R2": -0.7062000372474271,
            "Memory in Mb": 1.4321069717407229,
            "Time in s": 57.452517
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8672496542857573,
            "RMSE": 2.297532908897418,
            "R2": -0.6834092983276716,
            "Memory in Mb": 1.4874773025512695,
            "Time in s": 60.173386
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8593706057522699,
            "RMSE": 2.272389423762812,
            "R2": -0.6439286158863597,
            "Memory in Mb": 1.5595178604125977,
            "Time in s": 62.976048
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8551106332542915,
            "RMSE": 2.2487703297155224,
            "R2": -0.6019328469057044,
            "Memory in Mb": 1.619084358215332,
            "Time in s": 65.856537
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8437512715146732,
            "RMSE": 2.224375873084905,
            "R2": -0.5739713521606553,
            "Memory in Mb": 1.1261072158813477,
            "Time in s": 68.798174
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8344220404851989,
            "RMSE": 2.2010168562801016,
            "R2": -0.5664083310843888,
            "Memory in Mb": 1.167832374572754,
            "Time in s": 71.779904
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.825939320609599,
            "RMSE": 2.179009982884269,
            "R2": -0.5482654902802699,
            "Memory in Mb": 1.1199464797973633,
            "Time in s": 74.829165
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8156984309758435,
            "RMSE": 2.1571048007400404,
            "R2": -0.5331573747015668,
            "Memory in Mb": 1.1733713150024414,
            "Time in s": 77.929016
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.806477335746804,
            "RMSE": 2.1360065895495888,
            "R2": -0.5325097322303367,
            "Memory in Mb": 1.2283296585083008,
            "Time in s": 81.05698100000001
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.8008625237630099,
            "RMSE": 2.1159877488140326,
            "R2": -0.5292346593649373,
            "Memory in Mb": 1.2836008071899414,
            "Time in s": 84.241983
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Adaptive Random Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.800378499538596,
            "RMSE": 2.1149541843634605,
            "R2": -0.5287610996295022,
            "Memory in Mb": 1.2846193313598633,
            "Time in s": 87.445729
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.0878895070954884,
            "RMSE": 1.3778002085324723,
            "R2": -1.2599207317049026,
            "Memory in Mb": 0.1791715621948242,
            "Time in s": 0.003809
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.15171477394762,
            "RMSE": 1.5218208011368886,
            "R2": -1.3974856828423898,
            "Memory in Mb": 0.3313665390014648,
            "Time in s": 0.017797
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.2596040860169628,
            "RMSE": 1.630698561429495,
            "R2": -0.8214033882315572,
            "Memory in Mb": 0.4835615158081054,
            "Time in s": 0.056943
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.147002532502157,
            "RMSE": 1.5136945038262,
            "R2": -0.7860708992998826,
            "Memory in Mb": 0.6357030868530273,
            "Time in s": 0.120895
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.7448650745312246,
            "RMSE": 2.8901942810902064,
            "R2": -0.6023944619968462,
            "Memory in Mb": 0.795161247253418,
            "Time in s": 0.341288
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 1.974173643458203,
            "RMSE": 3.1122799656868354,
            "R2": 0.1967701507194095,
            "Memory in Mb": 0.949946403503418,
            "Time in s": 0.602886
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 2.3465039451978784,
            "RMSE": 3.868783481489585,
            "R2": 0.1653904369447871,
            "Memory in Mb": 1.1044378280639648,
            "Time in s": 0.885897
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 2.3152944739841907,
            "RMSE": 3.751470845606434,
            "R2": 0.286453015670338,
            "Memory in Mb": 1.2595434188842771,
            "Time in s": 1.213122
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 2.485126688481329,
            "RMSE": 3.8753788781661274,
            "R2": 0.3615628965518305,
            "Memory in Mb": 1.4176397323608398,
            "Time in s": 1.708637
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 2.679180085056696,
            "RMSE": 4.098463178184459,
            "R2": 0.5005082908479199,
            "Memory in Mb": 1.580409049987793,
            "Time in s": 2.233256
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 2.993112128155013,
            "RMSE": 4.501608187312601,
            "R2": 0.5353065115430311,
            "Memory in Mb": 1.7385053634643557,
            "Time in s": 2.789253
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.049130101089184,
            "RMSE": 4.474860576824222,
            "R2": 0.624267329970883,
            "Memory in Mb": 1.8972959518432615,
            "Time in s": 3.530617
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.129389359320645,
            "RMSE": 4.535626207267123,
            "R2": 0.6870855629914132,
            "Memory in Mb": 2.0540571212768555,
            "Time in s": 4.307795
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.2350921629171503,
            "RMSE": 4.614317779917637,
            "R2": 0.7245583098520811,
            "Memory in Mb": 2.21335506439209,
            "Time in s": 5.238077
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.615407192454655,
            "RMSE": 5.434402308521257,
            "R2": 0.6928112980835472,
            "Memory in Mb": 2.370730400085449,
            "Time in s": 6.215347
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.842899644735678,
            "RMSE": 5.8926781106586255,
            "R2": 0.7087106044563829,
            "Memory in Mb": 2.5251951217651367,
            "Time in s": 7.308114
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 3.939333513046091,
            "RMSE": 5.936527515565436,
            "R2": 0.7578865873655871,
            "Memory in Mb": 2.680434226989746,
            "Time in s": 8.444739
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 4.1526220464224926,
            "RMSE": 6.160116941975886,
            "R2": 0.7926170753106898,
            "Memory in Mb": 2.8339643478393555,
            "Time in s": 9.747256
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 4.486090256229248,
            "RMSE": 6.857164593682279,
            "R2": 0.7881489392686998,
            "Memory in Mb": 2.990111351013184,
            "Time in s": 11.107311
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 5.095083445923365,
            "RMSE": 8.268326900050806,
            "R2": 0.7303274183124314,
            "Memory in Mb": 3.147219657897949,
            "Time in s": 12.601651
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 5.345901760482457,
            "RMSE": 8.651953805757511,
            "R2": 0.7474084291359289,
            "Memory in Mb": 3.301150321960449,
            "Time in s": 14.172197999999998
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 5.775936882313693,
            "RMSE": 9.234098241635358,
            "R2": 0.7685060952534608,
            "Memory in Mb": 3.4575910568237305,
            "Time in s": 15.876551999999998
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 6.050411841877211,
            "RMSE": 9.480574702158652,
            "R2": 0.7880472652798773,
            "Memory in Mb": 3.6158742904663086,
            "Time in s": 17.675130999999997
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 6.7396819662512994,
            "RMSE": 10.861908099063555,
            "R2": 0.7457953067175733,
            "Memory in Mb": 3.77274227142334,
            "Time in s": 19.599013
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 7.418933110619537,
            "RMSE": 12.596893007879746,
            "R2": 0.699156722346497,
            "Memory in Mb": 3.926619529724121,
            "Time in s": 21.625011
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 7.830180870941,
            "RMSE": 13.02165358749325,
            "R2": 0.7215679622698357,
            "Memory in Mb": 4.082179069519043,
            "Time in s": 23.771258
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 8.059624975297776,
            "RMSE": 13.201631143135527,
            "R2": 0.7517949935656911,
            "Memory in Mb": 4.237311363220215,
            "Time in s": 26.095147
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 8.517266870602596,
            "RMSE": 14.029786197157003,
            "R2": 0.750336177123377,
            "Memory in Mb": 4.390841484069824,
            "Time in s": 28.501657
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 9.872910663629112,
            "RMSE": 17.67011178426297,
            "R2": 0.6406578335650022,
            "Memory in Mb": 4.544772148132324,
            "Time in s": 31.026265
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 10.355957081475973,
            "RMSE": 18.251720539867826,
            "R2": 0.671924837978655,
            "Memory in Mb": 4.698409080505371,
            "Time in s": 33.677708
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 10.779061369126929,
            "RMSE": 18.644503325392748,
            "R2": 0.6934349036095702,
            "Memory in Mb": 4.852313041687012,
            "Time in s": 36.483969
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 10.97013178962945,
            "RMSE": 18.69029492717773,
            "R2": 0.7199342471488321,
            "Memory in Mb": 5.009421348571777,
            "Time in s": 39.412921
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 11.836385670325258,
            "RMSE": 20.411474322578705,
            "R2": 0.6756306209292051,
            "Memory in Mb": 5.165541648864746,
            "Time in s": 42.477176
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 12.650208752532226,
            "RMSE": 22.152599191433616,
            "R2": 0.6487731216482631,
            "Memory in Mb": 5.323611259460449,
            "Time in s": 45.685202
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 13.26433375884341,
            "RMSE": 22.74111870549559,
            "R2": 0.672536034672935,
            "Memory in Mb": 5.478930473327637,
            "Time in s": 49.011467
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 13.285084454056172,
            "RMSE": 22.62858691877232,
            "R2": 0.6976709876564118,
            "Memory in Mb": 5.63400936126709,
            "Time in s": 52.447627
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 14.297859574888522,
            "RMSE": 24.603705237609702,
            "R2": 0.6677818184200794,
            "Memory in Mb": 5.789168357849121,
            "Time in s": 55.986709
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 15.277775247208368,
            "RMSE": 26.91758918665374,
            "R2": 0.6267299649165277,
            "Memory in Mb": 5.945448875427246,
            "Time in s": 59.629264
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 16.148002577856595,
            "RMSE": 27.91235298687263,
            "R2": 0.643353503146777,
            "Memory in Mb": 6.099112510681152,
            "Time in s": 63.379206
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 16.450833155107055,
            "RMSE": 28.053185003016477,
            "R2": 0.6652347923635655,
            "Memory in Mb": 6.252856254577637,
            "Time in s": 67.23493599999999
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 16.938736394119786,
            "RMSE": 28.680885446607185,
            "R2": 0.6649461832952053,
            "Memory in Mb": 6.407908439636231,
            "Time in s": 71.205463
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 18.465286457846624,
            "RMSE": 32.222162406640614,
            "R2": 0.6027938253530374,
            "Memory in Mb": 6.562827110290527,
            "Time in s": 75.286683
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 19.36878629272608,
            "RMSE": 33.403615991184594,
            "R2": 0.6231055060350865,
            "Memory in Mb": 6.717398643493652,
            "Time in s": 79.474485
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 19.88015130963188,
            "RMSE": 33.764210229402664,
            "R2": 0.6360141173956066,
            "Memory in Mb": 6.872824668884277,
            "Time in s": 83.769797
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 20.57744796303998,
            "RMSE": 34.830627929035586,
            "R2": 0.6356250399764956,
            "Memory in Mb": 7.029131889343262,
            "Time in s": 88.176271
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 21.43571571603741,
            "RMSE": 36.40788480688662,
            "R2": 0.6134430891768862,
            "Memory in Mb": 7.184878349304199,
            "Time in s": 92.694929
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 22.34914238062968,
            "RMSE": 37.807266067412606,
            "R2": 0.6066317565796657,
            "Memory in Mb": 7.340197563171387,
            "Time in s": 97.332285
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 23.191315994328228,
            "RMSE": 38.81894260965106,
            "R2": 0.6271697641288401,
            "Memory in Mb": 7.495863914489746,
            "Time in s": 102.073572
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 23.34075784343543,
            "RMSE": 38.827434948624926,
            "R2": 0.6423969913213963,
            "Memory in Mb": 7.652411460876465,
            "Time in s": 106.920364
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 24.12545732554984,
            "RMSE": 39.99965605849559,
            "R2": 0.6321733437483394,
            "Memory in Mb": 7.811335563659668,
            "Time in s": 111.876093
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 24.859407485948264,
            "RMSE": 40.9180834433101,
            "R2": 0.6319179521646502,
            "Memory in Mb": 7.9698591232299805,
            "Time in s": 116.942977
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 25.582967433016183,
            "RMSE": 41.65667948828452,
            "R2": 0.6471310448579161,
            "Memory in Mb": 8.12806224822998,
            "Time in s": 122.12293
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ChickWeights",
            "MAE": 25.674172622955844,
            "RMSE": 41.71227980537356,
            "R2": 0.65479005999511,
            "Memory in Mb": 8.21412181854248,
            "Time in s": 127.415096
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3812789990066343,
            "RMSE": 0.4856864156914124,
            "R2": 0.4734504440676397,
            "Memory in Mb": 0.3661947250366211,
            "Time in s": 0.012803
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3903932807396207,
            "RMSE": 0.4802129236445582,
            "R2": 0.908098150441852,
            "Memory in Mb": 0.7077703475952148,
            "Time in s": 0.066318
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3553562094560649,
            "RMSE": 0.4475448539758346,
            "R2": 0.8908737885344612,
            "Memory in Mb": 1.0465993881225586,
            "Time in s": 0.161186
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3785078228066897,
            "RMSE": 0.4818104291982039,
            "R2": 0.8725877843301283,
            "Memory in Mb": 1.386988639831543,
            "Time in s": 0.310355
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3456451525369771,
            "RMSE": 0.450476311872574,
            "R2": 0.9301027529077078,
            "Memory in Mb": 1.7262754440307615,
            "Time in s": 0.520575
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3369671927041528,
            "RMSE": 0.4421642502671299,
            "R2": 0.9427860880043346,
            "Memory in Mb": 2.0684385299682617,
            "Time in s": 0.828496
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3170957614007029,
            "RMSE": 0.4217273000916425,
            "R2": 0.9461011323760548,
            "Memory in Mb": 2.404311180114746,
            "Time in s": 1.349971
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3307037984070857,
            "RMSE": 0.4315519243898653,
            "R2": 0.9502341257934384,
            "Memory in Mb": 2.7412595748901367,
            "Time in s": 1.938101
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3239117556806251,
            "RMSE": 0.4198186275021798,
            "R2": 0.9586532343987924,
            "Memory in Mb": 3.0777502059936523,
            "Time in s": 2.6707590000000003
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3216990324082377,
            "RMSE": 0.4152317221827294,
            "R2": 0.959406710806771,
            "Memory in Mb": 3.414671897888184,
            "Time in s": 3.525266
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3195426619101423,
            "RMSE": 0.4098153846782661,
            "R2": 0.95731130106893,
            "Memory in Mb": 3.7566747665405273,
            "Time in s": 4.592894
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3205833893003068,
            "RMSE": 0.409734240531711,
            "R2": 0.9569909127297423,
            "Memory in Mb": 4.096526145935059,
            "Time in s": 5.7511
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3096350275266986,
            "RMSE": 0.3977121378847216,
            "R2": 0.958918388812615,
            "Memory in Mb": 4.436213493347168,
            "Time in s": 7.098098
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3021514917324106,
            "RMSE": 0.3881456980787764,
            "R2": 0.9590118642619369,
            "Memory in Mb": 4.772730827331543,
            "Time in s": 8.655558000000001
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.302378432925199,
            "RMSE": 0.3879302261175293,
            "R2": 0.9597410141114792,
            "Memory in Mb": 5.1073408126831055,
            "Time in s": 10.324296
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3042635511277332,
            "RMSE": 0.3880820602227424,
            "R2": 0.9577019017103428,
            "Memory in Mb": 5.440821647644043,
            "Time in s": 12.208908
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3061116805473403,
            "RMSE": 0.391104192749731,
            "R2": 0.9546026616524738,
            "Memory in Mb": 5.773791313171387,
            "Time in s": 14.314788
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3092553456162419,
            "RMSE": 0.3953517094261167,
            "R2": 0.9532980843409116,
            "Memory in Mb": 6.1096906661987305,
            "Time in s": 16.588556
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3076082401740039,
            "RMSE": 0.3960205626085123,
            "R2": 0.9515479192781826,
            "Memory in Mb": 6.445483207702637,
            "Time in s": 19.05639
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.3014609513967445,
            "RMSE": 0.3890658925747077,
            "R2": 0.951945723428325,
            "Memory in Mb": 6.780200004577637,
            "Time in s": 21.697867
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2971138293692631,
            "RMSE": 0.3834166944817816,
            "R2": 0.9518088379060108,
            "Memory in Mb": 7.116557121276856,
            "Time in s": 24.511965000000004
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2982326339454942,
            "RMSE": 0.3845174635941775,
            "R2": 0.952475485177767,
            "Memory in Mb": 7.451247215270996,
            "Time in s": 27.506667000000004
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2946274143925286,
            "RMSE": 0.3801223802157071,
            "R2": 0.9560358463571956,
            "Memory in Mb": 7.78644847869873,
            "Time in s": 30.697063000000004
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2933968019133882,
            "RMSE": 0.3767220961039539,
            "R2": 0.9578595845961764,
            "Memory in Mb": 8.120524406433105,
            "Time in s": 34.045785
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2879691623817681,
            "RMSE": 0.3709865810494578,
            "R2": 0.9600287871527096,
            "Memory in Mb": 8.45413875579834,
            "Time in s": 37.543006000000005
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2858512762877924,
            "RMSE": 0.3680336140311482,
            "R2": 0.9606162857565064,
            "Memory in Mb": 8.791060447692871,
            "Time in s": 41.194255000000005
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.28337361966731,
            "RMSE": 0.3643610952909248,
            "R2": 0.9615619008486128,
            "Memory in Mb": 9.128493309020996,
            "Time in s": 45.008334000000005
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2882996011532734,
            "RMSE": 0.3724151060029248,
            "R2": 0.9588932716362208,
            "Memory in Mb": 9.463343620300291,
            "Time in s": 48.98956
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.289315517198266,
            "RMSE": 0.3729583387798602,
            "R2": 0.957758997678865,
            "Memory in Mb": 9.801314353942873,
            "Time in s": 53.13082800000001
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2880445309367084,
            "RMSE": 0.3714720231862385,
            "R2": 0.9585805866298192,
            "Memory in Mb": 10.13992977142334,
            "Time in s": 57.44083900000001
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.285913070387579,
            "RMSE": 0.3694806072400069,
            "R2": 0.95966894305211,
            "Memory in Mb": 10.477011680603027,
            "Time in s": 61.917696000000014
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2840899599351511,
            "RMSE": 0.3669642572161526,
            "R2": 0.9609793991220156,
            "Memory in Mb": 10.80936336517334,
            "Time in s": 66.56801000000002
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2804371592513609,
            "RMSE": 0.3629082548929102,
            "R2": 0.9621252180674722,
            "Memory in Mb": 11.1486234664917,
            "Time in s": 71.37699000000002
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2832721366095781,
            "RMSE": 0.3646482252308528,
            "R2": 0.9611623224331388,
            "Memory in Mb": 11.485033988952637,
            "Time in s": 76.34970200000002
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2853757262809053,
            "RMSE": 0.3664704272728199,
            "R2": 0.959741096022156,
            "Memory in Mb": 11.82703685760498,
            "Time in s": 81.48889300000002
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2846995678315971,
            "RMSE": 0.3663721647933076,
            "R2": 0.9588788359612516,
            "Memory in Mb": 12.1649808883667,
            "Time in s": 86.79821800000002
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.284389692089141,
            "RMSE": 0.365623460665911,
            "R2": 0.9590812376103318,
            "Memory in Mb": 12.5026273727417,
            "Time in s": 92.27027700000002
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2812524955317089,
            "RMSE": 0.3622785856535135,
            "R2": 0.9593969665626948,
            "Memory in Mb": 12.84118938446045,
            "Time in s": 97.89633500000002
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2784736419799919,
            "RMSE": 0.3590495394564995,
            "R2": 0.9599459478528628,
            "Memory in Mb": 13.18101406097412,
            "Time in s": 103.67983800000002
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.28122680710979,
            "RMSE": 0.3614117991183927,
            "R2": 0.9590552347518728,
            "Memory in Mb": 13.522452354431152,
            "Time in s": 109.62063100000002
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2798414038154103,
            "RMSE": 0.3599105705870861,
            "R2": 0.958953025104572,
            "Memory in Mb": 13.858756065368652,
            "Time in s": 115.71824100000002
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2792299366421054,
            "RMSE": 0.358810295818463,
            "R2": 0.9588293518961978,
            "Memory in Mb": 14.19906520843506,
            "Time in s": 121.97670500000002
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2757234931419036,
            "RMSE": 0.3557294429539717,
            "R2": 0.9596100235239656,
            "Memory in Mb": 14.53821849822998,
            "Time in s": 128.39866500000002
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2725087918367814,
            "RMSE": 0.3526976163964828,
            "R2": 0.9604999212537026,
            "Memory in Mb": 14.877989768981934,
            "Time in s": 134.987331
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2707423985398595,
            "RMSE": 0.3505322158445511,
            "R2": 0.9608236269181288,
            "Memory in Mb": 15.214400291442873,
            "Time in s": 141.746125
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2714968277868111,
            "RMSE": 0.3507195370917735,
            "R2": 0.960138783514385,
            "Memory in Mb": 15.551268577575684,
            "Time in s": 148.677278
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2704179121014184,
            "RMSE": 0.350599255928843,
            "R2": 0.9598313134304426,
            "Memory in Mb": 15.892088890075684,
            "Time in s": 155.784091
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2707082259086565,
            "RMSE": 0.3516525290937312,
            "R2": 0.9591696518431828,
            "Memory in Mb": 16.229090690612793,
            "Time in s": 163.071856
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2709225398475326,
            "RMSE": 0.3517696828828596,
            "R2": 0.9583487676398438,
            "Memory in Mb": 16.574454307556152,
            "Time in s": 170.541967
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.2686954199893275,
            "RMSE": 0.349579763566054,
            "R2": 0.9581740736545136,
            "Memory in Mb": 16.91306972503662,
            "Time in s": 178.198313
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Aggregated Mondrian Forest",
            "dataset": "TrumpApproval",
            "MAE": 0.268533139095725,
            "RMSE": 0.3494211343568523,
            "R2": 0.9581842100200092,
            "Memory in Mb": 16.932257652282715,
            "Time in s": 186.03359
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 4.664574314574316,
            "RMSE": 12.7079745317607,
            "R2": -206.87879383707747,
            "Memory in Mb": 0.0196142196655273,
            "Time in s": 0.000715
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 2.767694704637076,
            "RMSE": 9.018587183866767,
            "R2": -85.14025986830408,
            "Memory in Mb": 0.0211782455444335,
            "Time in s": 0.002248
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 2.3093367298127023,
            "RMSE": 7.420500566500976,
            "R2": -37.24267181629702,
            "Memory in Mb": 0.0263471603393554,
            "Time in s": 0.0045
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 1.892363968348808,
            "RMSE": 6.441521936619904,
            "R2": -31.668094594906044,
            "Memory in Mb": 0.0274343490600585,
            "Time in s": 0.007522
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 2.1129412159858934,
            "RMSE": 6.114058653243701,
            "R2": -6.297346571779499,
            "Memory in Mb": 0.0340337753295898,
            "Time in s": 0.011341
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 2.832849782567835,
            "RMSE": 6.236602142425367,
            "R2": -2.2730130120415795,
            "Memory in Mb": 0.043257713317871,
            "Time in s": 0.016081
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 3.4069290990236856,
            "RMSE": 6.402381882180361,
            "R2": -1.3118663438824,
            "Memory in Mb": 0.0494871139526367,
            "Time in s": 0.021988
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 3.650377971160808,
            "RMSE": 6.321189272940957,
            "R2": -1.043267371916866,
            "Memory in Mb": 0.0551328659057617,
            "Time in s": 0.050945
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 4.035631404360372,
            "RMSE": 6.4483291916176695,
            "R2": -0.7783857772357967,
            "Memory in Mb": 0.0562467575073242,
            "Time in s": 0.083616
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 4.693189868957898,
            "RMSE": 7.0697740144659305,
            "R2": -0.4927792786841307,
            "Memory in Mb": 0.0576238632202148,
            "Time in s": 0.119642
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.274396860168236,
            "RMSE": 7.6542276724395,
            "R2": -0.3476225254437259,
            "Memory in Mb": 0.0577573776245117,
            "Time in s": 0.157993
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.216037157212015,
            "RMSE": 7.551012267266295,
            "R2": -0.0719037453282565,
            "Memory in Mb": 0.0578107833862304,
            "Time in s": 0.197604
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.030848211447775,
            "RMSE": 7.321940337412501,
            "R2": 0.1836709538125499,
            "Memory in Mb": 0.058394432067871,
            "Time in s": 0.238591
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 4.907406922429448,
            "RMSE": 7.137924382310331,
            "R2": 0.3406662269828342,
            "Memory in Mb": 0.0584478378295898,
            "Time in s": 0.28091
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.132506734403487,
            "RMSE": 7.341156657504303,
            "R2": 0.439370571581684,
            "Memory in Mb": 0.0584478378295898,
            "Time in s": 0.32452
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.292049153445915,
            "RMSE": 7.468652514259996,
            "R2": 0.5321251372519638,
            "Memory in Mb": 0.0590581893920898,
            "Time in s": 0.369448
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.31698748044205,
            "RMSE": 7.461166418014795,
            "R2": 0.6176873420824156,
            "Memory in Mb": 0.0591115951538085,
            "Time in s": 0.415771
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.300228902480157,
            "RMSE": 7.425148329077998,
            "R2": 0.6988181014109027,
            "Memory in Mb": 0.0590581893920898,
            "Time in s": 0.474994
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 5.830499581707958,
            "RMSE": 9.648698249017793,
            "R2": 0.5807452540036802,
            "Memory in Mb": 0.0252714157104492,
            "Time in s": 0.54427
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 6.400718854692065,
            "RMSE": 10.45569246424029,
            "R2": 0.5689754490886993,
            "Memory in Mb": 0.0314207077026367,
            "Time in s": 0.614353
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 6.611665150046439,
            "RMSE": 10.61745698030736,
            "R2": 0.6198209084753062,
            "Memory in Mb": 0.0365362167358398,
            "Time in s": 0.6853290000000001
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 7.029624246247838,
            "RMSE": 11.197269958950692,
            "R2": 0.6597654020329642,
            "Memory in Mb": 0.0410680770874023,
            "Time in s": 0.7572760000000001
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 7.254490759785878,
            "RMSE": 11.350610231674398,
            "R2": 0.6963529412438163,
            "Memory in Mb": 0.0445928573608398,
            "Time in s": 0.830219
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 7.784750145903498,
            "RMSE": 12.258358647532567,
            "R2": 0.6764200982742594,
            "Memory in Mb": 0.0446996688842773,
            "Time in s": 0.904176
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 8.342804112650073,
            "RMSE": 13.247943494163705,
            "R2": 0.6674407623884211,
            "Memory in Mb": 0.0446996688842773,
            "Time in s": 0.986871
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 8.88061114203256,
            "RMSE": 14.075280539927816,
            "R2": 0.6748649197186086,
            "Memory in Mb": 0.0452032089233398,
            "Time in s": 1.0705630000000002
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 9.50078499680378,
            "RMSE": 14.855892526018591,
            "R2": 0.6858683144490312,
            "Memory in Mb": 0.0452299118041992,
            "Time in s": 1.1552540000000002
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 10.07078824210446,
            "RMSE": 15.77018489177999,
            "R2": 0.6847321098344714,
            "Memory in Mb": 0.0452566146850585,
            "Time in s": 1.2409280000000005
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 10.988840488902907,
            "RMSE": 17.80174938329892,
            "R2": 0.6354464447499208,
            "Memory in Mb": 0.0452566146850585,
            "Time in s": 1.3276340000000002
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 11.635092222175304,
            "RMSE": 18.61329763011445,
            "R2": 0.6589287557789436,
            "Memory in Mb": 0.0452833175659179,
            "Time in s": 1.4153970000000002
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 11.7817306308102,
            "RMSE": 18.65165772134248,
            "R2": 0.6933268021215234,
            "Memory in Mb": 0.0452833175659179,
            "Time in s": 1.5042310000000003
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 11.878812775671824,
            "RMSE": 18.699040402285984,
            "R2": 0.7198024587207095,
            "Memory in Mb": 0.0452833175659179,
            "Time in s": 1.5941090000000002
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 12.712200605470676,
            "RMSE": 19.934033697107445,
            "R2": 0.690787203614232,
            "Memory in Mb": 0.0453100204467773,
            "Time in s": 1.685007
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 13.202927457133043,
            "RMSE": 20.9603625224819,
            "R2": 0.6857237785454591,
            "Memory in Mb": 0.0453367233276367,
            "Time in s": 1.776946
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 13.5542070698499,
            "RMSE": 21.51079994203591,
            "R2": 0.707149447507495,
            "Memory in Mb": 0.0453367233276367,
            "Time in s": 1.869942
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 13.642433072457155,
            "RMSE": 21.454130101613703,
            "R2": 0.7283852775805406,
            "Memory in Mb": 0.0453367233276367,
            "Time in s": 1.963987
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 14.50232093628697,
            "RMSE": 22.86556238504221,
            "R2": 0.7132152539462153,
            "Memory in Mb": 0.0456762313842773,
            "Time in s": 2.060696
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 15.245933470432924,
            "RMSE": 24.220098655355127,
            "R2": 0.6979521608965717,
            "Memory in Mb": 0.045729637145996,
            "Time in s": 2.158386
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 15.766409258920858,
            "RMSE": 25.08619072251902,
            "R2": 0.7120527209837302,
            "Memory in Mb": 0.045729637145996,
            "Time in s": 2.2570650000000003
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 15.931210335947624,
            "RMSE": 25.166941851240068,
            "R2": 0.7307081986676882,
            "Memory in Mb": 0.0456495285034179,
            "Time in s": 2.4439120000000005
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 16.418312975299003,
            "RMSE": 25.73673973791796,
            "R2": 0.7303482652633313,
            "Memory in Mb": 0.0461797714233398,
            "Time in s": 2.6336030000000004
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 17.4982370763817,
            "RMSE": 27.78944281741256,
            "R2": 0.7047111429028308,
            "Memory in Mb": 0.0469236373901367,
            "Time in s": 2.8262370000000003
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 18.254684132762545,
            "RMSE": 29.056725346353637,
            "R2": 0.7149358826261665,
            "Memory in Mb": 0.0469770431518554,
            "Time in s": 3.0200670000000005
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 18.58513038702809,
            "RMSE": 29.35463525495672,
            "R2": 0.7250038129485413,
            "Memory in Mb": 0.046950340270996,
            "Time in s": 3.2149970000000003
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 19.01404260598322,
            "RMSE": 29.86038018890717,
            "R2": 0.7323226450377984,
            "Memory in Mb": 0.0468969345092773,
            "Time in s": 3.430483
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 19.88342353555136,
            "RMSE": 31.26600741511644,
            "R2": 0.7150584356224581,
            "Memory in Mb": 0.0469770431518554,
            "Time in s": 3.648791
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 20.595063111922972,
            "RMSE": 32.24616798680886,
            "R2": 0.713982273554131,
            "Memory in Mb": 0.0470037460327148,
            "Time in s": 3.869932
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 21.38047446701005,
            "RMSE": 33.43504054753495,
            "R2": 0.7235347994633756,
            "Memory in Mb": 0.0470037460327148,
            "Time in s": 4.098743
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 21.53249764026729,
            "RMSE": 33.42135235584957,
            "R2": 0.735168024057878,
            "Memory in Mb": 0.0470037460327148,
            "Time in s": 4.328606
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 22.49918784329445,
            "RMSE": 35.002118414433774,
            "R2": 0.7184757368310433,
            "Memory in Mb": 0.0470304489135742,
            "Time in s": 4.559521999999999
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 23.19163412189557,
            "RMSE": 35.912468657285935,
            "R2": 0.7166015220750928,
            "Memory in Mb": 0.0470037460327148,
            "Time in s": 4.791517
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 24.04065682138389,
            "RMSE": 37.100860859043735,
            "R2": 0.7202195492645626,
            "Memory in Mb": 0.046950340270996,
            "Time in s": 5.02459
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "ChickWeights",
            "MAE": 24.19431912937701,
            "RMSE": 37.21658551958108,
            "R2": 0.7253190778127725,
            "Memory in Mb": 0.0469770431518554,
            "Time in s": 5.258551
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 2.695184981652336,
            "RMSE": 9.807184976514188,
            "R2": -224.6021011118197,
            "Memory in Mb": 0.0538091659545898,
            "Time in s": 0.004347
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 2.3994713447037435,
            "RMSE": 7.102066178895935,
            "R2": -19.27845129783118,
            "Memory in Mb": 0.0761518478393554,
            "Time in s": 0.011776
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.8170744682035584,
            "RMSE": 5.815253847056423,
            "R2": -17.329373299766118,
            "Memory in Mb": 0.0883970260620117,
            "Time in s": 0.021496
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.604995404573344,
            "RMSE": 5.081770494168446,
            "R2": -13.040545957103586,
            "Memory in Mb": 0.0980443954467773,
            "Time in s": 0.033628
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.824259078948539,
            "RMSE": 4.70488333223354,
            "R2": -6.5512954222403845,
            "Memory in Mb": 0.1071348190307617,
            "Time in s": 0.048339
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.918744608116588,
            "RMSE": 4.412336880489357,
            "R2": -4.634185300646759,
            "Memory in Mb": 0.1113233566284179,
            "Time in s": 0.066047
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.8761207739327503,
            "RMSE": 4.13187920011476,
            "R2": -4.105616799680584,
            "Memory in Mb": 0.1133375167846679,
            "Time in s": 0.086317
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.961232939518506,
            "RMSE": 3.976173487274506,
            "R2": -3.1695661963674864,
            "Memory in Mb": 0.1174459457397461,
            "Time in s": 0.109348
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 2.066134597500757,
            "RMSE": 3.873731518767916,
            "R2": -2.4756944369169624,
            "Memory in Mb": 0.1194601058959961,
            "Time in s": 0.13519
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 2.051125997923389,
            "RMSE": 3.731810291394655,
            "R2": -2.23527456693896,
            "Memory in Mb": 0.017618179321289,
            "Time in s": 0.169486
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 2.0738811328897206,
            "RMSE": 4.417664564856108,
            "R2": -3.890594467356201,
            "Memory in Mb": 0.0357999801635742,
            "Time in s": 0.205189
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.9726100065438288,
            "RMSE": 4.237524240975239,
            "R2": -3.5337340888030546,
            "Memory in Mb": 0.0414991378784179,
            "Time in s": 0.242476
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.8594315384151243,
            "RMSE": 4.074751007989252,
            "R2": -3.248610147038553,
            "Memory in Mb": 0.048842430114746,
            "Time in s": 0.281406
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.7773205119132678,
            "RMSE": 3.936654153117972,
            "R2": -3.1518424972300867,
            "Memory in Mb": 0.0637884140014648,
            "Time in s": 0.322149
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.8265705896173516,
            "RMSE": 3.8591002097544127,
            "R2": -2.923813511442849,
            "Memory in Mb": 0.0734968185424804,
            "Time in s": 0.364943
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.7442837931334845,
            "RMSE": 3.739506488697679,
            "R2": -2.866813933026025,
            "Memory in Mb": 0.0810766220092773,
            "Time in s": 0.409782
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6994316865849048,
            "RMSE": 3.638004990484729,
            "R2": -2.8674589929341425,
            "Memory in Mb": 0.0861921310424804,
            "Time in s": 0.456846
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6868885299887,
            "RMSE": 3.55458556923881,
            "R2": -2.7224500036418355,
            "Memory in Mb": 0.0937795639038086,
            "Time in s": 0.506202
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.637461983479605,
            "RMSE": 3.464628975063406,
            "R2": -2.658760364179245,
            "Memory in Mb": 0.0988950729370117,
            "Time in s": 0.560423
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.622197889515682,
            "RMSE": 3.392154183911459,
            "R2": -2.6064142473473755,
            "Memory in Mb": 0.1061124801635742,
            "Time in s": 0.624493
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6252883623828789,
            "RMSE": 3.33131196963583,
            "R2": -2.593313247083074,
            "Memory in Mb": 0.1101140975952148,
            "Time in s": 0.691125
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.663593439145693,
            "RMSE": 3.2993129689970107,
            "R2": -2.4608371725208844,
            "Memory in Mb": 0.1157598495483398,
            "Time in s": 0.760369
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6928806013876203,
            "RMSE": 3.26900202016339,
            "R2": -2.221881423949668,
            "Memory in Mb": 0.1238431930541992,
            "Time in s": 0.832438
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6463369530072471,
            "RMSE": 3.2036213976345094,
            "R2": -2.023106408032965,
            "Memory in Mb": 0.1315031051635742,
            "Time in s": 0.907505
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6312675040418116,
            "RMSE": 3.1569789450171624,
            "R2": -1.8741285299844173,
            "Memory in Mb": 0.0784368515014648,
            "Time in s": 0.99002
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6486177246548734,
            "RMSE": 3.1232792518100463,
            "R2": -1.81800645719813,
            "Memory in Mb": 0.0835790634155273,
            "Time in s": 1.082168
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.664948820150162,
            "RMSE": 3.091452157271598,
            "R2": -1.7507490735781142,
            "Memory in Mb": 0.0873861312866211,
            "Time in s": 1.179534
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6361907885919602,
            "RMSE": 3.043459997537018,
            "R2": -1.7295303491345493,
            "Memory in Mb": 0.0885534286499023,
            "Time in s": 1.466782
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6082012495575049,
            "RMSE": 2.9965453347231947,
            "R2": -1.7114709556760634,
            "Memory in Mb": 0.0890569686889648,
            "Time in s": 1.757406
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.622569336171024,
            "RMSE": 2.97009213510141,
            "R2": -1.634341750696236,
            "Memory in Mb": 0.0909147262573242,
            "Time in s": 2.050417
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.636890396487252,
            "RMSE": 2.946158197159977,
            "R2": -1.5525460315178896,
            "Memory in Mb": 0.0923452377319336,
            "Time in s": 2.345765
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.652159107256621,
            "RMSE": 2.9245287804119107,
            "R2": -1.4681901897894076,
            "Memory in Mb": 0.0944395065307617,
            "Time in s": 2.643466
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6570267761004454,
            "RMSE": 2.8972896524900835,
            "R2": -1.4050084478390592,
            "Memory in Mb": 0.0960302352905273,
            "Time in s": 2.943569
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.6362052297782712,
            "RMSE": 2.859601997032609,
            "R2": -1.379870428705038,
            "Memory in Mb": 0.0981245040893554,
            "Time in s": 3.2460560000000003
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.608205636538717,
            "RMSE": 2.821326923745488,
            "R2": -1.377433396876134,
            "Memory in Mb": 0.1015691757202148,
            "Time in s": 3.5543920000000004
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5855230254631891,
            "RMSE": 2.785659545407005,
            "R2": -1.3686218528413674,
            "Memory in Mb": 0.1027364730834961,
            "Time in s": 3.875571
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.583695771004626,
            "RMSE": 2.7597111871599203,
            "R2": -1.3233016566851918,
            "Memory in Mb": 0.1038503646850586,
            "Time in s": 4.202987
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5704020318609786,
            "RMSE": 2.7290361106702816,
            "R2": -1.2965538228485634,
            "Memory in Mb": 0.1038503646850586,
            "Time in s": 4.532954
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5638796853366008,
            "RMSE": 2.702190403614744,
            "R2": -1.2616800152467116,
            "Memory in Mb": 0.1064214706420898,
            "Time in s": 4.876142
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5494799828615766,
            "RMSE": 2.674411214594314,
            "R2": -1.2354538504080876,
            "Memory in Mb": 0.1070318222045898,
            "Time in s": 5.221917
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.533437809889996,
            "RMSE": 2.6465115200139584,
            "R2": -1.213096407446464,
            "Memory in Mb": 0.1085958480834961,
            "Time in s": 5.570086999999999
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5202839319169328,
            "RMSE": 2.6201051582792827,
            "R2": -1.189291971541785,
            "Memory in Mb": 0.1101598739624023,
            "Time in s": 5.920738999999999
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.5178574341866524,
            "RMSE": 2.5988091386120904,
            "R2": -1.1501373691585313,
            "Memory in Mb": 0.1107702255249023,
            "Time in s": 6.280333
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.4962844530295305,
            "RMSE": 2.571223801389781,
            "R2": -1.094275733877604,
            "Memory in Mb": 0.1112470626831054,
            "Time in s": 6.652339
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.4724252749133646,
            "RMSE": 2.5436398469986066,
            "R2": -1.0582196084183888,
            "Memory in Mb": 0.1116437911987304,
            "Time in s": 7.031402
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.4596881679466962,
            "RMSE": 2.5220256913044325,
            "R2": -1.056635177134157,
            "Memory in Mb": 0.1116704940795898,
            "Time in s": 7.413564
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.452139596196528,
            "RMSE": 2.5028075284250018,
            "R2": -1.0425932823285438,
            "Memory in Mb": 0.1127042770385742,
            "Time in s": 7.802334
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.4364147887122178,
            "RMSE": 2.481230554777158,
            "R2": -1.0285162299402342,
            "Memory in Mb": 0.1132078170776367,
            "Time in s": 8.193766
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.4186260884044517,
            "RMSE": 2.45780687839372,
            "R2": -1.029053861068545,
            "Memory in Mb": 0.1138181686401367,
            "Time in s": 8.587828
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.3997779646996389,
            "RMSE": 2.434572696055838,
            "R2": -1.024386017127401,
            "Memory in Mb": 0.1144285202026367,
            "Time in s": 8.984547
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Adaptive Model Rules",
            "dataset": "TrumpApproval",
            "MAE": 1.3984653255896196,
            "RMSE": 2.433357833975862,
            "R2": -1.0237164038272608,
            "Memory in Mb": 0.1144285202026367,
            "Time in s": 9.38293
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 4.674710287324511,
            "RMSE": 12.709622005759083,
            "R2": -206.93269654300337,
            "Memory in Mb": 0.1438665390014648,
            "Time in s": 0.053261
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.741934273684416,
            "RMSE": 9.017856101646904,
            "R2": -85.12629469646626,
            "Memory in Mb": 0.1680784225463867,
            "Time in s": 0.14276
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.35434760029741,
            "RMSE": 7.430504888974863,
            "R2": -37.34585890537725,
            "Memory in Mb": 0.2096052169799804,
            "Time in s": 0.266148
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 1.9327820011330463,
            "RMSE": 6.452362261246447,
            "R2": -31.77814024428305,
            "Memory in Mb": 0.2417478561401367,
            "Time in s": 0.646479
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.2606373648191784,
            "RMSE": 6.146136842066936,
            "R2": -6.374120366305681,
            "Memory in Mb": 0.3060827255249023,
            "Time in s": 1.057843
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.3521495161457717,
            "RMSE": 5.750947689984691,
            "R2": -1.7831107407377038,
            "Memory in Mb": 0.3567266464233398,
            "Time in s": 1.521792
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.707478618787897,
            "RMSE": 5.832856917221716,
            "R2": -0.9188552689556648,
            "Memory in Mb": 0.3732900619506836,
            "Time in s": 2.259814
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.60389034076398,
            "RMSE": 5.525482549715508,
            "R2": -0.5612341217350767,
            "Memory in Mb": 0.4128637313842773,
            "Time in s": 3.03269
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.7646559934763437,
            "RMSE": 5.466320467144536,
            "R2": -0.2779732207399938,
            "Memory in Mb": 0.4623746871948242,
            "Time in s": 3.85418
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 2.880719733615897,
            "RMSE": 5.407041915578862,
            "R2": 0.1268195431914148,
            "Memory in Mb": 0.5318593978881836,
            "Time in s": 4.717509000000001
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.0896780011355176,
            "RMSE": 5.466874267225462,
            "R2": 0.3125459405386915,
            "Memory in Mb": 0.5604543685913086,
            "Time in s": 5.631386000000001
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.270943191870578,
            "RMSE": 5.7618521847151385,
            "R2": 0.3758777549527384,
            "Memory in Mb": 0.1946859359741211,
            "Time in s": 6.649151000000001
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.24701597703502,
            "RMSE": 5.633009027852055,
            "R2": 0.5168368848346436,
            "Memory in Mb": 0.2288389205932617,
            "Time in s": 7.703019000000001
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.2192007860807728,
            "RMSE": 5.520141144427338,
            "R2": 0.6056681999848637,
            "Memory in Mb": 0.2577199935913086,
            "Time in s": 8.869892000000002
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.5165819956804767,
            "RMSE": 5.874797514643079,
            "R2": 0.6409683688760216,
            "Memory in Mb": 0.2627325057983398,
            "Time in s": 10.065309000000005
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.700430602978386,
            "RMSE": 6.068185859760413,
            "R2": 0.6911390854727877,
            "Memory in Mb": 0.2941198348999023,
            "Time in s": 11.324773000000002
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 3.803730902742884,
            "RMSE": 6.1218084380222,
            "R2": 0.7426259865968339,
            "Memory in Mb": 0.3320951461791992,
            "Time in s": 12.629055000000005
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 4.006649900662983,
            "RMSE": 6.578339511639692,
            "R2": 0.7635979888713487,
            "Memory in Mb": 0.2527418136596679,
            "Time in s": 13.981910000000005
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 4.229383118423565,
            "RMSE": 6.982583803939909,
            "R2": 0.780430075854037,
            "Memory in Mb": 0.3202161788940429,
            "Time in s": 15.391493000000002
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 4.825249759558611,
            "RMSE": 8.423350501384354,
            "R2": 0.720252540483964,
            "Memory in Mb": 0.3510808944702148,
            "Time in s": 16.880127
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 5.088028806665401,
            "RMSE": 8.669832171958772,
            "R2": 0.7465054715218886,
            "Memory in Mb": 0.3200139999389648,
            "Time in s": 18.399834
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 5.462442991686406,
            "RMSE": 9.175585237136575,
            "R2": 0.7715339230013022,
            "Memory in Mb": 0.3710927963256836,
            "Time in s": 20.020863
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 5.563619467556412,
            "RMSE": 9.260101660572657,
            "R2": 0.797901929856006,
            "Memory in Mb": 0.4192609786987304,
            "Time in s": 21.677784000000003
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 6.261116867150435,
            "RMSE": 10.599777327157994,
            "R2": 0.7580584961853923,
            "Memory in Mb": 0.3416013717651367,
            "Time in s": 23.387217000000003
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 6.742618468073929,
            "RMSE": 11.80224059778972,
            "R2": 0.7360625543191792,
            "Memory in Mb": 0.3569021224975586,
            "Time in s": 25.127202000000004
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 7.039594962415952,
            "RMSE": 12.249488193444416,
            "R2": 0.7537446936710837,
            "Memory in Mb": 0.3965520858764648,
            "Time in s": 26.911059000000005
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 7.148800229885712,
            "RMSE": 12.311677740983953,
            "R2": 0.7842510327710687,
            "Memory in Mb": 0.4258260726928711,
            "Time in s": 28.739538000000007
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 7.753683144422786,
            "RMSE": 13.244190950829555,
            "R2": 0.7776398094561477,
            "Memory in Mb": 0.4501142501831054,
            "Time in s": 30.59385600000001
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 8.773143666519827,
            "RMSE": 15.93975365978218,
            "R2": 0.7077199430319765,
            "Memory in Mb": 0.4718656539916992,
            "Time in s": 32.508295000000004
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 9.312574124937234,
            "RMSE": 16.796832021919023,
            "R2": 0.7222505421616592,
            "Memory in Mb": 0.3236379623413086,
            "Time in s": 34.514388000000004
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 9.544591695703463,
            "RMSE": 16.94083213248977,
            "R2": 0.7470058810264122,
            "Memory in Mb": 0.3676939010620117,
            "Time in s": 36.550995
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 9.680039805071171,
            "RMSE": 17.006622056031052,
            "R2": 0.7682275557667291,
            "Memory in Mb": 0.3629522323608398,
            "Time in s": 38.648436
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 10.417098847501563,
            "RMSE": 18.381838377902795,
            "R2": 0.7370670774420947,
            "Memory in Mb": 0.3571195602416992,
            "Time in s": 40.771216
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 11.080869197293334,
            "RMSE": 19.965812195666537,
            "R2": 0.7148404591067161,
            "Memory in Mb": 0.3998785018920898,
            "Time in s": 42.937715
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 11.60940210623338,
            "RMSE": 20.687378926969966,
            "R2": 0.7291406299077132,
            "Memory in Mb": 0.3288450241088867,
            "Time in s": 45.213373
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 11.737814918904208,
            "RMSE": 20.678726756260627,
            "R2": 0.7476640805491588,
            "Memory in Mb": 0.4024953842163086,
            "Time in s": 47.506899
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 12.682108791666492,
            "RMSE": 22.361726245252385,
            "R2": 0.7257144517605874,
            "Memory in Mb": 0.4475545883178711,
            "Time in s": 49.84079500000001
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 13.622708961705229,
            "RMSE": 24.146094170569185,
            "R2": 0.6997951546356598,
            "Memory in Mb": 0.4968290328979492,
            "Time in s": 52.212878
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 14.165217959113354,
            "RMSE": 24.88032134675199,
            "R2": 0.7167593971826183,
            "Memory in Mb": 0.5376424789428711,
            "Time in s": 54.630802
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 14.411006646174876,
            "RMSE": 24.97835315387625,
            "R2": 0.7347289581181171,
            "Memory in Mb": 0.5657072067260742,
            "Time in s": 57.077112
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 14.766578325445964,
            "RMSE": 25.376772271610328,
            "R2": 0.7378384948653763,
            "Memory in Mb": 0.2583265304565429,
            "Time in s": 59.570857
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 16.09445226127713,
            "RMSE": 28.12961105819035,
            "R2": 0.6974376845026461,
            "Memory in Mb": 0.3047628402709961,
            "Time in s": 62.101038
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 16.916275460891086,
            "RMSE": 29.341089843915015,
            "R2": 0.7093290035354769,
            "Memory in Mb": 0.3544912338256836,
            "Time in s": 64.67061
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 17.222566694739786,
            "RMSE": 29.549549967606488,
            "R2": 0.7213397403469026,
            "Memory in Mb": 0.3983259201049804,
            "Time in s": 67.26974899999999
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 17.854950072386483,
            "RMSE": 30.34354672604944,
            "R2": 0.7235900637963901,
            "Memory in Mb": 0.4324254989624023,
            "Time in s": 69.89740799999998
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 18.84874733203415,
            "RMSE": 31.79966974813451,
            "R2": 0.7052484004379906,
            "Memory in Mb": 0.4678411483764648,
            "Time in s": 72.66954099999998
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 19.785853660032195,
            "RMSE": 33.20181112471305,
            "R2": 0.6967783021275082,
            "Memory in Mb": 0.4975500106811523,
            "Time in s": 75.49558399999998
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 20.52664258005787,
            "RMSE": 34.100310164439925,
            "R2": 0.7124234805234935,
            "Memory in Mb": 0.5351285934448242,
            "Time in s": 78.36005299999998
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 20.766026265849117,
            "RMSE": 34.21097619783695,
            "R2": 0.7225061795517687,
            "Memory in Mb": 0.576685905456543,
            "Time in s": 81.26779099999997
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 21.840503815170692,
            "RMSE": 36.15896607268933,
            "R2": 0.6995590139862528,
            "Memory in Mb": 0.4753904342651367,
            "Time in s": 84.25568299999998
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 22.59690624313325,
            "RMSE": 37.108967777985264,
            "R2": 0.6974029137241997,
            "Memory in Mb": 0.5189352035522461,
            "Time in s": 87.27382099999997
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 23.534320250737128,
            "RMSE": 38.28067851879141,
            "R2": 0.7021424273708647,
            "Memory in Mb": 0.5585355758666992,
            "Time in s": 90.32555299999996
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "ChickWeights",
            "MAE": 23.709683411591413,
            "RMSE": 38.44162901827647,
            "R2": 0.7069383356385298,
            "Memory in Mb": 0.3551816940307617,
            "Time in s": 93.40141099999995
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 2.677140920600926,
            "RMSE": 9.804891856735376,
            "R2": -224.4966127051096,
            "Memory in Mb": 0.2373647689819336,
            "Time in s": 0.078317
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 2.42676306487335,
            "RMSE": 7.150663284447028,
            "R2": -19.556918338481843,
            "Memory in Mb": 0.3270711898803711,
            "Time in s": 0.2600639999999999
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.8116457742622056,
            "RMSE": 5.852230884873156,
            "R2": -17.563213740222555,
            "Memory in Mb": 0.3493108749389648,
            "Time in s": 0.628767
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.5261658032230545,
            "RMSE": 5.084894428469453,
            "R2": -13.057813649460384,
            "Memory in Mb": 0.3968191146850586,
            "Time in s": 1.163603
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.404885103917059,
            "RMSE": 4.580518627305071,
            "R2": -6.157363117938322,
            "Memory in Mb": 0.4107885360717773,
            "Time in s": 1.7740749999999998
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.2872329076385731,
            "RMSE": 4.198963935277897,
            "R2": -4.102442140657352,
            "Memory in Mb": 0.4562673568725586,
            "Time in s": 2.455989
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.4191481295394186,
            "RMSE": 4.9019146331166,
            "R2": -6.185954638838571,
            "Memory in Mb": 0.2026891708374023,
            "Time in s": 3.22825
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.329290869551211,
            "RMSE": 4.594852312450113,
            "R2": -4.568052693162012,
            "Memory in Mb": 0.3215742111206054,
            "Time in s": 4.121231
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.2559271503392595,
            "RMSE": 4.341680890984575,
            "R2": -3.3661470093978725,
            "Memory in Mb": 0.4017667770385742,
            "Time in s": 5.147797
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.169313410896163,
            "RMSE": 4.12134361195162,
            "R2": -2.94593273053925,
            "Memory in Mb": 0.4772901535034179,
            "Time in s": 6.338072
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.1066399346497042,
            "RMSE": 3.9344660517514094,
            "R2": -2.8792501333638807,
            "Memory in Mb": 0.5200605392456055,
            "Time in s": 7.615136
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.0535228972416335,
            "RMSE": 3.7704097053754206,
            "R2": -2.589291599563797,
            "Memory in Mb": 0.590418815612793,
            "Time in s": 8.98983
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 1.0002808672832586,
            "RMSE": 3.624331376507975,
            "R2": -2.3612477765650133,
            "Memory in Mb": 0.677699089050293,
            "Time in s": 10.49221
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9484528900796008,
            "RMSE": 3.4935839886686573,
            "R2": -2.269856713922535,
            "Memory in Mb": 0.7459287643432617,
            "Time in s": 12.09809
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9319658343242508,
            "RMSE": 3.3810597344709987,
            "R2": -2.011909605217061,
            "Memory in Mb": 0.8300580978393555,
            "Time in s": 13.828036
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9015525068993324,
            "RMSE": 3.2761126415748776,
            "R2": -1.9678527090537403,
            "Memory in Mb": 0.8134641647338867,
            "Time in s": 15.697273999999998
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9086073156973856,
            "RMSE": 3.206516550071244,
            "R2": -2.0044577988421626,
            "Memory in Mb": 0.7938528060913086,
            "Time in s": 17.678026
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9209686764414104,
            "RMSE": 3.130698586248577,
            "R2": -1.887576115168536,
            "Memory in Mb": 0.8660383224487305,
            "Time in s": 19.789752
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9054594388814018,
            "RMSE": 3.0518145886207013,
            "R2": -1.838813023440576,
            "Memory in Mb": 0.930495262145996,
            "Time in s": 22.025823
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9021459083449618,
            "RMSE": 2.9892737243691805,
            "R2": -1.8006304820861794,
            "Memory in Mb": 0.9046812057495116,
            "Time in s": 24.377516
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.9000900027115483,
            "RMSE": 2.937103674242639,
            "R2": -1.7932063526136273,
            "Memory in Mb": 0.2984609603881836,
            "Time in s": 26.835964
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.884833385913356,
            "RMSE": 2.873027664171451,
            "R2": -1.6243016536608597,
            "Memory in Mb": 0.3453207015991211,
            "Time in s": 29.357596
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.8690754265879537,
            "RMSE": 2.8131168800056585,
            "R2": -1.3859136859847618,
            "Memory in Mb": 0.3807516098022461,
            "Time in s": 31.984181
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.8473225380080763,
            "RMSE": 2.75510952719956,
            "R2": -1.235881587238783,
            "Memory in Mb": 0.4482488632202148,
            "Time in s": 34.68911
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.8286186581223807,
            "RMSE": 2.701061117260836,
            "R2": -1.1039316995995572,
            "Memory in Mb": 0.4975194931030273,
            "Time in s": 37.472375
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.8308331247066605,
            "RMSE": 2.676087993829765,
            "R2": -1.0688124961584973,
            "Memory in Mb": 0.3753881454467773,
            "Time in s": 40.349897
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.8063786739892863,
            "RMSE": 2.6263308571208617,
            "R2": -0.9852938090834252,
            "Memory in Mb": 0.4063673019409179,
            "Time in s": 43.316687
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7997929461413226,
            "RMSE": 2.582727501713279,
            "R2": -0.9656668153374994,
            "Memory in Mb": 0.4374494552612304,
            "Time in s": 46.3679
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7908850979728871,
            "RMSE": 2.541457165367321,
            "R2": -0.950423138286411,
            "Memory in Mb": 0.4967718124389648,
            "Time in s": 49.479346
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7789627943481009,
            "RMSE": 2.500361162030882,
            "R2": -0.8669718089652279,
            "Memory in Mb": 0.569575309753418,
            "Time in s": 52.654549
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7682254429218135,
            "RMSE": 2.461677332861117,
            "R2": -0.7820656947310429,
            "Memory in Mb": 0.6584272384643555,
            "Time in s": 55.885269
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.756836908225871,
            "RMSE": 2.4246570785119217,
            "R2": -0.6965531574296129,
            "Memory in Mb": 0.7120962142944336,
            "Time in s": 59.181412
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7406340846119412,
            "RMSE": 2.388088765643962,
            "R2": -0.6339309775627988,
            "Memory in Mb": 0.8089780807495117,
            "Time in s": 62.54643
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7257657440750075,
            "RMSE": 2.3532857176647086,
            "R2": -0.6117268738432657,
            "Memory in Mb": 0.8398160934448242,
            "Time in s": 65.979515
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7284794894639326,
            "RMSE": 2.325029779726661,
            "R2": -0.6145762958857721,
            "Memory in Mb": 0.9275884628295898,
            "Time in s": 69.48963400000001
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7231955460113827,
            "RMSE": 2.297270435922827,
            "R2": -0.6108826519065647,
            "Memory in Mb": 0.9087285995483398,
            "Time in s": 73.071921
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7217944839950929,
            "RMSE": 2.2699024953355416,
            "R2": -0.5717835473178023,
            "Memory in Mb": 0.8719320297241211,
            "Time in s": 76.723943
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7121024512438853,
            "RMSE": 2.241058668519108,
            "R2": -0.5486900768629306,
            "Memory in Mb": 0.929518699645996,
            "Time in s": 80.452493
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7019422114012909,
            "RMSE": 2.213016497735788,
            "R2": -0.5169405784918113,
            "Memory in Mb": 1.0446271896362305,
            "Time in s": 84.252351
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.7005931807120314,
            "RMSE": 2.188428332233621,
            "R2": -0.4968352306391974,
            "Memory in Mb": 1.1031560897827148,
            "Time in s": 88.13395700000001
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6997484436891046,
            "RMSE": 2.169363820936814,
            "R2": -0.4870225063787143,
            "Memory in Mb": 1.0328702926635742,
            "Time in s": 92.08914500000002
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6949195885567419,
            "RMSE": 2.14957176369946,
            "R2": -0.4735678496288336,
            "Memory in Mb": 0.7475957870483398,
            "Time in s": 96.10836100000002
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6920590805093112,
            "RMSE": 2.1264870362465933,
            "R2": -0.439603572136809,
            "Memory in Mb": 0.8119535446166992,
            "Time in s": 100.182244
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6882027439938415,
            "RMSE": 2.1038322601427426,
            "R2": -0.4020913886240724,
            "Memory in Mb": 0.8655576705932617,
            "Time in s": 104.313167
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6818594219129391,
            "RMSE": 2.085410616994055,
            "R2": -0.38345052454273,
            "Memory in Mb": 0.8467855453491211,
            "Time in s": 108.503439
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6756248333192205,
            "RMSE": 2.0637081851469703,
            "R2": -0.377066205838211,
            "Memory in Mb": 0.9400205612182616,
            "Time in s": 112.753186
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6689624136970388,
            "RMSE": 2.0428592411141837,
            "R2": -0.3608300191067024,
            "Memory in Mb": 0.8168668746948242,
            "Time in s": 117.061539
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6627773066160889,
            "RMSE": 2.022520414368002,
            "R2": -0.3478143420231987,
            "Memory in Mb": 0.9120321273803712,
            "Time in s": 121.43268700000002
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6600305544016135,
            "RMSE": 2.003593726688123,
            "R2": -0.348395800771305,
            "Memory in Mb": 0.9782476425170898,
            "Time in s": 125.86239700000002
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.657029407021691,
            "RMSE": 1.9853014454830336,
            "R2": -0.3461726175729922,
            "Memory in Mb": 1.0593442916870115,
            "Time in s": 130.37428000000003
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Streaming Random Patches",
            "dataset": "TrumpApproval",
            "MAE": 0.6566965628025029,
            "RMSE": 1.984335939466105,
            "R2": -0.3457614763231473,
            "Memory in Mb": 1.0646085739135742,
            "Time in s": 134.90266400000002
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 10.95559056599966,
            "RMSE": 17.7409835250609,
            "R2": -404.147256051216,
            "Memory in Mb": 0.1553668975830078,
            "Time in s": 0.005094
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 5.88626580700965,
            "RMSE": 12.566688603347808,
            "R2": -166.25182631838038,
            "Memory in Mb": 0.1681652069091797,
            "Time in s": 0.018278
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.383857039198176,
            "RMSE": 10.299865918219764,
            "R2": -72.67921052893462,
            "Memory in Mb": 0.2052059173583984,
            "Time in s": 0.039075
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 3.446496162870555,
            "RMSE": 8.931116231999566,
            "R2": -61.79980671874969,
            "Memory in Mb": 0.2209186553955078,
            "Time in s": 0.065167
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 3.3513349782155037,
            "RMSE": 8.247717183177938,
            "R2": -12.279242202465667,
            "Memory in Mb": 0.2687969207763672,
            "Time in s": 0.096566
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 3.889627188952696,
            "RMSE": 8.0458642201752,
            "R2": -4.4474976461238604,
            "Memory in Mb": 0.3383464813232422,
            "Time in s": 0.144605
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.337751636727128,
            "RMSE": 7.9681159743419645,
            "R2": -2.5808890563388096,
            "Memory in Mb": 0.3940753936767578,
            "Time in s": 0.201306
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.489908334389532,
            "RMSE": 7.740787033322287,
            "R2": -2.0640641214272355,
            "Memory in Mb": 0.4405231475830078,
            "Time in s": 0.274421
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.7831270806190425,
            "RMSE": 7.705843596650206,
            "R2": -1.5396388125269618,
            "Memory in Mb": 0.4615802764892578,
            "Time in s": 0.372843
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.73395080514245,
            "RMSE": 7.47334250555501,
            "R2": -0.6680701376440403,
            "Memory in Mb": 0.4910602569580078,
            "Time in s": 0.5845670000000001
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.733710015085173,
            "RMSE": 7.331306378435282,
            "R2": -0.236312465025352,
            "Memory in Mb": 0.5042209625244141,
            "Time in s": 0.806575
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.565752852065114,
            "RMSE": 7.0976416640915465,
            "R2": 0.0529485447239657,
            "Memory in Mb": 0.5126438140869141,
            "Time in s": 1.039517
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.439022558662509,
            "RMSE": 6.895745596080793,
            "R2": 0.2759386934515202,
            "Memory in Mb": 0.5216274261474609,
            "Time in s": 1.284562
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.362170284876481,
            "RMSE": 6.736533340066285,
            "R2": 0.4127346685162743,
            "Memory in Mb": 0.5262050628662109,
            "Time in s": 1.543379
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.647894929983432,
            "RMSE": 7.008861526290804,
            "R2": 0.4889753297409128,
            "Memory in Mb": 0.5290126800537109,
            "Time in s": 1.82575
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.817744211127824,
            "RMSE": 7.136288548419971,
            "R2": 0.5728405597677722,
            "Memory in Mb": 0.5066156387329102,
            "Time in s": 2.145522
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.867036081233358,
            "RMSE": 7.152118590173611,
            "R2": 0.6487028411390494,
            "Memory in Mb": 0.4790925979614258,
            "Time in s": 2.491984
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 4.887061675652274,
            "RMSE": 7.15502256260352,
            "R2": 0.720333392468735,
            "Memory in Mb": 0.3514680862426758,
            "Time in s": 2.944156
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 5.070260383978678,
            "RMSE": 7.484020932149266,
            "R2": 0.7477619935177958,
            "Memory in Mb": 0.3277406692504883,
            "Time in s": 3.412471
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 5.671227628293087,
            "RMSE": 8.602358503958763,
            "R2": 0.7082361492582977,
            "Memory in Mb": 0.3353548049926758,
            "Time in s": 3.897275
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 5.872335352103937,
            "RMSE": 8.83175934179542,
            "R2": 0.7369479677711775,
            "Memory in Mb": 0.372288703918457,
            "Time in s": 4.389179
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 6.107145463120707,
            "RMSE": 9.222510821361375,
            "R2": 0.769191114739663,
            "Memory in Mb": 0.3991250991821289,
            "Time in s": 4.889463
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 6.19844823305091,
            "RMSE": 9.33633324769997,
            "R2": 0.7945607849348244,
            "Memory in Mb": 0.4207086563110351,
            "Time in s": 5.506109
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 6.823605404288741,
            "RMSE": 10.586090935492884,
            "R2": 0.758682880699561,
            "Memory in Mb": 0.4333581924438476,
            "Time in s": 6.131382
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 7.289576170484155,
            "RMSE": 11.670233638164651,
            "R2": 0.7419337665758028,
            "Memory in Mb": 0.4418039321899414,
            "Time in s": 6.777342
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 7.579012857443305,
            "RMSE": 12.145524073459754,
            "R2": 0.75790700185782,
            "Memory in Mb": 0.4508142471313476,
            "Time in s": 7.439278
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 7.564986803201262,
            "RMSE": 12.135208564512553,
            "R2": 0.7903915740986345,
            "Memory in Mb": 0.4540948867797851,
            "Time in s": 8.115354
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 8.103353916061925,
            "RMSE": 13.02855032884451,
            "R2": 0.7848217554522041,
            "Memory in Mb": 0.4577798843383789,
            "Time in s": 8.913327
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 9.2182891996096,
            "RMSE": 15.75502466975724,
            "R2": 0.7144552709875674,
            "Memory in Mb": 0.4609994888305664,
            "Time in s": 9.721339
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 9.685083231372472,
            "RMSE": 16.400765556025647,
            "R2": 0.7351946818510116,
            "Memory in Mb": 0.4719209671020508,
            "Time in s": 10.546217
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 9.903299441393282,
            "RMSE": 16.527032528363478,
            "R2": 0.759214288686034,
            "Memory in Mb": 0.477086067199707,
            "Time in s": 11.387382
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 10.047801743751696,
            "RMSE": 16.62843798311862,
            "R2": 0.778421004008311,
            "Memory in Mb": 0.4848833084106445,
            "Time in s": 12.279877
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 10.963674059851892,
            "RMSE": 18.110346084278056,
            "R2": 0.7447765461541069,
            "Memory in Mb": 0.4873552322387695,
            "Time in s": 13.19145
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 11.492835005144466,
            "RMSE": 19.28081121430548,
            "R2": 0.7340717056357994,
            "Memory in Mb": 0.4739046096801758,
            "Time in s": 14.120497000000002
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 11.898657720927194,
            "RMSE": 19.94321338535613,
            "R2": 0.7482768269892894,
            "Memory in Mb": 0.4488801956176758,
            "Time in s": 15.069160000000002
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 12.0617729851989,
            "RMSE": 19.965773188137263,
            "R2": 0.7647640178574115,
            "Memory in Mb": 0.4161386489868164,
            "Time in s": 16.114715
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 12.97304553348899,
            "RMSE": 21.57136186484404,
            "R2": 0.7447607843499935,
            "Memory in Mb": 0.4060754776000976,
            "Time in s": 17.182106
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 13.747411939847144,
            "RMSE": 23.06575414024212,
            "R2": 0.7260576137332548,
            "Memory in Mb": 0.4295892715454101,
            "Time in s": 18.259955
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 14.305030376306712,
            "RMSE": 23.986335540211613,
            "R2": 0.7367482003695625,
            "Memory in Mb": 0.4628152847290039,
            "Time in s": 19.347052
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 14.526268288674354,
            "RMSE": 24.074522605416067,
            "R2": 0.7535790611891788,
            "Memory in Mb": 0.4899911880493164,
            "Time in s": 20.478651000000003
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 15.027594657922048,
            "RMSE": 24.671918598232004,
            "R2": 0.7521995995009789,
            "Memory in Mb": 0.5175485610961914,
            "Time in s": 21.623166
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 16.208274238827823,
            "RMSE": 27.03842360672758,
            "R2": 0.7204560380476568,
            "Memory in Mb": 0.5713090896606445,
            "Time in s": 22.784126
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 16.99589357541462,
            "RMSE": 28.364120175265192,
            "R2": 0.7283636722963454,
            "Memory in Mb": 0.5903940200805664,
            "Time in s": 23.973479
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 17.304815327407063,
            "RMSE": 28.547476213614512,
            "R2": 0.739918935022724,
            "Memory in Mb": 0.6084756851196289,
            "Time in s": 25.225522
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 17.747173803776352,
            "RMSE": 29.064129392830434,
            "R2": 0.7464079684248853,
            "Memory in Mb": 0.6325922012329102,
            "Time in s": 26.517497
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 18.655435380807354,
            "RMSE": 30.57773482627066,
            "R2": 0.7274654471662664,
            "Memory in Mb": 0.6401453018188477,
            "Time in s": 27.826703
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 19.38212758204995,
            "RMSE": 31.56694275275528,
            "R2": 0.7259045847606268,
            "Memory in Mb": 0.5900964736938477,
            "Time in s": 29.161388
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 20.16255538075237,
            "RMSE": 32.73116726334994,
            "R2": 0.7350525453098611,
            "Memory in Mb": 0.6013956069946289,
            "Time in s": 30.57764
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 20.34377517847412,
            "RMSE": 32.75647044736101,
            "R2": 0.7456003073902285,
            "Memory in Mb": 0.6148271560668945,
            "Time in s": 32.006392000000005
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 21.397093652240404,
            "RMSE": 34.43808497807088,
            "R2": 0.7274757471078548,
            "Memory in Mb": 0.6217546463012695,
            "Time in s": 33.45442800000001
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 22.130535392790676,
            "RMSE": 35.39551310036421,
            "R2": 0.7247017706467436,
            "Memory in Mb": 0.6181917190551758,
            "Time in s": 34.916661000000005
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 22.97609679727041,
            "RMSE": 36.53926451086616,
            "R2": 0.7286255260499503,
            "Memory in Mb": 0.6243486404418945,
            "Time in s": 36.463466
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "ChickWeights",
            "MAE": 23.114298050830318,
            "RMSE": 36.631109645590286,
            "R2": 0.7338934315030725,
            "Memory in Mb": 0.6280336380004883,
            "Time in s": 38.020312
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 6.57361785669815,
            "RMSE": 13.877675781396096,
            "R2": -450.7393063082519,
            "Memory in Mb": 0.3875865936279297,
            "Time in s": 0.030628
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 4.357601810962072,
            "RMSE": 9.93598927447802,
            "R2": -38.690592530050864,
            "Memory in Mb": 0.5688495635986328,
            "Time in s": 0.093522
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 3.120546196671925,
            "RMSE": 8.124382016407804,
            "R2": -34.775930157070896,
            "Memory in Mb": 0.6946392059326172,
            "Time in s": 0.180013
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.5823668216656817,
            "RMSE": 7.068571931029129,
            "R2": -26.16547256881584,
            "Memory in Mb": 0.7988948822021484,
            "Time in s": 0.365225
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.6103510398716643,
            "RMSE": 6.439797187103485,
            "R2": -13.147122820254191,
            "Memory in Mb": 0.9021625518798828,
            "Time in s": 0.589181
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.5653436103516496,
            "RMSE": 5.96335184363353,
            "R2": -9.29140495411716,
            "Memory in Mb": 0.9421710968017578,
            "Time in s": 0.842127
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.4314692166818666,
            "RMSE": 5.556159680491977,
            "R2": -8.232140838080387,
            "Memory in Mb": 0.9627094268798828,
            "Time in s": 1.43468
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.270493582871441,
            "RMSE": 5.217534738727647,
            "R2": -6.179445803611509,
            "Memory in Mb": 1.0016803741455078,
            "Time in s": 2.055929
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.1841879014169865,
            "RMSE": 4.9594120506005,
            "R2": -4.6969569828406526,
            "Memory in Mb": 0.9622507095336914,
            "Time in s": 2.757735
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 2.030794616399332,
            "RMSE": 4.7110231793054895,
            "R2": -4.155876544063708,
            "Memory in Mb": 0.5397500991821289,
            "Time in s": 3.551711
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.922882727301643,
            "RMSE": 4.50300441964265,
            "R2": -4.081371242371108,
            "Memory in Mb": 0.3774957656860351,
            "Time in s": 4.407055
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.8390508968191757,
            "RMSE": 4.321014818317665,
            "R2": -3.714147473566389,
            "Memory in Mb": 0.4312639236450195,
            "Time in s": 5.281937999999999
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.7379678526387643,
            "RMSE": 4.155226166492631,
            "R2": -3.4180849750109363,
            "Memory in Mb": 0.4941263198852539,
            "Time in s": 6.197258999999999
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.7042826877160742,
            "RMSE": 4.0269186303191065,
            "R2": -3.3444224917120184,
            "Memory in Mb": 0.5997896194458008,
            "Time in s": 7.197467999999999
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.6796571065333832,
            "RMSE": 3.9174008876388,
            "R2": -3.043265693703045,
            "Memory in Mb": 0.6906900405883789,
            "Time in s": 8.219126999999999
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.5891460162001485,
            "RMSE": 3.793680488164568,
            "R2": -2.979662055693274,
            "Memory in Mb": 0.757817268371582,
            "Time in s": 9.288978999999998
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.5335884019062007,
            "RMSE": 3.685003453386448,
            "R2": -2.968029890458662,
            "Memory in Mb": 0.7969903945922852,
            "Time in s": 10.383406999999998
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.54418408246079,
            "RMSE": 3.606838798974545,
            "R2": -2.832696164635261,
            "Memory in Mb": 0.8751077651977539,
            "Time in s": 11.515104999999998
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.5054402320411853,
            "RMSE": 3.517798427376237,
            "R2": -2.771919367898169,
            "Memory in Mb": 0.9264421463012696,
            "Time in s": 12.700466999999998
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.4723491084260332,
            "RMSE": 3.435525460733128,
            "R2": -2.699225318590951,
            "Memory in Mb": 0.9911317825317384,
            "Time in s": 13.924277999999996
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.429579158986208,
            "RMSE": 3.3562143901072865,
            "R2": -2.6472359354971333,
            "Memory in Mb": 0.9703760147094728,
            "Time in s": 15.190464999999998
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.3992424504019558,
            "RMSE": 3.2853835752695946,
            "R2": -2.431676192315116,
            "Memory in Mb": 1.0316247940063477,
            "Time in s": 16.527614999999997
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.365864594828797,
            "RMSE": 3.217129802398014,
            "R2": -2.120443637805541,
            "Memory in Mb": 1.1097803115844729,
            "Time in s": 17.906522
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.3301487592579586,
            "RMSE": 3.151695763852486,
            "R2": -1.9259010739386908,
            "Memory in Mb": 1.1814966201782229,
            "Time in s": 19.341224
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.2968821746115176,
            "RMSE": 3.0904885141585767,
            "R2": -1.7543370405557224,
            "Memory in Mb": 1.2276010513305664,
            "Time in s": 20.84359
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.2678501702074907,
            "RMSE": 3.0331483120333496,
            "R2": -1.657710331787236,
            "Memory in Mb": 1.2783823013305664,
            "Time in s": 22.421223
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.2343399552126226,
            "RMSE": 2.9775564396478966,
            "R2": -1.551795811786203,
            "Memory in Mb": 1.2796869277954102,
            "Time in s": 24.086658
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.220715255826944,
            "RMSE": 2.9300367331798807,
            "R2": -1.5298738258017646,
            "Memory in Mb": 1.2170305252075195,
            "Time in s": 25.790581
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.1924146311245054,
            "RMSE": 2.8809984439523286,
            "R2": -1.506393751525562,
            "Memory in Mb": 1.0756006240844729,
            "Time in s": 27.649708999999994
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.1793821598427467,
            "RMSE": 2.837096711415006,
            "R2": -1.4037015974174163,
            "Memory in Mb": 0.9519128799438475,
            "Time in s": 29.574727
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.1645342598465298,
            "RMSE": 2.79612287562216,
            "R2": -1.2991852345603885,
            "Memory in Mb": 0.9679117202758788,
            "Time in s": 31.579398
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.1398425529628198,
            "RMSE": 2.753175690936408,
            "R2": -1.1874325743915652,
            "Memory in Mb": 0.936314582824707,
            "Time in s": 33.628169
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.1198821044801988,
            "RMSE": 2.7133180185933967,
            "R2": -1.1092797015680484,
            "Memory in Mb": 0.9601030349731444,
            "Time in s": 35.724068
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.103543375947734,
            "RMSE": 2.675681585437618,
            "R2": -1.0835838801311364,
            "Memory in Mb": 1.0132951736450195,
            "Time in s": 37.850435
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.0951788603095205,
            "RMSE": 2.643674463536044,
            "R2": -1.0874567422761272,
            "Memory in Mb": 1.0955934524536133,
            "Time in s": 40.041881
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.073603439060177,
            "RMSE": 2.607328103868497,
            "R2": -1.075061768905586,
            "Memory in Mb": 1.1506471633911133,
            "Time in s": 42.267731000000005
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.052216298294681,
            "RMSE": 2.5725220480150237,
            "R2": -1.0188151031858663,
            "Memory in Mb": 1.1900300979614258,
            "Time in s": 44.534549000000005
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.0329729065757678,
            "RMSE": 2.539265324444459,
            "R2": -0.9882648176410448,
            "Memory in Mb": 1.2228517532348633,
            "Time in s": 46.85075200000001
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.015201035443157,
            "RMSE": 2.5074934380267417,
            "R2": -0.9475063222432678,
            "Memory in Mb": 1.2825212478637695,
            "Time in s": 49.22632000000001
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.007374170791078,
            "RMSE": 2.4793027589713232,
            "R2": -0.9211818120686948,
            "Memory in Mb": 1.3126497268676758,
            "Time in s": 51.66223500000001
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 1.002386830132377,
            "RMSE": 2.4547936379778226,
            "R2": -0.9040692252875042,
            "Memory in Mb": 1.3594255447387695,
            "Time in s": 54.13772100000001
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9929186057762196,
            "RMSE": 2.428247138481691,
            "R2": -0.8804076589484491,
            "Memory in Mb": 1.397130012512207,
            "Time in s": 56.66204300000001
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9756374748391698,
            "RMSE": 2.400488599154532,
            "R2": -0.8344958433267429,
            "Memory in Mb": 1.4288606643676758,
            "Time in s": 59.23948900000001
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.964181960731443,
            "RMSE": 2.37450147105602,
            "R2": -0.7860721035239808,
            "Memory in Mb": 1.4496355056762695,
            "Time in s": 61.87688900000001
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9549728240782616,
            "RMSE": 2.3497625798451978,
            "R2": -0.7564202624419067,
            "Memory in Mb": 1.3498811721801758,
            "Time in s": 64.59788000000002
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9412862327577896,
            "RMSE": 2.3247867434211136,
            "R2": -0.747529388757789,
            "Memory in Mb": 1.1945161819458008,
            "Time in s": 67.39612200000002
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.934469347520636,
            "RMSE": 2.302477656767798,
            "R2": -0.7286928787152502,
            "Memory in Mb": 1.2202577590942385,
            "Time in s": 70.24630900000002
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9259837543593707,
            "RMSE": 2.280476047701142,
            "R2": -0.7135440601163805,
            "Memory in Mb": 1.2635469436645508,
            "Time in s": 73.13750900000002
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9196316545824528,
            "RMSE": 2.2597103614150886,
            "R2": -0.715155968132227,
            "Memory in Mb": 1.2794008255004885,
            "Time in s": 76.07904100000002
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9087747756519629,
            "RMSE": 2.2382775608394114,
            "R2": -0.7111012811273396,
            "Memory in Mb": 1.3157854080200195,
            "Time in s": 79.06112300000002
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Bagging",
            "dataset": "TrumpApproval",
            "MAE": 0.9082029688272106,
            "RMSE": 2.2371845268363217,
            "R2": -0.710571805505718,
            "Memory in Mb": 1.3157854080200195,
            "Time in s": 82.06893700000002
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 41.63636363636363,
            "RMSE": 41.64569169030137,
            "R2": -2231.5319148936137,
            "Memory in Mb": 0.0652570724487304,
            "Time in s": 0.004749
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 41.31818181818181,
            "RMSE": 41.32960638133835,
            "R2": -1808.0547045951903,
            "Memory in Mb": 0.0776433944702148,
            "Time in s": 0.02229
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 41.12121212121212,
            "RMSE": 41.13871582091424,
            "R2": -1174.393494897962,
            "Memory in Mb": 0.0973310470581054,
            "Time in s": 0.042479
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 41.159090909090914,
            "RMSE": 41.17451771534076,
            "R2": -1333.7620984139928,
            "Memory in Mb": 0.1087598800659179,
            "Time in s": 0.065964
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 41.5090909090909,
            "RMSE": 41.57075020645253,
            "R2": -336.3506066081568,
            "Memory in Mb": 0.1316785812377929,
            "Time in s": 0.1143329999999999
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 42.681818181818166,
            "RMSE": 42.82080349691271,
            "R2": -153.29834830483878,
            "Memory in Mb": 0.1604146957397461,
            "Time in s": 0.1705729999999999
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 43.50649350649351,
            "RMSE": 43.70978671356627,
            "R2": -106.75487995129542,
            "Memory in Mb": 0.1825284957885742,
            "Time in s": 0.2318889999999999
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 44.21590909090909,
            "RMSE": 44.43649707984724,
            "R2": -99.97346126163,
            "Memory in Mb": 0.2035512924194336,
            "Time in s": 0.308411
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 45.05050505050505,
            "RMSE": 45.309262771858165,
            "R2": -86.8022342468144,
            "Memory in Mb": 0.2153043746948242,
            "Time in s": 0.393152
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 46.16363636363636,
            "RMSE": 46.52487115902242,
            "R2": -63.64797006437341,
            "Memory in Mb": 0.2280874252319336,
            "Time in s": 0.484559
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 47.21487603305785,
            "RMSE": 47.67304278378361,
            "R2": -51.27707184490422,
            "Memory in Mb": 0.2377805709838867,
            "Time in s": 0.583103
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 48.29545454545455,
            "RMSE": 48.843054157105485,
            "R2": -43.84882422437649,
            "Memory in Mb": 0.2479772567749023,
            "Time in s": 0.792791
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 49.44055944055945,
            "RMSE": 50.100318941519305,
            "R2": -37.220279564063546,
            "Memory in Mb": 0.2207241058349609,
            "Time in s": 1.018133
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 50.532467532467535,
            "RMSE": 51.29137544271156,
            "R2": -33.04474826644667,
            "Memory in Mb": 0.2406787872314453,
            "Time in s": 1.254223
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 51.690909090909095,
            "RMSE": 52.61253451297311,
            "R2": -27.795548438273773,
            "Memory in Mb": 0.2568111419677734,
            "Time in s": 1.5160939999999998
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 53.00568181818182,
            "RMSE": 54.11860921749895,
            "R2": -23.566226925646237,
            "Memory in Mb": 0.2727985382080078,
            "Time in s": 1.7876089999999998
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 54.41176470588235,
            "RMSE": 55.733754017636336,
            "R2": -20.33250305682894,
            "Memory in Mb": 0.2873516082763672,
            "Time in s": 2.079546
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 56.02525252525252,
            "RMSE": 57.635786091488654,
            "R2": -17.146924852486976,
            "Memory in Mb": 0.300180435180664,
            "Time in s": 2.3857599999999994
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 57.5645933014354,
            "RMSE": 59.46206220864915,
            "R2": -14.922837840066968,
            "Memory in Mb": 0.2762508392333984,
            "Time in s": 2.7086299999999994
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 58.69090909090908,
            "RMSE": 60.81327606250582,
            "R2": -13.581197962556498,
            "Memory in Mb": 0.2926349639892578,
            "Time in s": 3.0480419999999997
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 60.25541125541125,
            "RMSE": 62.66764529032318,
            "R2": -12.244451024360147,
            "Memory in Mb": 0.3073635101318359,
            "Time in s": 3.437715999999999
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 62.17355371900826,
            "RMSE": 65.06963847478845,
            "R2": -10.489760184397111,
            "Memory in Mb": 0.3215885162353515,
            "Time in s": 3.8493299999999993
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 63.93675889328063,
            "RMSE": 67.17295239601157,
            "R2": -9.634560128382748,
            "Memory in Mb": 0.3348064422607422,
            "Time in s": 4.393024
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 65.10606060606062,
            "RMSE": 68.57980310513724,
            "R2": -9.127665748505592,
            "Memory in Mb": 0.3451099395751953,
            "Time in s": 4.977281
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 66.61454545454548,
            "RMSE": 70.46451073219248,
            "R2": -8.408339126213217,
            "Memory in Mb": 0.3548030853271484,
            "Time in s": 5.586244
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 68.48951048951052,
            "RMSE": 72.8020594498525,
            "R2": -7.6983532427125105,
            "Memory in Mb": 0.3655261993408203,
            "Time in s": 6.228505
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 70.55218855218858,
            "RMSE": 75.3669362796119,
            "R2": -7.08492451355157,
            "Memory in Mb": 0.3711223602294922,
            "Time in s": 6.899176000000001
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 72.39285714285718,
            "RMSE": 77.65033596401675,
            "R2": -6.643510181414674,
            "Memory in Mb": 0.3809375762939453,
            "Time in s": 7.597348
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 73.45454545454551,
            "RMSE": 79.15086186624424,
            "R2": -6.206879640065647,
            "Memory in Mb": 0.3927364349365234,
            "Time in s": 8.345726
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 75.77878787878792,
            "RMSE": 82.20832738177494,
            "R2": -5.653192449779911,
            "Memory in Mb": 0.4039859771728515,
            "Time in s": 9.225203
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 77.92375366568919,
            "RMSE": 84.89106353805269,
            "R2": -5.352795814687307,
            "Memory in Mb": 0.4136791229248047,
            "Time in s": 10.124705
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 80.04545454545458,
            "RMSE": 87.49376601169416,
            "R2": -5.134510311668016,
            "Memory in Mb": 0.4233722686767578,
            "Time in s": 11.048248
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 80.99724517906337,
            "RMSE": 88.57562798692558,
            "R2": -5.105139086016474,
            "Memory in Mb": 0.4330654144287109,
            "Time in s": 11.989622
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 82.77807486631018,
            "RMSE": 90.83029071422122,
            "R2": -4.901675845817959,
            "Memory in Mb": 0.4524784088134765,
            "Time in s": 12.967698
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 85.1766233766234,
            "RMSE": 93.99517810235533,
            "R2": -4.591702735915359,
            "Memory in Mb": 0.4681224822998047,
            "Time in s": 14.032748
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 87.26767676767678,
            "RMSE": 96.48964983485284,
            "R2": -4.494054297851511,
            "Memory in Mb": 0.484659194946289,
            "Time in s": 15.12168
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 89.00737100737103,
            "RMSE": 98.71879502607636,
            "R2": -4.345544683073043,
            "Memory in Mb": 0.4991130828857422,
            "Time in s": 16.236767999999998
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 90.57416267942588,
            "RMSE": 100.72635724110243,
            "R2": -4.224084264201084,
            "Memory in Mb": 0.5109386444091797,
            "Time in s": 17.416859999999996
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 93.12121212121215,
            "RMSE": 104.19735398794236,
            "R2": -3.967717840349581,
            "Memory in Mb": 0.5206584930419922,
            "Time in s": 18.643557999999995
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 95.41818181818184,
            "RMSE": 107.03565676064125,
            "R2": -3.8710119659250095,
            "Memory in Mb": 0.5303516387939453,
            "Time in s": 19.910713999999995
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 97.16629711751663,
            "RMSE": 109.07665280092142,
            "R2": -3.843505105397095,
            "Memory in Mb": 0.5280742645263672,
            "Time in s": 21.225085999999997
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 98.71645021645024,
            "RMSE": 111.1763643167196,
            "R2": -3.72620239405422,
            "Memory in Mb": 0.5443019866943359,
            "Time in s": 22.607732999999996
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 101.54122621564484,
            "RMSE": 115.2058457378686,
            "R2": -3.48124047566686,
            "Memory in Mb": 0.5577869415283203,
            "Time in s": 24.015635999999997
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 103.77066115702482,
            "RMSE": 117.90601559037044,
            "R2": -3.4365483842712585,
            "Memory in Mb": 0.5712184906005859,
            "Time in s": 25.474227999999997
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 106.02424242424244,
            "RMSE": 120.71525892518191,
            "R2": -3.37467008920777,
            "Memory in Mb": 0.5825443267822266,
            "Time in s": 26.96779499999999
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 107.31620553359684,
            "RMSE": 122.26004165941237,
            "R2": -3.356924458603192,
            "Memory in Mb": 2.7805843353271484,
            "Time in s": 30.43480299999999
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 109.39651837524178,
            "RMSE": 124.91233289427784,
            "R2": -3.291877964737682,
            "Memory in Mb": 2.825040817260742,
            "Time in s": 33.93932499999999
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 112.36553030303028,
            "RMSE": 129.1106745698386,
            "R2": -3.1225038051323804,
            "Memory in Mb": 2.876035690307617,
            "Time in s": 37.48648499999999
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 114.52504638218922,
            "RMSE": 131.65752925403248,
            "R2": -3.109734667916423,
            "Memory in Mb": 2.927671432495117,
            "Time in s": 41.07985699999999
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 115.89999999999996,
            "RMSE": 133.35909826820617,
            "R2": -3.0866973064470367,
            "Memory in Mb": 2.9773387908935547,
            "Time in s": 44.71417799999999
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 117.86452762923346,
            "RMSE": 135.8046463151548,
            "R2": -3.0526234314410727,
            "Memory in Mb": 3.02082633972168,
            "Time in s": 48.39640499999999
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 120.54020979020974,
            "RMSE": 139.4624607986965,
            "R2": -2.953338846956928,
            "Memory in Mb": 3.065652847290039,
            "Time in s": 52.12007199999999
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "ChickWeights",
            "MAE": 121.81833910034597,
            "RMSE": 141.00422703423635,
            "R2": -2.942935834251463,
            "Memory in Mb": 3.092409133911133,
            "Time in s": 55.88513699999999
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 43.8732195,
            "RMSE": 43.87807788634269,
            "R2": -4514.954899312423,
            "Memory in Mb": 0.1445150375366211,
            "Time in s": 0.017697
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 42.4932955,
            "RMSE": 42.52255283421693,
            "R2": -725.9491167623446,
            "Memory in Mb": 0.2117376327514648,
            "Time in s": 0.059669
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 42.2167785,
            "RMSE": 42.2386240157387,
            "R2": -966.0073736019044,
            "Memory in Mb": 0.2583265304565429,
            "Time in s": 0.116093
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 41.975705625,
            "RMSE": 41.99760868559829,
            "R2": -957.9655948743646,
            "Memory in Mb": 0.3003568649291992,
            "Time in s": 0.194541
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 41.37550450000001,
            "RMSE": 41.410913785433536,
            "R2": -583.9966399141301,
            "Memory in Mb": 0.3407926559448242,
            "Time in s": 0.295523
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.936110000000006,
            "RMSE": 40.97829382197767,
            "R2": -484.9611418859003,
            "Memory in Mb": 0.3709287643432617,
            "Time in s": 0.510712
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.6885472857143,
            "RMSE": 40.72961738075088,
            "R2": -495.1050461477588,
            "Memory in Mb": 0.3974485397338867,
            "Time in s": 0.760252
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.35105437500001,
            "RMSE": 40.39801158334292,
            "R2": -429.4078677932073,
            "Memory in Mb": 0.3402233123779297,
            "Time in s": 1.044132
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.00981655555555,
            "RMSE": 40.06373388340122,
            "R2": -370.7794659133543,
            "Memory in Mb": 0.3811016082763672,
            "Time in s": 1.367502
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.80633095,
            "RMSE": 39.860362966711,
            "R2": -368.1089073295326,
            "Memory in Mb": 0.3127880096435547,
            "Time in s": 1.794637
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.727043136363626,
            "RMSE": 39.77723500009918,
            "R2": -395.5019807293188,
            "Memory in Mb": 0.3578624725341797,
            "Time in s": 2.266575
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.56323079166665,
            "RMSE": 39.61325406766278,
            "R2": -395.19837684116754,
            "Memory in Mb": 0.3875255584716797,
            "Time in s": 2.775551
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.42014538461535,
            "RMSE": 39.46968290441584,
            "R2": -397.63185900832246,
            "Memory in Mb": 0.420846939086914,
            "Time in s": 3.358614
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.33200189285712,
            "RMSE": 39.37942345737111,
            "R2": -414.4560159350036,
            "Memory in Mb": 0.4701480865478515,
            "Time in s": 4.097303
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.18435719999999,
            "RMSE": 39.23275803924839,
            "R2": -404.5402138221895,
            "Memory in Mb": 0.5117359161376953,
            "Time in s": 4.882924
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.13568690624999,
            "RMSE": 39.1818628962716,
            "R2": -423.5167725219512,
            "Memory in Mb": 0.5480670928955078,
            "Time in s": 5.740529
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.14620944117645,
            "RMSE": 39.18989510023786,
            "R2": -447.7943063391533,
            "Memory in Mb": 0.5615406036376953,
            "Time in s": 6.72918
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.24072974999997,
            "RMSE": 39.28395553300239,
            "R2": -453.6543473793619,
            "Memory in Mb": 0.5990085601806641,
            "Time in s": 7.76074
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.29597665789471,
            "RMSE": 39.33769921546023,
            "R2": -470.6701690846498,
            "Memory in Mb": 0.6312580108642578,
            "Time in s": 8.924786000000001
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.35730624999997,
            "RMSE": 39.39781946688104,
            "R2": -485.4842825426507,
            "Memory in Mb": 0.6682605743408203,
            "Time in s": 10.154856
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.40549083333331,
            "RMSE": 39.44465897881697,
            "R2": -502.7799504226928,
            "Memory in Mb": 0.6983966827392578,
            "Time in s": 11.469727
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.49730674999998,
            "RMSE": 39.53710368662846,
            "R2": -495.9856416828035,
            "Memory in Mb": 0.7316226959228516,
            "Time in s": 12.901862
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.61474728260867,
            "RMSE": 39.65658853240579,
            "R2": -473.14358309219216,
            "Memory in Mb": 0.7705020904541016,
            "Time in s": 14.448849
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.71032456249997,
            "RMSE": 39.75304758270976,
            "R2": -464.4916761787406,
            "Memory in Mb": 0.8079357147216797,
            "Time in s": 16.094285
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.80313951999997,
            "RMSE": 39.84667590965187,
            "R2": -456.8750824508669,
            "Memory in Mb": 2.9298267364501958,
            "Time in s": 19.825027
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.87354713461536,
            "RMSE": 39.916931033645376,
            "R2": -459.2932847271911,
            "Memory in Mb": 3.0076160430908203,
            "Time in s": 23.629967
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.94649651851849,
            "RMSE": 39.98996046818772,
            "R2": -459.28610565666287,
            "Memory in Mb": 3.105920791625977,
            "Time in s": 27.509295
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 39.97606614285712,
            "RMSE": 40.018487723609816,
            "R2": -470.926187706672,
            "Memory in Mb": 3.203706741333008,
            "Time in s": 31.453258
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.00338510344825,
            "RMSE": 40.044755101652726,
            "R2": -483.2331705341176,
            "Memory in Mb": 3.296670913696289,
            "Time in s": 35.460995000000004
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.07393431666663,
            "RMSE": 40.11569326301364,
            "R2": -479.5746686678817,
            "Memory in Mb": 3.391347885131836,
            "Time in s": 39.544454
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.1459417741935,
            "RMSE": 40.18827077358568,
            "R2": -473.96334667177865,
            "Memory in Mb": 3.4906063079833984,
            "Time in s": 43.697410000000005
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.21943815624997,
            "RMSE": 40.26249426545423,
            "R2": -466.8085709746123,
            "Memory in Mb": 3.5870800018310547,
            "Time in s": 47.92464
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.28296777272724,
            "RMSE": 40.32626722721455,
            "R2": -464.9172853497744,
            "Memory in Mb": 3.686498641967773,
            "Time in s": 52.218165000000006
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.31998279411761,
            "RMSE": 40.36256991107017,
            "R2": -473.1325264408024,
            "Memory in Mb": 3.782560348510742,
            "Time in s": 56.58359200000001
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.31359012857138,
            "RMSE": 40.35509446667054,
            "R2": -485.40526703956544,
            "Memory in Mb": 3.816682815551758,
            "Time in s": 61.02307200000001
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.31730695833329,
            "RMSE": 40.357915759594896,
            "R2": -496.1610725544049,
            "Memory in Mb": 3.917215347290039,
            "Time in s": 65.52718500000002
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.36653568918915,
            "RMSE": 40.40711941642496,
            "R2": -497.0742803710164,
            "Memory in Mb": 4.021100997924805,
            "Time in s": 70.10250300000001
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.40314367105261,
            "RMSE": 40.443256311482514,
            "R2": -503.3712175162706,
            "Memory in Mb": 4.113973617553711,
            "Time in s": 74.743136
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.44545064102563,
            "RMSE": 40.48534274444009,
            "R2": -506.6856716110208,
            "Memory in Mb": 4.221334457397461,
            "Time in s": 79.45160200000001
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.47854825,
            "RMSE": 40.518050685964006,
            "R2": -512.1052117095793,
            "Memory in Mb": 4.33137321472168,
            "Time in s": 84.22367000000001
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.50894034146341,
            "RMSE": 40.5479845946661,
            "R2": -518.5068774177179,
            "Memory in Mb": 4.393171310424805,
            "Time in s": 89.06994900000001
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.5406558690476,
            "RMSE": 40.57931089736599,
            "R2": -524.140575335229,
            "Memory in Mb": 4.501546859741211,
            "Time in s": 93.986539
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.58371181395347,
            "RMSE": 40.62239247493601,
            "R2": -524.3496319016275,
            "Memory in Mb": 4.600507736206055,
            "Time in s": 98.97766
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.62855514772725,
            "RMSE": 40.66738601007716,
            "R2": -522.897851512946,
            "Memory in Mb": 4.697576522827148,
            "Time in s": 104.03937600000002
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.664104233333326,
            "RMSE": 40.702738445808535,
            "R2": -526.020768835918,
            "Memory in Mb": 4.774164199829102,
            "Time in s": 109.17863200000002
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.68274704347825,
            "RMSE": 40.72073961991632,
            "R2": -535.1540147256861,
            "Memory in Mb": 4.872934341430664,
            "Time in s": 114.38942200000002
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.70972619148935,
            "RMSE": 40.74737437775791,
            "R2": -540.4099749760601,
            "Memory in Mb": 4.975519180297852,
            "Time in s": 119.67171900000002
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.73400636458332,
            "RMSE": 40.771242977826994,
            "R2": -546.7118652484228,
            "Memory in Mb": 5.07771110534668,
            "Time in s": 125.02115000000002
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.74031829795916,
            "RMSE": 40.77684015923968,
            "R2": -557.5026042066913,
            "Memory in Mb": 5.174932479858398,
            "Time in s": 130.44017000000002
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.75359492299998,
            "RMSE": 40.78950075300399,
            "R2": -567.2567645513548,
            "Memory in Mb": 5.274145126342773,
            "Time in s": 135.92720000000003
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "Exponentially Weighted Average",
            "dataset": "TrumpApproval",
            "MAE": 40.75458054545452,
            "RMSE": 40.7904615623717,
            "R2": -567.6629514867817,
            "Memory in Mb": 5.276128768920898,
            "Time in s": 141.45243100000002
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 41.63636363636363,
            "RMSE": 41.64569169030137,
            "R2": -2231.5319148936137,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.004659
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 41.31818181818181,
            "RMSE": 41.32960638133835,
            "R2": -1808.0547045951903,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.035685
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 41.12121212121212,
            "RMSE": 41.13871582091424,
            "R2": -1174.393494897962,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.0849989999999999
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 41.159090909090914,
            "RMSE": 41.17451771534076,
            "R2": -1333.7620984139928,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.154054
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 41.5090909090909,
            "RMSE": 41.57075020645253,
            "R2": -336.3506066081568,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.236038
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 42.681818181818166,
            "RMSE": 42.82080349691271,
            "R2": -153.29834830483878,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.334153
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 43.46421300395698,
            "RMSE": 43.66282826571568,
            "R2": -106.52347713504813,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.4453709999999999
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 43.359772412267546,
            "RMSE": 43.583709810639945,
            "R2": -96.13505707304522,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 0.810611
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 39.34760833403674,
            "RMSE": 41.28110871337288,
            "R2": -71.88434940071843,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 1.1795
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 36.27694842893514,
            "RMSE": 39.43109665219568,
            "R2": -45.43679588251114,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 1.551937
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 33.38449530211604,
            "RMSE": 37.62985177124845,
            "R2": -31.570957412576163,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 1.927681
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 30.760956861305427,
            "RMSE": 36.03410144813446,
            "R2": -23.41028390603237,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 2.306782
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 28.636527077105512,
            "RMSE": 34.63559483719005,
            "R2": -17.266619380249022,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 2.6893580000000004
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 26.848366395937333,
            "RMSE": 33.39569685051843,
            "R2": -13.432529594168455,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 3.0876050000000004
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 25.68994399106157,
            "RMSE": 32.40192925941153,
            "R2": -9.92165984317062,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 3.562508
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 24.410830110997512,
            "RMSE": 31.4363281477476,
            "R2": -7.289127728255313,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 4.041374
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 23.27797268834062,
            "RMSE": 30.533192270092133,
            "R2": -5.402500905628177,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 4.523515000000001
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 22.21718064008457,
            "RMSE": 29.702466677215767,
            "R2": -3.8195183008370286,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 5.01074
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.55319621821813,
            "RMSE": 29.08035323359505,
            "R2": -2.8083766468986493,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 5.506907
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.47717514737632,
            "RMSE": 28.87553300521557,
            "R2": -2.287429329651187,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 6.006767
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.952511346795177,
            "RMSE": 28.33784041981669,
            "R2": -1.7081998467380504,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 6.546588
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.676711476832995,
            "RMSE": 27.952207916118613,
            "R2": -1.120246781438643,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 7.091828
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.0995501155626,
            "RMSE": 27.40917062551413,
            "R2": -0.77060809797316,
            "Memory in Mb": 0.0121526718139648,
            "Time in s": 7.64039
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.480542447806847,
            "RMSE": 27.75611161124588,
            "R2": -0.6589532289622051,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 8.194426
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.614496901205563,
            "RMSE": 28.041519628611827,
            "R2": -0.4899619312470022,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 8.751968
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.565278129073285,
            "RMSE": 27.847512109279503,
            "R2": -0.2726896536826668,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 9.312993
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.274958424672484,
            "RMSE": 27.62568723918364,
            "R2": -0.0862766099689866,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 9.883614
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 20.45327995927562,
            "RMSE": 27.912230969749725,
            "R2": 0.0123677325099795,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 10.459328
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.51025107964545,
            "RMSE": 30.009813508826145,
            "R2": -0.0360067042108638,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 11.038549
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.665590739767385,
            "RMSE": 30.044848619277115,
            "R2": 0.1113341277332687,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 11.621241
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.89048226594194,
            "RMSE": 30.334415208142868,
            "R2": 0.1888294001405642,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 12.207835
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 21.89395295521016,
            "RMSE": 30.339570241246864,
            "R2": 0.2623598804373043,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 12.797939
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 22.90533819708786,
            "RMSE": 32.054250800509514,
            "R2": 0.2004634102060014,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 13.393067000000002
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 23.763742364378043,
            "RMSE": 33.85198840163,
            "R2": 0.1802483296948254,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 13.997035000000002
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 24.57154278807733,
            "RMSE": 34.76894700117602,
            "R2": 0.2349038768732488,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 14.642537000000004
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 24.36284577450351,
            "RMSE": 34.48838301267373,
            "R2": 0.2980969129506975,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 15.292230000000002
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 25.734101326034637,
            "RMSE": 37.062399123466015,
            "R2": 0.2465415113840201,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 15.945417000000004
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 27.11119186006235,
            "RMSE": 39.928390080533305,
            "R2": 0.1791051768225413,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 16.606412000000002
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 28.3590406143643,
            "RMSE": 42.09339312084405,
            "R2": 0.1892790232513257,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 17.270793
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 29.357663164641018,
            "RMSE": 43.68705243766196,
            "R2": 0.1885388580498291,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 17.938627
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 30.691095011752385,
            "RMSE": 45.67489043760892,
            "R2": 0.1507194354669618,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 18.61722
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 32.58469239048663,
            "RMSE": 49.95891321104316,
            "R2": 0.0456375461688204,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 19.304175
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 34.457204466549335,
            "RMSE": 53.83603157260298,
            "R2": 0.0214223438020899,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 19.9947
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 37.61656772325176,
            "RMSE": 59.47905507802133,
            "R2": -0.1290194303344141,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 20.688692000000003
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 39.835053793820734,
            "RMSE": 63.30264151550531,
            "R2": -0.2029972425035688,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 21.389042000000003
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 40.84375246428709,
            "RMSE": 64.75828138125749,
            "R2": -0.2223668969879733,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 22.096762
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 42.3259867290128,
            "RMSE": 66.7403629812066,
            "R2": -0.2252193711452539,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 22.959028000000004
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 43.90376331145991,
            "RMSE": 69.27444073484561,
            "R2": -0.1868144391113539,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 23.825387000000003
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 45.11725117254523,
            "RMSE": 70.97054614693485,
            "R2": -0.1942044281482897,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 24.695185
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 46.19146939493793,
            "RMSE": 72.84904016514736,
            "R2": -0.2194804408254527,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 25.570022
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 48.0255382358928,
            "RMSE": 75.55118081102547,
            "R2": -0.2542655857337756,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 26.453531
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 49.60861685612801,
            "RMSE": 77.95895414232838,
            "R2": -0.2353254830584423,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 27.340524
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "ChickWeights",
            "MAE": 51.40782550111089,
            "RMSE": 80.92025038917566,
            "R2": -0.298583502299673,
            "Memory in Mb": 0.012312889099121,
            "Time in s": 28.229463000000003
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 28.203089584036217,
            "RMSE": 31.678254793976468,
            "R2": -2352.839799462937,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.018592
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 17.631407237579232,
            "RMSE": 23.536801219235823,
            "R2": -221.7205207554288,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.0539339999999999
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 13.441671937224772,
            "RMSE": 19.739075566761823,
            "R2": -210.18539534147197,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.098078
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 11.19674929006134,
            "RMSE": 17.292913087737123,
            "R2": -161.5886474703317,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.159515
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 9.529407951935296,
            "RMSE": 15.54264880746251,
            "R2": -81.40884208187767,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.228076
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 8.478754286735066,
            "RMSE": 14.272499783288554,
            "R2": -57.95136830581733,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.332328
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 7.525552058981039,
            "RMSE": 13.242333407520348,
            "R2": -51.44233495767236,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.527456
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 6.729532853932534,
            "RMSE": 12.401843141618142,
            "R2": -39.56324503441056,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.7296090000000001
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 6.20494414148211,
            "RMSE": 11.727398222866162,
            "R2": -30.855608065765253,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 0.938725
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 5.707613016041334,
            "RMSE": 11.135875265707485,
            "R2": -27.80850643367628,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 1.173453
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 5.35235544657082,
            "RMSE": 10.636236352263047,
            "R2": -27.34993958822678,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 1.423387
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 4.997211310189409,
            "RMSE": 10.191758203807838,
            "R2": -25.22586832784644,
            "Memory in Mb": 0.0131101608276367,
            "Time in s": 1.696442
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 4.698339965696975,
            "RMSE": 9.799142308635478,
            "R2": -23.570888426665658,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 2.044166
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 4.429952698677103,
            "RMSE": 9.448184269747657,
            "R2": -22.91569767610472,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 2.398587
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 4.185436867704573,
            "RMSE": 9.131292683908228,
            "R2": -20.968518634865895,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 2.759636
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.989857840855361,
            "RMSE": 8.848493522992882,
            "R2": -20.65027251080777,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 3.127609
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.793510888989401,
            "RMSE": 8.58729864958044,
            "R2": -20.548263158423392,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 3.5072970000000003
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.624008920532304,
            "RMSE": 8.350732680595982,
            "R2": -19.54471351213204,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 3.994133
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.4723941591948395,
            "RMSE": 8.130732570333006,
            "R2": -19.15022282865096,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 4.488831
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.327129028584169,
            "RMSE": 7.926491124989248,
            "R2": -18.69184448676573,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 4.996594
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.1988914312464622,
            "RMSE": 7.737168953530663,
            "R2": -18.383340677896445,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 5.512642
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 3.090541865220404,
            "RMSE": 7.562941397323993,
            "R2": -17.185096454486196,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 6.041213
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.9841087219087,
            "RMSE": 7.398658950448711,
            "R2": -15.50384711789857,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 6.671723
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.878027938067315,
            "RMSE": 7.243616567021465,
            "R2": -14.455461195017085,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 7.311147
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.790174040420949,
            "RMSE": 7.099353406661882,
            "R2": -13.534510391092628,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 7.962598
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.702735665583147,
            "RMSE": 6.962851553400364,
            "R2": -13.005371203657658,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 8.621042
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.619923274637493,
            "RMSE": 6.8334980874356335,
            "R2": -12.440396167539378,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 9.286046
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.556848015725479,
            "RMSE": 6.714676061099242,
            "R2": -12.286263553450382,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 9.968405999999998
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.4920466556079988,
            "RMSE": 6.599727625727584,
            "R2": -12.1527109643015,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 10.662936999999998
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.4260558633236777,
            "RMSE": 6.490118235625791,
            "R2": -11.578750092830704,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 11.381531999999998
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.3708694907142864,
            "RMSE": 6.387338726311831,
            "R2": -10.997792654674662,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 12.131809999999998
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.309077397643504,
            "RMSE": 6.287531812954472,
            "R2": -10.40846497658843,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 12.902857999999998
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.253417256192923,
            "RMSE": 6.192441467899733,
            "R2": -9.986430076809746,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 13.765244
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.1933714736526424,
            "RMSE": 6.100884478116631,
            "R2": -9.832475924452435,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 14.638727
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.1444840100167197,
            "RMSE": 6.014053532220149,
            "R2": -9.80279442231031,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 15.530555
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.088914979350032,
            "RMSE": 5.930058413028094,
            "R2": -9.733901359629304,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 16.434104
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 2.038014375475162,
            "RMSE": 5.849577408393744,
            "R2": -9.43824097776182,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 17.347853
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.990139846596363,
            "RMSE": 5.772270602035659,
            "R2": -9.274280741061778,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 18.296023
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.946515411702069,
            "RMSE": 5.69815370877383,
            "R2": -9.05697999731458,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 19.263123
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.908897117108588,
            "RMSE": 5.627293726045093,
            "R2": -8.897112526821198,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 20.241821
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.8732261968689676,
            "RMSE": 5.559226632327132,
            "R2": -8.765208356441784,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 21.227083
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.8347271749400444,
            "RMSE": 5.492864392938861,
            "R2": -8.621969919695442,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 22.223141
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.8001515928803729,
            "RMSE": 5.4291765082898245,
            "R2": -8.383942958793503,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 23.230427
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.762610565031098,
            "RMSE": 5.367211780988228,
            "R2": -8.125392758933815,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 24.244373000000003
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.7278213800286455,
            "RMSE": 5.307357454879676,
            "R2": -7.960601204549325,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 25.346781000000004
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.6959197142820022,
            "RMSE": 5.249600105314111,
            "R2": -7.910676780558388,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 26.455778
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.6672680101890094,
            "RMSE": 5.193857129216991,
            "R2": -7.796440957593809,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 27.578615000000003
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.637208742738251,
            "RMSE": 5.139738169534271,
            "R2": -7.704147396017831,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 28.708325
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.6082702309133736,
            "RMSE": 5.087224346398139,
            "R2": -7.692803163516414,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 29.852185
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.582128560540168,
            "RMSE": 5.036439630005545,
            "R2": -7.663534315499042,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 31.047385
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "River MLP",
            "dataset": "TrumpApproval",
            "MAE": 1.5805783932319006,
            "RMSE": 5.033923389051291,
            "R2": -7.660658200179739,
            "Memory in Mb": 0.013350486755371,
            "Time in s": 32.243154000000004
          },
          {
            "step": 11,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 4.664574314574316,
            "RMSE": 12.7079745317607,
            "R2": -206.87879383707747,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.000258
          },
          {
            "step": 22,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 2.767694704637076,
            "RMSE": 9.018587183866767,
            "R2": -85.14025986830408,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.000737
          },
          {
            "step": 33,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 2.3093367298127023,
            "RMSE": 7.420500566500976,
            "R2": -37.24267181629702,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.00134
          },
          {
            "step": 44,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 1.892363968348808,
            "RMSE": 6.441521936619904,
            "R2": -31.668094594906044,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.002066
          },
          {
            "step": 55,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 2.1129412159858934,
            "RMSE": 6.114058653243701,
            "R2": -6.297346571779499,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.00291
          },
          {
            "step": 66,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 2.832849782567835,
            "RMSE": 6.236602142425367,
            "R2": -2.2730130120415795,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.003872
          },
          {
            "step": 77,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 3.4069290990236856,
            "RMSE": 6.402381882180361,
            "R2": -1.3118663438824,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.004952
          },
          {
            "step": 88,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 3.650377971160808,
            "RMSE": 6.321189272940957,
            "R2": -1.043267371916866,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.006149
          },
          {
            "step": 99,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 4.035631404360372,
            "RMSE": 6.4483291916176695,
            "R2": -0.7783857772357967,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.007464
          },
          {
            "step": 110,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 4.693189868957898,
            "RMSE": 7.0697740144659305,
            "R2": -0.4927792786841307,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.008896
          },
          {
            "step": 121,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 5.274396860168236,
            "RMSE": 7.6542276724395,
            "R2": -0.3476225254437259,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.010446
          },
          {
            "step": 132,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 5.875758254207378,
            "RMSE": 8.194624755054596,
            "R2": -0.2624191661321591,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.012113
          },
          {
            "step": 143,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 6.530760796045927,
            "RMSE": 8.870097879563003,
            "R2": -0.1980355424044948,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.013898
          },
          {
            "step": 154,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 7.121466111912466,
            "RMSE": 9.458403141043558,
            "R2": -0.1577027852151795,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.015801
          },
          {
            "step": 165,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 7.772438504082036,
            "RMSE": 10.375670403553157,
            "R2": -0.1198999930450892,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0178219999999999
          },
          {
            "step": 176,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 8.565827130563894,
            "RMSE": 11.410434180005833,
            "R2": -0.0920676568626532,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0199609999999999
          },
          {
            "step": 187,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 9.429958588641576,
            "RMSE": 12.495061319237752,
            "R2": -0.0722153171628203,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0222169999999999
          },
          {
            "step": 198,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 10.47731537859646,
            "RMSE": 13.900491647656429,
            "R2": -0.0555502703757588,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0245899999999999
          },
          {
            "step": 209,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 11.43172675762076,
            "RMSE": 15.229123619635446,
            "R2": -0.0444565128716372,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.027079
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 11.97432098008114,
            "RMSE": 16.22368260926648,
            "R2": -0.0377560869847111,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.029685
          },
          {
            "step": 231,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 12.9382196746461,
            "RMSE": 17.489503190785292,
            "R2": -0.0315781972827118,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.032406
          },
          {
            "step": 242,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 14.229204186206864,
            "RMSE": 19.43725798629848,
            "R2": -0.0252367718674193,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.035243
          },
          {
            "step": 253,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 15.339413196393396,
            "RMSE": 20.82023831254592,
            "R2": -0.0216497893038387,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.041904
          },
          {
            "step": 264,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 15.948617107030818,
            "RMSE": 21.75817315507082,
            "R2": -0.0194401851240946,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.048726
          },
          {
            "step": 275,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 16.794155127707494,
            "RMSE": 23.16724301729152,
            "R2": -0.0169996193237813,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.055688
          },
          {
            "step": 286,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 17.990009992534457,
            "RMSE": 24.865985915258104,
            "R2": -0.0147547133955299,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.062787
          },
          {
            "step": 297,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 19.34919450213405,
            "RMSE": 26.67620929760368,
            "R2": -0.0128904565600072,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.070018
          },
          {
            "step": 308,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 20.46881241431745,
            "RMSE": 28.248013022827838,
            "R2": -0.011537481517321,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.077383
          },
          {
            "step": 319,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 20.993702124162965,
            "RMSE": 29.63814114349949,
            "R2": -0.0105036731193923,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0848839999999999
          },
          {
            "step": 330,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 22.586872779548436,
            "RMSE": 32.01796640002603,
            "R2": -0.0092202379520505,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0925169999999999
          },
          {
            "step": 341,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 23.97345887210737,
            "RMSE": 33.821533603903084,
            "R2": -0.0083877019037323,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1002819999999999
          },
          {
            "step": 352,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 25.315991788770976,
            "RMSE": 35.461698606860665,
            "R2": -0.0077313021586467,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1081779999999999
          },
          {
            "step": 363,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 25.615062978866305,
            "RMSE": 35.981300981590465,
            "R2": -0.0074437490312051,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1162059999999999
          },
          {
            "step": 374,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 26.673321526932543,
            "RMSE": 37.51836715700961,
            "R2": -0.0069358461242559,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1243619999999999
          },
          {
            "step": 385,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 28.27694482780972,
            "RMSE": 39.8753298933956,
            "R2": -0.0063325109838794,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1326399999999999
          },
          {
            "step": 396,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 29.55612496209691,
            "RMSE": 41.28848705945016,
            "R2": -0.0059801818919071,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1410409999999999
          },
          {
            "step": 407,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 30.56167711268285,
            "RMSE": 42.81802042618151,
            "R2": -0.0056467231500465,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1495659999999999
          },
          {
            "step": 418,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 31.39346669137945,
            "RMSE": 44.18765357092498,
            "R2": -0.0053697143301307,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1582139999999999
          },
          {
            "step": 429,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 33.10612890637694,
            "RMSE": 46.865579751152914,
            "R2": -0.0049663660706051,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1669849999999999
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 34.54914638861108,
            "RMSE": 48.61167278858254,
            "R2": -0.0047161238549726,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1758829999999999
          },
          {
            "step": 451,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 35.43263419295921,
            "RMSE": 49.67507127970072,
            "R2": -0.0045536938071879,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1849059999999999
          },
          {
            "step": 462,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 36.308550382896186,
            "RMSE": 51.2507761435036,
            "R2": -0.0043573774895468,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.1940549999999999
          },
          {
            "step": 473,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 38.26330298063241,
            "RMSE": 54.53225049728104,
            "R2": -0.0040516612048955,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2033279999999999
          },
          {
            "step": 484,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 39.59866234800828,
            "RMSE": 56.08659790201894,
            "R2": -0.0039023944795495,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2127249999999999
          },
          {
            "step": 495,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 40.94697327298068,
            "RMSE": 57.823326559810994,
            "R2": -0.0037535911132069,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2222449999999999
          },
          {
            "step": 506,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 41.42384714758024,
            "RMSE": 58.67984594201592,
            "R2": -0.0036652347211194,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2318889999999999
          },
          {
            "step": 517,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 42.72663002099646,
            "RMSE": 60.40151056768402,
            "R2": -0.0035345422299792,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2416599999999999
          },
          {
            "step": 528,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 44.77321528369677,
            "RMSE": 63.69509749878913,
            "R2": -0.0033415055563215,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2515539999999999
          },
          {
            "step": 539,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 45.99579764939489,
            "RMSE": 65.0494992510053,
            "R2": -0.003252609562637,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2615709999999999
          },
          {
            "step": 550,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 46.57020777663759,
            "RMSE": 66.07332710234044,
            "R2": -0.0031815200825582,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2717109999999999
          },
          {
            "step": 561,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 47.75825760640621,
            "RMSE": 67.5643396193493,
            "R2": -0.0030950009187136,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2819719999999999
          },
          {
            "step": 572,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 49.49138874897682,
            "RMSE": 70.24569214117749,
            "R2": -0.0029719424061886,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.2923559999999999
          },
          {
            "step": 578,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "ChickWeights",
            "MAE": 50.250899455914585,
            "RMSE": 71.11438743304103,
            "R2": -0.0029294686391043,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.3028349999999999
          },
          {
            "step": 20,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 2.695184981652336,
            "RMSE": 9.807184976514188,
            "R2": -224.6021011118197,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.001338
          },
          {
            "step": 40,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 2.3994713447037435,
            "RMSE": 7.102066178895935,
            "R2": -19.27845129783118,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.003825
          },
          {
            "step": 60,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.8170744682035584,
            "RMSE": 5.815253847056423,
            "R2": -17.329373299766118,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.00717
          },
          {
            "step": 80,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.604995404573344,
            "RMSE": 5.081770494168446,
            "R2": -13.040545957103586,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.0113569999999999
          },
          {
            "step": 100,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.824259078948539,
            "RMSE": 4.70488333223354,
            "R2": -6.5512954222403845,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.020929
          },
          {
            "step": 120,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.918744608116588,
            "RMSE": 4.412336880489357,
            "R2": -4.634185300646759,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.030834
          },
          {
            "step": 140,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.8761207739327503,
            "RMSE": 4.13187920011476,
            "R2": -4.105616799680584,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.041039
          },
          {
            "step": 160,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.961232939518506,
            "RMSE": 3.976173487274506,
            "R2": -3.1695661963674864,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.051538
          },
          {
            "step": 180,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 2.066134597500757,
            "RMSE": 3.873731518767916,
            "R2": -2.4756944369169624,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.062312
          },
          {
            "step": 200,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 2.051125997923389,
            "RMSE": 3.731810291394655,
            "R2": -2.23527456693896,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.073408
          },
          {
            "step": 220,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.94095193468414,
            "RMSE": 3.56902990398404,
            "R2": -2.19210047340805,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.084777
          },
          {
            "step": 240,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.9366756524315063,
            "RMSE": 3.4612902974772624,
            "R2": -2.024876884626847,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.096419
          },
          {
            "step": 260,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.9250039777458068,
            "RMSE": 3.363327951159923,
            "R2": -1.8945640461454525,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.108333
          },
          {
            "step": 280,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.8726934920539136,
            "RMSE": 3.257010428159885,
            "R2": -1.8420037280027224,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.120517
          },
          {
            "step": 300,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.8907476896224935,
            "RMSE": 3.1958821895815714,
            "R2": -1.6910252267675163,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.133002
          },
          {
            "step": 320,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.819623890420079,
            "RMSE": 3.103812605138666,
            "R2": -1.663886258690169,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.145758
          },
          {
            "step": 340,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7396293145937214,
            "RMSE": 3.014220627768389,
            "R2": -1.654906383755708,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.158784
          },
          {
            "step": 360,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7350691203787965,
            "RMSE": 2.9569384317632506,
            "R2": -1.5759385016835008,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.172076
          },
          {
            "step": 380,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6987131960417108,
            "RMSE": 2.8893997308323693,
            "R2": -1.5446951110541192,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.185636
          },
          {
            "step": 400,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.673610627740774,
            "RMSE": 2.82935583501861,
            "R2": -1.5089937655143242,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.199488
          },
          {
            "step": 420,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6410137122925974,
            "RMSE": 2.7701802079251965,
            "R2": -1.484737486096575,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.213608
          },
          {
            "step": 440,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6565972573555454,
            "RMSE": 2.7427790467379385,
            "R2": -1.391750010744973,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.227993
          },
          {
            "step": 460,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.699464840115161,
            "RMSE": 2.73946740401384,
            "R2": -1.2626191030939884,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.242643
          },
          {
            "step": 480,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7224824441896145,
            "RMSE": 2.7219018737730583,
            "R2": -1.182307732575659,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.25756
          },
          {
            "step": 500,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7446092142173422,
            "RMSE": 2.70580354422956,
            "R2": -1.1113262021905803,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.272747
          },
          {
            "step": 520,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7464998751860934,
            "RMSE": 2.677192702589883,
            "R2": -1.0705208906620065,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.288233
          },
          {
            "step": 540,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7535492786865423,
            "RMSE": 2.653885630983747,
            "R2": -1.027170706279252,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.303987
          },
          {
            "step": 560,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7201019899937544,
            "RMSE": 2.614359234374483,
            "R2": -1.0141103337708768,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.320009
          },
          {
            "step": 580,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6887559504032663,
            "RMSE": 2.5757257291728384,
            "R2": -1.0033760803823184,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.336298
          },
          {
            "step": 600,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.701917368353294,
            "RMSE": 2.561424763732869,
            "R2": -0.9592753712060648,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.3528799999999999
          },
          {
            "step": 620,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7178157166185173,
            "RMSE": 2.551346895968156,
            "R2": -0.9142580419512064,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.369731
          },
          {
            "step": 640,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7365901196485038,
            "RMSE": 2.545046385321895,
            "R2": -0.8692105635365064,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.386852
          },
          {
            "step": 660,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.7465677425181807,
            "RMSE": 2.532051562790666,
            "R2": -0.8368676529707118,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.40424
          },
          {
            "step": 680,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.731617734826669,
            "RMSE": 2.504226186170861,
            "R2": -0.8251107974736909,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.4218949999999999
          },
          {
            "step": 700,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6973720107412231,
            "RMSE": 2.47026789197972,
            "R2": -0.8225927549994396,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.439849
          },
          {
            "step": 720,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6698372433333928,
            "RMSE": 2.4400355004771077,
            "R2": -0.81732226470892,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.458072
          },
          {
            "step": 740,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6732482399922957,
            "RMSE": 2.425592833263792,
            "R2": -0.7947920429290933,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.4765629999999999
          },
          {
            "step": 760,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6653913599894004,
            "RMSE": 2.404136439714782,
            "R2": -0.7822814452716051,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.4953209999999999
          },
          {
            "step": 780,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6644612180457288,
            "RMSE": 2.387561393188575,
            "R2": -0.7656652158374817,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.514347
          },
          {
            "step": 800,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6556359332933146,
            "RMSE": 2.368497267913513,
            "R2": -0.7532954885990883,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.533661
          },
          {
            "step": 820,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6452077788467467,
            "RMSE": 2.348678653798561,
            "R2": -0.7430103139622937,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.5532450000000001
          },
          {
            "step": 840,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6374623223784903,
            "RMSE": 2.3305035344735936,
            "R2": -0.7320713255917544,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.5730930000000001
          },
          {
            "step": 860,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6419505315856449,
            "RMSE": 2.320208013716276,
            "R2": -0.7138439732116804,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.6284980000000001
          },
          {
            "step": 880,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6490002164922652,
            "RMSE": 2.3126155324510744,
            "R2": -0.6941855677649247,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.6842080000000001
          },
          {
            "step": 900,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6474991175923384,
            "RMSE": 2.299197536504521,
            "R2": -0.6816400531907807,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.7401880000000002
          },
          {
            "step": 920,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6301006788336792,
            "RMSE": 2.2779225390149764,
            "R2": -0.6777843948800273,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.7964830000000002
          },
          {
            "step": 940,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6221876471839871,
            "RMSE": 2.262378737250057,
            "R2": -0.6690049120995847,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.8530460000000002
          },
          {
            "step": 960,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.6124120493571743,
            "RMSE": 2.245866476718547,
            "R2": -0.6619276404267609,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.9098760000000002
          },
          {
            "step": 980,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.5867001120604314,
            "RMSE": 2.223758235975506,
            "R2": -0.661013659831075,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 0.9669740000000002
          },
          {
            "step": 1000,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.5681359363812415,
            "RMSE": 2.2037391763141216,
            "R2": -0.6587014308970958,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 1.0243380000000002
          },
          {
            "step": 1001,
            "track": "Regression",
            "model": "[baseline] Mean predictor",
            "dataset": "TrumpApproval",
            "MAE": 1.567554989468773,
            "RMSE": 2.202858861923226,
            "R2": -0.6584830635688459,
            "Memory in Mb": 0.0004901885986328,
            "Time in s": 1.081765
          }
        ]
      },
      "params": [
        {
          "name": "models",
          "select": {
            "type": "point",
            "fields": [
              "model"
            ]
          },
          "bind": "legend"
        },
        {
          "name": "Dataset",
          "value": "ChickWeights",
          "bind": {
            "input": "select",
            "options": [
              "ChickWeights",
              "TrumpApproval"
            ]
          }
        },
        {
          "name": "grid",
          "select": "interval",
          "bind": "scales"
        }
      ],
      "transform": [
        {
          "filter": {
            "field": "dataset",
            "equal": {
              "expr": "Dataset"
            }
          }
        }
      ],
      "repeat": {
        "row": [
          "MAE",
          "RMSE",
          "R2",
          "Memory in Mb",
          "Time in s"
        ]
      },
      "spec": {
        "width": "container",
        "mark": "line",
        "encoding": {
          "x": {
            "field": "step",
            "type": "quantitative",
            "axis": {
              "titleFontSize": 18,
              "labelFontSize": 18,
              "title": "Instance"
            }
          },
          "y": {
            "field": {
              "repeat": "row"
            },
            "type": "quantitative",
            "axis": {
              "titleFontSize": 18,
              "labelFontSize": 18
            }
          },
          "color": {
            "field": "model",
            "type": "ordinal",
            "scale": {
              "scheme": "category20b"
            },
            "title": "Models",
            "legend": {
              "titleFontSize": 18,
              "labelFontSize": 18,
              "labelLimit": 500
            }
          },
          "opacity": {
            "condition": {
              "param": "models",
              "value": 1
            },
            "value": 0.2
          }
        }
      }
    }
    ```

            

## Datasets

???- abstract "ChickWeights"

    Chick weights along time.

    The stream contains 578 items and 3 features. The goal is to predict the weight of each chick
    along time, according to the diet the chick is on. The data is ordered by time and then by
    chick.

        Name  ChickWeights                                                                                                  
        Task  Regression                                                                                                    
     Samples  578                                                                                                           
    Features  3                                                                                                             
      Sparse  False                                                                                                         
        Path  /Users/mastelini/miniconda3/envs/river-benchmark/lib/python3.10/site-packages/river/datasets/chick-weights.csv

<span />

???- abstract "TrumpApproval"

    Donald Trump approval ratings.

    This dataset was obtained by reshaping the data used by FiveThirtyEight for analyzing Donald
    Trump's approval ratings. It contains 5 features, which are approval ratings collected by
    5 polling agencies. The target is the approval rating from FiveThirtyEight's model. The goal of
    this task is to see if we can reproduce FiveThirtyEight's model.

        Name  TrumpApproval                                                                                                     
        Task  Regression                                                                                                        
     Samples  1,001                                                                                                             
    Features  6                                                                                                                 
      Sparse  False                                                                                                             
        Path  /Users/mastelini/miniconda3/envs/river-benchmark/lib/python3.10/site-packages/river/datasets/trump_approval.csv.gz

<span />

## Models

???- example "Linear Regression"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      LinearRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=Squared ()
        l2=0.
        l1=0.
        intercept_init=0.
        intercept_lr=Constant (
          learning_rate=0.01
        )
        clip_gradient=1e+12
        initializer=Zeros ()
      )
    )</pre>

<span />

???- example "Linear Regression with l1 regularization"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      LinearRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=Squared ()
        l2=0.
        l1=1.
        intercept_init=0.
        intercept_lr=Constant (
          learning_rate=0.01
        )
        clip_gradient=1e+12
        initializer=Zeros ()
      )
    )</pre>

<span />

???- example "Linear Regression with l2 regularization"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      LinearRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=Squared ()
        l2=1.
        l1=0.
        intercept_init=0.
        intercept_lr=Constant (
          learning_rate=0.01
        )
        clip_gradient=1e+12
        initializer=Zeros ()
      )
    )</pre>

<span />

???- example "Passive-Aggressive Regressor, mode 1"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      PARegressor (
        C=1.
        mode=1
        eps=0.1
        learn_intercept=True
      )
    )</pre>

<span />

???- example "Passive-Aggressive Regressor, mode 2"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      PARegressor (
        C=1.
        mode=2
        eps=0.1
        learn_intercept=True
      )
    )</pre>

<span />

???- example "k-Nearest Neighbors"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      KNNRegressor (
        n_neighbors=5
        engine=SWINN (
          graph_k=20
          dist_func=FunctionWrapper (
            distance_function=functools.partial(<function minkowski_distance at 0x1380aa200>, p=2)
          )
          maxlen=1000
          warm_up=500
          max_candidates=50
          delta=0.0001
          prune_prob=0.
          n_iters=10
          seed=None
        )
        aggregation_method="mean"
      )
    )</pre>

<span />

???- example "Hoeffding Tree"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      HoeffdingTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
      )
    )</pre>

<span />

???- example "Hoeffding Adaptive Tree"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=True
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=42
      )
    )</pre>

<span />

???- example "Stochastic Gradient Tree"

    <pre>SGTRegressor (
      delta=1e-07
      grace_period=200
      init_pred=0.
      max_depth=inf
      lambda_value=0.1
      gamma=1.
      nominal_attributes=[]
      feature_quantizer=StaticQuantizer (
        n_bins=64
        warm_start=100
        buckets=None
      )
    )</pre>

<span />

???- example "Adaptive Random Forest"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      []
    )</pre>

<span />

???- example "Aggregated Mondrian Forest"

    <pre>[]</pre>

<span />

???- example "Adaptive Model Rules"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      AMRules (
        n_min=200
        delta=1e-07
        tau=0.05
        pred_type="adaptive"
        pred_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        splitter=TEBSTSplitter (
          digits=1
        )
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        fading_factor=0.99
        anomaly_threshold=-0.75
        m_min=30
        ordered_rule_set=True
        min_samples_split=5
      )
    )</pre>

<span />

???- example "Streaming Random Patches"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      SRPRegressor (
        model=HoeffdingTreeRegressor (
          grace_period=50
          max_depth=inf
          delta=0.01
          tau=0.05
          leaf_prediction="adaptive"
          leaf_model=LinearRegression (
            optimizer=SGD (
              lr=Constant (
                learning_rate=0.01
              )
            )
            loss=Squared ()
            l2=0.
            l1=0.
            intercept_init=0.
            intercept_lr=Constant (
              learning_rate=0.01
            )
            clip_gradient=1e+12
            initializer=Zeros ()
          )
          model_selector_decay=0.95
          nominal_attributes=None
          splitter=TEBSTSplitter (
            digits=1
          )
          min_samples_split=5
          binary_split=False
          max_size=500.
          memory_estimate_period=1000000
          stop_mem_management=False
          remove_poor_attrs=False
          merit_preprune=True
        )
        n_models=10
        subspace_size=0.6
        training_method="patches"
        lam=6
        drift_detector=ADWIN (
          delta=1e-05
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        warning_detector=ADWIN (
          delta=0.0001
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        disable_detector="off"
        disable_weighted_vote=True
        drift_detection_criteria="error"
        aggregation_method="mean"
        seed=42
        metric=MAE ()
      )
    )</pre>

<span />

???- example "Bagging"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      [HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=False
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      )]
    )</pre>

<span />

???- example "Exponentially Weighted Average"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      [LinearRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=Squared ()
        l2=0.
        l1=0.
        intercept_init=0.
        intercept_lr=Constant (
          learning_rate=0.01
        )
        clip_gradient=1e+12
        initializer=Zeros ()
      ), HoeffdingAdaptiveTreeRegressor (
        grace_period=200
        max_depth=inf
        delta=1e-07
        tau=0.05
        leaf_prediction="adaptive"
        leaf_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        model_selector_decay=0.95
        nominal_attributes=None
        splitter=TEBSTSplitter (
          digits=1
        )
        min_samples_split=5
        bootstrap_sampling=True
        drift_window_threshold=300
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        switch_significance=0.05
        binary_split=False
        max_size=500.
        memory_estimate_period=1000000
        stop_mem_management=False
        remove_poor_attrs=False
        merit_preprune=True
        seed=None
      ), KNNRegressor (
        n_neighbors=5
        engine=SWINN (
          graph_k=20
          dist_func=FunctionWrapper (
            distance_function=functools.partial(<function minkowski_distance at 0x1380aa200>, p=2)
          )
          maxlen=1000
          warm_up=500
          max_candidates=50
          delta=0.0001
          prune_prob=0.
          n_iters=10
          seed=None
        )
        aggregation_method="mean"
      ), AMRules (
        n_min=200
        delta=1e-07
        tau=0.05
        pred_type="adaptive"
        pred_model=LinearRegression (
          optimizer=SGD (
            lr=Constant (
              learning_rate=0.01
            )
          )
          loss=Squared ()
          l2=0.
          l1=0.
          intercept_init=0.
          intercept_lr=Constant (
            learning_rate=0.01
          )
          clip_gradient=1e+12
          initializer=Zeros ()
        )
        splitter=TEBSTSplitter (
          digits=1
        )
        drift_detector=ADWIN (
          delta=0.002
          clock=32
          max_buckets=5
          min_window_length=5
          grace_period=10
        )
        fading_factor=0.99
        anomaly_threshold=-0.75
        m_min=30
        ordered_rule_set=True
        min_samples_split=5
      )]
    )</pre>

<span />

???- example "River MLP"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      MLPRegressor (
        hidden_dims=(5,)
        activations=(<class 'river.neural_net.activations.ReLU'>, <class 'river.neural_net.activations.ReLU'>, <class 'river.neural_net.activations.Identity'>)
        loss=Squared ()
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.001
          )
        )
        seed=42
      )
    )</pre>

<span />

???- example "[baseline] Mean predictor"

    <pre>StatisticRegressor (
      statistic=Mean ()
    )</pre>

<span />

## Environment

<pre>Python implementation: CPython
Python version       : 3.10.13
IPython version      : 8.16.1

river       : 0.19.0
numpy       : 1.25.2
scikit-learn: 1.3.1
pandas      : 2.1.1
scipy       : 1.11.3

Compiler    : Clang 14.0.6 
OS          : Darwin
Release     : 22.6.0
Machine     : arm64
Processor   : arm
CPU cores   : 8
Architecture: 64bit
</pre>

