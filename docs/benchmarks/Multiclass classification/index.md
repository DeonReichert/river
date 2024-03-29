# Multiclass classification



=== "Table"

    | Model                      | Dataset       |   Accuracy |   MicroF1 |   MacroF1 |   Memory in Mb |   Time in s |
    |:---------------------------|:--------------|-----------:|----------:|----------:|---------------:|------------:|
    | ADWIN Bagging              | ImageSegments |   0.777826 |  0.777826 |  0.765011 |     4.11628    |   3543.55   |
    | ADWIN Bagging              | Insects       |   0.579465 |  0.579465 |  0.570198 |    15.3074     |  60279.4    |
    | ADWIN Bagging              | Keystroke     |   0.81656  |  0.81656  |  0.815908 |    37.8558     |  41308      |
    | AdaBoost                   | ImageSegments |   0.804677 |  0.804677 |  0.79777  |     4.09839    |   3350.88   |
    | AdaBoost                   | Insects       |   0.563532 |  0.563532 |  0.554622 |    27.943      |  60335.7    |
    | AdaBoost                   | Keystroke     |   0.834796 |  0.834796 |  0.836062 |   194.794      |  51861.3    |
    | Adaptive Random Forest     | ImageSegments |   0.818536 |  0.818536 |  0.814535 |     3.06348    |   1574.18   |
    | Adaptive Random Forest     | Insects       |   0.745378 |  0.745378 |  0.743302 |     0.361794   |  25383.5    |
    | Adaptive Random Forest     | Keystroke     |   0.969116 |  0.969116 |  0.969111 |     1.63546    |   7363.05   |
    | Aggregated Mondrian Forest | ImageSegments |   0.901689 |  0.901689 |  0.900381 |    17.0502     |   2997.7    |
    | Aggregated Mondrian Forest | Insects       |   0.646981 |  0.646981 |  0.644352 |  1365.41       |  76295.7    |
    | Aggregated Mondrian Forest | Keystroke     |   0.881073 |  0.881073 |  0.879928 |   338.139      |  35528.4    |
    | Bagging                    | ImageSegments |   0.77696  |  0.77696  |  0.764564 |     4.15507    |   3634.88   |
    | Bagging                    | Insects       |   0.606392 |  0.606392 |  0.598542 |     3.69162    |  65237      |
    | Bagging                    | Keystroke     |   0.669739 |  0.669739 |  0.669981 |    50.3449     |  55411.4    |
    | Hoeffding Adaptive Tree    | ImageSegments |   0.774361 |  0.774361 |  0.763362 |     0.423797   |    457.311  |
    | Hoeffding Adaptive Tree    | Insects       |   0.613337 |  0.613337 |  0.604219 |     0.143826   |  11292.9    |
    | Hoeffding Adaptive Tree    | Keystroke     |   0.723124 |  0.723124 |  0.721825 |     0.724475   |   8998.46   |
    | Hoeffding Tree             | ImageSegments |   0.776094 |  0.776094 |  0.763137 |     0.417154   |    328.067  |
    | Hoeffding Tree             | Insects       |   0.537306 |  0.537306 |  0.527364 |     2.51923    |   7445.36   |
    | Hoeffding Tree             | Keystroke     |   0.648218 |  0.648218 |  0.647249 |     5.09445    |   7138.73   |
    | Leveraging Bagging         | ImageSegments |   0.778259 |  0.778259 |  0.766016 |     4.1005     |   8561.3    |
    | Leveraging Bagging         | Insects       |   0.695858 |  0.695858 |  0.690508 |    13.831      |  99120.2    |
    | Leveraging Bagging         | Keystroke     |   0.956616 |  0.956616 |  0.95665  |     7.40999    |  37049.1    |
    | Naive Bayes                | ImageSegments |   0.731919 |  0.731919 |  0.730419 |     0.390004   |    248.959  |
    | Naive Bayes                | Insects       |   0.506897 |  0.506897 |  0.493019 |     0.611693   |   4263.77   |
    | Naive Bayes                | Keystroke     |   0.652532 |  0.652532 |  0.651577 |     4.86901    |   3544.69   |
    | Stacking                   | ImageSegments |   0.867908 |  0.867908 |  0.865603 |     9.18162    |   5416.88   |
    | Stacking                   | Insects       |   0.754745 |  0.754745 |  0.752818 |    10.5864     |  72115      |
    | Stacking                   | Keystroke     |   0.975489 |  0.975489 |  0.975486 |    18.7111     |  42471.8    |
    | Streaming Random Patches   | ImageSegments |   0.766999 |  0.766999 |  0.764707 |     8.92653    |   6441.81   |
    | Streaming Random Patches   | Insects       |   0.736163 |  0.736163 |  0.734622 |     9.632      |  90031.6    |
    | Streaming Random Patches   | Keystroke     |   0.955929 |  0.955929 |  0.95592  |    39.636      |  31009.8    |
    | Voting                     | ImageSegments |   0.80641  |  0.80641  |  0.798999 |     6.07392    |   3157.94   |
    | Voting                     | Insects       |   0.648533 |  0.648533 |  0.638    |     9.40652    |  48163.7    |
    | Voting                     | Keystroke     |   0.779107 |  0.779107 |  0.784136 |    16.3925     |  29779.2    |
    | [baseline] Last Class      | ImageSegments |   0.148116 |  0.148116 |  0.148116 |     0.00136948 |     31.4159 |
    | [baseline] Last Class      | Insects       |   0.289761 |  0.289761 |  0.289763 |     0.00138664 |    679.004  |
    | [baseline] Last Class      | Keystroke     |   0.997549 |  0.997549 |  0.997549 |     0.00504208 |    274.675  |
    | k-Nearest Neighbors        | ImageSegments |   0.873538 |  0.873538 |  0.872136 |     5.26871    |   2666.29   |
    | k-Nearest Neighbors        | Insects       |   0.713115 |  0.713115 |  0.711381 |     6.27269    |  40639.9    |
    | k-Nearest Neighbors        | Keystroke     |   0.910486 |  0.910486 |  0.910328 |     6.32511    |  21326.5    |

=== "Chart"

    *Try reloading the page if something is buggy*

    ```vegalite
    {
      "$schema": "https://vega.github.io/schema/vega-lite/v5.json",
      "data": {
        "values": [
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.4666666666666667,
            "MicroF1": 0.4666666666666667,
            "MacroF1": 0.4009102009102009,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 0.450679
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5604395604395604,
            "MicroF1": 0.5604395604395604,
            "MacroF1": 0.5279334700387331,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 1.152847
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5474452554744526,
            "MicroF1": 0.5474452554744526,
            "MacroF1": 0.5191892873237387,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 2.278305
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5573770491803278,
            "MicroF1": 0.5573770491803278,
            "MacroF1": 0.5225713529323662,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 3.449742
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5545851528384279,
            "MicroF1": 0.5545851528384279,
            "MacroF1": 0.5217226223148511,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 4.939578
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.56,
            "MicroF1": 0.56,
            "MacroF1": 0.5450388711329709,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 6.667081
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5825545171339563,
            "MicroF1": 0.5825545171339563,
            "MacroF1": 0.5566705826058684,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 8.548779999999999
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5940054495912807,
            "MicroF1": 0.5940054495912807,
            "MacroF1": 0.5613773296963412,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 10.607026
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.5980629539951574,
            "MicroF1": 0.5980629539951574,
            "MacroF1": 0.5624927052752284,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 12.811145
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.599128540305011,
            "MicroF1": 0.599128540305011,
            "MacroF1": 0.5669821167583783,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 15.144022
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6099009900990099,
            "MicroF1": 0.6099009900990099,
            "MacroF1": 0.592228619098681,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 17.683543
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6116152450090744,
            "MicroF1": 0.6116152450090744,
            "MacroF1": 0.5983340184133136,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 20.357047
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6180904522613065,
            "MicroF1": 0.6180904522613065,
            "MacroF1": 0.611527101723203,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 23.213992
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6158631415241057,
            "MicroF1": 0.6158631415241057,
            "MacroF1": 0.6113311881078581,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 26.205369
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6182873730043541,
            "MicroF1": 0.6182873730043541,
            "MacroF1": 0.6150189987146761,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 29.350024
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.617687074829932,
            "MicroF1": 0.617687074829932,
            "MacroF1": 0.6157912419016742,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 32.567265
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6274007682458387,
            "MicroF1": 0.6274007682458387,
            "MacroF1": 0.6216325704223051,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 36.027093
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6324062877871826,
            "MicroF1": 0.6324062877871826,
            "MacroF1": 0.6280704917469789,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 39.646129
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6426116838487973,
            "MicroF1": 0.6426116838487973,
            "MacroF1": 0.6349558095046656,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 43.417442
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6485310119695321,
            "MicroF1": 0.6485310119695321,
            "MacroF1": 0.6384515982514894,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 47.360213
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6507772020725389,
            "MicroF1": 0.6507772020725389,
            "MacroF1": 0.6399118827528387,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 51.459671
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6508407517309595,
            "MicroF1": 0.6508407517309595,
            "MacroF1": 0.6387857120889422,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 55.677121
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6537369914853358,
            "MicroF1": 0.6537369914853358,
            "MacroF1": 0.6398811322847953,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 60.129657
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.658204895738894,
            "MicroF1": 0.658204895738894,
            "MacroF1": 0.6463297068165035,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 64.716333
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6640557006092254,
            "MicroF1": 0.6640557006092254,
            "MacroF1": 0.6508930463144657,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 69.425449
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6702928870292887,
            "MicroF1": 0.6702928870292887,
            "MacroF1": 0.6599370641329333,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 74.368592
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6736502820306205,
            "MicroF1": 0.6736502820306205,
            "MacroF1": 0.669511465798708,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 79.42749
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6822066822066822,
            "MicroF1": 0.6822066822066822,
            "MacroF1": 0.6790074545382362,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 84.676077
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6841710427606902,
            "MicroF1": 0.6841710427606902,
            "MacroF1": 0.6834974476087327,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 90.04929600000001
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6874546773023931,
            "MicroF1": 0.6874546773023931,
            "MacroF1": 0.687676692272135,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 95.54439700000002
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.6919298245614035,
            "MicroF1": 0.6919298245614035,
            "MacroF1": 0.6930786661709784,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 101.25523300000002
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.698844323589395,
            "MicroF1": 0.698844323589395,
            "MacroF1": 0.6985606658027719,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 107.09626300000002
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7027027027027027,
            "MicroF1": 0.7027027027027027,
            "MacroF1": 0.7017787722939461,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 113.17857300000004
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7056941778630839,
            "MicroF1": 0.7056941778630839,
            "MacroF1": 0.7062915374924865,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 119.38367200000005
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7078931013051585,
            "MicroF1": 0.7078931013051585,
            "MacroF1": 0.7081385387673028,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 125.72760100000004
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7093655589123867,
            "MicroF1": 0.7093655589123867,
            "MacroF1": 0.7109488618373111,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 132.27559300000004
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7101704879482658,
            "MicroF1": 0.7101704879482658,
            "MacroF1": 0.7132092257742534,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 138.94755600000005
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7143674871207785,
            "MicroF1": 0.7143674871207784,
            "MacroF1": 0.7178399485500211,
            "Memory in Mb": 0.3899507522583008,
            "Time in s": 145.68584300000003
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7172336865588399,
            "MicroF1": 0.7172336865588399,
            "MacroF1": 0.7191260584555579,
            "Memory in Mb": 0.3899774551391601,
            "Time in s": 152.67811600000005
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7199564980967917,
            "MicroF1": 0.7199564980967917,
            "MacroF1": 0.7217017555070446,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 159.82058900000004
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7204244031830239,
            "MicroF1": 0.7204244031830238,
            "MacroF1": 0.7234495525792994,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 167.13449700000004
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7219057483169342,
            "MicroF1": 0.7219057483169342,
            "MacroF1": 0.7238483512148008,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 174.57489300000003
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.723823975720789,
            "MicroF1": 0.723823975720789,
            "MacroF1": 0.7251399238639739,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 182.21825900000005
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.726643598615917,
            "MicroF1": 0.726643598615917,
            "MacroF1": 0.7268553573885639,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 189.97396200000009
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7269212179797003,
            "MicroF1": 0.7269212179797003,
            "MacroF1": 0.7276782991451582,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 197.92708900000005
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7286052009456265,
            "MicroF1": 0.7286052009456266,
            "MacroF1": 0.7283656039279267,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 206.04766600000005
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7306802406293382,
            "MicroF1": 0.7306802406293383,
            "MacroF1": 0.7303992643507475,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 214.36632800000004
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.733574988672406,
            "MicroF1": 0.733574988672406,
            "MacroF1": 0.7322842940126589,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 222.77231300000005
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7314691522414558,
            "MicroF1": 0.7314691522414558,
            "MacroF1": 0.7300322879925133,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 231.40748800000003
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7316224445411048,
            "MicroF1": 0.7316224445411048,
            "MacroF1": 0.7300416811383057,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 240.14309800000004
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "ImageSegments",
            "Accuracy": 0.7319185794716327,
            "MicroF1": 0.7319185794716329,
            "MacroF1": 0.7304188192194185,
            "Memory in Mb": 0.3900041580200195,
            "Time in s": 248.95897400000004
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.623696682464455,
            "MicroF1": 0.623696682464455,
            "MacroF1": 0.5870724729616662,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 4.116407
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6148744670772146,
            "MicroF1": 0.6148744670772146,
            "MacroF1": 0.5800776869595596,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 12.008893
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6065677297126618,
            "MicroF1": 0.6065677297126618,
            "MacroF1": 0.5714781230184183,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 23.636521
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6043097324177126,
            "MicroF1": 0.6043097324177126,
            "MacroF1": 0.5697541737710122,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 38.735534
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6088274294373934,
            "MicroF1": 0.6088274294373934,
            "MacroF1": 0.5727560614138387,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 57.253764
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6023677979479084,
            "MicroF1": 0.6023677979479084,
            "MacroF1": 0.5679597008529512,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 79.038555
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5995129211202814,
            "MicroF1": 0.5995129211202814,
            "MacroF1": 0.5652603100832261,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 104.109779
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6019888717888008,
            "MicroF1": 0.6019888717888008,
            "MacroF1": 0.5673514925692325,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 132.296427
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5993896664211301,
            "MicroF1": 0.5993896664211301,
            "MacroF1": 0.5644951651039589,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 163.68164199999998
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5994885879344635,
            "MicroF1": 0.5994885879344635,
            "MacroF1": 0.564565538599863,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 198.252114
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5972449418854929,
            "MicroF1": 0.5972449418854929,
            "MacroF1": 0.5631227877868952,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 235.999104
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6001894088864336,
            "MicroF1": 0.6001894088864336,
            "MacroF1": 0.5684733590606373,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 276.973484
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6120783856632913,
            "MicroF1": 0.6120783856632913,
            "MacroF1": 0.5935173038317552,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 321.087465
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.6024487587093282,
            "MicroF1": 0.6024487587093282,
            "MacroF1": 0.5841270876002982,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 368.414891
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5676494728202538,
            "MicroF1": 0.5676494728202538,
            "MacroF1": 0.5507155080701159,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 418.926748
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5418762947617638,
            "MicroF1": 0.5418762947617638,
            "MacroF1": 0.5256197352354142,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 472.672831
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5232020500250683,
            "MicroF1": 0.5232020500250683,
            "MacroF1": 0.5066898143269706,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 529.5973250000001
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5118640500868101,
            "MicroF1": 0.5118640500868101,
            "MacroF1": 0.4926543583964285,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 589.87103
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5103922643672432,
            "MicroF1": 0.5103922643672432,
            "MacroF1": 0.4900586962359796,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 653.257514
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5115772527108291,
            "MicroF1": 0.5115772527108291,
            "MacroF1": 0.4910837640903744,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 719.720849
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5140022547914318,
            "MicroF1": 0.5140022547914318,
            "MacroF1": 0.4932541888231957,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 789.2473650000001
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5154319659076234,
            "MicroF1": 0.5154319659076234,
            "MacroF1": 0.4943013417599926,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 861.9200270000001
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5184254951208466,
            "MicroF1": 0.5184254951208466,
            "MacroF1": 0.4965832238311332,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 937.628382
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5225111470623052,
            "MicroF1": 0.5225111470623052,
            "MacroF1": 0.499893079239698,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1016.433905
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5257396113489148,
            "MicroF1": 0.5257396113489148,
            "MacroF1": 0.5022487669255871,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1098.325454
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5301402294663996,
            "MicroF1": 0.5301402294663996,
            "MacroF1": 0.5051550433324518,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1183.302333
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5277261407877661,
            "MicroF1": 0.5277261407877661,
            "MacroF1": 0.5036945145235058,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1271.323869
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5204450908107011,
            "MicroF1": 0.5204450908107011,
            "MacroF1": 0.4989008712312768,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1362.446785
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5147111648107632,
            "MicroF1": 0.5147111648107632,
            "MacroF1": 0.495826840073632,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1456.7074690000002
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5105590454244137,
            "MicroF1": 0.5105590454244137,
            "MacroF1": 0.4941101813344875,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1553.9918670000002
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5075607148312204,
            "MicroF1": 0.5075607148312204,
            "MacroF1": 0.4931947798921405,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1654.355087
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5044538486579266,
            "MicroF1": 0.5044538486579266,
            "MacroF1": 0.4905626123916189,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1757.6376
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5020231296811777,
            "MicroF1": 0.5020231296811777,
            "MacroF1": 0.487879842488124,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1863.925375
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4998746622844887,
            "MicroF1": 0.4998746622844887,
            "MacroF1": 0.4853435061152475,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 1973.177917
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4967937444194918,
            "MicroF1": 0.4967937444194918,
            "MacroF1": 0.4819418474093529,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2085.445724
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4955938445350519,
            "MicroF1": 0.4955938445350519,
            "MacroF1": 0.4801892436835747,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2200.821931
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4940237004427836,
            "MicroF1": 0.4940237004427836,
            "MacroF1": 0.478380783820526,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2319.178703
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.493508111745209,
            "MicroF1": 0.493508111745209,
            "MacroF1": 0.4785213801670671,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2440.443075
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4936988563242114,
            "MicroF1": 0.4936988563242114,
            "MacroF1": 0.4794201499427274,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2564.583087
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4938800634484718,
            "MicroF1": 0.4938800634484718,
            "MacroF1": 0.4802377497532935,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2691.651665
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4943757939715902,
            "MicroF1": 0.4943757939715902,
            "MacroF1": 0.4812132921167227,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2821.601336
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.494036211133909,
            "MicroF1": 0.494036211133909,
            "MacroF1": 0.4812388919618418,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 2954.377766
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4944832294580131,
            "MicroF1": 0.4944832294580131,
            "MacroF1": 0.4818441874360225,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3089.8310679999995
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4945225232981082,
            "MicroF1": 0.4945225232981082,
            "MacroF1": 0.4820791268335544,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3227.9665449999998
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4956333256171216,
            "MicroF1": 0.4956333256171216,
            "MacroF1": 0.4833168636021498,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3368.688097999999
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4970869788986104,
            "MicroF1": 0.4970869788986104,
            "MacroF1": 0.4846703771634363,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3511.887438999999
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.4987608551107171,
            "MicroF1": 0.4987608551107171,
            "MacroF1": 0.4862426724473749,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3657.6494079999993
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5009568528419516,
            "MicroF1": 0.5009568528419516,
            "MacroF1": 0.4881725476999718,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3806.011259
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5034497419940862,
            "MicroF1": 0.5034497419940862,
            "MacroF1": 0.4903712806540024,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 3956.893516
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5068467205818292,
            "MicroF1": 0.5068467205818292,
            "MacroF1": 0.4930025316136313,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 4110.278735
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Insects",
            "Accuracy": 0.5068972694760346,
            "MicroF1": 0.5068972694760346,
            "MacroF1": 0.4930190627831494,
            "Memory in Mb": 0.6116933822631836,
            "Time in s": 4263.766907
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.9852579852579852,
            "MicroF1": 0.9852579852579852,
            "MacroF1": 0.6962686567164179,
            "Memory in Mb": 0.1935644149780273,
            "Time in s": 0.780775
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.947239263803681,
            "MicroF1": 0.947239263803681,
            "MacroF1": 0.7418606503288051,
            "Memory in Mb": 0.2889022827148437,
            "Time in s": 2.463269
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.884709730171709,
            "MicroF1": 0.884709730171709,
            "MacroF1": 0.8705899666065842,
            "Memory in Mb": 0.3842401504516601,
            "Time in s": 5.15507
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8933169834457388,
            "MicroF1": 0.8933169834457388,
            "MacroF1": 0.8791291775937072,
            "Memory in Mb": 0.4795780181884765,
            "Time in s": 8.960951
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8921039725355566,
            "MicroF1": 0.8921039725355566,
            "MacroF1": 0.8831785360852743,
            "Memory in Mb": 0.575160026550293,
            "Time in s": 14.051639
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.851655087862689,
            "MicroF1": 0.851655087862689,
            "MacroF1": 0.8581984289516641,
            "Memory in Mb": 0.6704978942871094,
            "Time in s": 20.582882
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8598949211908932,
            "MicroF1": 0.8598949211908932,
            "MacroF1": 0.8469962214365346,
            "Memory in Mb": 0.7658357620239258,
            "Time in s": 28.649143
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8513637756665645,
            "MicroF1": 0.8513637756665645,
            "MacroF1": 0.8281280134770846,
            "Memory in Mb": 0.8611736297607422,
            "Time in s": 38.532046
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8422773086352493,
            "MicroF1": 0.8422773086352493,
            "MacroF1": 0.8409307955747314,
            "Memory in Mb": 0.9565114974975586,
            "Time in s": 50.273206
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8367246874233881,
            "MicroF1": 0.8367246874233881,
            "MacroF1": 0.8249418657104467,
            "Memory in Mb": 1.0523834228515625,
            "Time in s": 63.882498
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8203699576554491,
            "MicroF1": 0.8203699576554491,
            "MacroF1": 0.8300896799820437,
            "Memory in Mb": 1.147721290588379,
            "Time in s": 79.531469
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8192032686414709,
            "MicroF1": 0.8192032686414709,
            "MacroF1": 0.8269731591910484,
            "Memory in Mb": 1.243059158325195,
            "Time in s": 97.310117
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.8172732415613804,
            "MicroF1": 0.8172732415613804,
            "MacroF1": 0.8027823390848743,
            "Memory in Mb": 1.3383970260620115,
            "Time in s": 117.35519
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7961828051129399,
            "MicroF1": 0.7961828051129399,
            "MacroF1": 0.8002006091139847,
            "Memory in Mb": 1.433734893798828,
            "Time in s": 139.817583
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.793920575257395,
            "MicroF1": 0.793920575257395,
            "MacroF1": 0.7746960355921345,
            "Memory in Mb": 1.5290727615356443,
            "Time in s": 164.727582
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7688064960931515,
            "MicroF1": 0.7688064960931515,
            "MacroF1": 0.7622487598340326,
            "Memory in Mb": 1.624410629272461,
            "Time in s": 192.151707
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7568853640951694,
            "MicroF1": 0.7568853640951694,
            "MacroF1": 0.757813781660983,
            "Memory in Mb": 1.7197484970092771,
            "Time in s": 222.243586
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7669889690862045,
            "MicroF1": 0.7669889690862046,
            "MacroF1": 0.7643943615019536,
            "Memory in Mb": 1.8150863647460935,
            "Time in s": 255.230678
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7676428847890595,
            "MicroF1": 0.7676428847890595,
            "MacroF1": 0.7655695901071293,
            "Memory in Mb": 1.9104242324829104,
            "Time in s": 291.218411
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7714180659394534,
            "MicroF1": 0.7714180659394533,
            "MacroF1": 0.7672011803374248,
            "Memory in Mb": 2.0057621002197266,
            "Time in s": 330.398823
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7702813120112058,
            "MicroF1": 0.7702813120112058,
            "MacroF1": 0.7699263138193525,
            "Memory in Mb": 2.1021223068237305,
            "Time in s": 372.827664
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7680222841225627,
            "MicroF1": 0.7680222841225627,
            "MacroF1": 0.7682287234686136,
            "Memory in Mb": 2.197460174560547,
            "Time in s": 418.63015
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7659597143770649,
            "MicroF1": 0.7659597143770649,
            "MacroF1": 0.7643546547243014,
            "Memory in Mb": 2.2927980422973637,
            "Time in s": 468.011111
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7586559084873864,
            "MicroF1": 0.7586559084873864,
            "MacroF1": 0.7552148692020618,
            "Memory in Mb": 2.38813591003418,
            "Time in s": 521.0847249999999
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7505637807628199,
            "MicroF1": 0.7505637807628199,
            "MacroF1": 0.7430512224080145,
            "Memory in Mb": 2.483473777770996,
            "Time in s": 577.917349
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7290468558499105,
            "MicroF1": 0.7290468558499106,
            "MacroF1": 0.715756093271779,
            "Memory in Mb": 2.5788116455078125,
            "Time in s": 638.790947
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7217430776214253,
            "MicroF1": 0.7217430776214253,
            "MacroF1": 0.7173640789896896,
            "Memory in Mb": 2.674149513244629,
            "Time in s": 703.666983
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7151361288628206,
            "MicroF1": 0.7151361288628206,
            "MacroF1": 0.7011862635194489,
            "Memory in Mb": 2.7694873809814453,
            "Time in s": 772.6431349999999
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.705603921900093,
            "MicroF1": 0.705603921900093,
            "MacroF1": 0.6976881379682607,
            "Memory in Mb": 2.8648252487182617,
            "Time in s": 845.8350979999999
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7094533867146009,
            "MicroF1": 0.7094533867146009,
            "MacroF1": 0.7058405389403433,
            "Memory in Mb": 2.960163116455078,
            "Time in s": 923.50335
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.7053846762077963,
            "MicroF1": 0.7053846762077963,
            "MacroF1": 0.6965736948063982,
            "Memory in Mb": 3.0555009841918945,
            "Time in s": 1005.753677
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6927613941018766,
            "MicroF1": 0.6927613941018766,
            "MacroF1": 0.6842255816736498,
            "Memory in Mb": 3.150838851928711,
            "Time in s": 1092.707972
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6890737577063062,
            "MicroF1": 0.6890737577063062,
            "MacroF1": 0.6845669389392289,
            "Memory in Mb": 3.246176719665528,
            "Time in s": 1184.483965
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6873332852714296,
            "MicroF1": 0.6873332852714296,
            "MacroF1": 0.68390545518227,
            "Memory in Mb": 3.341514587402344,
            "Time in s": 1281.216395
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.682960991666083,
            "MicroF1": 0.682960991666083,
            "MacroF1": 0.6781566371919944,
            "Memory in Mb": 3.43685245513916,
            "Time in s": 1383.039909
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.686185061619119,
            "MicroF1": 0.686185061619119,
            "MacroF1": 0.6843713776162116,
            "Memory in Mb": 3.532190322875977,
            "Time in s": 1489.909884
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6928784365684001,
            "MicroF1": 0.6928784365684001,
            "MacroF1": 0.6911392400672977,
            "Memory in Mb": 3.627528190612793,
            "Time in s": 1601.996709
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6913500612784622,
            "MicroF1": 0.6913500612784622,
            "MacroF1": 0.687359772989117,
            "Memory in Mb": 3.72286605834961,
            "Time in s": 1719.445985
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6819810194205267,
            "MicroF1": 0.6819810194205267,
            "MacroF1": 0.674915944935936,
            "Memory in Mb": 3.818203926086426,
            "Time in s": 1842.197498
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6726515105092223,
            "MicroF1": 0.6726515105092223,
            "MacroF1": 0.6670192172011686,
            "Memory in Mb": 3.913541793823242,
            "Time in s": 1970.358299
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6695163508100676,
            "MicroF1": 0.6695163508100676,
            "MacroF1": 0.6664051037977977,
            "Memory in Mb": 4.008879661560059,
            "Time in s": 2103.939399
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6650131310183834,
            "MicroF1": 0.6650131310183834,
            "MacroF1": 0.6608988619616458,
            "Memory in Mb": 4.1063079833984375,
            "Time in s": 2242.845385
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6568431853160804,
            "MicroF1": 0.6568431853160804,
            "MacroF1": 0.6531382897719189,
            "Memory in Mb": 4.201645851135254,
            "Time in s": 2386.822189
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6556180714166342,
            "MicroF1": 0.6556180714166342,
            "MacroF1": 0.6538448358590968,
            "Memory in Mb": 4.29698371887207,
            "Time in s": 2536.044428
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6614194672912468,
            "MicroF1": 0.6614194672912468,
            "MacroF1": 0.6603186829199909,
            "Memory in Mb": 4.392321586608887,
            "Time in s": 2690.5476860000003
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6669686151222891,
            "MicroF1": 0.6669686151222891,
            "MacroF1": 0.6662293616554571,
            "Memory in Mb": 4.487659454345703,
            "Time in s": 2850.3140810000004
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6579921773142112,
            "MicroF1": 0.6579921773142112,
            "MacroF1": 0.6554177118629491,
            "Memory in Mb": 4.58299732208252,
            "Time in s": 3015.4823350000006
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6622580809886126,
            "MicroF1": 0.6622580809886126,
            "MacroF1": 0.6609360990360078,
            "Memory in Mb": 4.678335189819336,
            "Time in s": 3186.2814100000005
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6562453103896754,
            "MicroF1": 0.6562453103896754,
            "MacroF1": 0.6545704957554572,
            "Memory in Mb": 4.773673057556152,
            "Time in s": 3362.6238980000007
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Naive Bayes",
            "dataset": "Keystroke",
            "Accuracy": 0.6525319868621011,
            "MicroF1": 0.6525319868621011,
            "MacroF1": 0.6515767870317885,
            "Memory in Mb": 4.869010925292969,
            "Time in s": 3544.6906370000006
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.3555555555555555,
            "MicroF1": 0.3555555555555555,
            "MacroF1": 0.2537942449707155,
            "Memory in Mb": 0.4170856475830078,
            "Time in s": 0.290301
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.4945054945054945,
            "MicroF1": 0.4945054945054945,
            "MacroF1": 0.5043329927491418,
            "Memory in Mb": 0.4170818328857422,
            "Time in s": 0.82046
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.5328467153284672,
            "MicroF1": 0.5328467153284672,
            "MacroF1": 0.5564033878668025,
            "Memory in Mb": 0.4171772003173828,
            "Time in s": 1.675423
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6010928961748634,
            "MicroF1": 0.6010928961748634,
            "MacroF1": 0.622766496539645,
            "Memory in Mb": 0.4171772003173828,
            "Time in s": 2.801183
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6375545851528385,
            "MicroF1": 0.6375545851528385,
            "MacroF1": 0.6539827168809461,
            "Memory in Mb": 0.4172000885009765,
            "Time in s": 4.271522
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6509090909090909,
            "MicroF1": 0.6509090909090909,
            "MacroF1": 0.6671561759164943,
            "Memory in Mb": 0.4172496795654297,
            "Time in s": 5.954744
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.67601246105919,
            "MicroF1": 0.67601246105919,
            "MacroF1": 0.6756614325426025,
            "Memory in Mb": 0.4172496795654297,
            "Time in s": 7.864603
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7029972752043597,
            "MicroF1": 0.7029972752043597,
            "MacroF1": 0.6993447851636564,
            "Memory in Mb": 0.4172229766845703,
            "Time in s": 10.008665
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7142857142857143,
            "MicroF1": 0.7142857142857143,
            "MacroF1": 0.7108606838045498,
            "Memory in Mb": 0.4171428680419922,
            "Time in s": 12.399438
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7145969498910676,
            "MicroF1": 0.7145969498910676,
            "MacroF1": 0.7090365931960759,
            "Memory in Mb": 0.4172191619873047,
            "Time in s": 15.01004
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7207920792079208,
            "MicroF1": 0.7207920792079208,
            "MacroF1": 0.7126631585949761,
            "Memory in Mb": 0.4172191619873047,
            "Time in s": 17.873655
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7223230490018149,
            "MicroF1": 0.7223230490018149,
            "MacroF1": 0.7157730164623107,
            "Memory in Mb": 0.4171123504638672,
            "Time in s": 20.946971
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7286432160804021,
            "MicroF1": 0.7286432160804021,
            "MacroF1": 0.7216745323124732,
            "Memory in Mb": 0.4171352386474609,
            "Time in s": 24.255884
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7278382581648523,
            "MicroF1": 0.7278382581648523,
            "MacroF1": 0.7229105183087501,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 27.838412
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7314949201741655,
            "MicroF1": 0.7314949201741654,
            "MacroF1": 0.7263583447448078,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 31.647636
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7333333333333333,
            "MicroF1": 0.7333333333333333,
            "MacroF1": 0.729431071218305,
            "Memory in Mb": 0.4171352386474609,
            "Time in s": 35.743157
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7387964148527529,
            "MicroF1": 0.7387964148527529,
            "MacroF1": 0.7349287389986899,
            "Memory in Mb": 0.4171352386474609,
            "Time in s": 40.06309
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7376058041112454,
            "MicroF1": 0.7376058041112454,
            "MacroF1": 0.7356226390109741,
            "Memory in Mb": 0.4171352386474609,
            "Time in s": 44.599844
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7445589919816724,
            "MicroF1": 0.7445589919816724,
            "MacroF1": 0.7409366047432264,
            "Memory in Mb": 0.4171352386474609,
            "Time in s": 49.398729
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7453754080522307,
            "MicroF1": 0.7453754080522307,
            "MacroF1": 0.7408438328939173,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 54.404894
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7471502590673575,
            "MicroF1": 0.7471502590673575,
            "MacroF1": 0.7416651838589269,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 59.665949
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7467853610286844,
            "MicroF1": 0.7467853610286844,
            "MacroF1": 0.7416356251822,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 65.211169
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7492904446546831,
            "MicroF1": 0.7492904446546831,
            "MacroF1": 0.7430778844390783,
            "Memory in Mb": 0.4171085357666015,
            "Time in s": 70.961377
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7515865820489573,
            "MicroF1": 0.7515865820489573,
            "MacroF1": 0.7451256886686588,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 76.969446
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7536988685813751,
            "MicroF1": 0.7536988685813751,
            "MacroF1": 0.7468312166689606,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 83.201851
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7564853556485356,
            "MicroF1": 0.7564853556485356,
            "MacroF1": 0.7503479321738041,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 89.604352
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7566478646253022,
            "MicroF1": 0.7566478646253022,
            "MacroF1": 0.7509717522131719,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 96.307026
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7614607614607615,
            "MicroF1": 0.7614607614607615,
            "MacroF1": 0.7547643483779538,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 103.262462
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7614403600900225,
            "MicroF1": 0.7614403600900225,
            "MacroF1": 0.7551060921605869,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 110.41488900000002
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7621464829586657,
            "MicroF1": 0.7621464829586658,
            "MacroF1": 0.7562209880685912,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 117.799886
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7642105263157895,
            "MicroF1": 0.7642105263157895,
            "MacroF1": 0.7575332274919562,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 125.46176800000002
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7688647178789939,
            "MicroF1": 0.768864717878994,
            "MacroF1": 0.760438686053582,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 133.360363
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7705998681608438,
            "MicroF1": 0.7705998681608438,
            "MacroF1": 0.7612069012840872,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 141.48549400000002
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7709532949456174,
            "MicroF1": 0.7709532949456174,
            "MacroF1": 0.7622701654854867,
            "Memory in Mb": 0.4171581268310547,
            "Time in s": 149.83563600000002
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7712865133623369,
            "MicroF1": 0.771286513362337,
            "MacroF1": 0.7617247271717752,
            "Memory in Mb": 0.4171810150146484,
            "Time in s": 158.439217
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7709969788519637,
            "MicroF1": 0.7709969788519637,
            "MacroF1": 0.7615629120572474,
            "Memory in Mb": 0.4171810150146484,
            "Time in s": 167.22864700000002
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.770135214579659,
            "MicroF1": 0.770135214579659,
            "MacroF1": 0.7627316365695143,
            "Memory in Mb": 0.4171810150146484,
            "Time in s": 176.30742800000002
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7727532913566113,
            "MicroF1": 0.7727532913566113,
            "MacroF1": 0.7649467707214076,
            "Memory in Mb": 0.4171810150146484,
            "Time in s": 185.609237
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7741215839375348,
            "MicroF1": 0.7741215839375348,
            "MacroF1": 0.7649332326562149,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 195.107308
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7754214246873301,
            "MicroF1": 0.7754214246873301,
            "MacroF1": 0.7664700790631908,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 204.88888000000003
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7740053050397878,
            "MicroF1": 0.7740053050397878,
            "MacroF1": 0.7655121135276625,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 214.87796100000003
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7742102537545313,
            "MicroF1": 0.7742102537545313,
            "MacroF1": 0.7648034036287765,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 225.10774000000004
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7754172989377845,
            "MicroF1": 0.7754172989377845,
            "MacroF1": 0.7656013068970459,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 235.56491900000003
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7770637666831438,
            "MicroF1": 0.7770637666831438,
            "MacroF1": 0.7660878232247856,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 246.31694000000005
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7762203963267279,
            "MicroF1": 0.7762203963267279,
            "MacroF1": 0.7654829214385931,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 257.28426500000006
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7768321513002364,
            "MicroF1": 0.7768321513002364,
            "MacroF1": 0.7653071619305024,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 268.5154150000001
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7778806108283203,
            "MicroF1": 0.7778806108283203,
            "MacroF1": 0.7659351904174982,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 279.94414300000005
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7797915722700498,
            "MicroF1": 0.7797915722700498,
            "MacroF1": 0.7668192864082087,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 291.65328600000004
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7767421216156236,
            "MicroF1": 0.7767421216156236,
            "MacroF1": 0.7637794374955548,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 303.618395
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7759895606785558,
            "MicroF1": 0.7759895606785558,
            "MacroF1": 0.763026662835187,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 315.80512400000003
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.776093546990039,
            "MicroF1": 0.776093546990039,
            "MacroF1": 0.7631372452021826,
            "Memory in Mb": 0.417154312133789,
            "Time in s": 328.06738900000005
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6218009478672986,
            "MicroF1": 0.6218009478672986,
            "MacroF1": 0.5852663107194211,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 7.68277
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6153481762198011,
            "MicroF1": 0.6153481762198011,
            "MacroF1": 0.5806436317780949,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 22.565114
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6071992421850332,
            "MicroF1": 0.6071992421850332,
            "MacroF1": 0.572248584718361,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 43.997682
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6043097324177126,
            "MicroF1": 0.6043097324177126,
            "MacroF1": 0.5697573109597247,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 71.858443
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6088274294373934,
            "MicroF1": 0.6088274294373934,
            "MacroF1": 0.5727379077413696,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 105.92484
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6026835043409629,
            "MicroF1": 0.6026835043409629,
            "MacroF1": 0.568251333238805,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 146.287253
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.600189419564335,
            "MicroF1": 0.600189419564335,
            "MacroF1": 0.5659762112716077,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 192.863981
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.60258079791642,
            "MicroF1": 0.60258079791642,
            "MacroF1": 0.5679781484640408,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 245.806734
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5998105861306956,
            "MicroF1": 0.5998105861306956,
            "MacroF1": 0.5649597336877693,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 305.14044
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5998674116867128,
            "MicroF1": 0.5998674116867128,
            "MacroF1": 0.5650173260529011,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 370.680891
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5974171330176495,
            "MicroF1": 0.5974171330176495,
            "MacroF1": 0.5633067089377387,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 442.338443
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6001894088864336,
            "MicroF1": 0.6001894088864336,
            "MacroF1": 0.5684760329567131,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 520.121563
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6120783856632913,
            "MicroF1": 0.6120783856632913,
            "MacroF1": 0.5935956771555828,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 604.039429
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.6024487587093282,
            "MicroF1": 0.6024487587093282,
            "MacroF1": 0.5842148300149193,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 694.113241
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5677757434181451,
            "MicroF1": 0.5677757434181451,
            "MacroF1": 0.5509250187877572,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 790.19156
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5419354838709678,
            "MicroF1": 0.5419354838709678,
            "MacroF1": 0.5257359157219258,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 892.361186
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5233691716338923,
            "MicroF1": 0.5233691716338923,
            "MacroF1": 0.5068581838352059,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 1000.471748
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5121271110643447,
            "MicroF1": 0.5121271110643447,
            "MacroF1": 0.4929289906509415,
            "Memory in Mb": 0.6579360961914062,
            "Time in s": 1114.494528
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5120370831879579,
            "MicroF1": 0.5120370831879579,
            "MacroF1": 0.4920970323041603,
            "Memory in Mb": 1.3099584579467771,
            "Time in s": 1234.20565
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5173066906577016,
            "MicroF1": 0.5173066906577016,
            "MacroF1": 0.4973447169836249,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 1358.925583
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5229312288613304,
            "MicroF1": 0.5229312288613304,
            "MacroF1": 0.5026343687424488,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 1488.370808
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5301536739701261,
            "MicroF1": 0.5301536739701261,
            "MacroF1": 0.5095132087733324,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 1622.41448
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5351422571746202,
            "MicroF1": 0.5351422571746202,
            "MacroF1": 0.5135975374357353,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 1760.8970379999998
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5403069881229531,
            "MicroF1": 0.5403069881229531,
            "MacroF1": 0.5180803411538233,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 1903.591145
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5441493995984696,
            "MicroF1": 0.5441493995984696,
            "MacroF1": 0.5209012984387186,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2050.469487
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5475869604807867,
            "MicroF1": 0.5475869604807867,
            "MacroF1": 0.5230407124785976,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2201.55681
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5442460804601733,
            "MicroF1": 0.5442460804601733,
            "MacroF1": 0.5199893698637053,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2356.711105
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5439848479724017,
            "MicroF1": 0.5439848479724017,
            "MacroF1": 0.5225387960194383,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2516.62263
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5449825294713124,
            "MicroF1": 0.5449825294713124,
            "MacroF1": 0.5260472440529832,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2681.546079
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5469238296663405,
            "MicroF1": 0.5469238296663405,
            "MacroF1": 0.5300194392617626,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 2851.622305
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5492286543455017,
            "MicroF1": 0.5492286543455017,
            "MacroF1": 0.5337692045397758,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 3026.797274
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5448196265277737,
            "MicroF1": 0.5448196265277737,
            "MacroF1": 0.5298516474077153,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 3207.119826
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.539357763939507,
            "MicroF1": 0.539357763939507,
            "MacroF1": 0.5246413689313029,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 3392.401024
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5352756037099964,
            "MicroF1": 0.5352756037099964,
            "MacroF1": 0.5204658240271913,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 3582.6817720000004
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5307232338537298,
            "MicroF1": 0.5307232338537298,
            "MacroF1": 0.5158458403074864,
            "Memory in Mb": 1.310713768005371,
            "Time in s": 3778.309285
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5287912666052874,
            "MicroF1": 0.5287912666052874,
            "MacroF1": 0.5138605376143625,
            "Memory in Mb": 1.8479537963867188,
            "Time in s": 3978.822433
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5245322617798367,
            "MicroF1": 0.5245322617798367,
            "MacroF1": 0.5100329616180462,
            "Memory in Mb": 1.9625730514526367,
            "Time in s": 4184.1075280000005
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5244847608841927,
            "MicroF1": 0.5244847608841927,
            "MacroF1": 0.5114466799524962,
            "Memory in Mb": 1.9625730514526367,
            "Time in s": 4393.646320000001
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5269650098341548,
            "MicroF1": 0.5269650098341548,
            "MacroF1": 0.5145630920489553,
            "Memory in Mb": 1.9625730514526367,
            "Time in s": 4606.675677000001
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5290608205686688,
            "MicroF1": 0.5290608205686688,
            "MacroF1": 0.5171452370879218,
            "Memory in Mb": 1.9625730514526367,
            "Time in s": 4823.052294000001
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5316318281556762,
            "MicroF1": 0.5316318281556762,
            "MacroF1": 0.5200714653059241,
            "Memory in Mb": 1.9625730514526367,
            "Time in s": 5042.794587000001
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5332912448422809,
            "MicroF1": 0.5332912448422809,
            "MacroF1": 0.521951703681177,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 5266.308108000001
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5350937080185875,
            "MicroF1": 0.5350937080185875,
            "MacroF1": 0.5236272112757866,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 5493.659660000001
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5374168693368917,
            "MicroF1": 0.5374168693368917,
            "MacroF1": 0.5257977177437826,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 5724.562244000002
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5359540394368568,
            "MicroF1": 0.5359540394368568,
            "MacroF1": 0.5247049329892776,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 5959.275286000002
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5333196088522902,
            "MicroF1": 0.5333196088522902,
            "MacroF1": 0.5224640186909637,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 6197.987866000002
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5314017448771937,
            "MicroF1": 0.5314017448771937,
            "MacroF1": 0.5209076603734537,
            "Memory in Mb": 1.9633283615112305,
            "Time in s": 6440.583835000002
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5322271982954209,
            "MicroF1": 0.5322271982954209,
            "MacroF1": 0.5219695808096345,
            "Memory in Mb": 2.081958770751953,
            "Time in s": 6687.224874000002
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5377345727924551,
            "MicroF1": 0.5377345727924551,
            "MacroF1": 0.5274876060436412,
            "Memory in Mb": 2.3156700134277344,
            "Time in s": 6937.746409000002
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5370366863008769,
            "MicroF1": 0.5370366863008769,
            "MacroF1": 0.5270872650003847,
            "Memory in Mb": 2.519227981567383,
            "Time in s": 7191.466386000002
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Insects",
            "Accuracy": 0.5373058073305959,
            "MicroF1": 0.5373058073305959,
            "MacroF1": 0.5273644947479657,
            "Memory in Mb": 2.519227981567383,
            "Time in s": 7445.3631460000015
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.9803439803439804,
            "MicroF1": 0.9803439803439804,
            "MacroF1": 0.4950372208436724,
            "Memory in Mb": 0.2240447998046875,
            "Time in s": 0.863228
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.9423312883435584,
            "MicroF1": 0.9423312883435584,
            "MacroF1": 0.7661667470992702,
            "Memory in Mb": 0.3196687698364258,
            "Time in s": 3.107641
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8830744071954211,
            "MicroF1": 0.883074407195421,
            "MacroF1": 0.8761191747044462,
            "Memory in Mb": 0.415292739868164,
            "Time in s": 7.048775
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8902513795217658,
            "MicroF1": 0.8902513795217658,
            "MacroF1": 0.8767853151263398,
            "Memory in Mb": 0.5114049911499023,
            "Time in s": 13.087732
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8891613536047082,
            "MicroF1": 0.8891613536047082,
            "MacroF1": 0.8807858055314012,
            "Memory in Mb": 0.6185035705566406,
            "Time in s": 21.551525
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.848385778504291,
            "MicroF1": 0.848385778504291,
            "MacroF1": 0.8522513926518692,
            "Memory in Mb": 0.7141275405883789,
            "Time in s": 32.816222999999994
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8563922942206655,
            "MicroF1": 0.8563922942206655,
            "MacroF1": 0.8440193478447516,
            "Memory in Mb": 0.8097515106201172,
            "Time in s": 47.080319
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8482991112473184,
            "MicroF1": 0.8482991112473184,
            "MacroF1": 0.8269786301577753,
            "Memory in Mb": 0.9053754806518556,
            "Time in s": 64.636989
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8392808499046581,
            "MicroF1": 0.8392808499046581,
            "MacroF1": 0.8374924160046072,
            "Memory in Mb": 1.0009994506835938,
            "Time in s": 85.706576
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8323118411375338,
            "MicroF1": 0.8323118411375338,
            "MacroF1": 0.8182261307945194,
            "Memory in Mb": 1.1217241287231443,
            "Time in s": 110.709782
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8159126365054602,
            "MicroF1": 0.8159126365054602,
            "MacroF1": 0.8260965842218733,
            "Memory in Mb": 1.2173480987548828,
            "Time in s": 139.812165
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8149131767109296,
            "MicroF1": 0.8149131767109296,
            "MacroF1": 0.8221314665977922,
            "Memory in Mb": 1.312972068786621,
            "Time in s": 173.369773
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8125589289081652,
            "MicroF1": 0.8125589289081652,
            "MacroF1": 0.797613058026624,
            "Memory in Mb": 1.4085960388183594,
            "Time in s": 211.780209
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7907546839432674,
            "MicroF1": 0.7907546839432674,
            "MacroF1": 0.7936708037520236,
            "Memory in Mb": 1.5042200088500977,
            "Time in s": 255.273991
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7886909625755842,
            "MicroF1": 0.7886909625755842,
            "MacroF1": 0.7694478218498494,
            "Memory in Mb": 1.599843978881836,
            "Time in s": 304.294734
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7635973647924008,
            "MicroF1": 0.7635973647924008,
            "MacroF1": 0.75687960152136,
            "Memory in Mb": 1.6954679489135742,
            "Time in s": 359.144129
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.75155010814708,
            "MicroF1": 0.7515501081470799,
            "MacroF1": 0.7521509466338959,
            "Memory in Mb": 1.7910919189453125,
            "Time in s": 420.221142
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7611330518861501,
            "MicroF1": 0.7611330518861501,
            "MacroF1": 0.7576671162861806,
            "Memory in Mb": 1.8881807327270508,
            "Time in s": 487.76956500000006
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7617081666881693,
            "MicroF1": 0.7617081666881692,
            "MacroF1": 0.7593340838982119,
            "Memory in Mb": 1.983804702758789,
            "Time in s": 562.1432000000001
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7655349920333374,
            "MicroF1": 0.7655349920333374,
            "MacroF1": 0.7610505848438686,
            "Memory in Mb": 2.079428672790528,
            "Time in s": 643.5514560000001
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7644449632310026,
            "MicroF1": 0.7644449632310025,
            "MacroF1": 0.7639417799779614,
            "Memory in Mb": 2.223102569580078,
            "Time in s": 732.3349550000001
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7624512534818941,
            "MicroF1": 0.7624512534818941,
            "MacroF1": 0.7625605608371232,
            "Memory in Mb": 2.3187265396118164,
            "Time in s": 828.9274100000001
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7605243525524885,
            "MicroF1": 0.7605243525524885,
            "MacroF1": 0.7588384348689571,
            "Memory in Mb": 2.4143505096435547,
            "Time in s": 933.484588
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.753344908589521,
            "MicroF1": 0.753344908589521,
            "MacroF1": 0.7499438215834663,
            "Memory in Mb": 2.509974479675293,
            "Time in s": 1046.19484
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7450730463770958,
            "MicroF1": 0.7450730463770959,
            "MacroF1": 0.7369660419615974,
            "Memory in Mb": 2.6055984497070312,
            "Time in s": 1167.344916
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7240501555576506,
            "MicroF1": 0.7240501555576506,
            "MacroF1": 0.7111305646829175,
            "Memory in Mb": 2.701222419738769,
            "Time in s": 1296.919782
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7166591012256015,
            "MicroF1": 0.7166591012256015,
            "MacroF1": 0.7122511515574346,
            "Memory in Mb": 2.796846389770508,
            "Time in s": 1434.776076
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.710146196270682,
            "MicroF1": 0.710146196270682,
            "MacroF1": 0.6963016796632095,
            "Memory in Mb": 2.892470359802246,
            "Time in s": 1580.7280859999998
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7005324993660722,
            "MicroF1": 0.7005324993660722,
            "MacroF1": 0.6925666211338901,
            "Memory in Mb": 2.9880943298339844,
            "Time in s": 1735.0271709999995
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7043876133671052,
            "MicroF1": 0.7043876133671052,
            "MacroF1": 0.7007845610449206,
            "Memory in Mb": 3.0837182998657227,
            "Time in s": 1897.652612
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7004032576895707,
            "MicroF1": 0.7004032576895707,
            "MacroF1": 0.6915775762792657,
            "Memory in Mb": 3.179342269897461,
            "Time in s": 2069.0860809999995
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6877058598238223,
            "MicroF1": 0.6877058598238223,
            "MacroF1": 0.6789768292873962,
            "Memory in Mb": 3.274966239929199,
            "Time in s": 2249.389177
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6838743222164451,
            "MicroF1": 0.6838743222164451,
            "MacroF1": 0.6791243465680947,
            "Memory in Mb": 3.370590209960937,
            "Time in s": 2438.693149
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6822146925239708,
            "MicroF1": 0.6822146925239708,
            "MacroF1": 0.6786558938530485,
            "Memory in Mb": 3.466214179992676,
            "Time in s": 2637.684102
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6777085230058127,
            "MicroF1": 0.6777085230058127,
            "MacroF1": 0.6725285130045525,
            "Memory in Mb": 3.561838150024414,
            "Time in s": 2845.828808
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6807380676788997,
            "MicroF1": 0.6807380676788997,
            "MacroF1": 0.6786761142186741,
            "Memory in Mb": 3.657462120056152,
            "Time in s": 3062.994215
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6873799271281882,
            "MicroF1": 0.6873799271281882,
            "MacroF1": 0.6854839306484398,
            "Memory in Mb": 3.75308609008789,
            "Time in s": 3290.055422
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6858027478552539,
            "MicroF1": 0.6858027478552539,
            "MacroF1": 0.6816808496509055,
            "Memory in Mb": 3.848710060119629,
            "Time in s": 3526.69202
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6765759537426937,
            "MicroF1": 0.6765759537426937,
            "MacroF1": 0.6694713281964946,
            "Memory in Mb": 3.944334030151367,
            "Time in s": 3772.997519
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6673815797536614,
            "MicroF1": 0.6673815797536614,
            "MacroF1": 0.6617321933140904,
            "Memory in Mb": 4.0399580001831055,
            "Time in s": 4029.133223
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6643151790518323,
            "MicroF1": 0.6643151790518323,
            "MacroF1": 0.661178029358405,
            "Memory in Mb": 4.135581970214844,
            "Time in s": 4295.086238
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6598774438284214,
            "MicroF1": 0.6598774438284214,
            "MacroF1": 0.655734247886306,
            "Memory in Mb": 4.32945728302002,
            "Time in s": 4570.827071
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6518269395200365,
            "MicroF1": 0.6518269395200365,
            "MacroF1": 0.6481085155228206,
            "Memory in Mb": 4.425081253051758,
            "Time in s": 4856.254143
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6507158375577963,
            "MicroF1": 0.6507158375577963,
            "MacroF1": 0.6489368995854258,
            "Memory in Mb": 4.520705223083496,
            "Time in s": 5151.869359
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6566806470940683,
            "MicroF1": 0.6566806470940683,
            "MacroF1": 0.6555764711123695,
            "Memory in Mb": 4.616329193115234,
            "Time in s": 5457.498716
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.662279533223211,
            "MicroF1": 0.662279533223211,
            "MacroF1": 0.6615432060687808,
            "Memory in Mb": 4.711953163146973,
            "Time in s": 5772.982264
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6534028683181226,
            "MicroF1": 0.6534028683181226,
            "MacroF1": 0.6508089832432514,
            "Memory in Mb": 4.807577133178711,
            "Time in s": 6098.679956
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6577643874789358,
            "MicroF1": 0.6577643874789358,
            "MacroF1": 0.6564201177589184,
            "Memory in Mb": 4.903201103210449,
            "Time in s": 6434.678037
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6518433294982742,
            "MicroF1": 0.6518433294982742,
            "MacroF1": 0.6501496360982542,
            "Memory in Mb": 4.998825073242188,
            "Time in s": 6781.324361
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Hoeffding Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6482180499044071,
            "MicroF1": 0.6482180499044071,
            "MacroF1": 0.6472493759146578,
            "Memory in Mb": 5.094449043273926,
            "Time in s": 7138.730487
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.3777777777777777,
            "MicroF1": 0.3777777777777777,
            "MacroF1": 0.2811210847975554,
            "Memory in Mb": 0.4234571456909179,
            "Time in s": 0.325579
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.5164835164835165,
            "MicroF1": 0.5164835164835165,
            "MacroF1": 0.5335477748411618,
            "Memory in Mb": 0.4235143661499023,
            "Time in s": 1.056326
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.5474452554744526,
            "MicroF1": 0.5474452554744526,
            "MacroF1": 0.5743273066802479,
            "Memory in Mb": 0.4236364364624023,
            "Time in s": 2.202996
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6120218579234973,
            "MicroF1": 0.6120218579234973,
            "MacroF1": 0.6355989308336889,
            "Memory in Mb": 0.4237203598022461,
            "Time in s": 3.699294
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6375545851528385,
            "MicroF1": 0.6375545851528385,
            "MacroF1": 0.6557923943920432,
            "Memory in Mb": 0.4237203598022461,
            "Time in s": 5.564336
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.6509090909090909,
            "MicroF1": 0.6509090909090909,
            "MacroF1": 0.66910740948952,
            "Memory in Mb": 0.4237699508666992,
            "Time in s": 7.749814
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.67601246105919,
            "MicroF1": 0.67601246105919,
            "MacroF1": 0.678427291711157,
            "Memory in Mb": 0.4238309860229492,
            "Time in s": 10.278631
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7002724795640327,
            "MicroF1": 0.7002724795640327,
            "MacroF1": 0.6988359939675117,
            "Memory in Mb": 0.4238042831420898,
            "Time in s": 13.125556
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.711864406779661,
            "MicroF1": 0.711864406779661,
            "MacroF1": 0.7104564330601258,
            "Memory in Mb": 0.4237241744995117,
            "Time in s": 16.369918000000002
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7124183006535948,
            "MicroF1": 0.7124183006535948,
            "MacroF1": 0.7087721216219991,
            "Memory in Mb": 0.4238004684448242,
            "Time in s": 19.921878000000003
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7207920792079208,
            "MicroF1": 0.7207920792079208,
            "MacroF1": 0.7145025942185106,
            "Memory in Mb": 0.4238004684448242,
            "Time in s": 23.844357
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7223230490018149,
            "MicroF1": 0.7223230490018149,
            "MacroF1": 0.7174926871575792,
            "Memory in Mb": 0.4236936569213867,
            "Time in s": 28.111685
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7269681742043551,
            "MicroF1": 0.7269681742043551,
            "MacroF1": 0.7216367248754637,
            "Memory in Mb": 0.4237165451049804,
            "Time in s": 32.752989
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7262830482115086,
            "MicroF1": 0.7262830482115085,
            "MacroF1": 0.7230014848259525,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 37.712808
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7300435413642961,
            "MicroF1": 0.7300435413642961,
            "MacroF1": 0.7265684058467008,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 43.006145
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7319727891156462,
            "MicroF1": 0.7319727891156461,
            "MacroF1": 0.7296570819427115,
            "Memory in Mb": 0.4237775802612304,
            "Time in s": 48.68780100000001
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.737516005121639,
            "MicroF1": 0.737516005121639,
            "MacroF1": 0.7350906419548328,
            "Memory in Mb": 0.4237775802612304,
            "Time in s": 54.69172
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7363966142684402,
            "MicroF1": 0.7363966142684402,
            "MacroF1": 0.7359651798179677,
            "Memory in Mb": 0.4237775802612304,
            "Time in s": 60.98272
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7422680412371134,
            "MicroF1": 0.7422680412371134,
            "MacroF1": 0.7398886847335938,
            "Memory in Mb": 0.4237775802612304,
            "Time in s": 67.641769
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7421109902067464,
            "MicroF1": 0.7421109902067464,
            "MacroF1": 0.738912026501458,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 74.649906
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7419689119170985,
            "MicroF1": 0.7419689119170985,
            "MacroF1": 0.7379593683174607,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 81.98079
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7418397626112759,
            "MicroF1": 0.741839762611276,
            "MacroF1": 0.7380802548116379,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 89.699811
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7436140018921475,
            "MicroF1": 0.7436140018921475,
            "MacroF1": 0.7390703652035102,
            "Memory in Mb": 0.4237508773803711,
            "Time in s": 97.738161
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7461468721668177,
            "MicroF1": 0.7461468721668177,
            "MacroF1": 0.7413714574148674,
            "Memory in Mb": 0.4238004684448242,
            "Time in s": 106.141078
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7476066144473456,
            "MicroF1": 0.7476066144473456,
            "MacroF1": 0.742441565911322,
            "Memory in Mb": 0.4238004684448242,
            "Time in s": 114.875735
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7506276150627615,
            "MicroF1": 0.7506276150627615,
            "MacroF1": 0.7460917536510117,
            "Memory in Mb": 0.4234342575073242,
            "Time in s": 123.973121
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7510072522159549,
            "MicroF1": 0.7510072522159549,
            "MacroF1": 0.7470578866974922,
            "Memory in Mb": 0.4235563278198242,
            "Time in s": 133.391788
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.756021756021756,
            "MicroF1": 0.7560217560217559,
            "MacroF1": 0.7510482446555896,
            "Memory in Mb": 0.4236173629760742,
            "Time in s": 143.113173
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7569392348087022,
            "MicroF1": 0.7569392348087022,
            "MacroF1": 0.7522366633133313,
            "Memory in Mb": 0.4236173629760742,
            "Time in s": 153.228885
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7585206671501088,
            "MicroF1": 0.7585206671501088,
            "MacroF1": 0.7544196711061472,
            "Memory in Mb": 0.4236783981323242,
            "Time in s": 163.64661999999998
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7614035087719299,
            "MicroF1": 0.7614035087719299,
            "MacroF1": 0.7567964121564391,
            "Memory in Mb": 0.4236783981323242,
            "Time in s": 174.36664399999998
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7654656696125085,
            "MicroF1": 0.7654656696125085,
            "MacroF1": 0.7591802078998249,
            "Memory in Mb": 0.4236783981323242,
            "Time in s": 185.463757
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7673038892551087,
            "MicroF1": 0.7673038892551087,
            "MacroF1": 0.7600352016074767,
            "Memory in Mb": 0.4237394332885742,
            "Time in s": 196.90308
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7677543186180422,
            "MicroF1": 0.7677543186180422,
            "MacroF1": 0.7612494392404334,
            "Memory in Mb": 0.4237394332885742,
            "Time in s": 208.647576
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7675574891236793,
            "MicroF1": 0.7675574891236793,
            "MacroF1": 0.7602773300593106,
            "Memory in Mb": 0.4237623214721679,
            "Time in s": 220.786107
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.76797583081571,
            "MicroF1": 0.76797583081571,
            "MacroF1": 0.7607906010792568,
            "Memory in Mb": 0.4237623214721679,
            "Time in s": 233.2194
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7677836566725456,
            "MicroF1": 0.7677836566725456,
            "MacroF1": 0.7627036277641847,
            "Memory in Mb": 0.4237623214721679,
            "Time in s": 245.952092
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7710360618202633,
            "MicroF1": 0.7710360618202633,
            "MacroF1": 0.7657334796773966,
            "Memory in Mb": 0.4237623214721679,
            "Time in s": 259.02703
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7724484104852203,
            "MicroF1": 0.7724484104852203,
            "MacroF1": 0.7657758298578787,
            "Memory in Mb": 0.4237356185913086,
            "Time in s": 272.394107
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7737901033170201,
            "MicroF1": 0.77379010331702,
            "MacroF1": 0.767302943564198,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 286.067762
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7724137931034483,
            "MicroF1": 0.7724137931034483,
            "MacroF1": 0.7666353585191567,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 300.095471
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7731745209735889,
            "MicroF1": 0.7731745209735889,
            "MacroF1": 0.7666634536176192,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 314.417396
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7738998482549317,
            "MicroF1": 0.7738998482549316,
            "MacroF1": 0.7665909326930368,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 329.067854
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7750865051903114,
            "MicroF1": 0.7750865051903113,
            "MacroF1": 0.7662611838286661,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 344.01511700000003
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7747704204929918,
            "MicroF1": 0.7747704204929918,
            "MacroF1": 0.7660645062500586,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 359.290159
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7754137115839244,
            "MicroF1": 0.7754137115839244,
            "MacroF1": 0.7658988206988366,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 374.882405
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7760296159185562,
            "MicroF1": 0.7760296159185563,
            "MacroF1": 0.7660708746783081,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 390.75768
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.777979157227005,
            "MicroF1": 0.7779791572270048,
            "MacroF1": 0.7670029065892423,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 407.002801
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7749667110519307,
            "MicroF1": 0.7749667110519308,
            "MacroF1": 0.7639707440456852,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 423.546299
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7742496737712049,
            "MicroF1": 0.7742496737712049,
            "MacroF1": 0.7632394528829524,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 440.393364
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "ImageSegments",
            "Accuracy": 0.7743611953226505,
            "MicroF1": 0.7743611953226506,
            "MacroF1": 0.7633622232911937,
            "Memory in Mb": 0.4237966537475586,
            "Time in s": 457.310729
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6161137440758294,
            "MicroF1": 0.6161137440758294,
            "MacroF1": 0.581384151333148,
            "Memory in Mb": 0.6645784378051758,
            "Time in s": 11.249192
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6120322122216959,
            "MicroF1": 0.6120322122216959,
            "MacroF1": 0.5792161554760864,
            "Memory in Mb": 0.6646394729614258,
            "Time in s": 32.358705
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6049889485317335,
            "MicroF1": 0.6049889485317335,
            "MacroF1": 0.5721633809277145,
            "Memory in Mb": 0.6647005081176758,
            "Time in s": 62.851539
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.603125739995264,
            "MicroF1": 0.603125739995264,
            "MacroF1": 0.5703574432462961,
            "Memory in Mb": 0.6647005081176758,
            "Time in s": 102.700179
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6061754120098504,
            "MicroF1": 0.6061754120098504,
            "MacroF1": 0.5722430970062696,
            "Memory in Mb": 0.6647615432739258,
            "Time in s": 151.914202
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5995264404104184,
            "MicroF1": 0.5995264404104184,
            "MacroF1": 0.5671511237518188,
            "Memory in Mb": 0.6647615432739258,
            "Time in s": 210.432187
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5972128264104992,
            "MicroF1": 0.5972128264104992,
            "MacroF1": 0.5650210504998666,
            "Memory in Mb": 0.6647615432739258,
            "Time in s": 278.267755
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5989108559251806,
            "MicroF1": 0.5989108559251806,
            "MacroF1": 0.566418690076869,
            "Memory in Mb": 0.6647615432739258,
            "Time in s": 355.204938
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5962327685993897,
            "MicroF1": 0.5962327685993897,
            "MacroF1": 0.5633780031885509,
            "Memory in Mb": 0.6647615432739258,
            "Time in s": 441.186739
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5964579979164694,
            "MicroF1": 0.5964579979164694,
            "MacroF1": 0.5634236596216465,
            "Memory in Mb": 0.6648225784301758,
            "Time in s": 536.283653
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.594317692638829,
            "MicroF1": 0.594317692638829,
            "MacroF1": 0.5620068495149612,
            "Memory in Mb": 0.6648225784301758,
            "Time in s": 640.2689049999999
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5975061163286244,
            "MicroF1": 0.5975061163286244,
            "MacroF1": 0.567518061449456,
            "Memory in Mb": 0.6648225784301758,
            "Time in s": 753.0441599999999
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6097472135207984,
            "MicroF1": 0.6097472135207984,
            "MacroF1": 0.5927729676671933,
            "Memory in Mb": 0.6648225784301758,
            "Time in s": 874.528885
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6001488195900697,
            "MicroF1": 0.6001488195900697,
            "MacroF1": 0.5832911478837771,
            "Memory in Mb": 0.6645174026489258,
            "Time in s": 1004.55011
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5673969316244712,
            "MicroF1": 0.5673969316244712,
            "MacroF1": 0.5522471754341495,
            "Memory in Mb": 0.8876123428344727,
            "Time in s": 1142.6522839999998
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5712340929269014,
            "MicroF1": 0.5712340929269014,
            "MacroF1": 0.5590383236849579,
            "Memory in Mb": 1.4319400787353516,
            "Time in s": 1288.8770269999998
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5741184335134533,
            "MicroF1": 0.5741184335134533,
            "MacroF1": 0.5632919959429028,
            "Memory in Mb": 1.8629226684570312,
            "Time in s": 1445.4718369999998
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5867312042931552,
            "MicroF1": 0.5867312042931552,
            "MacroF1": 0.5723846445183198,
            "Memory in Mb": 0.4819307327270508,
            "Time in s": 1609.073978
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5966704879629168,
            "MicroF1": 0.5966704879629168,
            "MacroF1": 0.5796820575913003,
            "Memory in Mb": 0.6649179458618164,
            "Time in s": 1780.2710459999998
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5984658364505895,
            "MicroF1": 0.5984658364505895,
            "MacroF1": 0.5810209140208816,
            "Memory in Mb": 0.6650400161743164,
            "Time in s": 1958.819581
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6001803833145434,
            "MicroF1": 0.6001803833145434,
            "MacroF1": 0.5822125955100945,
            "Memory in Mb": 1.2073478698730469,
            "Time in s": 2144.726031
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6020403770823468,
            "MicroF1": 0.6020403770823468,
            "MacroF1": 0.5837921358595156,
            "Memory in Mb": 1.321575164794922,
            "Time in s": 2339.531046
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6047268085807221,
            "MicroF1": 0.6047268085807221,
            "MacroF1": 0.5859785990228289,
            "Memory in Mb": 1.321636199951172,
            "Time in s": 2543.839083
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6069131515605887,
            "MicroF1": 0.6069131515605887,
            "MacroF1": 0.587737290445056,
            "Memory in Mb": 1.321758270263672,
            "Time in s": 2757.206681
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6094927838175689,
            "MicroF1": 0.6094927838175689,
            "MacroF1": 0.5895162861993263,
            "Memory in Mb": 1.321758270263672,
            "Time in s": 2979.334505
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6105991622655254,
            "MicroF1": 0.6105991622655254,
            "MacroF1": 0.5896134687358237,
            "Memory in Mb": 1.321941375732422,
            "Time in s": 3211.082358
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6106064326049595,
            "MicroF1": 0.6106064326049595,
            "MacroF1": 0.5910741826972655,
            "Memory in Mb": 1.321941375732422,
            "Time in s": 3451.544855
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6099029323231981,
            "MicroF1": 0.6099029323231981,
            "MacroF1": 0.5935355609859342,
            "Memory in Mb": 1.321941375732422,
            "Time in s": 3700.712954
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6088887437546942,
            "MicroF1": 0.6088887437546942,
            "MacroF1": 0.5952474102625339,
            "Memory in Mb": 1.321453094482422,
            "Time in s": 3958.532225
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6088891694813598,
            "MicroF1": 0.6088891694813598,
            "MacroF1": 0.5975058139751561,
            "Memory in Mb": 1.321697235107422,
            "Time in s": 4224.837575
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6095921796242554,
            "MicroF1": 0.6095921796242554,
            "MacroF1": 0.5998546240309938,
            "Memory in Mb": 1.321758270263672,
            "Time in s": 4499.473663
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6043917019324673,
            "MicroF1": 0.6043917019324673,
            "MacroF1": 0.595080118632132,
            "Memory in Mb": 0.6649713516235352,
            "Time in s": 4783.331389999999
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6034378856142566,
            "MicroF1": 0.6034378856142566,
            "MacroF1": 0.5941773754098104,
            "Memory in Mb": 0.6650934219360352,
            "Time in s": 5073.360361999999
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6029022644347269,
            "MicroF1": 0.6029022644347269,
            "MacroF1": 0.5935512429191343,
            "Memory in Mb": 0.6651544570922852,
            "Time in s": 5369.406481999999
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6013690846613815,
            "MicroF1": 0.6013690846613815,
            "MacroF1": 0.5919623858291095,
            "Memory in Mb": 0.6651544570922852,
            "Time in s": 5671.388488999999
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6010259108246745,
            "MicroF1": 0.6010259108246745,
            "MacroF1": 0.5912597483191937,
            "Memory in Mb": 0.6651544570922852,
            "Time in s": 5979.127636999999
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6003429653707353,
            "MicroF1": 0.6003429653707353,
            "MacroF1": 0.5902279082897147,
            "Memory in Mb": 0.6648492813110352,
            "Time in s": 6292.481400999999
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5961322800109652,
            "MicroF1": 0.5961322800109652,
            "MacroF1": 0.5867765456240649,
            "Memory in Mb": 0.6648492813110352,
            "Time in s": 6611.499413
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5939829541315591,
            "MicroF1": 0.5939829541315591,
            "MacroF1": 0.585290407267574,
            "Memory in Mb": 0.6650323867797852,
            "Time in s": 6936.132393
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5925803167688629,
            "MicroF1": 0.5925803167688629,
            "MacroF1": 0.5844470095695741,
            "Memory in Mb": 0.6650934219360352,
            "Time in s": 7266.407125
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5911306155445202,
            "MicroF1": 0.5911306155445202,
            "MacroF1": 0.5835517912214992,
            "Memory in Mb": 0.6651544570922852,
            "Time in s": 7602.391688
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.58959211742689,
            "MicroF1": 0.58959211742689,
            "MacroF1": 0.58246410272577,
            "Memory in Mb": 1.1046571731567385,
            "Time in s": 7943.862096
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5875746030347744,
            "MicroF1": 0.5875746030347744,
            "MacroF1": 0.5808874407233396,
            "Memory in Mb": 1.3207244873046875,
            "Time in s": 8291.951918
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5862083808621914,
            "MicroF1": 0.5862083808621914,
            "MacroF1": 0.5791892600330408,
            "Memory in Mb": 1.3209075927734375,
            "Time in s": 8644.890712
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5879332477535302,
            "MicroF1": 0.5879332477535302,
            "MacroF1": 0.5810233099134106,
            "Memory in Mb": 1.3210525512695312,
            "Time in s": 9004.012781000001
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5928152341739578,
            "MicroF1": 0.5928152341739578,
            "MacroF1": 0.5858160887305829,
            "Memory in Mb": 1.3216018676757812,
            "Time in s": 9370.107000000002
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.5979327436481231,
            "MicroF1": 0.5979327436481231,
            "MacroF1": 0.5906079347867982,
            "Memory in Mb": 1.3215408325195312,
            "Time in s": 9743.028377000002
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6027383747311934,
            "MicroF1": 0.6027383747311934,
            "MacroF1": 0.594893758427483,
            "Memory in Mb": 1.3217239379882812,
            "Time in s": 10122.858893000002
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6077923583866417,
            "MicroF1": 0.6077923583866417,
            "MacroF1": 0.5993180348311721,
            "Memory in Mb": 1.3217239379882812,
            "Time in s": 10509.572003000005
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.612985094414667,
            "MicroF1": 0.612985094414667,
            "MacroF1": 0.6039181082054342,
            "Memory in Mb": 0.1438255310058593,
            "Time in s": 10901.200853000002
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Insects",
            "Accuracy": 0.6133366132420005,
            "MicroF1": 0.6133366132420005,
            "MacroF1": 0.604218855594392,
            "Memory in Mb": 0.1438255310058593,
            "Time in s": 11292.868844000002
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.9803439803439804,
            "MicroF1": 0.9803439803439804,
            "MacroF1": 0.4950372208436724,
            "Memory in Mb": 0.230626106262207,
            "Time in s": 0.871514
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.943558282208589,
            "MicroF1": 0.943558282208589,
            "MacroF1": 0.7669956277713079,
            "Memory in Mb": 0.3262500762939453,
            "Time in s": 3.583779
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8863450531479967,
            "MicroF1": 0.8863450531479967,
            "MacroF1": 0.8786592421362933,
            "Memory in Mb": 0.4218740463256836,
            "Time in s": 8.686347999999999
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.891477621091355,
            "MicroF1": 0.891477621091355,
            "MacroF1": 0.8818548670971931,
            "Memory in Mb": 0.5179252624511719,
            "Time in s": 16.685395
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.889651790093183,
            "MicroF1": 0.889651790093183,
            "MacroF1": 0.8812768038030504,
            "Memory in Mb": 0.6251459121704102,
            "Time in s": 28.245741
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8414384961176952,
            "MicroF1": 0.8414384961176952,
            "MacroF1": 0.8420581397672002,
            "Memory in Mb": 0.7206478118896484,
            "Time in s": 43.571154
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8500875656742557,
            "MicroF1": 0.8500875656742557,
            "MacroF1": 0.8345582037188519,
            "Memory in Mb": 0.8163328170776367,
            "Time in s": 63.099422
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8406374501992032,
            "MicroF1": 0.8406374501992032,
            "MacroF1": 0.8151418555553325,
            "Memory in Mb": 0.911895751953125,
            "Time in s": 87.33095300000001
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8321983110868973,
            "MicroF1": 0.8321983110868973,
            "MacroF1": 0.8307198315203921,
            "Memory in Mb": 1.0075807571411133,
            "Time in s": 116.498805
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.826182887962736,
            "MicroF1": 0.826182887962736,
            "MacroF1": 0.8123767856033619,
            "Memory in Mb": 1.128366470336914,
            "Time in s": 151.118073
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.809226654780477,
            "MicroF1": 0.809226654780477,
            "MacroF1": 0.8196273526663149,
            "Memory in Mb": 1.2239294052124023,
            "Time in s": 191.820305
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8081716036772216,
            "MicroF1": 0.8081716036772216,
            "MacroF1": 0.815232111826365,
            "Memory in Mb": 1.3194313049316406,
            "Time in s": 239.061616
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.8057703186875353,
            "MicroF1": 0.8057703186875353,
            "MacroF1": 0.7903391475861199,
            "Memory in Mb": 1.415055274963379,
            "Time in s": 293.29488000000003
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7860269655051655,
            "MicroF1": 0.7860269655051656,
            "MacroF1": 0.7895763142947654,
            "Memory in Mb": 1.5108013153076172,
            "Time in s": 355.22640600000005
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.784441902271613,
            "MicroF1": 0.784441902271613,
            "MacroF1": 0.7657785418705475,
            "Memory in Mb": 1.6062421798706057,
            "Time in s": 425.240619
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7585414432357898,
            "MicroF1": 0.7585414432357898,
            "MacroF1": 0.751418836389106,
            "Memory in Mb": 1.7020492553710938,
            "Time in s": 503.467226
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7473684210526316,
            "MicroF1": 0.7473684210526316,
            "MacroF1": 0.7484284412750404,
            "Memory in Mb": 1.797490119934082,
            "Time in s": 590.6999010000001
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7565027917744791,
            "MicroF1": 0.7565027917744791,
            "MacroF1": 0.7526701844923946,
            "Memory in Mb": 1.8947620391845703,
            "Time in s": 687.248946
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7577086827506129,
            "MicroF1": 0.7577086827506129,
            "MacroF1": 0.755735065870518,
            "Memory in Mb": 1.9903860092163088,
            "Time in s": 793.498598
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7617355068023042,
            "MicroF1": 0.7617355068023042,
            "MacroF1": 0.7576049653668414,
            "Memory in Mb": 2.085948944091797,
            "Time in s": 909.902095
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7604762460604646,
            "MicroF1": 0.7604762460604646,
            "MacroF1": 0.7596175662696861,
            "Memory in Mb": 2.2296838760375977,
            "Time in s": 1036.556796
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.756991643454039,
            "MicroF1": 0.7569916434540391,
            "MacroF1": 0.7575313939177277,
            "Memory in Mb": 2.325368881225586,
            "Time in s": 1173.436632
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7558350207822658,
            "MicroF1": 0.7558350207822658,
            "MacroF1": 0.7548436696787698,
            "Memory in Mb": 2.420870780944824,
            "Time in s": 1320.145727
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.748340312531917,
            "MicroF1": 0.7483403125319169,
            "MacroF1": 0.744390859626019,
            "Memory in Mb": 2.5164337158203125,
            "Time in s": 1476.992513
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7393862143347387,
            "MicroF1": 0.7393862143347387,
            "MacroF1": 0.7315892779928432,
            "Memory in Mb": 2.612057685852051,
            "Time in s": 1644.1937280000002
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7196191194494201,
            "MicroF1": 0.7196191194494201,
            "MacroF1": 0.7089541376321258,
            "Memory in Mb": 2.707803726196289,
            "Time in s": 1822.193822
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7123921924648207,
            "MicroF1": 0.7123921924648208,
            "MacroF1": 0.7092068316988943,
            "Memory in Mb": 2.8033666610717773,
            "Time in s": 2011.0989090000005
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7062943184802591,
            "MicroF1": 0.7062943184802591,
            "MacroF1": 0.6946713230955313,
            "Memory in Mb": 2.898990631103516,
            "Time in s": 2211.8042590000005
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6967289324655566,
            "MicroF1": 0.6967289324655566,
            "MacroF1": 0.690232830798306,
            "Memory in Mb": 2.994553565979004,
            "Time in s": 2423.5715250000003
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7007108423890841,
            "MicroF1": 0.7007108423890841,
            "MacroF1": 0.6983689907908355,
            "Memory in Mb": 3.090177536010742,
            "Time in s": 2646.6754960000003
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6969241717403337,
            "MicroF1": 0.6969241717403337,
            "MacroF1": 0.6892508246262707,
            "Memory in Mb": 3.1858625411987305,
            "Time in s": 2881.7592360000003
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6836461126005362,
            "MicroF1": 0.6836461126005362,
            "MacroF1": 0.6755391962059192,
            "Memory in Mb": 3.2815475463867188,
            "Time in s": 3128.5577150000004
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6793433855752804,
            "MicroF1": 0.6793433855752804,
            "MacroF1": 0.6754035266161623,
            "Memory in Mb": 3.377110481262207,
            "Time in s": 3387.355816
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6769519140653161,
            "MicroF1": 0.6769519140653161,
            "MacroF1": 0.6742482232309566,
            "Memory in Mb": 3.4728565216064453,
            "Time in s": 3658.0697
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6728762518383641,
            "MicroF1": 0.6728762518383641,
            "MacroF1": 0.6689356443053495,
            "Memory in Mb": 3.5684194564819336,
            "Time in s": 3940.688111
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6762442976782188,
            "MicroF1": 0.6762442976782188,
            "MacroF1": 0.6753292472514647,
            "Memory in Mb": 3.663982391357422,
            "Time in s": 4235.610853
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6830076184166942,
            "MicroF1": 0.6830076184166942,
            "MacroF1": 0.6822311287838643,
            "Memory in Mb": 3.75966739654541,
            "Time in s": 4542.8267670000005
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6818035218989873,
            "MicroF1": 0.6818035218989873,
            "MacroF1": 0.6788656596145114,
            "Memory in Mb": 3.8552303314208975,
            "Time in s": 4862.152597
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6816039218150964,
            "MicroF1": 0.6816039218150964,
            "MacroF1": 0.6801525397911032,
            "Memory in Mb": 0.2705574035644531,
            "Time in s": 5190.397888
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6858263373981249,
            "MicroF1": 0.6858263373981249,
            "MacroF1": 0.685191280018575,
            "Memory in Mb": 0.4621334075927734,
            "Time in s": 5522.880902000001
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6896634184253004,
            "MicroF1": 0.6896634184253004,
            "MacroF1": 0.6890226069872224,
            "Memory in Mb": 0.6535873413085938,
            "Time in s": 5860.018685000001
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6925007295010213,
            "MicroF1": 0.6925007295010213,
            "MacroF1": 0.6918635442211969,
            "Memory in Mb": 0.9691534042358398,
            "Time in s": 6202.345681000001
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.6990252522373597,
            "MicroF1": 0.6990252522373597,
            "MacroF1": 0.6986638608261282,
            "Memory in Mb": 0.2649049758911133,
            "Time in s": 6547.073149000001
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7038605091638349,
            "MicroF1": 0.7038605091638349,
            "MacroF1": 0.7032543903990934,
            "Memory in Mb": 0.579315185546875,
            "Time in s": 6893.121988000001
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.710114930007081,
            "MicroF1": 0.7101149300070809,
            "MacroF1": 0.70950849929648,
            "Memory in Mb": 0.2349414825439453,
            "Time in s": 7240.035665000001
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.715351414717323,
            "MicroF1": 0.715351414717323,
            "MacroF1": 0.7146010079934133,
            "Memory in Mb": 0.3305654525756836,
            "Time in s": 7588.155090000001
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7179139504563233,
            "MicroF1": 0.7179139504563233,
            "MacroF1": 0.7169858006379833,
            "Memory in Mb": 0.4260063171386719,
            "Time in s": 7937.751954000001
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7223612316805392,
            "MicroF1": 0.7223612316805392,
            "MacroF1": 0.7214649429496548,
            "Memory in Mb": 0.5217523574829102,
            "Time in s": 8289.115139000001
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7219248661897854,
            "MicroF1": 0.7219248661897855,
            "MacroF1": 0.7206428236711905,
            "Memory in Mb": 0.6287288665771484,
            "Time in s": 8642.591702000002
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Hoeffding Adaptive Tree",
            "dataset": "Keystroke",
            "Accuracy": 0.7231236825334575,
            "MicroF1": 0.7231236825334575,
            "MacroF1": 0.7218249685926471,
            "Memory in Mb": 0.7244749069213867,
            "Time in s": 8998.461289
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.4222222222222222,
            "MicroF1": 0.4222222222222222,
            "MacroF1": 0.3590236094437775,
            "Memory in Mb": 0.9685115814208984,
            "Time in s": 1.326052
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.5604395604395604,
            "MicroF1": 0.5604395604395604,
            "MacroF1": 0.5746538615446178,
            "Memory in Mb": 1.0556058883666992,
            "Time in s": 4.053487
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.5766423357664233,
            "MicroF1": 0.5766423357664233,
            "MacroF1": 0.598257695340355,
            "Memory in Mb": 1.344954490661621,
            "Time in s": 8.154789999999998
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6229508196721312,
            "MicroF1": 0.6229508196721312,
            "MacroF1": 0.6451744040758778,
            "Memory in Mb": 1.4133405685424805,
            "Time in s": 13.553012999999998
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6506550218340611,
            "MicroF1": 0.6506550218340611,
            "MacroF1": 0.6680655280025949,
            "Memory in Mb": 1.5576086044311523,
            "Time in s": 20.188933
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6727272727272727,
            "MicroF1": 0.6727272727272727,
            "MacroF1": 0.6900672130049011,
            "Memory in Mb": 1.7550430297851562,
            "Time in s": 28.051384
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7040498442367601,
            "MicroF1": 0.7040498442367601,
            "MacroF1": 0.7087861936875776,
            "Memory in Mb": 1.832967758178711,
            "Time in s": 37.15395
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7302452316076294,
            "MicroF1": 0.7302452316076294,
            "MacroF1": 0.7285991575377422,
            "Memory in Mb": 1.971024513244629,
            "Time in s": 47.432602
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7457627118644068,
            "MicroF1": 0.7457627118644068,
            "MacroF1": 0.7430362907281778,
            "Memory in Mb": 1.991847038269043,
            "Time in s": 58.97377399999999
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7342047930283224,
            "MicroF1": 0.7342047930283224,
            "MacroF1": 0.7271744800226857,
            "Memory in Mb": 1.8101978302001955,
            "Time in s": 71.823928
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7405940594059406,
            "MicroF1": 0.7405940594059406,
            "MacroF1": 0.7304322149686578,
            "Memory in Mb": 1.7132930755615234,
            "Time in s": 85.827474
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7368421052631579,
            "MicroF1": 0.7368421052631579,
            "MacroF1": 0.7267508109083203,
            "Memory in Mb": 1.5079193115234375,
            "Time in s": 101.049314
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7403685092127303,
            "MicroF1": 0.7403685092127302,
            "MacroF1": 0.7318978254380314,
            "Memory in Mb": 1.6471452713012695,
            "Time in s": 117.420156
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7325038880248833,
            "MicroF1": 0.7325038880248833,
            "MacroF1": 0.7248107612258207,
            "Memory in Mb": 1.7740907669067385,
            "Time in s": 135.017443
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7242380261248186,
            "MicroF1": 0.7242380261248187,
            "MacroF1": 0.7153272190465999,
            "Memory in Mb": 1.913142204284668,
            "Time in s": 153.656893
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7251700680272108,
            "MicroF1": 0.725170068027211,
            "MacroF1": 0.7148466398758337,
            "Memory in Mb": 2.0619029998779297,
            "Time in s": 173.429455
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7259923175416133,
            "MicroF1": 0.7259923175416134,
            "MacroF1": 0.7134712280209221,
            "Memory in Mb": 2.0208959579467773,
            "Time in s": 194.315292
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.727932285368803,
            "MicroF1": 0.727932285368803,
            "MacroF1": 0.7177600265828429,
            "Memory in Mb": 2.224555015563965,
            "Time in s": 216.352158
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7353951890034365,
            "MicroF1": 0.7353951890034366,
            "MacroF1": 0.7262567978322628,
            "Memory in Mb": 2.300021171569824,
            "Time in s": 239.599524
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7431991294885746,
            "MicroF1": 0.7431991294885745,
            "MacroF1": 0.7345004589126253,
            "Memory in Mb": 2.4412155151367188,
            "Time in s": 263.99359400000003
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7471502590673575,
            "MicroF1": 0.7471502590673575,
            "MacroF1": 0.7368855656689403,
            "Memory in Mb": 2.474191665649414,
            "Time in s": 289.66420500000004
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7546983184965381,
            "MicroF1": 0.754698318496538,
            "MacroF1": 0.7446216664767904,
            "Memory in Mb": 2.5655078887939453,
            "Time in s": 316.44421900000003
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.760643330179754,
            "MicroF1": 0.760643330179754,
            "MacroF1": 0.7502594177262459,
            "Memory in Mb": 2.798956871032715,
            "Time in s": 344.45448600000003
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7624660018132366,
            "MicroF1": 0.7624660018132366,
            "MacroF1": 0.7523020427630668,
            "Memory in Mb": 2.48898983001709,
            "Time in s": 373.71735
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7650130548302873,
            "MicroF1": 0.7650130548302874,
            "MacroF1": 0.7555087521342715,
            "Memory in Mb": 2.3284912109375,
            "Time in s": 404.061966
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7690376569037657,
            "MicroF1": 0.7690376569037657,
            "MacroF1": 0.7603504370239861,
            "Memory in Mb": 2.0560731887817383,
            "Time in s": 435.510035
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7719580983078163,
            "MicroF1": 0.7719580983078163,
            "MacroF1": 0.7638249032322542,
            "Memory in Mb": 2.11933708190918,
            "Time in s": 467.969641
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7746697746697747,
            "MicroF1": 0.7746697746697747,
            "MacroF1": 0.7668828628349821,
            "Memory in Mb": 2.277647018432617,
            "Time in s": 501.448754
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7771942985746436,
            "MicroF1": 0.7771942985746436,
            "MacroF1": 0.7696789046658701,
            "Memory in Mb": 2.3871631622314453,
            "Time in s": 535.887669
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7817258883248731,
            "MicroF1": 0.7817258883248731,
            "MacroF1": 0.7754511149783997,
            "Memory in Mb": 2.3104944229125977,
            "Time in s": 571.357393
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7866666666666666,
            "MicroF1": 0.7866666666666666,
            "MacroF1": 0.7797171864703156,
            "Memory in Mb": 2.4089183807373047,
            "Time in s": 607.784244
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7912984364377974,
            "MicroF1": 0.7912984364377974,
            "MacroF1": 0.7836430453045393,
            "Memory in Mb": 2.5425024032592773,
            "Time in s": 645.2286509999999
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7963085036255768,
            "MicroF1": 0.7963085036255768,
            "MacroF1": 0.7883976288226553,
            "Memory in Mb": 2.6389265060424805,
            "Time in s": 683.7451019999999
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7978246960972489,
            "MicroF1": 0.7978246960972489,
            "MacroF1": 0.790949738475821,
            "Memory in Mb": 2.283763885498047,
            "Time in s": 723.3862519999999
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.798011187072716,
            "MicroF1": 0.7980111870727161,
            "MacroF1": 0.7914720525222512,
            "Memory in Mb": 2.519012451171875,
            "Time in s": 764.1312649999999
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7981873111782477,
            "MicroF1": 0.7981873111782477,
            "MacroF1": 0.7919320984228655,
            "Memory in Mb": 2.307619094848633,
            "Time in s": 806.0160599999999
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.798941798941799,
            "MicroF1": 0.7989417989417988,
            "MacroF1": 0.7945012991620244,
            "Memory in Mb": 2.40640926361084,
            "Time in s": 848.960292
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8019461934745278,
            "MicroF1": 0.8019461934745278,
            "MacroF1": 0.797056036319667,
            "Memory in Mb": 2.447686195373535,
            "Time in s": 893.037184
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8047964305633017,
            "MicroF1": 0.8047964305633019,
            "MacroF1": 0.7993493873930555,
            "Memory in Mb": 2.5208606719970703,
            "Time in s": 938.202728
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8069603045133225,
            "MicroF1": 0.8069603045133223,
            "MacroF1": 0.8019867749609348,
            "Memory in Mb": 2.8025121688842773,
            "Time in s": 984.592034
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8084880636604774,
            "MicroF1": 0.8084880636604774,
            "MacroF1": 0.8043300839686539,
            "Memory in Mb": 2.9287471771240234,
            "Time in s": 1032.221691
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8114966338684619,
            "MicroF1": 0.8114966338684619,
            "MacroF1": 0.8071482324590065,
            "Memory in Mb": 2.977842330932617,
            "Time in s": 1081.048247
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8148710166919575,
            "MicroF1": 0.8148710166919576,
            "MacroF1": 0.8107088256390683,
            "Memory in Mb": 3.110445022583008,
            "Time in s": 1130.994965
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8161146811665843,
            "MicroF1": 0.8161146811665844,
            "MacroF1": 0.8110472160986095,
            "Memory in Mb": 3.3117494583129883,
            "Time in s": 1182.226115
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8173030449492509,
            "MicroF1": 0.8173030449492509,
            "MacroF1": 0.8127793203399477,
            "Memory in Mb": 2.7790603637695312,
            "Time in s": 1234.703432
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8193853427895981,
            "MicroF1": 0.8193853427895981,
            "MacroF1": 0.8144282151100146,
            "Memory in Mb": 2.8652515411376958,
            "Time in s": 1288.356269
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8199907450254512,
            "MicroF1": 0.8199907450254512,
            "MacroF1": 0.8150157846003385,
            "Memory in Mb": 2.925917625427246,
            "Time in s": 1343.2838700000002
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8205709107385591,
            "MicroF1": 0.8205709107385591,
            "MacroF1": 0.8153449009635614,
            "Memory in Mb": 2.785597801208496,
            "Time in s": 1399.325285
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8175765645805593,
            "MicroF1": 0.8175765645805593,
            "MacroF1": 0.813116129924445,
            "Memory in Mb": 2.868098258972168,
            "Time in s": 1456.6402850000002
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8186167899086559,
            "MicroF1": 0.8186167899086559,
            "MacroF1": 0.8144518819207099,
            "Memory in Mb": 3.062863349914551,
            "Time in s": 1515.2003170000005
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8185361628410567,
            "MicroF1": 0.8185361628410566,
            "MacroF1": 0.8145347387119569,
            "Memory in Mb": 3.063481330871582,
            "Time in s": 1574.1800910000002
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.6682464454976303,
            "MicroF1": 0.6682464454976303,
            "MacroF1": 0.6049011732627783,
            "Memory in Mb": 7.181946754455566,
            "Time in s": 32.418226
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.6944576030317385,
            "MicroF1": 0.6944576030317385,
            "MacroF1": 0.6288311688548281,
            "Memory in Mb": 9.89784336090088,
            "Time in s": 94.873564
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.6984527944426903,
            "MicroF1": 0.6984527944426903,
            "MacroF1": 0.625371849015863,
            "Memory in Mb": 13.448436737060549,
            "Time in s": 186.837042
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.706369879232773,
            "MicroF1": 0.706369879232773,
            "MacroF1": 0.6266042661686886,
            "Memory in Mb": 17.43436622619629,
            "Time in s": 307.272577
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7107406705815495,
            "MicroF1": 0.7107406705815495,
            "MacroF1": 0.6273487761971507,
            "Memory in Mb": 20.93905258178711,
            "Time in s": 452.99825
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7108129439621153,
            "MicroF1": 0.7108129439621153,
            "MacroF1": 0.6274052515282983,
            "Memory in Mb": 25.022296905517575,
            "Time in s": 622.602665
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7127587606548504,
            "MicroF1": 0.7127587606548504,
            "MacroF1": 0.6273117178459473,
            "Memory in Mb": 28.81925773620605,
            "Time in s": 816.020547
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7164673848703682,
            "MicroF1": 0.7164673848703682,
            "MacroF1": 0.6293431255193823,
            "Memory in Mb": 32.80279922485352,
            "Time in s": 1032.257355
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.721666842049879,
            "MicroF1": 0.721666842049879,
            "MacroF1": 0.63170101976307,
            "Memory in Mb": 32.88048076629639,
            "Time in s": 1271.699652
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.724405720238659,
            "MicroF1": 0.724405720238659,
            "MacroF1": 0.6339052025360064,
            "Memory in Mb": 29.71586036682129,
            "Time in s": 1533.827375
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7244080929832114,
            "MicroF1": 0.7244080929832114,
            "MacroF1": 0.6334336343217646,
            "Memory in Mb": 33.71169948577881,
            "Time in s": 1818.162347
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7225949017441402,
            "MicroF1": 0.7225949017441402,
            "MacroF1": 0.6332595599893077,
            "Memory in Mb": 29.64934635162353,
            "Time in s": 2125.062078
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7416769869600058,
            "MicroF1": 0.7416769869600057,
            "MacroF1": 0.7385871869253197,
            "Memory in Mb": 11.750191688537598,
            "Time in s": 2443.236189
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7472096326861936,
            "MicroF1": 0.7472096326861937,
            "MacroF1": 0.7473000008879964,
            "Memory in Mb": 7.712667465209961,
            "Time in s": 2772.229259
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7404507860344719,
            "MicroF1": 0.7404507860344719,
            "MacroF1": 0.7427443120881612,
            "Memory in Mb": 5.854048728942871,
            "Time in s": 3118.280673
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.73666765315182,
            "MicroF1": 0.73666765315182,
            "MacroF1": 0.7407696345938622,
            "Memory in Mb": 9.543391227722168,
            "Time in s": 3480.1200929999995
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7295972369227341,
            "MicroF1": 0.7295972369227341,
            "MacroF1": 0.7347001031972082,
            "Memory in Mb": 14.625198364257812,
            "Time in s": 3856.632275
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.739780081022781,
            "MicroF1": 0.7397800810227809,
            "MacroF1": 0.7407912307996387,
            "Memory in Mb": 5.110816955566406,
            "Time in s": 4245.133706999999
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7434581069630664,
            "MicroF1": 0.7434581069630664,
            "MacroF1": 0.7402037922066672,
            "Memory in Mb": 3.8148155212402335,
            "Time in s": 4646.574114999999
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.745111037454425,
            "MicroF1": 0.7451110374544251,
            "MacroF1": 0.7386209934273732,
            "Memory in Mb": 7.313493728637695,
            "Time in s": 5063.578879
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7462006764374295,
            "MicroF1": 0.7462006764374295,
            "MacroF1": 0.7365944363606786,
            "Memory in Mb": 12.210733413696287,
            "Time in s": 5495.973683
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7483965391072274,
            "MicroF1": 0.7483965391072274,
            "MacroF1": 0.7360584061499352,
            "Memory in Mb": 11.241872787475586,
            "Time in s": 5944.2105440000005
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7495779635195784,
            "MicroF1": 0.7495779635195785,
            "MacroF1": 0.7345443205753824,
            "Memory in Mb": 12.262273788452148,
            "Time in s": 6407.867088000001
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7508582251509293,
            "MicroF1": 0.7508582251509293,
            "MacroF1": 0.7336140903014292,
            "Memory in Mb": 15.815716743469238,
            "Time in s": 6885.995097000001
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7510890564036516,
            "MicroF1": 0.7510890564036516,
            "MacroF1": 0.7317409587301968,
            "Memory in Mb": 20.072275161743164,
            "Time in s": 7378.034229000001
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7520670187579676,
            "MicroF1": 0.7520670187579677,
            "MacroF1": 0.7304776676466566,
            "Memory in Mb": 23.249674797058105,
            "Time in s": 7884.702304
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7487285609063169,
            "MicroF1": 0.7487285609063169,
            "MacroF1": 0.7285292321096271,
            "Memory in Mb": 2.702430725097656,
            "Time in s": 8406.670172
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7464741096492712,
            "MicroF1": 0.7464741096492712,
            "MacroF1": 0.7309964825863351,
            "Memory in Mb": 6.2935638427734375,
            "Time in s": 8940.901067
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7457793162002416,
            "MicroF1": 0.7457793162002416,
            "MacroF1": 0.7347045068936117,
            "Memory in Mb": 9.350909233093262,
            "Time in s": 9487.04409
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.745036143817671,
            "MicroF1": 0.745036143817671,
            "MacroF1": 0.7375864352537521,
            "Memory in Mb": 14.599569320678713,
            "Time in s": 10044.836672
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7451962731021842,
            "MicroF1": 0.7451962731021842,
            "MacroF1": 0.7406480970104784,
            "Memory in Mb": 19.12519836425781,
            "Time in s": 10615.117300000002
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7402858749371134,
            "MicroF1": 0.7402858749371134,
            "MacroF1": 0.7370798749337869,
            "Memory in Mb": 6.808139801025391,
            "Time in s": 11202.653786000004
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7366200820730623,
            "MicroF1": 0.7366200820730623,
            "MacroF1": 0.7333315604235389,
            "Memory in Mb": 5.8602495193481445,
            "Time in s": 11807.700361000005
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.733921956382475,
            "MicroF1": 0.7339219563824751,
            "MacroF1": 0.7303171015411175,
            "Memory in Mb": 9.36469554901123,
            "Time in s": 12429.747970000002
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7304039611461349,
            "MicroF1": 0.7304039611461349,
            "MacroF1": 0.7265687877692525,
            "Memory in Mb": 14.848862648010254,
            "Time in s": 13069.446785000002
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7276864395633302,
            "MicroF1": 0.7276864395633302,
            "MacroF1": 0.7236022807953257,
            "Memory in Mb": 19.807891845703125,
            "Time in s": 13727.939023000004
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7250134370760922,
            "MicroF1": 0.7250134370760921,
            "MacroF1": 0.7209989950382084,
            "Memory in Mb": 16.71243381500244,
            "Time in s": 14405.601845000005
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7235028783612032,
            "MicroF1": 0.7235028783612032,
            "MacroF1": 0.7198278735760195,
            "Memory in Mb": 8.331427574157715,
            "Time in s": 15101.835691000002
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.723623825364835,
            "MicroF1": 0.723623825364835,
            "MacroF1": 0.7203262236880287,
            "Memory in Mb": 6.9819841384887695,
            "Time in s": 15814.868539000005
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7240464973129098,
            "MicroF1": 0.7240464973129098,
            "MacroF1": 0.7211005399097123,
            "Memory in Mb": 10.71219539642334,
            "Time in s": 16543.112989
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7245409400623629,
            "MicroF1": 0.7245409400623629,
            "MacroF1": 0.721844297210525,
            "Memory in Mb": 10.330558776855469,
            "Time in s": 17285.760894000003
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7248765529525828,
            "MicroF1": 0.7248765529525828,
            "MacroF1": 0.7223628081683402,
            "Memory in Mb": 13.299851417541504,
            "Time in s": 18041.694028
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7254167859581122,
            "MicroF1": 0.7254167859581122,
            "MacroF1": 0.7228420559832612,
            "Memory in Mb": 15.662115097045898,
            "Time in s": 18810.181113
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7263844349267159,
            "MicroF1": 0.7263844349267159,
            "MacroF1": 0.7236482152790997,
            "Memory in Mb": 19.25161361694336,
            "Time in s": 19591.516438
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7265304404553968,
            "MicroF1": 0.7265304404553967,
            "MacroF1": 0.7240124567772878,
            "Memory in Mb": 14.065608024597168,
            "Time in s": 20387.990038000004
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7304374678332476,
            "MicroF1": 0.7304374678332476,
            "MacroF1": 0.7281756207358935,
            "Memory in Mb": 7.354809761047363,
            "Time in s": 21197.413376000004
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7344603171404969,
            "MicroF1": 0.7344603171404969,
            "MacroF1": 0.7322565876518081,
            "Memory in Mb": 7.006095886230469,
            "Time in s": 22016.972025000003
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7380590684001815,
            "MicroF1": 0.7380590684001815,
            "MacroF1": 0.7356981427827818,
            "Memory in Mb": 10.14159107208252,
            "Time in s": 22847.182754
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7420134124422627,
            "MicroF1": 0.7420134124422627,
            "MacroF1": 0.7394134340953542,
            "Memory in Mb": 13.563420295715332,
            "Time in s": 23688.037606
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7451466883842497,
            "MicroF1": 0.7451466883842497,
            "MacroF1": 0.7430487162081567,
            "Memory in Mb": 0.3614501953125,
            "Time in s": 24535.706056000003
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Insects",
            "Accuracy": 0.7453781671618067,
            "MicroF1": 0.7453781671618067,
            "MacroF1": 0.7433023109254195,
            "Memory in Mb": 0.3617935180664062,
            "Time in s": 25383.518073000003
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9803439803439804,
            "MicroF1": 0.9803439803439804,
            "MacroF1": 0.4950372208436724,
            "Memory in Mb": 0.3354053497314453,
            "Time in s": 3.23067
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9730061349693252,
            "MicroF1": 0.9730061349693252,
            "MacroF1": 0.8116978142719798,
            "Memory in Mb": 0.988037109375,
            "Time in s": 11.21298
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9730171708912512,
            "MicroF1": 0.9730171708912512,
            "MacroF1": 0.9579161898493525,
            "Memory in Mb": 2.195523262023926,
            "Time in s": 25.427007
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9693439607602696,
            "MicroF1": 0.9693439607602696,
            "MacroF1": 0.9069773132409142,
            "Memory in Mb": 3.526730537414551,
            "Time in s": 46.453054
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9666503187837177,
            "MicroF1": 0.9666503187837177,
            "MacroF1": 0.9303026980117672,
            "Memory in Mb": 5.496582984924316,
            "Time in s": 74.431187
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9660809154066204,
            "MicroF1": 0.9660809154066204,
            "MacroF1": 0.955517866483744,
            "Memory in Mb": 2.29970645904541,
            "Time in s": 107.969459
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9691768826619964,
            "MicroF1": 0.9691768826619964,
            "MacroF1": 0.9674134048328416,
            "Memory in Mb": 3.376467704772949,
            "Time in s": 146.96126800000002
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9672080907140668,
            "MicroF1": 0.9672080907140668,
            "MacroF1": 0.9546197483047236,
            "Memory in Mb": 4.62060546875,
            "Time in s": 192.073824
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9684009806592208,
            "MicroF1": 0.968400980659221,
            "MacroF1": 0.9654409635782653,
            "Memory in Mb": 3.119338035583496,
            "Time in s": 243.354323
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9644520715861732,
            "MicroF1": 0.9644520715861732,
            "MacroF1": 0.95030552665756,
            "Memory in Mb": 4.705347061157227,
            "Time in s": 301.433133
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9661243592600848,
            "MicroF1": 0.9661243592600848,
            "MacroF1": 0.9659906155964958,
            "Memory in Mb": 1.508072853088379,
            "Time in s": 365.412759
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9677221654749744,
            "MicroF1": 0.9677221654749744,
            "MacroF1": 0.96768641848376,
            "Memory in Mb": 2.487558364868164,
            "Time in s": 434.672843
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9685083914765228,
            "MicroF1": 0.9685083914765228,
            "MacroF1": 0.9677400809149086,
            "Memory in Mb": 2.8771514892578125,
            "Time in s": 509.854138
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9690071791279986,
            "MicroF1": 0.9690071791279986,
            "MacroF1": 0.968698427792926,
            "Memory in Mb": 4.140267372131348,
            "Time in s": 591.7133210000001
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9671514953423762,
            "MicroF1": 0.9671514953423762,
            "MacroF1": 0.9635575047511442,
            "Memory in Mb": 5.121949195861816,
            "Time in s": 681.1937680000001
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9675195342423778,
            "MicroF1": 0.9675195342423778,
            "MacroF1": 0.9673223823066148,
            "Memory in Mb": 2.1385393142700195,
            "Time in s": 777.2102420000001
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.968565248738284,
            "MicroF1": 0.968565248738284,
            "MacroF1": 0.9688652926813892,
            "Memory in Mb": 2.7864933013916016,
            "Time in s": 879.0640510000001
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9686776521857552,
            "MicroF1": 0.9686776521857552,
            "MacroF1": 0.9682274153773373,
            "Memory in Mb": 3.314570426940918,
            "Time in s": 987.062921
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9682621597213262,
            "MicroF1": 0.9682621597213262,
            "MacroF1": 0.9674704101631952,
            "Memory in Mb": 4.690197944641113,
            "Time in s": 1101.141854
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.96727540139723,
            "MicroF1": 0.96727540139723,
            "MacroF1": 0.9662379529396136,
            "Memory in Mb": 5.223731994628906,
            "Time in s": 1221.487909
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9677833547332788,
            "MicroF1": 0.9677833547332788,
            "MacroF1": 0.9678822443058488,
            "Memory in Mb": 4.885932922363281,
            "Time in s": 1347.980617
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9686908077994428,
            "MicroF1": 0.9686908077994428,
            "MacroF1": 0.9690861219789196,
            "Memory in Mb": 6.402636528015137,
            "Time in s": 1480.694289
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9683470105509964,
            "MicroF1": 0.9683470105509964,
            "MacroF1": 0.9680699356268632,
            "Memory in Mb": 6.928671836853027,
            "Time in s": 1620.259773
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.96864467367991,
            "MicroF1": 0.96864467367991,
            "MacroF1": 0.9687197530276812,
            "Memory in Mb": 5.552419662475586,
            "Time in s": 1766.078849
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9684282772820864,
            "MicroF1": 0.9684282772820866,
            "MacroF1": 0.9682582636163196,
            "Memory in Mb": 2.695918083190918,
            "Time in s": 1917.758924
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9673800320543038,
            "MicroF1": 0.9673800320543038,
            "MacroF1": 0.9668238422002586,
            "Memory in Mb": 3.239151954650879,
            "Time in s": 2074.190769
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9676804357694052,
            "MicroF1": 0.9676804357694052,
            "MacroF1": 0.9678040910458204,
            "Memory in Mb": 4.023995399475098,
            "Time in s": 2235.420867
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9677842948437364,
            "MicroF1": 0.9677842948437364,
            "MacroF1": 0.9678364439490078,
            "Memory in Mb": 4.695375442504883,
            "Time in s": 2402.164192
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9677119432000676,
            "MicroF1": 0.9677119432000676,
            "MacroF1": 0.9677086079179034,
            "Memory in Mb": 5.258674621582031,
            "Time in s": 2574.870699
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.968706593675954,
            "MicroF1": 0.968706593675954,
            "MacroF1": 0.9690716756618885,
            "Memory in Mb": 6.001680374145508,
            "Time in s": 2753.36713
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9688463667272872,
            "MicroF1": 0.9688463667272872,
            "MacroF1": 0.9689334511448672,
            "Memory in Mb": 5.217698097229004,
            "Time in s": 2937.769964
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9687476062811184,
            "MicroF1": 0.9687476062811184,
            "MacroF1": 0.968764477893114,
            "Memory in Mb": 5.266051292419434,
            "Time in s": 3127.802403
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9687291094109782,
            "MicroF1": 0.9687291094109782,
            "MacroF1": 0.9687736841624996,
            "Memory in Mb": 6.279603958129883,
            "Time in s": 3323.370395
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9695047220820416,
            "MicroF1": 0.9695047220820416,
            "MacroF1": 0.9697384724636318,
            "Memory in Mb": 4.041820526123047,
            "Time in s": 3524.041026
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9682750892919672,
            "MicroF1": 0.9682750892919672,
            "MacroF1": 0.9680357071263168,
            "Memory in Mb": 2.1731691360473637,
            "Time in s": 3729.110149
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9686797848437394,
            "MicroF1": 0.9686797848437394,
            "MacroF1": 0.9688099431838716,
            "Memory in Mb": 2.4900379180908203,
            "Time in s": 3938.33843
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9692613448161644,
            "MicroF1": 0.9692613448161644,
            "MacroF1": 0.9694122553904638,
            "Memory in Mb": 2.7789316177368164,
            "Time in s": 4151.996270000001
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9694897761723538,
            "MicroF1": 0.9694897761723538,
            "MacroF1": 0.969571649124791,
            "Memory in Mb": 3.946505546569824,
            "Time in s": 4370.227344000001
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9694550939601534,
            "MicroF1": 0.9694550939601534,
            "MacroF1": 0.9694916672888816,
            "Memory in Mb": 4.345325469970703,
            "Time in s": 4594.050341000001
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9695447024940254,
            "MicroF1": 0.9695447024940254,
            "MacroF1": 0.9695954968773725,
            "Memory in Mb": 3.909954071044922,
            "Time in s": 4823.361799000001
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9692114545345848,
            "MicroF1": 0.9692114545345848,
            "MacroF1": 0.9692084456743588,
            "Memory in Mb": 1.764338493347168,
            "Time in s": 5057.2303470000015
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9696527575138604,
            "MicroF1": 0.9696527575138604,
            "MacroF1": 0.9697329621491684,
            "Memory in Mb": 1.7167367935180664,
            "Time in s": 5295.013901000001
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9696745140511884,
            "MicroF1": 0.9696745140511884,
            "MacroF1": 0.9697082565052514,
            "Memory in Mb": 2.814372062683105,
            "Time in s": 5537.319837000001
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.968748259149908,
            "MicroF1": 0.968748259149908,
            "MacroF1": 0.968705960089485,
            "Memory in Mb": 2.951136589050293,
            "Time in s": 5784.484584000001
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9690070265264992,
            "MicroF1": 0.9690070265264992,
            "MacroF1": 0.9690448168177233,
            "Memory in Mb": 3.5441465377807617,
            "Time in s": 6036.117893000001
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9690946874833484,
            "MicroF1": 0.9690946874833484,
            "MacroF1": 0.9691164520527108,
            "Memory in Mb": 4.379698753356934,
            "Time in s": 6292.729193000001
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.968761408083442,
            "MicroF1": 0.968761408083442,
            "MacroF1": 0.9687617227117352,
            "Memory in Mb": 3.8120603561401367,
            "Time in s": 6554.348831000001
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9689526630240516,
            "MicroF1": 0.9689526630240516,
            "MacroF1": 0.9689629146490384,
            "Memory in Mb": 2.019772529602051,
            "Time in s": 6819.891372000001
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9692861787804512,
            "MicroF1": 0.9692861787804512,
            "MacroF1": 0.9692901573177236,
            "Memory in Mb": 1.256450653076172,
            "Time in s": 7089.584863000001
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Adaptive Random Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9691161331437816,
            "MicroF1": 0.9691161331437816,
            "MacroF1": 0.9691108096285476,
            "Memory in Mb": 1.6354646682739258,
            "Time in s": 7363.046142000001
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.5333333333333333,
            "MicroF1": 0.5333333333333333,
            "MacroF1": 0.5005728607232367,
            "Memory in Mb": 0.8510866165161133,
            "Time in s": 0.941842
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6153846153846154,
            "MicroF1": 0.6153846153846154,
            "MacroF1": 0.596131344383025,
            "Memory in Mb": 1.5052366256713867,
            "Time in s": 2.918201
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6496350364963503,
            "MicroF1": 0.6496350364963503,
            "MacroF1": 0.6567305057749026,
            "Memory in Mb": 2.146304130554199,
            "Time in s": 6.147886
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.6994535519125683,
            "MicroF1": 0.6994535519125683,
            "MacroF1": 0.7070190759413217,
            "Memory in Mb": 2.7665939331054688,
            "Time in s": 10.824064
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7379912663755459,
            "MicroF1": 0.7379912663755459,
            "MacroF1": 0.7433871451842025,
            "Memory in Mb": 3.2484235763549805,
            "Time in s": 16.931166
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7490909090909091,
            "MicroF1": 0.7490909090909091,
            "MacroF1": 0.7566070103930901,
            "Memory in Mb": 3.776392936706543,
            "Time in s": 24.729994
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7694704049844237,
            "MicroF1": 0.7694704049844237,
            "MacroF1": 0.7681721604320974,
            "Memory in Mb": 4.142314910888672,
            "Time in s": 34.173162000000005
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.784741144414169,
            "MicroF1": 0.7847411444141691,
            "MacroF1": 0.7789718513534348,
            "Memory in Mb": 4.497910499572754,
            "Time in s": 45.384105000000005
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7990314769975787,
            "MicroF1": 0.7990314769975787,
            "MacroF1": 0.7943771701942021,
            "Memory in Mb": 4.869846343994141,
            "Time in s": 58.265676000000006
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.7973856209150327,
            "MicroF1": 0.7973856209150327,
            "MacroF1": 0.7916511033189314,
            "Memory in Mb": 5.3911848068237305,
            "Time in s": 73.08883800000001
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.805940594059406,
            "MicroF1": 0.805940594059406,
            "MacroF1": 0.8010859843658406,
            "Memory in Mb": 5.806554794311523,
            "Time in s": 89.87625100000001
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8076225045372051,
            "MicroF1": 0.8076225045372051,
            "MacroF1": 0.8036838079612314,
            "Memory in Mb": 6.295863151550293,
            "Time in s": 108.5993
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8174204355108877,
            "MicroF1": 0.8174204355108878,
            "MacroF1": 0.8156009215135775,
            "Memory in Mb": 6.727802276611328,
            "Time in s": 129.48595400000002
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8211508553654744,
            "MicroF1": 0.8211508553654744,
            "MacroF1": 0.8207645722848749,
            "Memory in Mb": 7.18087100982666,
            "Time in s": 152.525841
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8229317851959361,
            "MicroF1": 0.8229317851959362,
            "MacroF1": 0.8226135245892084,
            "Memory in Mb": 7.561182022094727,
            "Time in s": 177.86541200000002
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8231292517006803,
            "MicroF1": 0.8231292517006803,
            "MacroF1": 0.8228959515200417,
            "Memory in Mb": 7.975464820861816,
            "Time in s": 205.499576
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8309859154929577,
            "MicroF1": 0.8309859154929577,
            "MacroF1": 0.8306123687436626,
            "Memory in Mb": 8.301925659179688,
            "Time in s": 235.39408200000003
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8343409915356711,
            "MicroF1": 0.834340991535671,
            "MacroF1": 0.835521648488366,
            "Memory in Mb": 8.722038269042969,
            "Time in s": 267.718494
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8407789232531501,
            "MicroF1": 0.8407789232531501,
            "MacroF1": 0.8414965916969209,
            "Memory in Mb": 9.057206153869627,
            "Time in s": 302.46008700000004
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8443960826985855,
            "MicroF1": 0.8443960826985855,
            "MacroF1": 0.8446110045111287,
            "Memory in Mb": 9.38282871246338,
            "Time in s": 339.623661
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8466321243523316,
            "MicroF1": 0.8466321243523316,
            "MacroF1": 0.8462590694093756,
            "Memory in Mb": 9.696897506713867,
            "Time in s": 379.342347
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8516320474777448,
            "MicroF1": 0.8516320474777448,
            "MacroF1": 0.8504483916737715,
            "Memory in Mb": 9.949009895324709,
            "Time in s": 421.625642
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8571428571428571,
            "MicroF1": 0.8571428571428571,
            "MacroF1": 0.8557487568785946,
            "Memory in Mb": 10.2299222946167,
            "Time in s": 466.542637
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8603807796917498,
            "MicroF1": 0.8603807796917498,
            "MacroF1": 0.8594481550185353,
            "Memory in Mb": 10.524299621582031,
            "Time in s": 514.218423
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8624891209747607,
            "MicroF1": 0.8624891209747607,
            "MacroF1": 0.8612253786789881,
            "Memory in Mb": 10.737759590148926,
            "Time in s": 564.599929
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8652719665271966,
            "MicroF1": 0.8652719665271966,
            "MacroF1": 0.8642881992026393,
            "Memory in Mb": 11.010127067565918,
            "Time in s": 617.836337
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8670427074939565,
            "MicroF1": 0.8670427074939565,
            "MacroF1": 0.8663181473795101,
            "Memory in Mb": 11.261144638061523,
            "Time in s": 674.05967
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8694638694638694,
            "MicroF1": 0.8694638694638694,
            "MacroF1": 0.8687259920464652,
            "Memory in Mb": 11.505732536315918,
            "Time in s": 733.385389
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8709677419354839,
            "MicroF1": 0.8709677419354839,
            "MacroF1": 0.870193396369452,
            "Memory in Mb": 11.826444625854492,
            "Time in s": 796.067675
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8745467730239304,
            "MicroF1": 0.8745467730239304,
            "MacroF1": 0.874089581073643,
            "Memory in Mb": 12.086430549621582,
            "Time in s": 861.584672
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8771929824561403,
            "MicroF1": 0.8771929824561403,
            "MacroF1": 0.8759011931352845,
            "Memory in Mb": 12.29430866241455,
            "Time in s": 930.204519
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8796736913664174,
            "MicroF1": 0.8796736913664174,
            "MacroF1": 0.877566397675441,
            "Memory in Mb": 12.500163078308104,
            "Time in s": 1001.8141389999998
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8826631509558339,
            "MicroF1": 0.8826631509558339,
            "MacroF1": 0.8803270226288138,
            "Memory in Mb": 12.740474700927734,
            "Time in s": 1076.488215
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8841970569417786,
            "MicroF1": 0.8841970569417786,
            "MacroF1": 0.8822041640143002,
            "Memory in Mb": 12.987508773803713,
            "Time in s": 1154.350794
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.886886264760721,
            "MicroF1": 0.886886264760721,
            "MacroF1": 0.8850836875294148,
            "Memory in Mb": 13.252826690673828,
            "Time in s": 1235.463166
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.888821752265861,
            "MicroF1": 0.888821752265861,
            "MacroF1": 0.8870702351165313,
            "Memory in Mb": 13.500110626220703,
            "Time in s": 1319.86391
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8912404467960023,
            "MicroF1": 0.8912404467960025,
            "MacroF1": 0.8905987472429445,
            "Memory in Mb": 13.767583847045898,
            "Time in s": 1407.541035
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8929593589009731,
            "MicroF1": 0.892959358900973,
            "MacroF1": 0.8920318510221457,
            "Memory in Mb": 14.030475616455078,
            "Time in s": 1498.676265
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.894032348020078,
            "MicroF1": 0.894032348020078,
            "MacroF1": 0.8925886559949978,
            "Memory in Mb": 14.271255493164062,
            "Time in s": 1593.100327
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8945078847199565,
            "MicroF1": 0.8945078847199565,
            "MacroF1": 0.8931986390525462,
            "Memory in Mb": 14.574835777282717,
            "Time in s": 1691.005218
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.896551724137931,
            "MicroF1": 0.896551724137931,
            "MacroF1": 0.8956464025201587,
            "Memory in Mb": 14.834091186523438,
            "Time in s": 1792.408733
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8964267219057483,
            "MicroF1": 0.8964267219057483,
            "MacroF1": 0.8951782213786073,
            "Memory in Mb": 15.134613037109377,
            "Time in s": 1897.156299
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8973191704602934,
            "MicroF1": 0.8973191704602934,
            "MacroF1": 0.8961901832930852,
            "Memory in Mb": 15.326050758361816,
            "Time in s": 2005.31409
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8986653484923381,
            "MicroF1": 0.8986653484923381,
            "MacroF1": 0.8970310627029995,
            "Memory in Mb": 15.549851417541504,
            "Time in s": 2116.877653
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.8994683421942967,
            "MicroF1": 0.8994683421942967,
            "MacroF1": 0.8980105869909577,
            "Memory in Mb": 15.81621551513672,
            "Time in s": 2232.114727
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.900709219858156,
            "MicroF1": 0.900709219858156,
            "MacroF1": 0.8989778942952686,
            "Memory in Mb": 15.957537651062012,
            "Time in s": 2350.8625340000003
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.9000462748727441,
            "MicroF1": 0.9000462748727441,
            "MacroF1": 0.8982611856050026,
            "Memory in Mb": 16.206623077392578,
            "Time in s": 2473.2186990000005
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.9012233801540552,
            "MicroF1": 0.9012233801540552,
            "MacroF1": 0.8993036839855942,
            "Memory in Mb": 16.400617599487305,
            "Time in s": 2599.1257530000003
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.9014647137150466,
            "MicroF1": 0.9014647137150466,
            "MacroF1": 0.8999821457114682,
            "Memory in Mb": 16.693093299865723,
            "Time in s": 2728.6827460000004
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.9016963897346671,
            "MicroF1": 0.9016963897346671,
            "MacroF1": 0.9003174232892135,
            "Memory in Mb": 16.988688468933105,
            "Time in s": 2861.834306
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "ImageSegments",
            "Accuracy": 0.9016890428757036,
            "MicroF1": 0.9016890428757036,
            "MacroF1": 0.9003808534937335,
            "Memory in Mb": 17.050235748291016,
            "Time in s": 2997.696193
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6511848341232227,
            "MicroF1": 0.6511848341232227,
            "MacroF1": 0.5805974192561721,
            "Memory in Mb": 27.882014274597168,
            "Time in s": 41.422615
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6830885836096636,
            "MicroF1": 0.6830885836096636,
            "MacroF1": 0.6159001145696381,
            "Memory in Mb": 53.9009017944336,
            "Time in s": 137.16292
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6889801073571203,
            "MicroF1": 0.6889801073571203,
            "MacroF1": 0.6135176771695448,
            "Memory in Mb": 79.45620250701904,
            "Time in s": 291.10856
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6954771489462468,
            "MicroF1": 0.6954771489462468,
            "MacroF1": 0.6159765684907534,
            "Memory in Mb": 104.90542316436768,
            "Time in s": 501.70617
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7003220306876302,
            "MicroF1": 0.7003220306876302,
            "MacroF1": 0.6217575035584229,
            "Memory in Mb": 130.7021541595459,
            "Time in s": 768.289754
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7021310181531176,
            "MicroF1": 0.7021310181531176,
            "MacroF1": 0.622391174421368,
            "Memory in Mb": 156.0168752670288,
            "Time in s": 1090.319759
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7027465836828576,
            "MicroF1": 0.7027465836828576,
            "MacroF1": 0.6232948240709647,
            "Memory in Mb": 180.8397483825684,
            "Time in s": 1466.44078
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7040369361903634,
            "MicroF1": 0.7040369361903634,
            "MacroF1": 0.6235946437988805,
            "Memory in Mb": 205.63252925872803,
            "Time in s": 1896.370643
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7105124697463959,
            "MicroF1": 0.7105124697463959,
            "MacroF1": 0.6284709935917355,
            "Memory in Mb": 229.19151210784912,
            "Time in s": 2381.431795
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7140827729898664,
            "MicroF1": 0.7140827729898664,
            "MacroF1": 0.6302854833117341,
            "Memory in Mb": 253.17632389068604,
            "Time in s": 2925.98814
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.71562634524322,
            "MicroF1": 0.7156263452432199,
            "MacroF1": 0.6305326785921538,
            "Memory in Mb": 277.4567346572876,
            "Time in s": 3530.852036
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7145450240707126,
            "MicroF1": 0.7145450240707125,
            "MacroF1": 0.6284185449457835,
            "Memory in Mb": 301.7114896774292,
            "Time in s": 4201.052974
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.7057623661397247,
            "MicroF1": 0.7057623661397247,
            "MacroF1": 0.6885364031919957,
            "Memory in Mb": 327.2237205505371,
            "Time in s": 4936.820951
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6967462625989312,
            "MicroF1": 0.6967462625989312,
            "MacroF1": 0.69194472505998,
            "Memory in Mb": 352.6018476486206,
            "Time in s": 5738.465999
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.676684134099375,
            "MicroF1": 0.676684134099375,
            "MacroF1": 0.673854549025314,
            "Memory in Mb": 384.9730758666992,
            "Time in s": 6613.285946
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6698431488606097,
            "MicroF1": 0.6698431488606097,
            "MacroF1": 0.668750254945471,
            "Memory in Mb": 415.2214603424072,
            "Time in s": 7559.921071
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6646983454960727,
            "MicroF1": 0.6646983454960727,
            "MacroF1": 0.6646134205077884,
            "Memory in Mb": 444.32067584991455,
            "Time in s": 8589.520858
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6620192560635555,
            "MicroF1": 0.6620192560635555,
            "MacroF1": 0.6605985532750915,
            "Memory in Mb": 472.75781440734863,
            "Time in s": 9705.665905
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6597717190848826,
            "MicroF1": 0.6597717190848826,
            "MacroF1": 0.6570293922418718,
            "Memory in Mb": 499.4876089096069,
            "Time in s": 10901.076562
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6539608882996354,
            "MicroF1": 0.6539608882996354,
            "MacroF1": 0.6496192149174075,
            "Memory in Mb": 528.8777961730957,
            "Time in s": 12166.701144
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6547463359639233,
            "MicroF1": 0.6547463359639233,
            "MacroF1": 0.6484047117859243,
            "Memory in Mb": 557.1920728683472,
            "Time in s": 13501.384366
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6583444535319185,
            "MicroF1": 0.6583444535319185,
            "MacroF1": 0.6499882024630633,
            "Memory in Mb": 584.0554361343384,
            "Time in s": 14901.095396
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6611767612302878,
            "MicroF1": 0.6611767612302878,
            "MacroF1": 0.6506059068013808,
            "Memory in Mb": 610.3706150054932,
            "Time in s": 16366.700533
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6659827171210986,
            "MicroF1": 0.6659827171210986,
            "MacroF1": 0.6532433614752314,
            "Memory in Mb": 635.6853046417236,
            "Time in s": 17901.739193
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6702526610856472,
            "MicroF1": 0.6702526610856472,
            "MacroF1": 0.6554263220708306,
            "Memory in Mb": 660.4025926589966,
            "Time in s": 19504.786084
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6745947914769623,
            "MicroF1": 0.6745947914769623,
            "MacroF1": 0.6575507550972549,
            "Memory in Mb": 684.36501121521,
            "Time in s": 21172.086014
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6705482094630143,
            "MicroF1": 0.6705482094630143,
            "MacroF1": 0.6539581966383304,
            "Memory in Mb": 712.6770572662354,
            "Time in s": 22902.746936
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6644231744850678,
            "MicroF1": 0.6644231744850678,
            "MacroF1": 0.6512239029866641,
            "Memory in Mb": 743.5559530258179,
            "Time in s": 24691.477434
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6622799856317148,
            "MicroF1": 0.6622799856317148,
            "MacroF1": 0.6527566844616065,
            "Memory in Mb": 772.5478630065918,
            "Time in s": 26538.585641
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6621736797247388,
            "MicroF1": 0.6621736797247388,
            "MacroF1": 0.6557760097374935,
            "Memory in Mb": 800.5439138412476,
            "Time in s": 28440.416189000003
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6623797159004124,
            "MicroF1": 0.6623797159004124,
            "MacroF1": 0.6584479912704261,
            "Memory in Mb": 827.4998264312744,
            "Time in s": 30418.714512
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6575123553608949,
            "MicroF1": 0.6575123553608949,
            "MacroF1": 0.6541419435809196,
            "Memory in Mb": 857.7161102294922,
            "Time in s": 32439.386127
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6519069073377909,
            "MicroF1": 0.6519069073377909,
            "MacroF1": 0.6481893367707658,
            "Memory in Mb": 888.8327789306641,
            "Time in s": 34499.720344
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.647550343982397,
            "MicroF1": 0.647550343982397,
            "MacroF1": 0.643407015045196,
            "Memory in Mb": 919.6311988830566,
            "Time in s": 36599.09766
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6444438431775752,
            "MicroF1": 0.6444438431775752,
            "MacroF1": 0.6400224052225335,
            "Memory in Mb": 949.7819452285768,
            "Time in s": 38735.650911
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6425358411153492,
            "MicroF1": 0.6425358411153492,
            "MacroF1": 0.6377821595167165,
            "Memory in Mb": 979.4456567764282,
            "Time in s": 40896.763765
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6414476209976709,
            "MicroF1": 0.6414476209976709,
            "MacroF1": 0.6370415360917451,
            "Memory in Mb": 1009.0255756378174,
            "Time in s": 43085.847267
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6409898572033793,
            "MicroF1": 0.6409898572033793,
            "MacroF1": 0.636858231937463,
            "Memory in Mb": 1037.841980934143,
            "Time in s": 45303.144751
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6414782798727631,
            "MicroF1": 0.6414782798727631,
            "MacroF1": 0.637272014233453,
            "Memory in Mb": 1065.1163549423218,
            "Time in s": 47540.369251
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6428419233409882,
            "MicroF1": 0.6428419233409882,
            "MacroF1": 0.6385110475108609,
            "Memory in Mb": 1091.8334274291992,
            "Time in s": 49803.522006
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6441159487238711,
            "MicroF1": 0.6441159487238711,
            "MacroF1": 0.6396283228479406,
            "Memory in Mb": 1118.1560363769531,
            "Time in s": 52086.93226
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.645058735992424,
            "MicroF1": 0.645058735992424,
            "MacroF1": 0.6403851797193834,
            "Memory in Mb": 1144.4119939804075,
            "Time in s": 54391.61903
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6469266853128373,
            "MicroF1": 0.6469266853128373,
            "MacroF1": 0.6418265850265934,
            "Memory in Mb": 1169.9601306915283,
            "Time in s": 56719.958571
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6487742935238792,
            "MicroF1": 0.6487742935238792,
            "MacroF1": 0.643191402092947,
            "Memory in Mb": 1194.640343666077,
            "Time in s": 59073.094705
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6459521454576065,
            "MicroF1": 0.6459521454576065,
            "MacroF1": 0.6406800374556137,
            "Memory in Mb": 1224.6073780059814,
            "Time in s": 61451.967815
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6443643849716932,
            "MicroF1": 0.6443643849716932,
            "MacroF1": 0.6398250343320808,
            "Memory in Mb": 1254.4350862503052,
            "Time in s": 63857.884093
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6446172754931394,
            "MicroF1": 0.6446172754931394,
            "MacroF1": 0.6406945505071863,
            "Memory in Mb": 1282.3891849517822,
            "Time in s": 66293.298766
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6461222798745241,
            "MicroF1": 0.6461222798745241,
            "MacroF1": 0.6426238276925219,
            "Memory in Mb": 1309.4736614227295,
            "Time in s": 68755.018108
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6489186943161394,
            "MicroF1": 0.6489186943161394,
            "MacroF1": 0.6457243405011626,
            "Memory in Mb": 1334.444143295288,
            "Time in s": 71244.151045
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6470577094263149,
            "MicroF1": 0.6470577094263149,
            "MacroF1": 0.6443966707674731,
            "Memory in Mb": 1363.999231338501,
            "Time in s": 73759.934152
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Insects",
            "Accuracy": 0.6469809071470471,
            "MicroF1": 0.6469809071470471,
            "MacroF1": 0.6443518314696601,
            "Memory in Mb": 1365.409776687622,
            "Time in s": 76295.692169
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9901719901719902,
            "MicroF1": 0.9901719901719902,
            "MacroF1": 0.8308395677472984,
            "Memory in Mb": 0.1227684020996093,
            "Time in s": 1.485322
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9914110429447852,
            "MicroF1": 0.9914110429447852,
            "MacroF1": 0.960934413925625,
            "Memory in Mb": 0.4158411026000976,
            "Time in s": 6.729082
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9893704006541292,
            "MicroF1": 0.9893704006541292,
            "MacroF1": 0.9580466011674303,
            "Memory in Mb": 1.2467107772827148,
            "Time in s": 20.14849
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9889638258736972,
            "MicroF1": 0.9889638258736972,
            "MacroF1": 0.9786672150923964,
            "Memory in Mb": 2.28104305267334,
            "Time in s": 50.264957
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.988719960765081,
            "MicroF1": 0.988719960765081,
            "MacroF1": 0.9803510904896324,
            "Memory in Mb": 3.352717399597168,
            "Time in s": 91.643431
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9885574172456068,
            "MicroF1": 0.9885574172456068,
            "MacroF1": 0.983046879237058,
            "Memory in Mb": 4.983606338500977,
            "Time in s": 148.278076
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9852889667250436,
            "MicroF1": 0.9852889667250436,
            "MacroF1": 0.9737767108051044,
            "Memory in Mb": 6.963967323303223,
            "Time in s": 227.073424
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9825314128102972,
            "MicroF1": 0.9825314128102972,
            "MacroF1": 0.9734338986941852,
            "Memory in Mb": 9.8344087600708,
            "Time in s": 324.702985
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.982293652955598,
            "MicroF1": 0.982293652955598,
            "MacroF1": 0.9788760747631072,
            "Memory in Mb": 12.7888765335083,
            "Time in s": 446.356435
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9806325079676392,
            "MicroF1": 0.9806325079676392,
            "MacroF1": 0.9749453255203756,
            "Memory in Mb": 16.445659637451172,
            "Time in s": 594.71846
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9801649208825496,
            "MicroF1": 0.9801649208825496,
            "MacroF1": 0.9779116862524244,
            "Memory in Mb": 20.943636894226078,
            "Time in s": 768.8230350000001
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9801838610827376,
            "MicroF1": 0.9801838610827376,
            "MacroF1": 0.978782474664832,
            "Memory in Mb": 24.856953620910645,
            "Time in s": 967.611442
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9768055817461814,
            "MicroF1": 0.9768055817461814,
            "MacroF1": 0.9702080932270808,
            "Memory in Mb": 28.10527801513672,
            "Time in s": 1191.0213970000002
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9746104009805638,
            "MicroF1": 0.9746104009805638,
            "MacroF1": 0.9718234131704068,
            "Memory in Mb": 32.14579772949219,
            "Time in s": 1440.171835
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9697663016832816,
            "MicroF1": 0.9697663016832816,
            "MacroF1": 0.9621279568251032,
            "Memory in Mb": 36.40912055969238,
            "Time in s": 1717.813161
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9656810173127012,
            "MicroF1": 0.9656810173127012,
            "MacroF1": 0.9634765255010708,
            "Memory in Mb": 42.20043754577637,
            "Time in s": 2023.330442
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9653929343907716,
            "MicroF1": 0.9653929343907716,
            "MacroF1": 0.9646253117338192,
            "Memory in Mb": 46.97204208374024,
            "Time in s": 2355.811343
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9635026555903582,
            "MicroF1": 0.9635026555903582,
            "MacroF1": 0.96110342818104,
            "Memory in Mb": 50.8284969329834,
            "Time in s": 2716.693574
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9610372855115468,
            "MicroF1": 0.9610372855115468,
            "MacroF1": 0.9585597537512924,
            "Memory in Mb": 55.062747955322266,
            "Time in s": 3108.019641
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9593087388160314,
            "MicroF1": 0.9593087388160314,
            "MacroF1": 0.9577319445930262,
            "Memory in Mb": 59.75967216491699,
            "Time in s": 3529.961458
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9598459203922026,
            "MicroF1": 0.9598459203922026,
            "MacroF1": 0.960171378024828,
            "Memory in Mb": 65.88526916503906,
            "Time in s": 3981.552133
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.959108635097493,
            "MicroF1": 0.959108635097493,
            "MacroF1": 0.9586518345557712,
            "Memory in Mb": 71.85272026062012,
            "Time in s": 4465.222941
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9573697111797932,
            "MicroF1": 0.9573697111797932,
            "MacroF1": 0.956135316427552,
            "Memory in Mb": 78.18439388275146,
            "Time in s": 4984.801354
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9555714431620876,
            "MicroF1": 0.9555714431620876,
            "MacroF1": 0.9546392488298882,
            "Memory in Mb": 85.86389446258545,
            "Time in s": 5537.4752260000005
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9486224139621532,
            "MicroF1": 0.9486224139621532,
            "MacroF1": 0.9433099305923252,
            "Memory in Mb": 94.35744285583496,
            "Time in s": 6127.477763000001
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.943150749505044,
            "MicroF1": 0.943150749505044,
            "MacroF1": 0.9403442056943528,
            "Memory in Mb": 104.1574821472168,
            "Time in s": 6756.480909000001
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9408987743985474,
            "MicroF1": 0.9408987743985474,
            "MacroF1": 0.9399975161043574,
            "Memory in Mb": 113.0038013458252,
            "Time in s": 7421.284759000001
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9380197846450145,
            "MicroF1": 0.9380197846450145,
            "MacroF1": 0.936341059397272,
            "Memory in Mb": 121.46645069122314,
            "Time in s": 8125.715779000001
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9322965091708224,
            "MicroF1": 0.9322965091708224,
            "MacroF1": 0.9294143034054052,
            "Memory in Mb": 131.1031150817871,
            "Time in s": 8872.899296000001
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9326742380913472,
            "MicroF1": 0.9326742380913472,
            "MacroF1": 0.9327603226303838,
            "Memory in Mb": 137.88959789276123,
            "Time in s": 9652.703167
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.927571756147703,
            "MicroF1": 0.927571756147703,
            "MacroF1": 0.9249549620362734,
            "Memory in Mb": 145.5888376235962,
            "Time in s": 10475.658214
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9247797778628878,
            "MicroF1": 0.9247797778628878,
            "MacroF1": 0.92370720847711,
            "Memory in Mb": 154.53871536254883,
            "Time in s": 11346.213643
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9238654088984624,
            "MicroF1": 0.9238654088984624,
            "MacroF1": 0.9233692422863464,
            "Memory in Mb": 161.3583574295044,
            "Time in s": 12266.045404
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9202653017086008,
            "MicroF1": 0.9202653017086008,
            "MacroF1": 0.9191663953636944,
            "Memory in Mb": 170.12918186187744,
            "Time in s": 13231.481182
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.916310666013026,
            "MicroF1": 0.916310666013026,
            "MacroF1": 0.9150341930556872,
            "Memory in Mb": 179.0350112915039,
            "Time in s": 14245.599713
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9161162933206236,
            "MicroF1": 0.9161162933206236,
            "MacroF1": 0.9160540991607554,
            "Memory in Mb": 184.834698677063,
            "Time in s": 15311.95464
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9145412388208016,
            "MicroF1": 0.9145412388208016,
            "MacroF1": 0.91429667624259,
            "Memory in Mb": 191.58009719848636,
            "Time in s": 16433.239395
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9105979487841064,
            "MicroF1": 0.9105979487841064,
            "MacroF1": 0.909716370830996,
            "Memory in Mb": 200.08039951324463,
            "Time in s": 17613.909715
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9068568914587392,
            "MicroF1": 0.9068568914587392,
            "MacroF1": 0.9060681758481206,
            "Memory in Mb": 210.5000762939453,
            "Time in s": 18848.20155
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9031190636681168,
            "MicroF1": 0.9031190636681168,
            "MacroF1": 0.9023660107991418,
            "Memory in Mb": 221.55222129821777,
            "Time in s": 20131.794746000003
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.9005799007592515,
            "MicroF1": 0.9005799007592515,
            "MacroF1": 0.9001704241319546,
            "Memory in Mb": 231.28063201904297,
            "Time in s": 21466.799965
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8989203384884739,
            "MicroF1": 0.8989203384884739,
            "MacroF1": 0.8987537815839572,
            "Memory in Mb": 248.11264038085935,
            "Time in s": 22840.808564000003
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.893746793592886,
            "MicroF1": 0.8937467935928861,
            "MacroF1": 0.892807745348426,
            "Memory in Mb": 267.53482723236084,
            "Time in s": 24265.711089000004
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8894212021614395,
            "MicroF1": 0.8894212021614395,
            "MacroF1": 0.8884694521151855,
            "Memory in Mb": 281.7739496231079,
            "Time in s": 25739.620728000005
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8911705430579008,
            "MicroF1": 0.8911705430579007,
            "MacroF1": 0.8908032768807751,
            "Memory in Mb": 288.0978307723999,
            "Time in s": 27256.627666000004
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8911387009111739,
            "MicroF1": 0.8911387009111739,
            "MacroF1": 0.8906428613252552,
            "Memory in Mb": 296.0527210235596,
            "Time in s": 28820.747713000004
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8886049543676662,
            "MicroF1": 0.8886049543676662,
            "MacroF1": 0.8879368647002966,
            "Memory in Mb": 307.6826677322388,
            "Time in s": 30435.23145800001
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8895470561201042,
            "MicroF1": 0.8895470561201042,
            "MacroF1": 0.889061241536932,
            "Memory in Mb": 313.4344787597656,
            "Time in s": 32089.799369000008
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8862488119653844,
            "MicroF1": 0.8862488119653844,
            "MacroF1": 0.8855123768505595,
            "Memory in Mb": 324.9442596435547,
            "Time in s": 33786.733744000005
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Aggregated Mondrian Forest",
            "dataset": "Keystroke",
            "Accuracy": 0.8810726015981175,
            "MicroF1": 0.8810726015981175,
            "MacroF1": 0.8799282628097613,
            "Memory in Mb": 338.1390075683594,
            "Time in s": 35528.434162000005
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.3555555555555555,
            "MicroF1": 0.3555555555555555,
            "MacroF1": 0.2468487394957983,
            "Memory in Mb": 2.5926971435546875,
            "Time in s": 5.672061
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.5274725274725275,
            "MicroF1": 0.5274725274725275,
            "MacroF1": 0.5392220990960486,
            "Memory in Mb": 2.5963096618652344,
            "Time in s": 17.740863
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.5401459854014599,
            "MicroF1": 0.5401459854014599,
            "MacroF1": 0.5661177456005042,
            "Memory in Mb": 2.5979232788085938,
            "Time in s": 35.937815
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.5956284153005464,
            "MicroF1": 0.5956284153005464,
            "MacroF1": 0.6144104879239446,
            "Memory in Mb": 2.6004638671875,
            "Time in s": 59.975895
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6200873362445415,
            "MicroF1": 0.6200873362445415,
            "MacroF1": 0.6319742698014011,
            "Memory in Mb": 2.6008224487304688,
            "Time in s": 89.681265
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6327272727272727,
            "MicroF1": 0.6327272727272727,
            "MacroF1": 0.6440706793955739,
            "Memory in Mb": 2.601276397705078,
            "Time in s": 125.043898
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6573208722741433,
            "MicroF1": 0.6573208722741433,
            "MacroF1": 0.6535377647060517,
            "Memory in Mb": 2.6028709411621094,
            "Time in s": 166.036362
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6784741144414169,
            "MicroF1": 0.6784741144414169,
            "MacroF1": 0.6717418242612484,
            "Memory in Mb": 2.6031723022460938,
            "Time in s": 212.735146
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6900726392251816,
            "MicroF1": 0.6900726392251816,
            "MacroF1": 0.6823551618652942,
            "Memory in Mb": 2.603717803955078,
            "Time in s": 265.175489
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6971677559912854,
            "MicroF1": 0.6971677559912854,
            "MacroF1": 0.686858403065277,
            "Memory in Mb": 2.60379409790039,
            "Time in s": 323.486791
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.699009900990099,
            "MicroF1": 0.699009900990099,
            "MacroF1": 0.6869845800125663,
            "Memory in Mb": 2.604084014892578,
            "Time in s": 387.600808
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6987295825771325,
            "MicroF1": 0.6987295825771325,
            "MacroF1": 0.6895132041566728,
            "Memory in Mb": 2.6040496826171875,
            "Time in s": 457.323817
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7035175879396985,
            "MicroF1": 0.7035175879396985,
            "MacroF1": 0.6939747146282641,
            "Memory in Mb": 2.6041183471679688,
            "Time in s": 532.682096
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.6998444790046656,
            "MicroF1": 0.6998444790046656,
            "MacroF1": 0.6913714585468268,
            "Memory in Mb": 2.6053123474121094,
            "Time in s": 613.490084
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7024673439767779,
            "MicroF1": 0.7024673439767779,
            "MacroF1": 0.6944906634267102,
            "Memory in Mb": 2.6058921813964844,
            "Time in s": 699.880084
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7020408163265306,
            "MicroF1": 0.7020408163265306,
            "MacroF1": 0.69548275919944,
            "Memory in Mb": 2.605987548828125,
            "Time in s": 791.65329
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.706786171574904,
            "MicroF1": 0.706786171574904,
            "MacroF1": 0.6991539785967766,
            "Memory in Mb": 2.6064224243164062,
            "Time in s": 888.981823
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7085852478839177,
            "MicroF1": 0.7085852478839177,
            "MacroF1": 0.70309750989463,
            "Memory in Mb": 2.6064682006835938,
            "Time in s": 991.647497
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.715922107674685,
            "MicroF1": 0.7159221076746849,
            "MacroF1": 0.7073525059690206,
            "Memory in Mb": 2.6064682006835938,
            "Time in s": 1099.573439
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7170837867247007,
            "MicroF1": 0.7170837867247007,
            "MacroF1": 0.707165908654469,
            "Memory in Mb": 2.6064682006835938,
            "Time in s": 1212.915424
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7160621761658031,
            "MicroF1": 0.716062176165803,
            "MacroF1": 0.7063689525089133,
            "Memory in Mb": 2.6064682006835938,
            "Time in s": 1331.559339
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7151335311572701,
            "MicroF1": 0.7151335311572701,
            "MacroF1": 0.7047830593764105,
            "Memory in Mb": 2.6064910888671875,
            "Time in s": 1455.3800170000002
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7152317880794702,
            "MicroF1": 0.7152317880794702,
            "MacroF1": 0.7037726227430311,
            "Memory in Mb": 2.606658935546875,
            "Time in s": 1584.327081
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.71441523118767,
            "MicroF1": 0.71441523118767,
            "MacroF1": 0.7026447500373862,
            "Memory in Mb": 2.6067771911621094,
            "Time in s": 1718.245947
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7162750217580505,
            "MicroF1": 0.7162750217580505,
            "MacroF1": 0.7030218527348165,
            "Memory in Mb": 2.6067771911621094,
            "Time in s": 1857.022931
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7179916317991631,
            "MicroF1": 0.7179916317991631,
            "MacroF1": 0.705575475090573,
            "Memory in Mb": 2.379610061645508,
            "Time in s": 2000.273372
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7155519742143432,
            "MicroF1": 0.7155519742143431,
            "MacroF1": 0.7053749246401603,
            "Memory in Mb": 3.185004234313965,
            "Time in s": 2147.034729
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7156177156177156,
            "MicroF1": 0.7156177156177156,
            "MacroF1": 0.7041730806550314,
            "Memory in Mb": 3.633350372314453,
            "Time in s": 2296.192092
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7149287321830458,
            "MicroF1": 0.7149287321830458,
            "MacroF1": 0.7045092702498074,
            "Memory in Mb": 4.368736267089844,
            "Time in s": 2447.850078
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7186366932559826,
            "MicroF1": 0.7186366932559827,
            "MacroF1": 0.7102131417787841,
            "Memory in Mb": 4.724300384521484,
            "Time in s": 2601.871177
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7256140350877193,
            "MicroF1": 0.7256140350877193,
            "MacroF1": 0.7174099613082184,
            "Memory in Mb": 4.89253044128418,
            "Time in s": 2758.036552
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7273963290278722,
            "MicroF1": 0.7273963290278722,
            "MacroF1": 0.7183919320082559,
            "Memory in Mb": 5.412370681762695,
            "Time in s": 2916.512936
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7211601845748187,
            "MicroF1": 0.7211601845748187,
            "MacroF1": 0.7136134581802791,
            "Memory in Mb": 6.487729072570801,
            "Time in s": 3077.492565
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7172104926423545,
            "MicroF1": 0.7172104926423546,
            "MacroF1": 0.7129536273040751,
            "Memory in Mb": 6.405126571655273,
            "Time in s": 3241.109
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7209446861404599,
            "MicroF1": 0.7209446861404599,
            "MacroF1": 0.7163536024764182,
            "Memory in Mb": 6.857941627502441,
            "Time in s": 3407.317179
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7238670694864048,
            "MicroF1": 0.7238670694864048,
            "MacroF1": 0.7196892738307762,
            "Memory in Mb": 7.034061431884766,
            "Time in s": 3576.258732
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7260435038212816,
            "MicroF1": 0.7260435038212816,
            "MacroF1": 0.7238533950478148,
            "Memory in Mb": 7.623349189758301,
            "Time in s": 3747.864612
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7309673726388094,
            "MicroF1": 0.7309673726388093,
            "MacroF1": 0.7286270619416129,
            "Memory in Mb": 8.106144905090332,
            "Time in s": 3922.063963000001
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7361963190184049,
            "MicroF1": 0.7361963190184049,
            "MacroF1": 0.7329274067865035,
            "Memory in Mb": 8.185744285583496,
            "Time in s": 4098.8506050000005
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7389885807504079,
            "MicroF1": 0.7389885807504077,
            "MacroF1": 0.7360694376974826,
            "Memory in Mb": 8.929247856140137,
            "Time in s": 4278.2789060000005
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7411140583554376,
            "MicroF1": 0.7411140583554376,
            "MacroF1": 0.7396669191579938,
            "Memory in Mb": 9.100563049316406,
            "Time in s": 4460.600751000001
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7431382703262558,
            "MicroF1": 0.7431382703262558,
            "MacroF1": 0.7411378754700444,
            "Memory in Mb": 9.223885536193848,
            "Time in s": 4645.683986000001
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7465857359635811,
            "MicroF1": 0.746585735963581,
            "MacroF1": 0.744200926808846,
            "Memory in Mb": 9.401692390441896,
            "Time in s": 4833.458731000001
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7508650519031141,
            "MicroF1": 0.7508650519031143,
            "MacroF1": 0.7476945996538615,
            "Memory in Mb": 9.481804847717283,
            "Time in s": 5024.230846
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7549540840985983,
            "MicroF1": 0.7549540840985983,
            "MacroF1": 0.7524477298078486,
            "Memory in Mb": 9.431160926818848,
            "Time in s": 5217.969956000001
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7583924349881797,
            "MicroF1": 0.7583924349881797,
            "MacroF1": 0.7554386161495508,
            "Memory in Mb": 9.549637794494627,
            "Time in s": 5414.604524000001
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7607589079130033,
            "MicroF1": 0.7607589079130033,
            "MacroF1": 0.7577216433051415,
            "Memory in Mb": 10.151451110839844,
            "Time in s": 5614.378132000002
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7648391481649298,
            "MicroF1": 0.7648391481649298,
            "MacroF1": 0.7614528787516565,
            "Memory in Mb": 9.14443588256836,
            "Time in s": 5817.274926000002
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7652019529516201,
            "MicroF1": 0.7652019529516201,
            "MacroF1": 0.762166830901651,
            "Memory in Mb": 8.801234245300293,
            "Time in s": 6023.198429000002
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7672901261418008,
            "MicroF1": 0.7672901261418008,
            "MacroF1": 0.7647372124971393,
            "Memory in Mb": 8.857858657836914,
            "Time in s": 6232.074878000002
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "ImageSegments",
            "Accuracy": 0.7669987007362494,
            "MicroF1": 0.7669987007362494,
            "MacroF1": 0.7647069285577738,
            "Memory in Mb": 8.926526069641113,
            "Time in s": 6441.814766000002
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6388625592417062,
            "MicroF1": 0.6388625592417062,
            "MacroF1": 0.6031100134310133,
            "Memory in Mb": 8.730474472045898,
            "Time in s": 177.190345
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.659403126480341,
            "MicroF1": 0.659403126480341,
            "MacroF1": 0.6244477305834598,
            "Memory in Mb": 21.138185501098636,
            "Time in s": 477.6689290000001
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6722450268392801,
            "MicroF1": 0.6722450268392801,
            "MacroF1": 0.6321534006670183,
            "Memory in Mb": 28.433568000793457,
            "Time in s": 884.814326
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.680322045938906,
            "MicroF1": 0.680322045938906,
            "MacroF1": 0.6340126191391743,
            "Memory in Mb": 39.2259521484375,
            "Time in s": 1406.7405990000002
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6878196628149271,
            "MicroF1": 0.6878196628149271,
            "MacroF1": 0.6395508722492685,
            "Memory in Mb": 32.51231288909912,
            "Time in s": 2046.4837620000003
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6876085240726125,
            "MicroF1": 0.6876085240726125,
            "MacroF1": 0.641396967542699,
            "Memory in Mb": 34.57641696929932,
            "Time in s": 2792.1074670000003
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6924638073332431,
            "MicroF1": 0.6924638073332431,
            "MacroF1": 0.6467777725107727,
            "Memory in Mb": 40.06835174560547,
            "Time in s": 3634.422347
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6949212738250267,
            "MicroF1": 0.6949212738250267,
            "MacroF1": 0.6476372139610082,
            "Memory in Mb": 43.01965808868408,
            "Time in s": 4571.1184410000005
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.6992528675155214,
            "MicroF1": 0.6992528675155214,
            "MacroF1": 0.6494082466298291,
            "Memory in Mb": 45.71251583099365,
            "Time in s": 5608.992399000001
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7013921772895161,
            "MicroF1": 0.7013921772895161,
            "MacroF1": 0.6506452100316108,
            "Memory in Mb": 50.31043148040772,
            "Time in s": 6744.395149000001
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7043478260869566,
            "MicroF1": 0.7043478260869566,
            "MacroF1": 0.6524912605091605,
            "Memory in Mb": 59.27919769287109,
            "Time in s": 7964.619750000001
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7079946334148843,
            "MicroF1": 0.7079946334148843,
            "MacroF1": 0.6596828376773001,
            "Memory in Mb": 72.61201000213623,
            "Time in s": 9269.589572
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7208421359364756,
            "MicroF1": 0.7208421359364756,
            "MacroF1": 0.7145906055666686,
            "Memory in Mb": 38.78250694274902,
            "Time in s": 10625.218377
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7285395386592708,
            "MicroF1": 0.7285395386592708,
            "MacroF1": 0.7256542392368915,
            "Memory in Mb": 15.54647731781006,
            "Time in s": 12027.231464
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7206263021655408,
            "MicroF1": 0.7206263021655408,
            "MacroF1": 0.7196216319492748,
            "Memory in Mb": 14.88278579711914,
            "Time in s": 13491.676191
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7171352471145309,
            "MicroF1": 0.7171352471145309,
            "MacroF1": 0.7175260611854538,
            "Memory in Mb": 21.28149700164795,
            "Time in s": 15025.812845
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7121051751991533,
            "MicroF1": 0.7121051751991533,
            "MacroF1": 0.7136617513297842,
            "Memory in Mb": 29.336480140686035,
            "Time in s": 16621.157643
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7205240174672489,
            "MicroF1": 0.720524017467249,
            "MacroF1": 0.7180961996594418,
            "Memory in Mb": 20.976608276367188,
            "Time in s": 18267.655245
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7261625878482779,
            "MicroF1": 0.7261625878482779,
            "MacroF1": 0.7198561207408494,
            "Memory in Mb": 15.994047164916992,
            "Time in s": 19960.279521
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7272598134381363,
            "MicroF1": 0.7272598134381363,
            "MacroF1": 0.7183389579277755,
            "Memory in Mb": 17.52824878692627,
            "Time in s": 21708.029386999995
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7281623449830891,
            "MicroF1": 0.7281623449830891,
            "MacroF1": 0.7167723651435352,
            "Memory in Mb": 22.240838050842285,
            "Time in s": 23503.558300999997
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7307477078042272,
            "MicroF1": 0.7307477078042272,
            "MacroF1": 0.7170791531651185,
            "Memory in Mb": 26.114503860473636,
            "Time in s": 25348.434525999997
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7325318071396221,
            "MicroF1": 0.7325318071396222,
            "MacroF1": 0.7165563330554671,
            "Memory in Mb": 27.97449111938477,
            "Time in s": 27240.683159999997
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7353904431203883,
            "MicroF1": 0.7353904431203884,
            "MacroF1": 0.7174524973348954,
            "Memory in Mb": 37.12833023071289,
            "Time in s": 29182.513668999996
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7367703322095533,
            "MicroF1": 0.7367703322095533,
            "MacroF1": 0.7168965346030137,
            "Memory in Mb": 31.575971603393555,
            "Time in s": 31184.058177999992
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.738371881260244,
            "MicroF1": 0.738371881260244,
            "MacroF1": 0.7164257197178175,
            "Memory in Mb": 35.22733116149902,
            "Time in s": 33213.34443999999
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7366279681526429,
            "MicroF1": 0.7366279681526429,
            "MacroF1": 0.7161250847684691,
            "Memory in Mb": 17.50509262084961,
            "Time in s": 35271.15690999999
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7354483038522678,
            "MicroF1": 0.7354483038522677,
            "MacroF1": 0.719616514898752,
            "Memory in Mb": 22.40646266937256,
            "Time in s": 37354.25785299999
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7348724814681775,
            "MicroF1": 0.7348724814681775,
            "MacroF1": 0.7237598149406717,
            "Memory in Mb": 31.22674369812012,
            "Time in s": 39459.62893099999
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7347769815966413,
            "MicroF1": 0.7347769815966413,
            "MacroF1": 0.7275990709197302,
            "Memory in Mb": 35.24118995666504,
            "Time in s": 41587.29474699999
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7351458683366427,
            "MicroF1": 0.7351458683366427,
            "MacroF1": 0.7308983066693725,
            "Memory in Mb": 48.40772724151611,
            "Time in s": 43729.93044799999
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7303423988636027,
            "MicroF1": 0.7303423988636027,
            "MacroF1": 0.7274356410957497,
            "Memory in Mb": 77.28174114227295,
            "Time in s": 45887.55412199999
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.726805750853732,
            "MicroF1": 0.726805750853732,
            "MacroF1": 0.723911701718825,
            "Memory in Mb": 53.16175174713135,
            "Time in s": 48068.300588999984
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7248976408656658,
            "MicroF1": 0.7248976408656659,
            "MacroF1": 0.7218080521646734,
            "Memory in Mb": 41.53026580810547,
            "Time in s": 50265.61973699999
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7215833761735978,
            "MicroF1": 0.7215833761735979,
            "MacroF1": 0.7182506744185386,
            "Memory in Mb": 35.33352756500244,
            "Time in s": 52485.18591199999
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7196369854004998,
            "MicroF1": 0.7196369854004999,
            "MacroF1": 0.7160236415660819,
            "Memory in Mb": 44.00273513793945,
            "Time in s": 54721.05808499999
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7175142688950884,
            "MicroF1": 0.7175142688950884,
            "MacroF1": 0.713988650041017,
            "Memory in Mb": 46.12203025817871,
            "Time in s": 56978.30571199999
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7158023276098388,
            "MicroF1": 0.7158023276098388,
            "MacroF1": 0.7126852582249207,
            "Memory in Mb": 27.841010093688965,
            "Time in s": 59249.54765999999
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7157322196051769,
            "MicroF1": 0.715732219605177,
            "MacroF1": 0.7129296468122535,
            "Memory in Mb": 21.849401473999023,
            "Time in s": 61534.70422899999
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7156656170837378,
            "MicroF1": 0.7156656170837377,
            "MacroF1": 0.7131576552849198,
            "Memory in Mb": 28.021278381347656,
            "Time in s": 63833.59664899999
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.715925626515764,
            "MicroF1": 0.715925626515764,
            "MacroF1": 0.7137513847694824,
            "Memory in Mb": 36.50454139709473,
            "Time in s": 66146.66403399999
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7161958016730176,
            "MicroF1": 0.7161958016730177,
            "MacroF1": 0.7143198962298327,
            "Memory in Mb": 46.888444900512695,
            "Time in s": 68474.34057599999
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7170260092056291,
            "MicroF1": 0.7170260092056291,
            "MacroF1": 0.7151715877390813,
            "Memory in Mb": 47.08374786376953,
            "Time in s": 70816.527322
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7181843617502098,
            "MicroF1": 0.7181843617502098,
            "MacroF1": 0.7162864260409335,
            "Memory in Mb": 43.18325901031494,
            "Time in s": 73172.526917
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7179023127591069,
            "MicroF1": 0.7179023127591069,
            "MacroF1": 0.716246618663062,
            "Memory in Mb": 54.80090522766113,
            "Time in s": 75543.857611
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7211528564076171,
            "MicroF1": 0.7211528564076171,
            "MacroF1": 0.719707905487922,
            "Memory in Mb": 60.4919376373291,
            "Time in s": 77931.086228
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7250710241582882,
            "MicroF1": 0.7250710241582882,
            "MacroF1": 0.7236001513027165,
            "Memory in Mb": 35.55128765106201,
            "Time in s": 80332.853368
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7288259316984631,
            "MicroF1": 0.7288259316984631,
            "MacroF1": 0.7271241427068512,
            "Memory in Mb": 21.017152786254883,
            "Time in s": 82746.274567
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7329107318864387,
            "MicroF1": 0.7329107318864386,
            "MacroF1": 0.7308784460773333,
            "Memory in Mb": 26.768343925476078,
            "Time in s": 85169.877802
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7359230288452433,
            "MicroF1": 0.7359230288452432,
            "MacroF1": 0.7343606492383059,
            "Memory in Mb": 9.57052230834961,
            "Time in s": 87600.592492
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Insects",
            "Accuracy": 0.7361628853104244,
            "MicroF1": 0.7361628853104244,
            "MacroF1": 0.7346220154259927,
            "Memory in Mb": 9.63199520111084,
            "Time in s": 90031.55993999999
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9901719901719902,
            "MicroF1": 0.9901719901719902,
            "MacroF1": 0.8308395677472984,
            "Memory in Mb": 1.027322769165039,
            "Time in s": 17.348128
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9877300613496932,
            "MicroF1": 0.9877300613496932,
            "MacroF1": 0.9320293882508496,
            "Memory in Mb": 2.6651391983032227,
            "Time in s": 54.406226
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.982829108748978,
            "MicroF1": 0.982829108748978,
            "MacroF1": 0.9464059415055076,
            "Memory in Mb": 5.679329872131348,
            "Time in s": 114.007104
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9828326180257512,
            "MicroF1": 0.9828326180257512,
            "MacroF1": 0.963209755030524,
            "Memory in Mb": 8.335807800292969,
            "Time in s": 201.582874
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.974987739087788,
            "MicroF1": 0.974987739087788,
            "MacroF1": 0.9373958892668122,
            "Memory in Mb": 12.631415367126465,
            "Time in s": 318.920922
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.970167552104618,
            "MicroF1": 0.970167552104618,
            "MacroF1": 0.957381800109682,
            "Memory in Mb": 16.891732215881348,
            "Time in s": 465.74626
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9660245183887916,
            "MicroF1": 0.9660245183887916,
            "MacroF1": 0.93947544504001,
            "Memory in Mb": 22.937668800354004,
            "Time in s": 641.328845
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9616916947594238,
            "MicroF1": 0.9616916947594238,
            "MacroF1": 0.9454054748805116,
            "Memory in Mb": 29.12161636352539,
            "Time in s": 847.207258
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9607736311631708,
            "MicroF1": 0.9607736311631708,
            "MacroF1": 0.953605417859829,
            "Memory in Mb": 28.669262886047363,
            "Time in s": 1081.626023
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9578328021573916,
            "MicroF1": 0.9578328021573916,
            "MacroF1": 0.9463612240153172,
            "Memory in Mb": 34.20732402801514,
            "Time in s": 1345.493591
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9589926454201024,
            "MicroF1": 0.9589926454201024,
            "MacroF1": 0.9613092683363472,
            "Memory in Mb": 18.652557373046875,
            "Time in s": 1636.499529
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.960776302349336,
            "MicroF1": 0.960776302349336,
            "MacroF1": 0.9605208703626084,
            "Memory in Mb": 20.81053066253662,
            "Time in s": 1952.783692
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9615312087497644,
            "MicroF1": 0.9615312087497644,
            "MacroF1": 0.960303314983038,
            "Memory in Mb": 27.91543483734131,
            "Time in s": 2294.145458
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9616529504465068,
            "MicroF1": 0.9616529504465068,
            "MacroF1": 0.9605387671994152,
            "Memory in Mb": 32.60424041748047,
            "Time in s": 2660.691575
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9597973525085798,
            "MicroF1": 0.9597973525085798,
            "MacroF1": 0.9561203427932812,
            "Memory in Mb": 39.11091995239258,
            "Time in s": 3053.193204
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9589397885705532,
            "MicroF1": 0.9589397885705532,
            "MacroF1": 0.9571591040678328,
            "Memory in Mb": 29.255366325378414,
            "Time in s": 3470.643733
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.959913482335977,
            "MicroF1": 0.959913482335977,
            "MacroF1": 0.9605956598361812,
            "Memory in Mb": 31.930577278137207,
            "Time in s": 3910.602191
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9602342366880022,
            "MicroF1": 0.9602342366880022,
            "MacroF1": 0.95986198823556,
            "Memory in Mb": 26.562703132629395,
            "Time in s": 4374.151898
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9601341762353244,
            "MicroF1": 0.9601341762353244,
            "MacroF1": 0.959651045460586,
            "Memory in Mb": 31.588034629821777,
            "Time in s": 4858.190889
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9584507905380562,
            "MicroF1": 0.9584507905380562,
            "MacroF1": 0.9567204261955368,
            "Memory in Mb": 39.12565612792969,
            "Time in s": 5363.543193
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9579782887825375,
            "MicroF1": 0.9579782887825375,
            "MacroF1": 0.957794146577291,
            "Memory in Mb": 44.816758155822754,
            "Time in s": 5892.06228
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9579944289693594,
            "MicroF1": 0.9579944289693594,
            "MacroF1": 0.9581242571113368,
            "Memory in Mb": 49.5586576461792,
            "Time in s": 6445.036349
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9570499840136416,
            "MicroF1": 0.9570499840136416,
            "MacroF1": 0.9565283447410108,
            "Memory in Mb": 50.18536758422852,
            "Time in s": 7025.065903
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9563885200694516,
            "MicroF1": 0.9563885200694516,
            "MacroF1": 0.9560487952418978,
            "Memory in Mb": 54.40623474121094,
            "Time in s": 7630.795018999999
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9532307088930289,
            "MicroF1": 0.9532307088930289,
            "MacroF1": 0.9512518567217172,
            "Memory in Mb": 66.82855319976807,
            "Time in s": 8267.200675
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9519185443574998,
            "MicroF1": 0.9519185443574998,
            "MacroF1": 0.9512557409849248,
            "Memory in Mb": 41.17615795135498,
            "Time in s": 8934.408603
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9528824330458464,
            "MicroF1": 0.9528824330458464,
            "MacroF1": 0.953398407731189,
            "Memory in Mb": 32.87209510803223,
            "Time in s": 9625.903537
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.953689923837871,
            "MicroF1": 0.953689923837871,
            "MacroF1": 0.9540175301991308,
            "Memory in Mb": 28.078542709350582,
            "Time in s": 10339.782646
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9542726734849124,
            "MicroF1": 0.9542726734849124,
            "MacroF1": 0.9545119777330118,
            "Memory in Mb": 20.280012130737305,
            "Time in s": 11070.86282
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.955470218155078,
            "MicroF1": 0.955470218155078,
            "MacroF1": 0.9559406438939212,
            "Memory in Mb": 21.54300308227539,
            "Time in s": 11820.445116
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9559579346880684,
            "MicroF1": 0.9559579346880684,
            "MacroF1": 0.9561632451269844,
            "Memory in Mb": 26.89114284515381,
            "Time in s": 12588.394717
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9558789735733436,
            "MicroF1": 0.9558789735733436,
            "MacroF1": 0.9559075747932771,
            "Memory in Mb": 21.382742881774902,
            "Time in s": 13375.587705000002
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9563247418851668,
            "MicroF1": 0.9563247418851668,
            "MacroF1": 0.9565051554876024,
            "Memory in Mb": 21.864919662475582,
            "Time in s": 14180.68998
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.956960565207988,
            "MicroF1": 0.956960565207988,
            "MacroF1": 0.9571856017401092,
            "Memory in Mb": 25.72835636138916,
            "Time in s": 15004.794290000002
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9566496253239022,
            "MicroF1": 0.9566496253239022,
            "MacroF1": 0.9566382966080724,
            "Memory in Mb": 21.764866828918457,
            "Time in s": 15848.339318000002
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.957241097569279,
            "MicroF1": 0.9572410975692792,
            "MacroF1": 0.957426459656079,
            "Memory in Mb": 25.14582061767578,
            "Time in s": 16708.048820000004
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9580655846306724,
            "MicroF1": 0.9580655846306724,
            "MacroF1": 0.958277362015896,
            "Memory in Mb": 26.658535957336422,
            "Time in s": 17588.164126000003
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9584596529703928,
            "MicroF1": 0.9584596529703928,
            "MacroF1": 0.9585840009788792,
            "Memory in Mb": 30.76789283752441,
            "Time in s": 18489.703328000003
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.958079316196342,
            "MicroF1": 0.958079316196342,
            "MacroF1": 0.9580713134265896,
            "Memory in Mb": 27.786094665527344,
            "Time in s": 19412.324967000004
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.958514614866107,
            "MicroF1": 0.958514614866107,
            "MacroF1": 0.9586173296332884,
            "Memory in Mb": 25.79348850250244,
            "Time in s": 20355.979039000005
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9577330065164106,
            "MicroF1": 0.9577330065164106,
            "MacroF1": 0.9576699214368118,
            "Memory in Mb": 33.630208015441895,
            "Time in s": 21321.132478000007
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9576305806828128,
            "MicroF1": 0.9576305806828128,
            "MacroF1": 0.9576693803774444,
            "Memory in Mb": 33.920249938964844,
            "Time in s": 22315.653729000005
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.956506868836573,
            "MicroF1": 0.956506868836573,
            "MacroF1": 0.9564470129227676,
            "Memory in Mb": 31.50515556335449,
            "Time in s": 23335.132930000003
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9563812600969306,
            "MicroF1": 0.9563812600969306,
            "MacroF1": 0.9564135249623557,
            "Memory in Mb": 19.79563045501709,
            "Time in s": 24372.247222
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9569148646440436,
            "MicroF1": 0.9569148646440436,
            "MacroF1": 0.9569804233582648,
            "Memory in Mb": 23.70892333984375,
            "Time in s": 25428.663478
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9574252677572336,
            "MicroF1": 0.9574252677572336,
            "MacroF1": 0.957475477736454,
            "Memory in Mb": 21.893744468688965,
            "Time in s": 26504.246634000003
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9568187744458932,
            "MicroF1": 0.9568187744458932,
            "MacroF1": 0.956806677474395,
            "Memory in Mb": 28.04871368408203,
            "Time in s": 27598.635240000003
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9567992646683348,
            "MicroF1": 0.9567992646683348,
            "MacroF1": 0.9568012672257532,
            "Memory in Mb": 32.11082458496094,
            "Time in s": 28712.463090000005
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9565304386974138,
            "MicroF1": 0.9565304386974138,
            "MacroF1": 0.9565268274864178,
            "Memory in Mb": 40.13526153564453,
            "Time in s": 29849.822929000005
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Streaming Random Patches",
            "dataset": "Keystroke",
            "Accuracy": 0.9559292122162852,
            "MicroF1": 0.9559292122162852,
            "MacroF1": 0.9559196349550496,
            "Memory in Mb": 39.63601016998291,
            "Time in s": 31009.846621000004
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.5111111111111111,
            "MicroF1": 0.5111111111111111,
            "MacroF1": 0.4093857832988268,
            "Memory in Mb": 0.0911636352539062,
            "Time in s": 0.155273
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.6043956043956044,
            "MicroF1": 0.6043956043956044,
            "MacroF1": 0.5940974230447915,
            "Memory in Mb": 0.16827392578125,
            "Time in s": 0.72683
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.6715328467153284,
            "MicroF1": 0.6715328467153284,
            "MacroF1": 0.6806196928151186,
            "Memory in Mb": 0.245431900024414,
            "Time in s": 1.742293
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7049180327868853,
            "MicroF1": 0.7049180327868853,
            "MacroF1": 0.7184732466987995,
            "Memory in Mb": 0.3220462799072265,
            "Time in s": 3.340711
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.74235807860262,
            "MicroF1": 0.74235807860262,
            "MacroF1": 0.7523809662907407,
            "Memory in Mb": 0.3991765975952148,
            "Time in s": 5.610709
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7490909090909091,
            "MicroF1": 0.7490909090909091,
            "MacroF1": 0.7611097615339608,
            "Memory in Mb": 0.4767560958862304,
            "Time in s": 8.7745
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7663551401869159,
            "MicroF1": 0.766355140186916,
            "MacroF1": 0.7725898650917747,
            "Memory in Mb": 0.5538606643676758,
            "Time in s": 12.918764
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.784741144414169,
            "MicroF1": 0.7847411444141691,
            "MacroF1": 0.7844949397573193,
            "Memory in Mb": 0.6304874420166016,
            "Time in s": 18.189003
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7990314769975787,
            "MicroF1": 0.7990314769975787,
            "MacroF1": 0.7976353129150817,
            "Memory in Mb": 0.7076187133789062,
            "Time in s": 24.731741
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7952069716775599,
            "MicroF1": 0.7952069716775599,
            "MacroF1": 0.7930763833747545,
            "Memory in Mb": 0.7847471237182617,
            "Time in s": 32.681045
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.7960396039603961,
            "MicroF1": 0.7960396039603961,
            "MacroF1": 0.7941234022368324,
            "Memory in Mb": 3.003793716430664,
            "Time in s": 61.21191
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8021778584392014,
            "MicroF1": 0.8021778584392014,
            "MacroF1": 0.8007250644998717,
            "Memory in Mb": 3.2264842987060547,
            "Time in s": 91.162029
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8090452261306532,
            "MicroF1": 0.8090452261306531,
            "MacroF1": 0.8095532779239047,
            "Memory in Mb": 3.4499826431274414,
            "Time in s": 122.67972799999998
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8164852255054432,
            "MicroF1": 0.8164852255054433,
            "MacroF1": 0.8176018556357175,
            "Memory in Mb": 3.6760778427124015,
            "Time in s": 155.77468699999997
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8214804063860668,
            "MicroF1": 0.8214804063860668,
            "MacroF1": 0.8221151176242331,
            "Memory in Mb": 3.8941650390625,
            "Time in s": 190.537277
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8272108843537415,
            "MicroF1": 0.8272108843537415,
            "MacroF1": 0.8281233770721121,
            "Memory in Mb": 4.128121376037598,
            "Time in s": 227.085503
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8361075544174136,
            "MicroF1": 0.8361075544174136,
            "MacroF1": 0.8364659566156888,
            "Memory in Mb": 4.367749214172363,
            "Time in s": 265.419762
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8403869407496977,
            "MicroF1": 0.8403869407496977,
            "MacroF1": 0.8412749002251585,
            "Memory in Mb": 4.601743698120117,
            "Time in s": 305.543518
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.845360824742268,
            "MicroF1": 0.845360824742268,
            "MacroF1": 0.8465057584066101,
            "Memory in Mb": 4.840575218200684,
            "Time in s": 347.501906
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8487486398258978,
            "MicroF1": 0.8487486398258978,
            "MacroF1": 0.8489576083149123,
            "Memory in Mb": 5.074535369873047,
            "Time in s": 391.430234
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8538860103626943,
            "MicroF1": 0.8538860103626943,
            "MacroF1": 0.8530581393966605,
            "Memory in Mb": 5.3079938888549805,
            "Time in s": 437.316456
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8585558852621167,
            "MicroF1": 0.8585558852621167,
            "MacroF1": 0.8570252804249208,
            "Memory in Mb": 5.479596138000488,
            "Time in s": 485.23685
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8628192999053926,
            "MicroF1": 0.8628192999053927,
            "MacroF1": 0.8611045332429007,
            "Memory in Mb": 5.435150146484375,
            "Time in s": 535.278485
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8631006346328196,
            "MicroF1": 0.8631006346328196,
            "MacroF1": 0.8616288881212748,
            "Memory in Mb": 5.355225563049316,
            "Time in s": 587.436372
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8668407310704961,
            "MicroF1": 0.8668407310704961,
            "MacroF1": 0.8650902600877293,
            "Memory in Mb": 5.281754493713379,
            "Time in s": 641.538536
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8719665271966527,
            "MicroF1": 0.8719665271966527,
            "MacroF1": 0.8702683106604537,
            "Memory in Mb": 5.235520362854004,
            "Time in s": 697.554251
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8759065269943593,
            "MicroF1": 0.8759065269943593,
            "MacroF1": 0.8740479640614998,
            "Memory in Mb": 5.142333984375,
            "Time in s": 755.471933
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8787878787878788,
            "MicroF1": 0.8787878787878788,
            "MacroF1": 0.8772603222806128,
            "Memory in Mb": 5.092559814453125,
            "Time in s": 815.138635
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8777194298574643,
            "MicroF1": 0.8777194298574643,
            "MacroF1": 0.8760741143565023,
            "Memory in Mb": 5.055940628051758,
            "Time in s": 876.491339
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8796229151559101,
            "MicroF1": 0.8796229151559101,
            "MacroF1": 0.8783130803325612,
            "Memory in Mb": 4.964084625244141,
            "Time in s": 939.483975
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8785964912280702,
            "MicroF1": 0.8785964912280702,
            "MacroF1": 0.8768931648451159,
            "Memory in Mb": 4.951287269592285,
            "Time in s": 1004.010152
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8769544527532291,
            "MicroF1": 0.8769544527532291,
            "MacroF1": 0.8748964905672628,
            "Memory in Mb": 4.969002723693848,
            "Time in s": 1070.168576
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8727752142386289,
            "MicroF1": 0.8727752142386289,
            "MacroF1": 0.8705110235515202,
            "Memory in Mb": 5.101251602172852,
            "Time in s": 1138.304608
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8688419705694178,
            "MicroF1": 0.8688419705694178,
            "MacroF1": 0.8667015278861958,
            "Memory in Mb": 5.262187957763672,
            "Time in s": 1208.4659419999998
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8651336233685519,
            "MicroF1": 0.8651336233685519,
            "MacroF1": 0.8631350462642483,
            "Memory in Mb": 5.320252418518066,
            "Time in s": 1280.5305069999995
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8640483383685801,
            "MicroF1": 0.8640483383685801,
            "MacroF1": 0.8620479268968886,
            "Memory in Mb": 5.35189151763916,
            "Time in s": 1354.3819709999998
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8647854203409759,
            "MicroF1": 0.8647854203409759,
            "MacroF1": 0.8635043959538364,
            "Memory in Mb": 5.359102249145508,
            "Time in s": 1430.0286029999995
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.866056096164854,
            "MicroF1": 0.866056096164854,
            "MacroF1": 0.864439618601765,
            "Memory in Mb": 5.402237892150879,
            "Time in s": 1507.5136589999995
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8683770217512549,
            "MicroF1": 0.8683770217512549,
            "MacroF1": 0.8664209902402824,
            "Memory in Mb": 5.3993330001831055,
            "Time in s": 1586.7199259999998
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8694942903752039,
            "MicroF1": 0.8694942903752039,
            "MacroF1": 0.867597342266498,
            "Memory in Mb": 5.4049272537231445,
            "Time in s": 1667.658732
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8710875331564987,
            "MicroF1": 0.8710875331564986,
            "MacroF1": 0.8694766742923737,
            "Memory in Mb": 5.4121294021606445,
            "Time in s": 1750.3169159999998
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8705334023821854,
            "MicroF1": 0.8705334023821854,
            "MacroF1": 0.8686918451193435,
            "Memory in Mb": 5.405803680419922,
            "Time in s": 1834.60998
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8715225088517956,
            "MicroF1": 0.8715225088517956,
            "MacroF1": 0.8698703895904014,
            "Memory in Mb": 5.395906448364258,
            "Time in s": 1920.517128
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8729609490855166,
            "MicroF1": 0.8729609490855166,
            "MacroF1": 0.870902914954928,
            "Memory in Mb": 5.386837959289551,
            "Time in s": 2008.106455
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8733687771870469,
            "MicroF1": 0.8733687771870469,
            "MacroF1": 0.8714525187304558,
            "Memory in Mb": 5.375288963317871,
            "Time in s": 2097.403794
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.875177304964539,
            "MicroF1": 0.875177304964539,
            "MacroF1": 0.8730645404016979,
            "Memory in Mb": 5.353263854980469,
            "Time in s": 2188.326937
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8745950948634891,
            "MicroF1": 0.8745950948634891,
            "MacroF1": 0.872417325547954,
            "Memory in Mb": 5.322790145874023,
            "Time in s": 2280.882375
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8753964657906661,
            "MicroF1": 0.8753964657906661,
            "MacroF1": 0.8732500176589647,
            "Memory in Mb": 5.30323600769043,
            "Time in s": 2374.975797
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8748335552596538,
            "MicroF1": 0.8748335552596538,
            "MacroF1": 0.8732733602208504,
            "Memory in Mb": 5.278659820556641,
            "Time in s": 2470.732765
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8742931709438887,
            "MicroF1": 0.8742931709438887,
            "MacroF1": 0.8727466012343671,
            "Memory in Mb": 5.262259483337402,
            "Time in s": 2568.119206
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "ImageSegments",
            "Accuracy": 0.8735383282806409,
            "MicroF1": 0.8735383282806409,
            "MacroF1": 0.8721361121313428,
            "Memory in Mb": 5.268708229064941,
            "Time in s": 2666.293295
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6597156398104266,
            "MicroF1": 0.6597156398104266,
            "MacroF1": 0.5853273709738578,
            "Memory in Mb": 6.371035575866699,
            "Time in s": 65.756564
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6807200378967314,
            "MicroF1": 0.6807200378967314,
            "MacroF1": 0.5992086579995298,
            "Memory in Mb": 6.278300285339356,
            "Time in s": 182.184591
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6842437638143354,
            "MicroF1": 0.6842437638143354,
            "MacroF1": 0.6001715208792017,
            "Memory in Mb": 6.298460006713867,
            "Time in s": 341.998975
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6848212171442103,
            "MicroF1": 0.6848212171442103,
            "MacroF1": 0.6051604277089342,
            "Memory in Mb": 6.265153884887695,
            "Time in s": 541.5068689999999
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6872513733661678,
            "MicroF1": 0.6872513733661678,
            "MacroF1": 0.611100448555976,
            "Memory in Mb": 6.2555742263793945,
            "Time in s": 777.52113
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6842936069455406,
            "MicroF1": 0.6842936069455406,
            "MacroF1": 0.6118525331169307,
            "Memory in Mb": 6.314010620117188,
            "Time in s": 1048.588472
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6852929238262752,
            "MicroF1": 0.6852929238262752,
            "MacroF1": 0.6157762907660722,
            "Memory in Mb": 6.288516998291016,
            "Time in s": 1352.458798
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6828459808215934,
            "MicroF1": 0.6828459808215934,
            "MacroF1": 0.6148503710479976,
            "Memory in Mb": 6.31680965423584,
            "Time in s": 1687.096094
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6851520572450805,
            "MicroF1": 0.6851520572450805,
            "MacroF1": 0.6155258331015067,
            "Memory in Mb": 6.223039627075195,
            "Time in s": 2051.649807
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6861445212614831,
            "MicroF1": 0.6861445212614831,
            "MacroF1": 0.6169474950376627,
            "Memory in Mb": 6.253497123718262,
            "Time in s": 2444.130945
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6873009040034438,
            "MicroF1": 0.6873009040034438,
            "MacroF1": 0.6200568175672779,
            "Memory in Mb": 6.251482009887695,
            "Time in s": 2863.128904
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6866072133217583,
            "MicroF1": 0.6866072133217583,
            "MacroF1": 0.623883491026523,
            "Memory in Mb": 6.276742935180664,
            "Time in s": 3309.082968
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7020470605376266,
            "MicroF1": 0.7020470605376266,
            "MacroF1": 0.6991473808978487,
            "Memory in Mb": 6.26933479309082,
            "Time in s": 3781.277509
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7077724413177299,
            "MicroF1": 0.7077724413177299,
            "MacroF1": 0.7078402863830927,
            "Memory in Mb": 6.244691848754883,
            "Time in s": 4278.402760999999
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7016857124818486,
            "MicroF1": 0.7016857124818486,
            "MacroF1": 0.704840832390747,
            "Memory in Mb": 6.350223541259766,
            "Time in s": 4805.403565999999
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6992009470257473,
            "MicroF1": 0.6992009470257473,
            "MacroF1": 0.7048178275842342,
            "Memory in Mb": 6.243149757385254,
            "Time in s": 5357.683726999999
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6922734109520361,
            "MicroF1": 0.6922734109520361,
            "MacroF1": 0.6995766929659905,
            "Memory in Mb": 6.218992233276367,
            "Time in s": 5935.240105999998
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6974272636397116,
            "MicroF1": 0.6974272636397116,
            "MacroF1": 0.7006862112488368,
            "Memory in Mb": 6.24652099609375,
            "Time in s": 6538.276384999998
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.699845486716842,
            "MicroF1": 0.699845486716842,
            "MacroF1": 0.6985118222305657,
            "Memory in Mb": 6.205791473388672,
            "Time in s": 7167.459726999999
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7016904209479615,
            "MicroF1": 0.7016904209479615,
            "MacroF1": 0.6971610909052677,
            "Memory in Mb": 6.218420028686523,
            "Time in s": 7825.840650999999
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7039909808342728,
            "MicroF1": 0.7039909808342728,
            "MacroF1": 0.6964197759629052,
            "Memory in Mb": 6.236072540283203,
            "Time in s": 8511.079801999998
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7076320433902974,
            "MicroF1": 0.7076320433902974,
            "MacroF1": 0.697368621848442,
            "Memory in Mb": 6.279313087463379,
            "Time in s": 9222.986801999998
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7098447729237863,
            "MicroF1": 0.7098447729237863,
            "MacroF1": 0.6967477548491564,
            "Memory in Mb": 6.2948198318481445,
            "Time in s": 9960.927248999997
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7127017322337529,
            "MicroF1": 0.712701732233753,
            "MacroF1": 0.6972185032799825,
            "Memory in Mb": 6.224791526794434,
            "Time in s": 10724.419586999997
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7145346414636918,
            "MicroF1": 0.7145346414636918,
            "MacroF1": 0.6967850611237018,
            "Memory in Mb": 6.263523101806641,
            "Time in s": 11512.986172999998
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7156437807321071,
            "MicroF1": 0.7156437807321071,
            "MacroF1": 0.6955595874776194,
            "Memory in Mb": 6.272575378417969,
            "Time in s": 12326.628602999996
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7130931921012942,
            "MicroF1": 0.7130931921012942,
            "MacroF1": 0.6943090782068162,
            "Memory in Mb": 6.22489070892334,
            "Time in s": 13165.433758999998
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7117732607298678,
            "MicroF1": 0.7117732607298677,
            "MacroF1": 0.6978751959025926,
            "Memory in Mb": 6.217726707458496,
            "Time in s": 14028.837757999998
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7122097769650263,
            "MicroF1": 0.7122097769650264,
            "MacroF1": 0.7026862643890369,
            "Memory in Mb": 6.243690490722656,
            "Time in s": 14916.319239
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7113545250797058,
            "MicroF1": 0.7113545250797058,
            "MacroF1": 0.7052714328980031,
            "Memory in Mb": 6.277059555053711,
            "Time in s": 15827.904481999998
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7111959676187567,
            "MicroF1": 0.7111959676187566,
            "MacroF1": 0.7078689284492299,
            "Memory in Mb": 6.295280456542969,
            "Time in s": 16762.400180999997
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7067562368678051,
            "MicroF1": 0.7067562368678051,
            "MacroF1": 0.704703743720216,
            "Memory in Mb": 6.183221817016602,
            "Time in s": 17721.950532
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7030734353028956,
            "MicroF1": 0.7030734353028956,
            "MacroF1": 0.7010614031639846,
            "Memory in Mb": 6.343389511108398,
            "Time in s": 18710.094933
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6998022449377489,
            "MicroF1": 0.6998022449377489,
            "MacroF1": 0.6976694331042329,
            "Memory in Mb": 6.273009300231934,
            "Time in s": 19725.980479
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6967179847939609,
            "MicroF1": 0.6967179847939609,
            "MacroF1": 0.6945045780432343,
            "Memory in Mb": 6.264690399169922,
            "Time in s": 20767.047301
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6941470472182033,
            "MicroF1": 0.6941470472182033,
            "MacroF1": 0.6917813776610243,
            "Memory in Mb": 6.265054702758789,
            "Time in s": 21835.556239
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.691996621535154,
            "MicroF1": 0.691996621535154,
            "MacroF1": 0.6898060776768534,
            "Memory in Mb": 6.200959205627441,
            "Time in s": 22932.108791
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6904328756199068,
            "MicroF1": 0.6904328756199068,
            "MacroF1": 0.6882031611963276,
            "Memory in Mb": 6.413609504699707,
            "Time in s": 24054.967875
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6916446106403128,
            "MicroF1": 0.6916446106403128,
            "MacroF1": 0.6892941373261507,
            "Memory in Mb": 6.310104370117188,
            "Time in s": 25204.026441
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.692535334643339,
            "MicroF1": 0.692535334643339,
            "MacroF1": 0.6900712004452627,
            "Memory in Mb": 6.22797966003418,
            "Time in s": 26378.286294
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6935904838895947,
            "MicroF1": 0.6935904838895947,
            "MacroF1": 0.6909354899104013,
            "Memory in Mb": 6.220904350280762,
            "Time in s": 27574.213319
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6941895334941715,
            "MicroF1": 0.6941895334941715,
            "MacroF1": 0.691322114366645,
            "Memory in Mb": 6.22946834564209,
            "Time in s": 28791.926615000004
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6950690422181602,
            "MicroF1": 0.6950690422181602,
            "MacroF1": 0.6917362410920441,
            "Memory in Mb": 6.2850341796875,
            "Time in s": 30030.670852000003
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6964466349568473,
            "MicroF1": 0.6964466349568473,
            "MacroF1": 0.6926338572817136,
            "Memory in Mb": 6.233500480651856,
            "Time in s": 31290.345387
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.6963530377322755,
            "MicroF1": 0.6963530377322755,
            "MacroF1": 0.6929015597977773,
            "Memory in Mb": 6.243911743164063,
            "Time in s": 32571.46119
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7006073082861555,
            "MicroF1": 0.7006073082861555,
            "MacroF1": 0.697843135408715,
            "Memory in Mb": 6.247167587280273,
            "Time in s": 33874.398319
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7046805424029337,
            "MicroF1": 0.7046805424029337,
            "MacroF1": 0.7023003034160373,
            "Memory in Mb": 6.246943473815918,
            "Time in s": 35198.416197
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7083867658373942,
            "MicroF1": 0.7083867658373942,
            "MacroF1": 0.7061355873839065,
            "Memory in Mb": 6.210485458374023,
            "Time in s": 36536.506394
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7126567844925884,
            "MicroF1": 0.7126567844925883,
            "MacroF1": 0.7104085577951368,
            "Memory in Mb": 6.270394325256348,
            "Time in s": 37890.628371
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7128544101214038,
            "MicroF1": 0.7128544101214038,
            "MacroF1": 0.7110869129037599,
            "Memory in Mb": 6.247260093688965,
            "Time in s": 39264.666928
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Insects",
            "Accuracy": 0.7131152194069673,
            "MicroF1": 0.7131152194069672,
            "MacroF1": 0.7113808258412672,
            "Memory in Mb": 6.272693634033203,
            "Time in s": 40639.937472
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9803439803439804,
            "MicroF1": 0.9803439803439804,
            "MacroF1": 0.4950372208436724,
            "Memory in Mb": 1.0294876098632812,
            "Time in s": 8.610537
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9251533742331288,
            "MicroF1": 0.9251533742331288,
            "MacroF1": 0.8588670451436246,
            "Memory in Mb": 5.3865966796875,
            "Time in s": 60.879099
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9247751430907604,
            "MicroF1": 0.9247751430907604,
            "MacroF1": 0.888226412135106,
            "Memory in Mb": 6.246823310852051,
            "Time in s": 137.71097600000002
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.927038626609442,
            "MicroF1": 0.927038626609442,
            "MacroF1": 0.893336805209695,
            "Memory in Mb": 6.212030410766602,
            "Time in s": 236.990146
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9298675821481118,
            "MicroF1": 0.9298675821481118,
            "MacroF1": 0.911424130088645,
            "Memory in Mb": 6.329436302185059,
            "Time in s": 359.011082
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9239885574172456,
            "MicroF1": 0.9239885574172456,
            "MacroF1": 0.912155547295492,
            "Memory in Mb": 6.208271026611328,
            "Time in s": 503.2068
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9169877408056042,
            "MicroF1": 0.9169877408056042,
            "MacroF1": 0.8816257260944811,
            "Memory in Mb": 6.284844398498535,
            "Time in s": 667.387655
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.908979466748391,
            "MicroF1": 0.908979466748391,
            "MacroF1": 0.9011431783951356,
            "Memory in Mb": 6.232160568237305,
            "Time in s": 850.70223
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.913375102152002,
            "MicroF1": 0.913375102152002,
            "MacroF1": 0.9125908871445696,
            "Memory in Mb": 6.234919548034668,
            "Time in s": 1054.346916
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9141946555528316,
            "MicroF1": 0.9141946555528316,
            "MacroF1": 0.9054789816810688,
            "Memory in Mb": 6.308258056640625,
            "Time in s": 1277.35851
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9057276576777356,
            "MicroF1": 0.9057276576777356,
            "MacroF1": 0.9087691557812896,
            "Memory in Mb": 6.274983406066895,
            "Time in s": 1518.241674
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.908682328907048,
            "MicroF1": 0.908682328907048,
            "MacroF1": 0.9101970481905532,
            "Memory in Mb": 6.210176467895508,
            "Time in s": 1774.8436390000002
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9092966245521404,
            "MicroF1": 0.9092966245521404,
            "MacroF1": 0.9045962329696908,
            "Memory in Mb": 6.311163902282715,
            "Time in s": 2048.2991580000003
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9110488530905272,
            "MicroF1": 0.9110488530905272,
            "MacroF1": 0.9114244990736602,
            "Memory in Mb": 6.304790496826172,
            "Time in s": 2337.0378760000003
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9089720542572316,
            "MicroF1": 0.9089720542572316,
            "MacroF1": 0.9032533666541098,
            "Memory in Mb": 6.217576026916504,
            "Time in s": 2640.3521840000003
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.907767734027884,
            "MicroF1": 0.907767734027884,
            "MacroF1": 0.9071900335968284,
            "Memory in Mb": 6.258184432983398,
            "Time in s": 2958.617579
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9105984138428262,
            "MicroF1": 0.9105984138428262,
            "MacroF1": 0.9126270814361048,
            "Memory in Mb": 6.1720380783081055,
            "Time in s": 3289.9253120000003
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9120250578782514,
            "MicroF1": 0.9120250578782514,
            "MacroF1": 0.9125633522308232,
            "Memory in Mb": 6.2164154052734375,
            "Time in s": 3633.832057000001
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9133015094826474,
            "MicroF1": 0.9133015094826474,
            "MacroF1": 0.9136330015220732,
            "Memory in Mb": 6.260525703430176,
            "Time in s": 3992.050824
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9148179924010296,
            "MicroF1": 0.9148179924010296,
            "MacroF1": 0.9154195917586072,
            "Memory in Mb": 6.291139602661133,
            "Time in s": 4363.477247000001
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9166569394186996,
            "MicroF1": 0.9166569394186996,
            "MacroF1": 0.917708642296068,
            "Memory in Mb": 6.216147422790527,
            "Time in s": 4747.269196000001
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9179944289693592,
            "MicroF1": 0.9179944289693592,
            "MacroF1": 0.9193727618453186,
            "Memory in Mb": 6.204837799072266,
            "Time in s": 5142.613476000001
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9180432697431524,
            "MicroF1": 0.9180432697431524,
            "MacroF1": 0.9181590265081532,
            "Memory in Mb": 6.197464942932129,
            "Time in s": 5549.1165660000015
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9166581554488816,
            "MicroF1": 0.9166581554488816,
            "MacroF1": 0.9168210748678532,
            "Memory in Mb": 6.232473373413086,
            "Time in s": 5968.023607000002
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9154819099911756,
            "MicroF1": 0.9154819099911756,
            "MacroF1": 0.9145218669909496,
            "Memory in Mb": 6.197787284851074,
            "Time in s": 6399.011787000002
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9126048835674556,
            "MicroF1": 0.9126048835674556,
            "MacroF1": 0.9111025938131312,
            "Memory in Mb": 6.2185258865356445,
            "Time in s": 6842.990199000003
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9106672719019518,
            "MicroF1": 0.9106672719019518,
            "MacroF1": 0.911227786024665,
            "Memory in Mb": 6.261377334594727,
            "Time in s": 7300.041981000002
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.910356298695614,
            "MicroF1": 0.910356298695614,
            "MacroF1": 0.9101104800687124,
            "Memory in Mb": 6.227293968200684,
            "Time in s": 7769.979179000002
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9092215366410278,
            "MicroF1": 0.9092215366410278,
            "MacroF1": 0.909418612123662,
            "Memory in Mb": 6.287784576416016,
            "Time in s": 8252.975566000001
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9110221423318898,
            "MicroF1": 0.9110221423318898,
            "MacroF1": 0.9118339797691072,
            "Memory in Mb": 6.31197452545166,
            "Time in s": 8747.696417000001
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.912627500593026,
            "MicroF1": 0.912627500593026,
            "MacroF1": 0.9131272841889786,
            "Memory in Mb": 6.279851913452148,
            "Time in s": 9255.008595
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9129069322098812,
            "MicroF1": 0.9129069322098812,
            "MacroF1": 0.913006147591119,
            "Memory in Mb": 6.346117973327637,
            "Time in s": 9774.692327
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9136150932184506,
            "MicroF1": 0.9136150932184506,
            "MacroF1": 0.9138210444048112,
            "Memory in Mb": 6.238006591796875,
            "Time in s": 10306.725428000002
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9137769447047798,
            "MicroF1": 0.9137769447047795,
            "MacroF1": 0.913931693448659,
            "Memory in Mb": 6.288792610168457,
            "Time in s": 10851.686584
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.91217872400028,
            "MicroF1": 0.91217872400028,
            "MacroF1": 0.9118234284090696,
            "Memory in Mb": 6.252389907836914,
            "Time in s": 11409.551357
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9133247089262612,
            "MicroF1": 0.9133247089262612,
            "MacroF1": 0.9136581918124824,
            "Memory in Mb": 6.268362998962402,
            "Time in s": 11980.223294
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9134150380920836,
            "MicroF1": 0.9134150380920836,
            "MacroF1": 0.9134700562544148,
            "Memory in Mb": 6.304409027099609,
            "Time in s": 12563.090191
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9127910726956072,
            "MicroF1": 0.9127910726956072,
            "MacroF1": 0.9127632118282708,
            "Memory in Mb": 6.222077369689941,
            "Time in s": 13158.500652
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9127019043429074,
            "MicroF1": 0.9127019043429074,
            "MacroF1": 0.9127365496247324,
            "Memory in Mb": 6.263586044311523,
            "Time in s": 13766.752283999998
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9113303511244562,
            "MicroF1": 0.9113303511244562,
            "MacroF1": 0.9110956080213112,
            "Memory in Mb": 6.256609916687012,
            "Time in s": 14388.121762
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.910384408441442,
            "MicroF1": 0.910384408441442,
            "MacroF1": 0.910332436025812,
            "Memory in Mb": 6.208023071289063,
            "Time in s": 15023.088924
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9113510358914504,
            "MicroF1": 0.9113510358914504,
            "MacroF1": 0.9114963483082136,
            "Memory in Mb": 6.223179817199707,
            "Time in s": 15670.063673
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9113606566721768,
            "MicroF1": 0.9113606566721768,
            "MacroF1": 0.9113826667045092,
            "Memory in Mb": 6.23558235168457,
            "Time in s": 16331.265293
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9114255473232687,
            "MicroF1": 0.911425547323269,
            "MacroF1": 0.9114384409485988,
            "Memory in Mb": 6.255133628845215,
            "Time in s": 17006.553944
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9126858761370444,
            "MicroF1": 0.9126858761370444,
            "MacroF1": 0.9127656000580756,
            "Memory in Mb": 6.270404815673828,
            "Time in s": 17693.792261
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9125059945649278,
            "MicroF1": 0.9125059945649276,
            "MacroF1": 0.9124701420883568,
            "Memory in Mb": 6.180520057678223,
            "Time in s": 18393.849908
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.912594524119948,
            "MicroF1": 0.912594524119948,
            "MacroF1": 0.9125632790621416,
            "Memory in Mb": 6.265439987182617,
            "Time in s": 19106.227212
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.913547464637696,
            "MicroF1": 0.913547464637696,
            "MacroF1": 0.9135225066457016,
            "Memory in Mb": 6.303133964538574,
            "Time in s": 19831.701162
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9111099994997748,
            "MicroF1": 0.9111099994997748,
            "MacroF1": 0.910917465793804,
            "Memory in Mb": 6.225028991699219,
            "Time in s": 20571.760391
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "k-Nearest Neighbors",
            "dataset": "Keystroke",
            "Accuracy": 0.9104858081278494,
            "MicroF1": 0.9104858081278494,
            "MacroF1": 0.910327982122686,
            "Memory in Mb": 6.325108528137207,
            "Time in s": 21326.45228
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.3111111111111111,
            "MicroF1": 0.3111111111111111,
            "MacroF1": 0.245764972655729,
            "Memory in Mb": 4.105147361755371,
            "Time in s": 2.153154
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.4835164835164835,
            "MicroF1": 0.4835164835164835,
            "MacroF1": 0.4934752395581889,
            "Memory in Mb": 4.108363151550293,
            "Time in s": 6.907408
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5328467153284672,
            "MicroF1": 0.5328467153284672,
            "MacroF1": 0.5528821792646677,
            "Memory in Mb": 4.108027458190918,
            "Time in s": 14.639156
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5956284153005464,
            "MicroF1": 0.5956284153005464,
            "MacroF1": 0.614143164890895,
            "Memory in Mb": 4.108977317810059,
            "Time in s": 25.443956
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.62882096069869,
            "MicroF1": 0.62882096069869,
            "MacroF1": 0.6441389332893815,
            "Memory in Mb": 3.881842613220215,
            "Time in s": 39.254234
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.64,
            "MicroF1": 0.64,
            "MacroF1": 0.6559607038460422,
            "Memory in Mb": 3.996514320373535,
            "Time in s": 55.768073
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6697819314641744,
            "MicroF1": 0.6697819314641744,
            "MacroF1": 0.6706320385346652,
            "Memory in Mb": 4.112936019897461,
            "Time in s": 74.877199
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6948228882833788,
            "MicroF1": 0.6948228882833788,
            "MacroF1": 0.6897433526546475,
            "Memory in Mb": 4.112924575805664,
            "Time in s": 96.687005
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.711864406779661,
            "MicroF1": 0.711864406779661,
            "MacroF1": 0.706570530482581,
            "Memory in Mb": 4.117301940917969,
            "Time in s": 121.290167
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7145969498910676,
            "MicroF1": 0.7145969498910676,
            "MacroF1": 0.7071122267088654,
            "Memory in Mb": 4.116390228271484,
            "Time in s": 148.551711
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7247524752475247,
            "MicroF1": 0.7247524752475247,
            "MacroF1": 0.7147973207987898,
            "Memory in Mb": 4.115703582763672,
            "Time in s": 178.365171
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7295825771324864,
            "MicroF1": 0.7295825771324864,
            "MacroF1": 0.7210771168277493,
            "Memory in Mb": 4.115436553955078,
            "Time in s": 210.796119
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7336683417085427,
            "MicroF1": 0.7336683417085426,
            "MacroF1": 0.7250288715672424,
            "Memory in Mb": 4.115207672119141,
            "Time in s": 245.953277
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7325038880248833,
            "MicroF1": 0.7325038880248833,
            "MacroF1": 0.7258924883659029,
            "Memory in Mb": 4.118658065795898,
            "Time in s": 283.80303000000004
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.737300435413643,
            "MicroF1": 0.737300435413643,
            "MacroF1": 0.7302536378735861,
            "Memory in Mb": 4.118425369262695,
            "Time in s": 324.296282
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7387755102040816,
            "MicroF1": 0.7387755102040816,
            "MacroF1": 0.7329631379486719,
            "Memory in Mb": 4.118097305297852,
            "Time in s": 367.43284
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7439180537772087,
            "MicroF1": 0.7439180537772088,
            "MacroF1": 0.7387105187530085,
            "Memory in Mb": 4.117616653442383,
            "Time in s": 413.28289
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7460701330108828,
            "MicroF1": 0.7460701330108827,
            "MacroF1": 0.7425025596154723,
            "Memory in Mb": 4.117326736450195,
            "Time in s": 461.953497
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7514318442153494,
            "MicroF1": 0.7514318442153494,
            "MacroF1": 0.7467163857842193,
            "Memory in Mb": 4.117303848266602,
            "Time in s": 513.2937440000001
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.750816104461371,
            "MicroF1": 0.750816104461371,
            "MacroF1": 0.7453933609147309,
            "Memory in Mb": 4.117105484008789,
            "Time in s": 567.431634
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7512953367875648,
            "MicroF1": 0.7512953367875648,
            "MacroF1": 0.7451117895470661,
            "Memory in Mb": 4.116701126098633,
            "Time in s": 624.2209760000001
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7507418397626113,
            "MicroF1": 0.7507418397626113,
            "MacroF1": 0.744963080481548,
            "Memory in Mb": 4.116399765014648,
            "Time in s": 683.8404210000001
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7511825922421949,
            "MicroF1": 0.7511825922421949,
            "MacroF1": 0.7446315489945475,
            "Memory in Mb": 4.117582321166992,
            "Time in s": 746.2097300000001
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7533998186763372,
            "MicroF1": 0.7533998186763373,
            "MacroF1": 0.7466082689908061,
            "Memory in Mb": 4.117956161499023,
            "Time in s": 811.1743250000002
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7563098346388164,
            "MicroF1": 0.7563098346388164,
            "MacroF1": 0.7491651771194966,
            "Memory in Mb": 4.117490768432617,
            "Time in s": 878.6809830000002
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7589958158995815,
            "MicroF1": 0.7589958158995815,
            "MacroF1": 0.7526420027035883,
            "Memory in Mb": 4.117303848266602,
            "Time in s": 948.8627130000002
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.75825946817083,
            "MicroF1": 0.7582594681708301,
            "MacroF1": 0.7524016178277559,
            "Memory in Mb": 4.11713981628418,
            "Time in s": 1021.5806660000002
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7637917637917638,
            "MicroF1": 0.7637917637917638,
            "MacroF1": 0.75666252908711,
            "Memory in Mb": 4.117353439331055,
            "Time in s": 1096.9757510000002
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7636909227306826,
            "MicroF1": 0.7636909227306825,
            "MacroF1": 0.7569484848610158,
            "Memory in Mb": 4.11726188659668,
            "Time in s": 1175.015685
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7650471356055112,
            "MicroF1": 0.7650471356055112,
            "MacroF1": 0.7590436403579585,
            "Memory in Mb": 4.11729621887207,
            "Time in s": 1255.693831
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.767719298245614,
            "MicroF1": 0.767719298245614,
            "MacroF1": 0.761211289695921,
            "Memory in Mb": 4.117136001586914,
            "Time in s": 1338.965745
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7722637661454793,
            "MicroF1": 0.7722637661454793,
            "MacroF1": 0.764056696643358,
            "Memory in Mb": 4.117197036743164,
            "Time in s": 1424.822234
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7732366512854317,
            "MicroF1": 0.7732366512854317,
            "MacroF1": 0.764234133414765,
            "Memory in Mb": 4.117246627807617,
            "Time in s": 1513.291691
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7735124760076776,
            "MicroF1": 0.7735124760076776,
            "MacroF1": 0.7653316001442944,
            "Memory in Mb": 4.117277145385742,
            "Time in s": 1604.2857379999998
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7737725295214419,
            "MicroF1": 0.7737725295214419,
            "MacroF1": 0.7647353044337893,
            "Memory in Mb": 4.11713981628418,
            "Time in s": 1697.9838939999995
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7734138972809668,
            "MicroF1": 0.7734138972809667,
            "MacroF1": 0.7645730180903108,
            "Memory in Mb": 4.116628646850586,
            "Time in s": 1794.3974679999997
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7724867724867724,
            "MicroF1": 0.7724867724867724,
            "MacroF1": 0.7656182355666586,
            "Memory in Mb": 4.116819381713867,
            "Time in s": 1893.301291
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7750429307384087,
            "MicroF1": 0.7750429307384087,
            "MacroF1": 0.7677424040514297,
            "Memory in Mb": 4.116933822631836,
            "Time in s": 1994.662727
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7763524818739542,
            "MicroF1": 0.7763524818739542,
            "MacroF1": 0.7677176136548693,
            "Memory in Mb": 4.116861343383789,
            "Time in s": 2098.663831
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7775965198477434,
            "MicroF1": 0.7775965198477434,
            "MacroF1": 0.7691578918725354,
            "Memory in Mb": 4.11646842956543,
            "Time in s": 2205.226802
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7761273209549071,
            "MicroF1": 0.7761273209549071,
            "MacroF1": 0.7681560201617949,
            "Memory in Mb": 4.116430282592773,
            "Time in s": 2314.321902
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7762817193164163,
            "MicroF1": 0.7762817193164163,
            "MacroF1": 0.7674170460709655,
            "Memory in Mb": 4.116365432739258,
            "Time in s": 2425.9767019999995
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7769347496206374,
            "MicroF1": 0.7769347496206374,
            "MacroF1": 0.7672843880004774,
            "Memory in Mb": 4.116201400756836,
            "Time in s": 2540.253238
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7790410281759763,
            "MicroF1": 0.7790410281759763,
            "MacroF1": 0.7681802739952505,
            "Memory in Mb": 4.116155624389648,
            "Time in s": 2657.1841359999994
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.778153697438376,
            "MicroF1": 0.7781536974383759,
            "MacroF1": 0.767530439166732,
            "Memory in Mb": 4.116151809692383,
            "Time in s": 2776.607733
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7787234042553192,
            "MicroF1": 0.778723404255319,
            "MacroF1": 0.7673415220519754,
            "Memory in Mb": 4.116128921508789,
            "Time in s": 2898.5867789999998
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7797316057380842,
            "MicroF1": 0.7797316057380842,
            "MacroF1": 0.7679341969633587,
            "Memory in Mb": 4.116201400756836,
            "Time in s": 3023.0016299999997
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7816039873130947,
            "MicroF1": 0.7816039873130947,
            "MacroF1": 0.7687944234581563,
            "Memory in Mb": 4.11619758605957,
            "Time in s": 3150.038225
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7785175321793165,
            "MicroF1": 0.7785175321793165,
            "MacroF1": 0.7657018899401807,
            "Memory in Mb": 4.116170883178711,
            "Time in s": 3279.4760369999995
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7777294475859069,
            "MicroF1": 0.7777294475859068,
            "MacroF1": 0.7649119672933203,
            "Memory in Mb": 4.116254806518555,
            "Time in s": 3411.201767
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7778258986574275,
            "MicroF1": 0.7778258986574276,
            "MacroF1": 0.765010539660814,
            "Memory in Mb": 4.116277694702148,
            "Time in s": 3543.54869
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6360189573459716,
            "MicroF1": 0.6360189573459716,
            "MacroF1": 0.5970323052762562,
            "Memory in Mb": 6.48949146270752,
            "Time in s": 90.340432
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.62482235907153,
            "MicroF1": 0.62482235907153,
            "MacroF1": 0.5890580890213498,
            "Memory in Mb": 6.490170478820801,
            "Time in s": 257.284509
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6157246605620461,
            "MicroF1": 0.6157246605620461,
            "MacroF1": 0.5802533923244894,
            "Memory in Mb": 6.491124153137207,
            "Time in s": 490.807794
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6107032914989344,
            "MicroF1": 0.6107032914989344,
            "MacroF1": 0.574850135712032,
            "Memory in Mb": 6.49120044708252,
            "Time in s": 783.3577379999999
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.614889183557492,
            "MicroF1": 0.614889183557492,
            "MacroF1": 0.5777842549225517,
            "Memory in Mb": 6.491948127746582,
            "Time in s": 1129.937274
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.608997632202052,
            "MicroF1": 0.608997632202052,
            "MacroF1": 0.5733157350789626,
            "Memory in Mb": 6.490735054016113,
            "Time in s": 1525.7763839999998
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6057367068055743,
            "MicroF1": 0.6057367068055743,
            "MacroF1": 0.5703382690867537,
            "Memory in Mb": 6.490704536437988,
            "Time in s": 1967.928226
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6069610512608027,
            "MicroF1": 0.6069610512608027,
            "MacroF1": 0.5711427916016896,
            "Memory in Mb": 6.490643501281738,
            "Time in s": 2456.105543
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6039145532989583,
            "MicroF1": 0.6039145532989583,
            "MacroF1": 0.5678102867297488,
            "Memory in Mb": 6.491009712219238,
            "Time in s": 2990.761064
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6034662373330808,
            "MicroF1": 0.6034662373330808,
            "MacroF1": 0.567425153452482,
            "Memory in Mb": 6.491185188293457,
            "Time in s": 3571.580702
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6005165733964701,
            "MicroF1": 0.6005165733964701,
            "MacroF1": 0.56512832395729,
            "Memory in Mb": 6.491345405578613,
            "Time in s": 4198.711386999999
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6031883829216321,
            "MicroF1": 0.6031883829216321,
            "MacroF1": 0.5703828979306638,
            "Memory in Mb": 6.491543769836426,
            "Time in s": 4874.277407999999
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6152108982297662,
            "MicroF1": 0.6152108982297662,
            "MacroF1": 0.5959760515786451,
            "Memory in Mb": 5.97607421875,
            "Time in s": 5593.125681999999
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6060339579246432,
            "MicroF1": 0.6060339579246432,
            "MacroF1": 0.5869142505177357,
            "Memory in Mb": 6.496403694152832,
            "Time in s": 6355.050274999999
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5713744554580465,
            "MicroF1": 0.5713744554580465,
            "MacroF1": 0.5537658591956377,
            "Memory in Mb": 6.4967546463012695,
            "Time in s": 7160.569073999999
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.545546019532406,
            "MicroF1": 0.545546019532406,
            "MacroF1": 0.5286479939306438,
            "Memory in Mb": 6.381303787231445,
            "Time in s": 8010.073855999999
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.526767311013314,
            "MicroF1": 0.526767311013314,
            "MacroF1": 0.509587529402725,
            "Memory in Mb": 6.497265815734863,
            "Time in s": 8901.233847
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.517756615983585,
            "MicroF1": 0.517756615983585,
            "MacroF1": 0.4976462434137419,
            "Memory in Mb": 4.685893058776856,
            "Time in s": 9829.81162
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5296815032647162,
            "MicroF1": 0.5296815032647162,
            "MacroF1": 0.5080882715573688,
            "Memory in Mb": 10.369908332824709,
            "Time in s": 10791.950057
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.539750935176855,
            "MicroF1": 0.539750935176855,
            "MacroF1": 0.5184934777423561,
            "Memory in Mb": 10.92272663116455,
            "Time in s": 11801.930673
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5468771138669674,
            "MicroF1": 0.5468771138669674,
            "MacroF1": 0.525970977438283,
            "Memory in Mb": 10.920933723449709,
            "Time in s": 12856.592968
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5551633593043778,
            "MicroF1": 0.5551633593043778,
            "MacroF1": 0.5340735310276195,
            "Memory in Mb": 12.231526374816896,
            "Time in s": 13957.460176
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5615761518507844,
            "MicroF1": 0.5615761518507844,
            "MacroF1": 0.5396852076547556,
            "Memory in Mb": 12.87682819366455,
            "Time in s": 15100.290122
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5679280274632048,
            "MicroF1": 0.5679280274632048,
            "MacroF1": 0.5455634192548013,
            "Memory in Mb": 13.528642654418944,
            "Time in s": 16285.362621
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5727868479866661,
            "MicroF1": 0.5727868479866661,
            "MacroF1": 0.5496374434570932,
            "Memory in Mb": 13.632143020629885,
            "Time in s": 17508.053461
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5754143143325442,
            "MicroF1": 0.5754143143325442,
            "MacroF1": 0.5513680135969626,
            "Memory in Mb": 13.630533218383787,
            "Time in s": 18766.96928
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5772859598049875,
            "MicroF1": 0.5772859598049875,
            "MacroF1": 0.5551350356863173,
            "Memory in Mb": 13.627862930297852,
            "Time in s": 20061.957755000003
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.577772516657084,
            "MicroF1": 0.577772516657084,
            "MacroF1": 0.5590861332292512,
            "Memory in Mb": 13.626611709594728,
            "Time in s": 21394.440888000005
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.578225516768442,
            "MicroF1": 0.578225516768442,
            "MacroF1": 0.5625516131192055,
            "Memory in Mb": 12.769641876220703,
            "Time in s": 22755.311286000004
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5795637488557088,
            "MicroF1": 0.5795637488557088,
            "MacroF1": 0.5663363640160616,
            "Memory in Mb": 12.768932342529297,
            "Time in s": 24150.336726000005
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5811211241790133,
            "MicroF1": 0.5811211241790133,
            "MacroF1": 0.5696723582178381,
            "Memory in Mb": 12.768062591552734,
            "Time in s": 25577.802283000005
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.575804208221124,
            "MicroF1": 0.575804208221124,
            "MacroF1": 0.5647934119551398,
            "Memory in Mb": 12.981294631958008,
            "Time in s": 27039.45595800001
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5701495107182828,
            "MicroF1": 0.5701495107182828,
            "MacroF1": 0.559068023359177,
            "Memory in Mb": 12.981256484985352,
            "Time in s": 28537.493337000007
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5657744478177311,
            "MicroF1": 0.5657744478177311,
            "MacroF1": 0.5542573482740075,
            "Memory in Mb": 12.983362197875977,
            "Time in s": 30069.70246600001
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5611894261208366,
            "MicroF1": 0.5611894261208366,
            "MacroF1": 0.5493152777162592,
            "Memory in Mb": 13.52482795715332,
            "Time in s": 31635.746830000007
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.558779429172695,
            "MicroF1": 0.558779429172695,
            "MacroF1": 0.5463982360776033,
            "Memory in Mb": 13.526559829711914,
            "Time in s": 33235.41425300001
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5546825010877633,
            "MicroF1": 0.5546825010877633,
            "MacroF1": 0.5426283860139581,
            "Memory in Mb": 14.304903030395508,
            "Time in s": 34865.73115700001
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5542153662122761,
            "MicroF1": 0.5542153662122761,
            "MacroF1": 0.5429626632180721,
            "Memory in Mb": 15.152182579040527,
            "Time in s": 36525.24862800001
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5541364155112547,
            "MicroF1": 0.5541364155112547,
            "MacroF1": 0.5435420562964655,
            "Memory in Mb": 15.252725601196287,
            "Time in s": 38211.297236000006
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5542981604678141,
            "MicroF1": 0.5542981604678141,
            "MacroF1": 0.544391400018036,
            "Memory in Mb": 15.251314163208008,
            "Time in s": 39923.86574200001
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.554151749624668,
            "MicroF1": 0.554151749624668,
            "MacroF1": 0.5448486588729107,
            "Memory in Mb": 13.424749374389648,
            "Time in s": 41664.47056700001
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5536290049829767,
            "MicroF1": 0.5536290049829767,
            "MacroF1": 0.5448029815059025,
            "Memory in Mb": 13.64866542816162,
            "Time in s": 43429.160590000014
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5541436342414165,
            "MicroF1": 0.5541436342414165,
            "MacroF1": 0.5454957405719211,
            "Memory in Mb": 14.18911075592041,
            "Time in s": 45215.90786900002
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5553020683124207,
            "MicroF1": 0.5553020683124207,
            "MacroF1": 0.546961663735647,
            "Memory in Mb": 15.156656265258787,
            "Time in s": 47024.86244100002
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5579662871693428,
            "MicroF1": 0.5579662871693428,
            "MacroF1": 0.5498636684303295,
            "Memory in Mb": 14.218542098999023,
            "Time in s": 48856.78116300002
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5627586206896552,
            "MicroF1": 0.5627586206896552,
            "MacroF1": 0.5545030394801858,
            "Memory in Mb": 14.845645904541016,
            "Time in s": 50711.77001700002
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5677701436602124,
            "MicroF1": 0.5677701436602124,
            "MacroF1": 0.5591808574875289,
            "Memory in Mb": 15.233248710632324,
            "Time in s": 52589.43568900003
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5730463432438297,
            "MicroF1": 0.5730463432438297,
            "MacroF1": 0.5639878919164368,
            "Memory in Mb": 15.890131950378418,
            "Time in s": 54487.48381000003
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5791894555785324,
            "MicroF1": 0.5791894555785324,
            "MacroF1": 0.5695807960578061,
            "Memory in Mb": 16.1916446685791,
            "Time in s": 56406.77001200003
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5794427924771303,
            "MicroF1": 0.5794427924771303,
            "MacroF1": 0.5701512686040561,
            "Memory in Mb": 15.30721950531006,
            "Time in s": 58342.70756100003
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5794652487369197,
            "MicroF1": 0.5794652487369197,
            "MacroF1": 0.5701984940722999,
            "Memory in Mb": 15.30735683441162,
            "Time in s": 60279.413314000034
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9828009828009828,
            "MicroF1": 0.9828009828009828,
            "MacroF1": 0.6067632850241546,
            "Memory in Mb": 2.100947380065918,
            "Time in s": 5.705318
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.943558282208589,
            "MicroF1": 0.943558282208589,
            "MacroF1": 0.7669956277713079,
            "Memory in Mb": 3.048105239868164,
            "Time in s": 25.352994
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8912510220768601,
            "MicroF1": 0.8912510220768601,
            "MacroF1": 0.8617021305177772,
            "Memory in Mb": 3.9921913146972656,
            "Time in s": 63.032035
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9031269160024524,
            "MicroF1": 0.9031269160024524,
            "MacroF1": 0.8868998230762756,
            "Memory in Mb": 4.944231986999512,
            "Time in s": 123.600275
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.898970083374203,
            "MicroF1": 0.898970083374203,
            "MacroF1": 0.888705938214812,
            "Memory in Mb": 5.993730545043945,
            "Time in s": 211.611387
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8598283612586841,
            "MicroF1": 0.8598283612586841,
            "MacroF1": 0.8569666636755086,
            "Memory in Mb": 6.37155818939209,
            "Time in s": 330.620683
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8669001751313485,
            "MicroF1": 0.8669001751313484,
            "MacroF1": 0.8547854134985733,
            "Memory in Mb": 7.318934440612793,
            "Time in s": 479.663409
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8581060373889059,
            "MicroF1": 0.8581060373889059,
            "MacroF1": 0.8327540420876277,
            "Memory in Mb": 8.264909744262695,
            "Time in s": 660.474615
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8490874421138654,
            "MicroF1": 0.8490874421138654,
            "MacroF1": 0.8463961237855363,
            "Memory in Mb": 8.926459312438965,
            "Time in s": 875.371562
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8421181662172101,
            "MicroF1": 0.84211816621721,
            "MacroF1": 0.8299816031455575,
            "Memory in Mb": 10.074895858764648,
            "Time in s": 1125.854174
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8301760641854246,
            "MicroF1": 0.8301760641854244,
            "MacroF1": 0.8400819204125556,
            "Memory in Mb": 11.044804573059082,
            "Time in s": 1412.144879
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8314606741573034,
            "MicroF1": 0.8314606741573034,
            "MacroF1": 0.8387821748480373,
            "Memory in Mb": 8.862092971801758,
            "Time in s": 1728.261118
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8333019045823119,
            "MicroF1": 0.8333019045823119,
            "MacroF1": 0.8299513887279447,
            "Memory in Mb": 9.715648651123049,
            "Time in s": 2074.079546
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8255997198389073,
            "MicroF1": 0.8255997198389075,
            "MacroF1": 0.831498100235552,
            "Memory in Mb": 10.513428688049316,
            "Time in s": 2449.732459
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8241542735741134,
            "MicroF1": 0.8241542735741134,
            "MacroF1": 0.813971923025991,
            "Memory in Mb": 11.555256843566896,
            "Time in s": 2856.066254
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8043511567335683,
            "MicroF1": 0.8043511567335683,
            "MacroF1": 0.8048077550156274,
            "Memory in Mb": 12.298343658447266,
            "Time in s": 3295.046229
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8002883922134102,
            "MicroF1": 0.8002883922134101,
            "MacroF1": 0.8062362865697692,
            "Memory in Mb": 11.726844787597656,
            "Time in s": 3768.473318
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8093422306959008,
            "MicroF1": 0.8093422306959008,
            "MacroF1": 0.813125473572493,
            "Memory in Mb": 9.433514595031738,
            "Time in s": 4267.304275
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8157657076506257,
            "MicroF1": 0.8157657076506257,
            "MacroF1": 0.8184378776785012,
            "Memory in Mb": 10.539642333984377,
            "Time in s": 4791.9677950000005
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8199534256649099,
            "MicroF1": 0.81995342566491,
            "MacroF1": 0.8213128379144453,
            "Memory in Mb": 11.364830017089844,
            "Time in s": 5345.1630700000005
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8247928096183028,
            "MicroF1": 0.8247928096183028,
            "MacroF1": 0.8275146627418534,
            "Memory in Mb": 12.672901153564451,
            "Time in s": 5929.400246
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8295264623955432,
            "MicroF1": 0.8295264623955433,
            "MacroF1": 0.8318915513040454,
            "Memory in Mb": 13.833264350891112,
            "Time in s": 6547.972923
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8319300863263348,
            "MicroF1": 0.8319300863263348,
            "MacroF1": 0.8336463894938194,
            "Memory in Mb": 14.741169929504396,
            "Time in s": 7204.877164
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8342355224185476,
            "MicroF1": 0.8342355224185476,
            "MacroF1": 0.8362542817352725,
            "Memory in Mb": 16.02083969116211,
            "Time in s": 7900.921468
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8343955289734287,
            "MicroF1": 0.8343955289734286,
            "MacroF1": 0.833886744496364,
            "Memory in Mb": 17.251243591308594,
            "Time in s": 8638.28045
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8258697086829452,
            "MicroF1": 0.8258697086829452,
            "MacroF1": 0.823298887298616,
            "Memory in Mb": 18.484009742736816,
            "Time in s": 9418.818077
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.825692237857467,
            "MicroF1": 0.825692237857467,
            "MacroF1": 0.827229896548608,
            "Memory in Mb": 17.053231239318848,
            "Time in s": 10241.512178
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8263153287227524,
            "MicroF1": 0.8263153287227524,
            "MacroF1": 0.8251000136898328,
            "Memory in Mb": 18.097841262817383,
            "Time in s": 11105.510711
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8257966359563857,
            "MicroF1": 0.8257966359563859,
            "MacroF1": 0.8251092059206939,
            "Memory in Mb": 19.1904354095459,
            "Time in s": 12012.672379
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8289892965111528,
            "MicroF1": 0.8289892965111528,
            "MacroF1": 0.8300645161883343,
            "Memory in Mb": 17.2155818939209,
            "Time in s": 12963.554855000002
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8324503834901558,
            "MicroF1": 0.8324503834901558,
            "MacroF1": 0.8328446288662702,
            "Memory in Mb": 17.090572357177734,
            "Time in s": 13955.688030000005
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8295672156261968,
            "MicroF1": 0.8295672156261968,
            "MacroF1": 0.8279815503081916,
            "Memory in Mb": 18.284998893737797,
            "Time in s": 14990.870602000005
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.828121518235163,
            "MicroF1": 0.828121518235163,
            "MacroF1": 0.8279872572314477,
            "Memory in Mb": 18.759904861450195,
            "Time in s": 16071.989638000005
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8300771393554899,
            "MicroF1": 0.8300771393554899,
            "MacroF1": 0.8300312724960401,
            "Memory in Mb": 19.937789916992188,
            "Time in s": 17198.739284000003
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8329714966034036,
            "MicroF1": 0.8329714966034036,
            "MacroF1": 0.8330653900337638,
            "Memory in Mb": 21.17230033874512,
            "Time in s": 18373.548754000003
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8360454823994008,
            "MicroF1": 0.8360454823994008,
            "MacroF1": 0.8362319050195895,
            "Memory in Mb": 22.12139320373535,
            "Time in s": 19591.296889000005
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8391520370983769,
            "MicroF1": 0.8391520370983769,
            "MacroF1": 0.8393677597260801,
            "Memory in Mb": 22.688467979431152,
            "Time in s": 20852.364231000003
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8400309617493389,
            "MicroF1": 0.8400309617493388,
            "MacroF1": 0.8398031059873,
            "Memory in Mb": 23.806550979614254,
            "Time in s": 22157.639176000004
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8335114072025642,
            "MicroF1": 0.8335114072025642,
            "MacroF1": 0.8310693286634668,
            "Memory in Mb": 25.06292724609375,
            "Time in s": 23499.792247000005
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8283595808566702,
            "MicroF1": 0.8283595808566702,
            "MacroF1": 0.826721014765785,
            "Memory in Mb": 26.060873985290527,
            "Time in s": 24886.958001000006
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.826747175225683,
            "MicroF1": 0.8267471752256829,
            "MacroF1": 0.8259678903415486,
            "Memory in Mb": 27.245673179626465,
            "Time in s": 26317.085564000008
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.821943390720747,
            "MicroF1": 0.821943390720747,
            "MacroF1": 0.8202405231953956,
            "Memory in Mb": 28.675668716430664,
            "Time in s": 27793.820666000007
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8182180926865417,
            "MicroF1": 0.8182180926865417,
            "MacroF1": 0.8170173651382093,
            "Memory in Mb": 29.74225902557373,
            "Time in s": 29319.213378000008
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.81878446883182,
            "MicroF1": 0.81878446883182,
            "MacroF1": 0.8179349229322325,
            "Memory in Mb": 30.87984085083008,
            "Time in s": 30892.43160700001
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.821123154855929,
            "MicroF1": 0.821123154855929,
            "MacroF1": 0.8204502524156659,
            "Memory in Mb": 32.019548416137695,
            "Time in s": 32513.434007000007
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8235200085256035,
            "MicroF1": 0.8235200085256035,
            "MacroF1": 0.8229965581236837,
            "Memory in Mb": 33.157379150390625,
            "Time in s": 34181.929457000006
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.819973924380704,
            "MicroF1": 0.819973924380704,
            "MacroF1": 0.8189812465563673,
            "Memory in Mb": 34.295823097229004,
            "Time in s": 35895.74071300001
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.821733135883164,
            "MicroF1": 0.821733135883164,
            "MacroF1": 0.8211010404575377,
            "Memory in Mb": 35.31475067138672,
            "Time in s": 37655.039070000006
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8188684908208694,
            "MicroF1": 0.8188684908208694,
            "MacroF1": 0.8180458262517715,
            "Memory in Mb": 36.57470226287842,
            "Time in s": 39458.702899
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "ADWIN Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.816559635276239,
            "MicroF1": 0.816559635276239,
            "MacroF1": 0.8159075588016685,
            "Memory in Mb": 37.85576725006104,
            "Time in s": 41308.014952000005
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.1111111111111111,
            "MicroF1": 0.1111111111111111,
            "MacroF1": 0.0815018315018315,
            "Memory in Mb": 3.4160032272338867,
            "Time in s": 1.208286
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.2307692307692307,
            "MicroF1": 0.2307692307692307,
            "MacroF1": 0.2226391771283412,
            "Memory in Mb": 4.099128723144531,
            "Time in s": 4.553382
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.4233576642335766,
            "MicroF1": 0.4233576642335766,
            "MacroF1": 0.4463537718619156,
            "Memory in Mb": 4.099002838134766,
            "Time in s": 10.351245
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.5355191256830601,
            "MicroF1": 0.5355191256830601,
            "MacroF1": 0.5617062146473912,
            "Memory in Mb": 4.099178314208984,
            "Time in s": 18.765494
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.5938864628820961,
            "MicroF1": 0.5938864628820961,
            "MacroF1": 0.6236530662596055,
            "Memory in Mb": 4.099166870117188,
            "Time in s": 30.180838
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.6290909090909091,
            "MicroF1": 0.6290909090909091,
            "MacroF1": 0.6558170665459355,
            "Memory in Mb": 4.099109649658203,
            "Time in s": 44.412895
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.660436137071651,
            "MicroF1": 0.660436137071651,
            "MacroF1": 0.678574720261515,
            "Memory in Mb": 4.098438262939453,
            "Time in s": 61.214822
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.6920980926430518,
            "MicroF1": 0.6920980926430518,
            "MacroF1": 0.7041680355881775,
            "Memory in Mb": 4.0984954833984375,
            "Time in s": 80.427396
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7167070217917676,
            "MicroF1": 0.7167070217917676,
            "MacroF1": 0.7259075149442813,
            "Memory in Mb": 4.097980499267578,
            "Time in s": 102.254145
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7254901960784313,
            "MicroF1": 0.7254901960784313,
            "MacroF1": 0.7325011710849479,
            "Memory in Mb": 4.098300933837891,
            "Time in s": 127.091256
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7386138613861386,
            "MicroF1": 0.7386138613861386,
            "MacroF1": 0.7428621938273078,
            "Memory in Mb": 4.098552703857422,
            "Time in s": 154.35838199999998
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7422867513611615,
            "MicroF1": 0.7422867513611615,
            "MacroF1": 0.7453719085253248,
            "Memory in Mb": 4.098358154296875,
            "Time in s": 184.303693
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7487437185929648,
            "MicroF1": 0.7487437185929648,
            "MacroF1": 0.7504522188790486,
            "Memory in Mb": 4.098468780517578,
            "Time in s": 216.734559
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7465007776049767,
            "MicroF1": 0.7465007776049767,
            "MacroF1": 0.7482323503576439,
            "Memory in Mb": 4.098541259765625,
            "Time in s": 252.139078
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7489114658925979,
            "MicroF1": 0.748911465892598,
            "MacroF1": 0.7488472102580618,
            "Memory in Mb": 4.098594665527344,
            "Time in s": 290.044846
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7523809523809524,
            "MicroF1": 0.7523809523809524,
            "MacroF1": 0.7518283723099097,
            "Memory in Mb": 4.098430633544922,
            "Time in s": 330.661237
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7541613316261203,
            "MicroF1": 0.7541613316261204,
            "MacroF1": 0.7531089046321314,
            "Memory in Mb": 4.098361968994141,
            "Time in s": 373.819675
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7557436517533253,
            "MicroF1": 0.7557436517533253,
            "MacroF1": 0.7552013614952863,
            "Memory in Mb": 4.098308563232422,
            "Time in s": 419.6867600000001
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7617411225658648,
            "MicroF1": 0.7617411225658649,
            "MacroF1": 0.7601066395856337,
            "Memory in Mb": 4.098381042480469,
            "Time in s": 467.91378800000007
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.763873775843308,
            "MicroF1": 0.763873775843308,
            "MacroF1": 0.7623480483274478,
            "Memory in Mb": 4.098400115966797,
            "Time in s": 518.622959
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7678756476683938,
            "MicroF1": 0.7678756476683938,
            "MacroF1": 0.7646598072570266,
            "Memory in Mb": 4.098423004150391,
            "Time in s": 571.868767
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7705242334322453,
            "MicroF1": 0.7705242334322453,
            "MacroF1": 0.7668271197983111,
            "Memory in Mb": 4.098529815673828,
            "Time in s": 627.754669
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7757805108798487,
            "MicroF1": 0.7757805108798487,
            "MacroF1": 0.7714920336037777,
            "Memory in Mb": 4.098388671875,
            "Time in s": 686.3790640000001
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7760652765185857,
            "MicroF1": 0.7760652765185856,
            "MacroF1": 0.7719206139767609,
            "Memory in Mb": 4.098537445068359,
            "Time in s": 747.748718
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7789382071366405,
            "MicroF1": 0.7789382071366405,
            "MacroF1": 0.7750313949659527,
            "Memory in Mb": 4.098442077636719,
            "Time in s": 811.629001
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7849372384937239,
            "MicroF1": 0.7849372384937239,
            "MacroF1": 0.7820003890472508,
            "Memory in Mb": 4.098487854003906,
            "Time in s": 878.060098
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7856567284448026,
            "MicroF1": 0.7856567284448026,
            "MacroF1": 0.7827470902102026,
            "Memory in Mb": 4.098438262939453,
            "Time in s": 947.241797
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7894327894327894,
            "MicroF1": 0.7894327894327894,
            "MacroF1": 0.785982924599392,
            "Memory in Mb": 4.0983428955078125,
            "Time in s": 1018.793017
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7906976744186046,
            "MicroF1": 0.7906976744186046,
            "MacroF1": 0.7876424482584368,
            "Memory in Mb": 4.098438262939453,
            "Time in s": 1093.078269
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7933284989122552,
            "MicroF1": 0.7933284989122552,
            "MacroF1": 0.7906471924204205,
            "Memory in Mb": 4.098392486572266,
            "Time in s": 1169.7117919999998
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.7978947368421052,
            "MicroF1": 0.7978947368421052,
            "MacroF1": 0.7945020166797493,
            "Memory in Mb": 4.098480224609375,
            "Time in s": 1248.577134
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8028552005438477,
            "MicroF1": 0.8028552005438477,
            "MacroF1": 0.7982243751921434,
            "Memory in Mb": 4.098472595214844,
            "Time in s": 1329.680821
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8035596572181938,
            "MicroF1": 0.8035596572181938,
            "MacroF1": 0.7981876534181912,
            "Memory in Mb": 4.098491668701172,
            "Time in s": 1413.4983189999998
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8035828534868842,
            "MicroF1": 0.8035828534868842,
            "MacroF1": 0.798634974540431,
            "Memory in Mb": 4.098518371582031,
            "Time in s": 1499.905218
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8048477315102548,
            "MicroF1": 0.8048477315102549,
            "MacroF1": 0.7997380784882049,
            "Memory in Mb": 4.098381042480469,
            "Time in s": 1588.836817
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8066465256797583,
            "MicroF1": 0.8066465256797583,
            "MacroF1": 0.80161945439383,
            "Memory in Mb": 4.098377227783203,
            "Time in s": 1680.249514
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8059964726631393,
            "MicroF1": 0.8059964726631393,
            "MacroF1": 0.8024858564723997,
            "Memory in Mb": 4.098514556884766,
            "Time in s": 1774.345382
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8070978820835718,
            "MicroF1": 0.8070978820835718,
            "MacroF1": 0.8029124203507955,
            "Memory in Mb": 4.098423004150391,
            "Time in s": 1871.065136
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8081427774679308,
            "MicroF1": 0.8081427774679307,
            "MacroF1": 0.8029834045630979,
            "Memory in Mb": 4.098461151123047,
            "Time in s": 1970.03779
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8069603045133225,
            "MicroF1": 0.8069603045133223,
            "MacroF1": 0.801927622716254,
            "Memory in Mb": 4.098594665527344,
            "Time in s": 2071.588776
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8053050397877984,
            "MicroF1": 0.8053050397877984,
            "MacroF1": 0.8006727596367825,
            "Memory in Mb": 4.098400115966797,
            "Time in s": 2175.772942
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8047643707923355,
            "MicroF1": 0.8047643707923355,
            "MacroF1": 0.7995493059800365,
            "Memory in Mb": 4.098396301269531,
            "Time in s": 2282.41088
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8057663125948407,
            "MicroF1": 0.8057663125948407,
            "MacroF1": 0.8003960406612564,
            "Memory in Mb": 4.098434448242188,
            "Time in s": 2391.59611
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8072170044488384,
            "MicroF1": 0.8072170044488384,
            "MacroF1": 0.8005625942078284,
            "Memory in Mb": 4.098430633544922,
            "Time in s": 2503.16971
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8066698888351861,
            "MicroF1": 0.8066698888351861,
            "MacroF1": 0.8002110568368,
            "Memory in Mb": 4.098316192626953,
            "Time in s": 2617.3694960000003
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.807565011820331,
            "MicroF1": 0.807565011820331,
            "MacroF1": 0.8005131307885663,
            "Memory in Mb": 4.0983428955078125,
            "Time in s": 2733.922308
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8079592781119852,
            "MicroF1": 0.8079592781119852,
            "MacroF1": 0.8006755955605837,
            "Memory in Mb": 4.098320007324219,
            "Time in s": 2852.747139
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8087902129587675,
            "MicroF1": 0.8087902129587675,
            "MacroF1": 0.8009921695193862,
            "Memory in Mb": 4.098320007324219,
            "Time in s": 2973.740681
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8060363959165557,
            "MicroF1": 0.8060363959165557,
            "MacroF1": 0.7987732120640717,
            "Memory in Mb": 4.0983428955078125,
            "Time in s": 3097.6149410000003
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8051326663766856,
            "MicroF1": 0.8051326663766856,
            "MacroF1": 0.798077892809675,
            "Memory in Mb": 4.0983428955078125,
            "Time in s": 3223.9293610000004
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "ImageSegments",
            "Accuracy": 0.8046773495019489,
            "MicroF1": 0.8046773495019489,
            "MacroF1": 0.7977695866822911,
            "Memory in Mb": 4.098388671875,
            "Time in s": 3350.8763620000004
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6360189573459716,
            "MicroF1": 0.6360189573459716,
            "MacroF1": 0.5992691812827112,
            "Memory in Mb": 6.474042892456055,
            "Time in s": 88.969298
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6110847939365229,
            "MicroF1": 0.6110847939365229,
            "MacroF1": 0.5773210074897359,
            "Memory in Mb": 6.473905563354492,
            "Time in s": 256.045675
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6043574360593622,
            "MicroF1": 0.6043574360593622,
            "MacroF1": 0.5704368753709179,
            "Memory in Mb": 6.473470687866211,
            "Time in s": 489.83548
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6014681506038362,
            "MicroF1": 0.6014681506038362,
            "MacroF1": 0.5676969561642586,
            "Memory in Mb": 6.473196029663086,
            "Time in s": 783.3519140000001
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6057965523773442,
            "MicroF1": 0.6057965523773442,
            "MacroF1": 0.5710016183775801,
            "Memory in Mb": 6.473196029663086,
            "Time in s": 1130.801617
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5966850828729282,
            "MicroF1": 0.5966850828729282,
            "MacroF1": 0.5635903588556204,
            "Memory in Mb": 6.473356246948242,
            "Time in s": 1527.884634
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5957245298335814,
            "MicroF1": 0.5957245298335814,
            "MacroF1": 0.5625002603439991,
            "Memory in Mb": 6.473814010620117,
            "Time in s": 1971.450931
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5982005445720374,
            "MicroF1": 0.5982005445720374,
            "MacroF1": 0.5646892369665863,
            "Memory in Mb": 6.474157333374023,
            "Time in s": 2461.351589
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.596337998526781,
            "MicroF1": 0.596337998526781,
            "MacroF1": 0.5627085514562804,
            "Memory in Mb": 6.47450065612793,
            "Time in s": 2997.75158
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5965527038545316,
            "MicroF1": 0.5965527038545316,
            "MacroF1": 0.5631320282838163,
            "Memory in Mb": 6.47468376159668,
            "Time in s": 3580.189969
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5953508394317693,
            "MicroF1": 0.5953508394317693,
            "MacroF1": 0.562671447170627,
            "Memory in Mb": 6.47468376159668,
            "Time in s": 4209.202801
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5979796385447084,
            "MicroF1": 0.5979796385447084,
            "MacroF1": 0.5680559575776837,
            "Memory in Mb": 6.474340438842773,
            "Time in s": 4886.872526
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.610767101333139,
            "MicroF1": 0.610767101333139,
            "MacroF1": 0.5941277335666079,
            "Memory in Mb": 6.473836898803711,
            "Time in s": 5609.570035
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.6019752418318338,
            "MicroF1": 0.6019752418318338,
            "MacroF1": 0.5851264744797859,
            "Memory in Mb": 6.473745346069336,
            "Time in s": 6378.998584999999
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5705536965717533,
            "MicroF1": 0.5705536965717533,
            "MacroF1": 0.5545059657048704,
            "Memory in Mb": 6.473974227905273,
            "Time in s": 7193.860588999999
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.548091151228174,
            "MicroF1": 0.548091151228174,
            "MacroF1": 0.5320735507355622,
            "Memory in Mb": 6.474386215209961,
            "Time in s": 8051.816493999999
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5307225224221492,
            "MicroF1": 0.5307225224221492,
            "MacroF1": 0.5138536287616571,
            "Memory in Mb": 6.474637985229492,
            "Time in s": 8952.059017
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5182827379386542,
            "MicroF1": 0.5182827379386542,
            "MacroF1": 0.4990809738484312,
            "Memory in Mb": 6.47486686706543,
            "Time in s": 9893.706361
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5182176145142801,
            "MicroF1": 0.5182176145142801,
            "MacroF1": 0.497867701567998,
            "Memory in Mb": 8.642622947692871,
            "Time in s": 10881.966771
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5272503432927695,
            "MicroF1": 0.5272503432927695,
            "MacroF1": 0.5067114684709674,
            "Memory in Mb": 15.437758445739746,
            "Time in s": 11917.076256
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.533032694475761,
            "MicroF1": 0.533032694475761,
            "MacroF1": 0.5127471323280748,
            "Memory in Mb": 16.81709384918213,
            "Time in s": 12999.258268
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5410442942619775,
            "MicroF1": 0.5410442942619775,
            "MacroF1": 0.5207771198745245,
            "Memory in Mb": 17.041016578674316,
            "Time in s": 14124.681759
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5459710956478775,
            "MicroF1": 0.5459710956478775,
            "MacroF1": 0.5251711652768184,
            "Memory in Mb": 17.038064002990723,
            "Time in s": 15290.808705
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5532099593576135,
            "MicroF1": 0.5532099593576135,
            "MacroF1": 0.5314216535856217,
            "Memory in Mb": 17.036622047424316,
            "Time in s": 16491.42669
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5607788173794462,
            "MicroF1": 0.5607788173794462,
            "MacroF1": 0.5375130024626694,
            "Memory in Mb": 17.14900016784668,
            "Time in s": 17723.115047
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5667091604443635,
            "MicroF1": 0.5667091604443635,
            "MacroF1": 0.5418496825562071,
            "Memory in Mb": 17.261820793151855,
            "Time in s": 18986.675501
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5692890463329943,
            "MicroF1": 0.5692890463329943,
            "MacroF1": 0.5455529487931667,
            "Memory in Mb": 17.26294231414795,
            "Time in s": 20283.404341
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5688436432509216,
            "MicroF1": 0.5688436432509216,
            "MacroF1": 0.5481992899375988,
            "Memory in Mb": 17.26337718963623,
            "Time in s": 21617.011828
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5687228553701467,
            "MicroF1": 0.5687228553701467,
            "MacroF1": 0.5505043481720591,
            "Memory in Mb": 17.26330852508545,
            "Time in s": 22980.237824
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5691467533697402,
            "MicroF1": 0.5691467533697402,
            "MacroF1": 0.5529220328647554,
            "Memory in Mb": 17.262804985046387,
            "Time in s": 24378.053405
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5703986558729189,
            "MicroF1": 0.5703986558729189,
            "MacroF1": 0.5556828084411201,
            "Memory in Mb": 17.262507438659668,
            "Time in s": 25809.039082
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5650025154626972,
            "MicroF1": 0.5650025154626972,
            "MacroF1": 0.5507695387439543,
            "Memory in Mb": 17.487704277038574,
            "Time in s": 27274.413314
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5587281545039745,
            "MicroF1": 0.5587281545039745,
            "MacroF1": 0.5445349362041821,
            "Memory in Mb": 17.929275512695312,
            "Time in s": 28775.770082
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5541876723393588,
            "MicroF1": 0.5541876723393588,
            "MacroF1": 0.5396635045593164,
            "Memory in Mb": 18.030207633972168,
            "Time in s": 30311.158157
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.549122000054114,
            "MicroF1": 0.549122000054114,
            "MacroF1": 0.5343517375956978,
            "Memory in Mb": 19.681435585021973,
            "Time in s": 31880.342243
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5473628830724714,
            "MicroF1": 0.5473628830724714,
            "MacroF1": 0.5321033552605493,
            "Memory in Mb": 21.71814346313477,
            "Time in s": 33482.866823
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5426787131120269,
            "MicroF1": 0.5426787131120269,
            "MacroF1": 0.52803892360078,
            "Memory in Mb": 22.487850189208984,
            "Time in s": 35116.535538
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5419293742367982,
            "MicroF1": 0.5419293742367982,
            "MacroF1": 0.5284857300708793,
            "Memory in Mb": 23.76238250732422,
            "Time in s": 36778.160189
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5417769467984362,
            "MicroF1": 0.5417769467984362,
            "MacroF1": 0.5296361895775551,
            "Memory in Mb": 23.860816955566406,
            "Time in s": 38464.674338
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5422240109851085,
            "MicroF1": 0.5422240109851085,
            "MacroF1": 0.5313111510734391,
            "Memory in Mb": 24.196860313415527,
            "Time in s": 40175.576413
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5444970550871925,
            "MicroF1": 0.5444970550871925,
            "MacroF1": 0.5344195798463859,
            "Memory in Mb": 24.296037673950195,
            "Time in s": 41906.99288399999
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5463461928705102,
            "MicroF1": 0.5463461928705102,
            "MacroF1": 0.5369578677381479,
            "Memory in Mb": 24.84640598297119,
            "Time in s": 43659.477485
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5482855066399454,
            "MicroF1": 0.5482855066399454,
            "MacroF1": 0.5392181145139481,
            "Memory in Mb": 25.28636360168457,
            "Time in s": 45430.571796
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5506532079288896,
            "MicroF1": 0.5506532079288896,
            "MacroF1": 0.5419048601727473,
            "Memory in Mb": 25.498303413391117,
            "Time in s": 47220.970484
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5514846692901787,
            "MicroF1": 0.5514846692901787,
            "MacroF1": 0.5429796926051395,
            "Memory in Mb": 25.82335567474365,
            "Time in s": 49033.125826
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5515388574369532,
            "MicroF1": 0.5515388574369532,
            "MacroF1": 0.543031483592694,
            "Memory in Mb": 25.821112632751465,
            "Time in s": 50867.580247
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.551953416211642,
            "MicroF1": 0.551953416211642,
            "MacroF1": 0.5433574148660688,
            "Memory in Mb": 26.09889411926269,
            "Time in s": 52723.913942
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5563359441276856,
            "MicroF1": 0.5563359441276856,
            "MacroF1": 0.5472854805195191,
            "Memory in Mb": 26.366034507751465,
            "Time in s": 54600.511787
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5623562607502464,
            "MicroF1": 0.5623562607502464,
            "MacroF1": 0.552981536157949,
            "Memory in Mb": 27.10032081604004,
            "Time in s": 56496.789585
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5634576412432054,
            "MicroF1": 0.5634576412432054,
            "MacroF1": 0.5545218292020726,
            "Memory in Mb": 27.943178176879883,
            "Time in s": 58415.671716
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Insects",
            "Accuracy": 0.5635324616345299,
            "MicroF1": 0.5635324616345299,
            "MacroF1": 0.5546220283668154,
            "Memory in Mb": 27.942995071411133,
            "Time in s": 60335.727696
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9877149877149876,
            "MicroF1": 0.9877149877149876,
            "MacroF1": 0.7696139476961394,
            "Memory in Mb": 2.1207275390625,
            "Time in s": 4.211814
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.988957055214724,
            "MicroF1": 0.988957055214724,
            "MacroF1": 0.9592655637573824,
            "Memory in Mb": 2.9369373321533203,
            "Time in s": 23.739993
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.983646770237122,
            "MicroF1": 0.983646770237122,
            "MacroF1": 0.9326470331192014,
            "Memory in Mb": 4.590028762817383,
            "Time in s": 86.527265
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9828326180257512,
            "MicroF1": 0.9828326180257512,
            "MacroF1": 0.9594506659780556,
            "Memory in Mb": 5.819695472717285,
            "Time in s": 184.232691
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9705738106915156,
            "MicroF1": 0.9705738106915156,
            "MacroF1": 0.9304838721924584,
            "Memory in Mb": 8.549582481384277,
            "Time in s": 323.308574
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9607682876992236,
            "MicroF1": 0.9607682876992236,
            "MacroF1": 0.9455756842664336,
            "Memory in Mb": 10.061903953552246,
            "Time in s": 491.40663400000005
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9541155866900176,
            "MicroF1": 0.9541155866900176,
            "MacroF1": 0.9254688528922778,
            "Memory in Mb": 12.678574562072754,
            "Time in s": 687.150288
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.943610174685872,
            "MicroF1": 0.943610174685872,
            "MacroF1": 0.9191430707434156,
            "Memory in Mb": 16.086813926696777,
            "Time in s": 906.458431
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9403432307273224,
            "MicroF1": 0.9403432307273224,
            "MacroF1": 0.9284235615798526,
            "Memory in Mb": 18.255277633666992,
            "Time in s": 1151.002639
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9338073057121844,
            "MicroF1": 0.9338073057121844,
            "MacroF1": 0.918242970538206,
            "Memory in Mb": 21.65336036682129,
            "Time in s": 1427.8669570000002
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9318029864051705,
            "MicroF1": 0.9318029864051705,
            "MacroF1": 0.9319119487505448,
            "Memory in Mb": 22.76876544952393,
            "Time in s": 1733.8095280000002
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9317671092951992,
            "MicroF1": 0.9317671092951992,
            "MacroF1": 0.9296889978700974,
            "Memory in Mb": 24.966033935546875,
            "Time in s": 2062.8329900000003
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9281538751650008,
            "MicroF1": 0.9281538751650008,
            "MacroF1": 0.919765356403914,
            "Memory in Mb": 29.062508583068848,
            "Time in s": 2423.731892
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9227805988443356,
            "MicroF1": 0.9227805988443356,
            "MacroF1": 0.9201475418022376,
            "Memory in Mb": 32.12655830383301,
            "Time in s": 2815.063536
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9177970256577872,
            "MicroF1": 0.9177970256577872,
            "MacroF1": 0.9072843264203106,
            "Memory in Mb": 37.27707767486572,
            "Time in s": 3238.118927
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9115979776313774,
            "MicroF1": 0.9115979776313774,
            "MacroF1": 0.909931232789514,
            "Memory in Mb": 41.43412208557129,
            "Time in s": 3706.915394
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.912905551550108,
            "MicroF1": 0.912905551550108,
            "MacroF1": 0.9153430596364792,
            "Memory in Mb": 44.48411560058594,
            "Time in s": 4207.758914
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9135230832084978,
            "MicroF1": 0.9135230832084978,
            "MacroF1": 0.9124682676754272,
            "Memory in Mb": 47.44067192077637,
            "Time in s": 4740.722969
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9121403689846472,
            "MicroF1": 0.9121403689846472,
            "MacroF1": 0.9121831707972876,
            "Memory in Mb": 51.03960132598877,
            "Time in s": 5307.755902000001
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.908689790415492,
            "MicroF1": 0.908689790415492,
            "MacroF1": 0.9062633734460516,
            "Memory in Mb": 56.064818382263184,
            "Time in s": 5918.019803000001
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.905918057663126,
            "MicroF1": 0.905918057663126,
            "MacroF1": 0.9058259471519292,
            "Memory in Mb": 61.820496559143066,
            "Time in s": 6575.962782000001
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.9042896935933148,
            "MicroF1": 0.9042896935933148,
            "MacroF1": 0.9043251050138336,
            "Memory in Mb": 64.74030494689941,
            "Time in s": 7280.842530000002
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.901843759991474,
            "MicroF1": 0.901843759991474,
            "MacroF1": 0.9009662752730246,
            "Memory in Mb": 68.81300067901611,
            "Time in s": 8035.1031440000015
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8971504442855683,
            "MicroF1": 0.8971504442855683,
            "MacroF1": 0.8956423708961025,
            "Memory in Mb": 74.25286674499512,
            "Time in s": 8855.073479000002
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8926365329934307,
            "MicroF1": 0.8926365329934307,
            "MacroF1": 0.8903074227158838,
            "Memory in Mb": 79.6785535812378,
            "Time in s": 9744.976722000005
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8846987838220043,
            "MicroF1": 0.8846987838220043,
            "MacroF1": 0.8819820059100918,
            "Memory in Mb": 85.28873825073242,
            "Time in s": 10726.537155000004
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8791647753064004,
            "MicroF1": 0.8791647753064004,
            "MacroF1": 0.8795835231396919,
            "Memory in Mb": 89.59383392333984,
            "Time in s": 11788.438997000005
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8759520266129738,
            "MicroF1": 0.8759520266129738,
            "MacroF1": 0.8744149508862001,
            "Memory in Mb": 94.86630344390868,
            "Time in s": 12917.703791000004
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.872200152142676,
            "MicroF1": 0.872200152142676,
            "MacroF1": 0.8717012117300328,
            "Memory in Mb": 100.15169906616212,
            "Time in s": 14117.771334000005
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8736824903995425,
            "MicroF1": 0.8736824903995425,
            "MacroF1": 0.8749440738646468,
            "Memory in Mb": 101.9357843399048,
            "Time in s": 15365.994884000003
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8717482406894915,
            "MicroF1": 0.8717482406894915,
            "MacroF1": 0.8710221211412438,
            "Memory in Mb": 107.46908473968506,
            "Time in s": 16670.526324000002
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8661815396399847,
            "MicroF1": 0.8661815396399847,
            "MacroF1": 0.8651994621744733,
            "Memory in Mb": 112.71690273284912,
            "Time in s": 18043.485216
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8642204560647702,
            "MicroF1": 0.8642204560647702,
            "MacroF1": 0.8645487273027374,
            "Memory in Mb": 116.56386756896973,
            "Time in s": 19480.298866
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8619421815298104,
            "MicroF1": 0.8619421815298104,
            "MacroF1": 0.862314869215492,
            "Memory in Mb": 121.52821636199953,
            "Time in s": 20980.471725
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.859163806989285,
            "MicroF1": 0.859163806989285,
            "MacroF1": 0.8592780138529494,
            "Memory in Mb": 125.80194187164308,
            "Time in s": 22534.622977
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8591952066453326,
            "MicroF1": 0.8591952066453326,
            "MacroF1": 0.8604793833246808,
            "Memory in Mb": 129.6016607284546,
            "Time in s": 24135.768584
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8607485922490891,
            "MicroF1": 0.8607485922490891,
            "MacroF1": 0.8621609789956539,
            "Memory in Mb": 132.68816757202148,
            "Time in s": 25779.863983
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8604141133974069,
            "MicroF1": 0.8604141133974069,
            "MacroF1": 0.8613237595899307,
            "Memory in Mb": 136.05841445922852,
            "Time in s": 27480.057181
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8536861290930803,
            "MicroF1": 0.8536861290930803,
            "MacroF1": 0.853192144751886,
            "Memory in Mb": 141.70578575134277,
            "Time in s": 29254.423593
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8493167473497151,
            "MicroF1": 0.849316747349715,
            "MacroF1": 0.8496464102754333,
            "Memory in Mb": 147.49746799468994,
            "Time in s": 31089.50572
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.846296407006636,
            "MicroF1": 0.846296407006636,
            "MacroF1": 0.8470383589757107,
            "Memory in Mb": 153.1935510635376,
            "Time in s": 32973.577156
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8411438576014006,
            "MicroF1": 0.8411438576014006,
            "MacroF1": 0.8410396667771575,
            "Memory in Mb": 156.28132915496826,
            "Time in s": 34948.88082
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8365729920766117,
            "MicroF1": 0.8365729920766117,
            "MacroF1": 0.8367907010021001,
            "Memory in Mb": 161.03080940246582,
            "Time in s": 36967.519165
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8355523369171634,
            "MicroF1": 0.8355523369171634,
            "MacroF1": 0.8362918425397341,
            "Memory in Mb": 166.63249397277832,
            "Time in s": 39016.229589
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.837572852551882,
            "MicroF1": 0.8375728525518821,
            "MacroF1": 0.8385662484273668,
            "Memory in Mb": 171.47760772705078,
            "Time in s": 41092.028593
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8390259498055097,
            "MicroF1": 0.8390259498055097,
            "MacroF1": 0.8401126675526959,
            "Memory in Mb": 175.70373821258545,
            "Time in s": 43194.947864
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8376531942633637,
            "MicroF1": 0.8376531942633637,
            "MacroF1": 0.838676297522501,
            "Memory in Mb": 180.87701034545896,
            "Time in s": 45330.650988
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8390951335341879,
            "MicroF1": 0.8390951335341879,
            "MacroF1": 0.8403338496937821,
            "Memory in Mb": 185.05438709259036,
            "Time in s": 47482.84587799999
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8372767745485469,
            "MicroF1": 0.8372767745485468,
            "MacroF1": 0.8385640183306876,
            "Memory in Mb": 190.1383810043335,
            "Time in s": 49661.2352
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "AdaBoost",
            "dataset": "Keystroke",
            "Accuracy": 0.8347958233246727,
            "MicroF1": 0.8347958233246727,
            "MacroF1": 0.8360623278174891,
            "Memory in Mb": 194.794171333313,
            "Time in s": 51861.27850099999
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.3111111111111111,
            "MicroF1": 0.3111111111111111,
            "MacroF1": 0.2457649726557289,
            "Memory in Mb": 4.149084091186523,
            "Time in s": 2.196675
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.4835164835164835,
            "MicroF1": 0.4835164835164835,
            "MacroF1": 0.4934752395581889,
            "Memory in Mb": 4.152299880981445,
            "Time in s": 7.023639
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5328467153284672,
            "MicroF1": 0.5328467153284672,
            "MacroF1": 0.5528821792646678,
            "Memory in Mb": 4.15202522277832,
            "Time in s": 15.046926
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5956284153005464,
            "MicroF1": 0.5956284153005464,
            "MacroF1": 0.6141431648908949,
            "Memory in Mb": 4.152608871459961,
            "Time in s": 26.297795
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.62882096069869,
            "MicroF1": 0.62882096069869,
            "MacroF1": 0.6441389332893815,
            "Memory in Mb": 4.151983261108398,
            "Time in s": 40.50873
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.64,
            "MicroF1": 0.64,
            "MacroF1": 0.6559607038460421,
            "Memory in Mb": 4.152521133422852,
            "Time in s": 57.698206
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6666666666666666,
            "MicroF1": 0.6666666666666666,
            "MacroF1": 0.6673617488913626,
            "Memory in Mb": 4.152231216430664,
            "Time in s": 77.585785
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6948228882833788,
            "MicroF1": 0.6948228882833788,
            "MacroF1": 0.6911959597548878,
            "Memory in Mb": 4.152448654174805,
            "Time in s": 100.185488
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.711864406779661,
            "MicroF1": 0.711864406779661,
            "MacroF1": 0.7079630503641953,
            "Memory in Mb": 4.152788162231445,
            "Time in s": 125.717288
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7124183006535948,
            "MicroF1": 0.7124183006535948,
            "MacroF1": 0.7065500352371009,
            "Memory in Mb": 4.152704238891602,
            "Time in s": 154.000542
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7207920792079208,
            "MicroF1": 0.7207920792079208,
            "MacroF1": 0.7127593158348896,
            "Memory in Mb": 4.152563095092773,
            "Time in s": 184.883226
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7259528130671506,
            "MicroF1": 0.7259528130671506,
            "MacroF1": 0.7192025503807162,
            "Memory in Mb": 4.152528762817383,
            "Time in s": 218.482328
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7319932998324958,
            "MicroF1": 0.7319932998324957,
            "MacroF1": 0.7251188986558661,
            "Memory in Mb": 4.152769088745117,
            "Time in s": 254.840787
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7309486780715396,
            "MicroF1": 0.7309486780715396,
            "MacroF1": 0.7259740406437201,
            "Memory in Mb": 4.152563095092773,
            "Time in s": 294.12903800000004
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7358490566037735,
            "MicroF1": 0.7358490566037735,
            "MacroF1": 0.7304359912942561,
            "Memory in Mb": 4.152692794799805,
            "Time in s": 336.073433
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7374149659863946,
            "MicroF1": 0.7374149659863947,
            "MacroF1": 0.733149934717071,
            "Memory in Mb": 4.152753829956055,
            "Time in s": 380.701162
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7426376440460948,
            "MicroF1": 0.7426376440460948,
            "MacroF1": 0.7385597120510639,
            "Memory in Mb": 4.152643203735352,
            "Time in s": 428.175969
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7436517533252721,
            "MicroF1": 0.7436517533252721,
            "MacroF1": 0.7412375783772316,
            "Memory in Mb": 4.152631759643555,
            "Time in s": 478.460063
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7491408934707904,
            "MicroF1": 0.7491408934707904,
            "MacroF1": 0.7454343548790067,
            "Memory in Mb": 4.153181076049805,
            "Time in s": 531.417765
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7486398258977149,
            "MicroF1": 0.7486398258977149,
            "MacroF1": 0.7441307384051415,
            "Memory in Mb": 4.153326034545898,
            "Time in s": 587.1362770000001
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7492227979274612,
            "MicroF1": 0.749222797927461,
            "MacroF1": 0.7439306216964366,
            "Memory in Mb": 4.153120040893555,
            "Time in s": 645.6842
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7487636003956478,
            "MicroF1": 0.7487636003956478,
            "MacroF1": 0.7437900284473965,
            "Memory in Mb": 4.153234481811523,
            "Time in s": 707.105172
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.750236518448439,
            "MicroF1": 0.7502365184484389,
            "MacroF1": 0.7448138061687654,
            "Memory in Mb": 4.153268814086914,
            "Time in s": 771.2868930000001
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7524932003626473,
            "MicroF1": 0.7524932003626473,
            "MacroF1": 0.7468314646869904,
            "Memory in Mb": 4.153234481811523,
            "Time in s": 838.222518
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7554395126196692,
            "MicroF1": 0.7554395126196692,
            "MacroF1": 0.7493227137357602,
            "Memory in Mb": 4.153413772583008,
            "Time in s": 907.556087
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7581589958158996,
            "MicroF1": 0.7581589958158996,
            "MacroF1": 0.7527652773681007,
            "Memory in Mb": 4.153318405151367,
            "Time in s": 979.579718
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7574536663980661,
            "MicroF1": 0.7574536663980661,
            "MacroF1": 0.7525915384194216,
            "Memory in Mb": 4.153432846069336,
            "Time in s": 1054.216781
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7622377622377622,
            "MicroF1": 0.7622377622377621,
            "MacroF1": 0.7563448085202398,
            "Memory in Mb": 4.153615951538086,
            "Time in s": 1131.5718310000002
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7621905476369092,
            "MicroF1": 0.7621905476369092,
            "MacroF1": 0.7566636999776912,
            "Memory in Mb": 4.153776168823242,
            "Time in s": 1211.5912470000003
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7635968092820885,
            "MicroF1": 0.7635968092820886,
            "MacroF1": 0.7587252257765656,
            "Memory in Mb": 4.153825759887695,
            "Time in s": 1294.4019940000005
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7663157894736842,
            "MicroF1": 0.7663157894736842,
            "MacroF1": 0.7609139797315134,
            "Memory in Mb": 4.153848648071289,
            "Time in s": 1379.8910190000004
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7709041468388851,
            "MicroF1": 0.7709041468388851,
            "MacroF1": 0.7637689949207689,
            "Memory in Mb": 4.153989791870117,
            "Time in s": 1467.9946540000003
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7719182597231378,
            "MicroF1": 0.7719182597231378,
            "MacroF1": 0.7639714255563932,
            "Memory in Mb": 4.154367446899414,
            "Time in s": 1558.8129900000004
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7722328854766475,
            "MicroF1": 0.7722328854766475,
            "MacroF1": 0.7650721335080709,
            "Memory in Mb": 4.154550552368164,
            "Time in s": 1652.2028900000005
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7725295214418894,
            "MicroF1": 0.7725295214418892,
            "MacroF1": 0.764505787280341,
            "Memory in Mb": 4.154642105102539,
            "Time in s": 1748.3782850000002
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7716012084592145,
            "MicroF1": 0.7716012084592145,
            "MacroF1": 0.7634170612719108,
            "Memory in Mb": 4.15452766418457,
            "Time in s": 1847.3163560000005
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7713109935332157,
            "MicroF1": 0.7713109935332157,
            "MacroF1": 0.7652815676598499,
            "Memory in Mb": 4.154825210571289,
            "Time in s": 1948.702894
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.77389811104751,
            "MicroF1": 0.77389811104751,
            "MacroF1": 0.7674409436090757,
            "Memory in Mb": 4.155008316040039,
            "Time in s": 2052.533374
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7752370329057445,
            "MicroF1": 0.7752370329057446,
            "MacroF1": 0.7674318582149376,
            "Memory in Mb": 4.155046463012695,
            "Time in s": 2159.053176
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7765089722675367,
            "MicroF1": 0.7765089722675368,
            "MacroF1": 0.7688731808749575,
            "Memory in Mb": 4.154977798461914,
            "Time in s": 2268.233507
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7750663129973475,
            "MicroF1": 0.7750663129973475,
            "MacroF1": 0.7678921362145585,
            "Memory in Mb": 4.154905319213867,
            "Time in s": 2379.837789
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7752459865354738,
            "MicroF1": 0.7752459865354739,
            "MacroF1": 0.7671636716269125,
            "Memory in Mb": 4.155000686645508,
            "Time in s": 2494.085284
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7759231158320687,
            "MicroF1": 0.7759231158320687,
            "MacroF1": 0.7670573130332384,
            "Memory in Mb": 4.154901504516602,
            "Time in s": 2611.052254
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7775580820563519,
            "MicroF1": 0.7775580820563519,
            "MacroF1": 0.7671264358471986,
            "Memory in Mb": 4.154878616333008,
            "Time in s": 2730.562491
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.77670372160464,
            "MicroF1": 0.7767037216046399,
            "MacroF1": 0.7665050383810529,
            "Memory in Mb": 4.15495491027832,
            "Time in s": 2852.439553
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7773049645390071,
            "MicroF1": 0.7773049645390071,
            "MacroF1": 0.766340416614934,
            "Memory in Mb": 4.15495491027832,
            "Time in s": 2976.99213
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7783433595557612,
            "MicroF1": 0.7783433595557612,
            "MacroF1": 0.766965714748886,
            "Memory in Mb": 4.155027389526367,
            "Time in s": 3104.012504
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.780244676030811,
            "MicroF1": 0.780244676030811,
            "MacroF1": 0.7678552364681828,
            "Memory in Mb": 4.155023574829102,
            "Time in s": 3233.660984
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7776298268974701,
            "MicroF1": 0.7776298268974701,
            "MacroF1": 0.7652407320979201,
            "Memory in Mb": 4.154973983764648,
            "Time in s": 3365.640643
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7768595041322314,
            "MicroF1": 0.7768595041322314,
            "MacroF1": 0.764461061100325,
            "Memory in Mb": 4.15504264831543,
            "Time in s": 3499.962334
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7769597228237333,
            "MicroF1": 0.7769597228237333,
            "MacroF1": 0.7645642360301897,
            "Memory in Mb": 4.155065536499023,
            "Time in s": 3634.881072
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6360189573459716,
            "MicroF1": 0.6360189573459716,
            "MacroF1": 0.5970323052762561,
            "Memory in Mb": 6.533428192138672,
            "Time in s": 93.097088
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.62482235907153,
            "MicroF1": 0.62482235907153,
            "MacroF1": 0.5890580890213498,
            "Memory in Mb": 6.533924102783203,
            "Time in s": 264.682132
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6157246605620461,
            "MicroF1": 0.6157246605620461,
            "MacroF1": 0.5802533923244892,
            "Memory in Mb": 6.534633636474609,
            "Time in s": 504.284209
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6107032914989344,
            "MicroF1": 0.6107032914989344,
            "MacroF1": 0.5748501357120321,
            "Memory in Mb": 6.535015106201172,
            "Time in s": 804.5259470000001
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.614889183557492,
            "MicroF1": 0.614889183557492,
            "MacroF1": 0.5777842549225517,
            "Memory in Mb": 6.535823822021484,
            "Time in s": 1159.582019
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.608997632202052,
            "MicroF1": 0.608997632202052,
            "MacroF1": 0.5733157350789625,
            "Memory in Mb": 6.535648345947266,
            "Time in s": 1564.000203
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6057367068055743,
            "MicroF1": 0.6057367068055743,
            "MacroF1": 0.5703382690867537,
            "Memory in Mb": 6.535068511962891,
            "Time in s": 2016.310233
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6069610512608027,
            "MicroF1": 0.6069610512608027,
            "MacroF1": 0.5711427916016896,
            "Memory in Mb": 6.534946441650391,
            "Time in s": 2516.339397
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6039145532989583,
            "MicroF1": 0.6039145532989583,
            "MacroF1": 0.5678102867297489,
            "Memory in Mb": 6.535068511962891,
            "Time in s": 3064.243813
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6034662373330808,
            "MicroF1": 0.6034662373330808,
            "MacroF1": 0.567425153452482,
            "Memory in Mb": 6.535427093505859,
            "Time in s": 3659.768381
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6005165733964701,
            "MicroF1": 0.6005165733964701,
            "MacroF1": 0.56512832395729,
            "Memory in Mb": 6.535404205322266,
            "Time in s": 4303.846419
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6031883829216321,
            "MicroF1": 0.6031883829216321,
            "MacroF1": 0.5703828979306639,
            "Memory in Mb": 6.535358428955078,
            "Time in s": 4997.310473
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6147009543235958,
            "MicroF1": 0.6147009543235958,
            "MacroF1": 0.5955104002005771,
            "Memory in Mb": 6.534030914306641,
            "Time in s": 5738.022631999999
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6051545694378678,
            "MicroF1": 0.6051545694378678,
            "MacroF1": 0.586271708420286,
            "Memory in Mb": 6.533008575439453,
            "Time in s": 6524.316427
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5703642906749163,
            "MicroF1": 0.5703642906749163,
            "MacroF1": 0.5530031721301686,
            "Memory in Mb": 6.534244537353516,
            "Time in s": 7355.370967999999
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5440662918023084,
            "MicroF1": 0.5440662918023084,
            "MacroF1": 0.5274181049148582,
            "Memory in Mb": 6.532741546630859,
            "Time in s": 8230.882624
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.524650437301543,
            "MicroF1": 0.524650437301543,
            "MacroF1": 0.5077439094080566,
            "Memory in Mb": 6.533657073974609,
            "Time in s": 9149.482306
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5142842110801283,
            "MicroF1": 0.5142842110801283,
            "MacroF1": 0.4945495171544722,
            "Memory in Mb": 5.423342704772949,
            "Time in s": 10110.1367
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5202611772915317,
            "MicroF1": 0.5202611772915317,
            "MacroF1": 0.499632175624185,
            "Memory in Mb": 13.463048934936523,
            "Time in s": 11121.939621
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5284814621904447,
            "MicroF1": 0.5284814621904447,
            "MacroF1": 0.5082299437323158,
            "Memory in Mb": 14.233846664428713,
            "Time in s": 12202.11771
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5344757609921083,
            "MicroF1": 0.5344757609921083,
            "MacroF1": 0.5148729059414189,
            "Memory in Mb": 14.772774696350098,
            "Time in s": 13344.394485
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5430674529723215,
            "MicroF1": 0.5430674529723215,
            "MacroF1": 0.5233933209280776,
            "Memory in Mb": 14.684733390808104,
            "Time in s": 14542.607494
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5502120475974801,
            "MicroF1": 0.5502120475974801,
            "MacroF1": 0.5298443248135049,
            "Memory in Mb": 16.20911407470703,
            "Time in s": 15791.070918
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5564061081955569,
            "MicroF1": 0.5564061081955569,
            "MacroF1": 0.5355525016331893,
            "Memory in Mb": 16.199478149414062,
            "Time in s": 17093.843057
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.561460661388689,
            "MicroF1": 0.561460661388689,
            "MacroF1": 0.5398397773012414,
            "Memory in Mb": 16.192718505859375,
            "Time in s": 18441.382026
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.564742305590967,
            "MicroF1": 0.564742305590967,
            "MacroF1": 0.5421523628031605,
            "Memory in Mb": 15.229331016540527,
            "Time in s": 19838.570208
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5680614499666795,
            "MicroF1": 0.5680614499666795,
            "MacroF1": 0.5472893783055924,
            "Memory in Mb": 13.71937370300293,
            "Time in s": 21280.868604
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5701288598775662,
            "MicroF1": 0.5701288598775662,
            "MacroF1": 0.55295508639855,
            "Memory in Mb": 11.343052864074709,
            "Time in s": 22768.358846
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5724128922705156,
            "MicroF1": 0.5724128922705156,
            "MacroF1": 0.5585792537754973,
            "Memory in Mb": 9.387857437133787,
            "Time in s": 24294.822849
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5749865841724802,
            "MicroF1": 0.5749865841724802,
            "MacroF1": 0.5636037623129485,
            "Memory in Mb": 9.38664436340332,
            "Time in s": 25857.719223
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5781884832747823,
            "MicroF1": 0.5781884832747823,
            "MacroF1": 0.5684564968293649,
            "Memory in Mb": 9.385660171508787,
            "Time in s": 27456.12944
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.575656239827173,
            "MicroF1": 0.575656239827173,
            "MacroF1": 0.5663415557568727,
            "Memory in Mb": 7.860757827758789,
            "Time in s": 29092.739018
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5754584325766924,
            "MicroF1": 0.5754584325766924,
            "MacroF1": 0.565994999425249,
            "Memory in Mb": 7.205549240112305,
            "Time in s": 30762.023764
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5763863743976827,
            "MicroF1": 0.5763863743976827,
            "MacroF1": 0.5665127709334143,
            "Memory in Mb": 6.54947566986084,
            "Time in s": 32461.363070000003
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5758813820720258,
            "MicroF1": 0.5758813820720258,
            "MacroF1": 0.56571927622701,
            "Memory in Mb": 6.547377586364746,
            "Time in s": 34189.07998
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5767460213073786,
            "MicroF1": 0.5767460213073786,
            "MacroF1": 0.5661110063916132,
            "Memory in Mb": 6.546515464782715,
            "Time in s": 35945.284935
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5764633615725219,
            "MicroF1": 0.5764633615725219,
            "MacroF1": 0.5659285794545608,
            "Memory in Mb": 6.543356895446777,
            "Time in s": 37730.818682000005
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.573454282652578,
            "MicroF1": 0.573454282652578,
            "MacroF1": 0.5636611811263741,
            "Memory in Mb": 8.510072708129883,
            "Time in s": 39542.33547700001
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5726391957846685,
            "MicroF1": 0.5726391957846685,
            "MacroF1": 0.5633960246210544,
            "Memory in Mb": 8.712862014770508,
            "Time in s": 41378.34519600001
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5723146854802433,
            "MicroF1": 0.5723146854802433,
            "MacroF1": 0.5635786987292998,
            "Memory in Mb": 10.13754653930664,
            "Time in s": 43237.00688100001
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5717981291142165,
            "MicroF1": 0.5717981291142165,
            "MacroF1": 0.5635967907133216,
            "Memory in Mb": 10.13637924194336,
            "Time in s": 45117.76335600001
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.571103244571712,
            "MicroF1": 0.571103244571712,
            "MacroF1": 0.5633625241299441,
            "Memory in Mb": 10.135028839111328,
            "Time in s": 47020.66134100001
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5712335102517233,
            "MicroF1": 0.5712335102517233,
            "MacroF1": 0.563808836162261,
            "Memory in Mb": 11.334146499633787,
            "Time in s": 48947.97157600001
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5728213847577642,
            "MicroF1": 0.5728213847577642,
            "MacroF1": 0.5658781423773395,
            "Memory in Mb": 12.350201606750488,
            "Time in s": 50897.74209700001
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.576863991245607,
            "MicroF1": 0.576863991245607,
            "MacroF1": 0.5703778478941884,
            "Memory in Mb": 16.125893592834473,
            "Time in s": 52890.49897200001
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5828512609366958,
            "MicroF1": 0.5828512609366958,
            "MacroF1": 0.5764029561430954,
            "Memory in Mb": 15.266244888305664,
            "Time in s": 54904.91240000001
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5890270194031956,
            "MicroF1": 0.5890270194031956,
            "MacroF1": 0.5823661991476956,
            "Memory in Mb": 14.839654922485352,
            "Time in s": 56940.07330000001
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.5947087024286306,
            "MicroF1": 0.5947087024286306,
            "MacroF1": 0.5876086024291545,
            "Memory in Mb": 12.465810775756836,
            "Time in s": 58994.29364000001
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.600718937827339,
            "MicroF1": 0.600718937827339,
            "MacroF1": 0.5930357853224563,
            "Memory in Mb": 11.884730339050291,
            "Time in s": 61065.77177200001
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6060342051932802,
            "MicroF1": 0.6060342051932802,
            "MacroF1": 0.5982060206393416,
            "Memory in Mb": 3.691446304321289,
            "Time in s": 63151.215841000005
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6063920373909588,
            "MicroF1": 0.6063920373909588,
            "MacroF1": 0.5985419438128344,
            "Memory in Mb": 3.691621780395508,
            "Time in s": 65236.99615100001
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9828009828009828,
            "MicroF1": 0.9828009828009828,
            "MacroF1": 0.6067632850241546,
            "Memory in Mb": 2.1448841094970703,
            "Time in s": 5.867596
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.943558282208589,
            "MicroF1": 0.943558282208589,
            "MacroF1": 0.7669956277713079,
            "Memory in Mb": 3.0916757583618164,
            "Time in s": 25.808269
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8912510220768601,
            "MicroF1": 0.8912510220768601,
            "MacroF1": 0.8617021305177773,
            "Memory in Mb": 4.035944938659668,
            "Time in s": 63.939426
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9031269160024524,
            "MicroF1": 0.9031269160024524,
            "MacroF1": 0.8868998230762758,
            "Memory in Mb": 4.988290786743164,
            "Time in s": 125.34339
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.898970083374203,
            "MicroF1": 0.898970083374203,
            "MacroF1": 0.888705938214812,
            "Memory in Mb": 6.037667274475098,
            "Time in s": 214.307845
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8594196975888844,
            "MicroF1": 0.8594196975888844,
            "MacroF1": 0.8547805855679916,
            "Memory in Mb": 6.993380546569824,
            "Time in s": 335.016386
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8651488616462347,
            "MicroF1": 0.8651488616462347,
            "MacroF1": 0.8483773016417727,
            "Memory in Mb": 7.939821243286133,
            "Time in s": 488.1215580000001
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8553478394115844,
            "MicroF1": 0.8553478394115844,
            "MacroF1": 0.8302147847543373,
            "Memory in Mb": 8.885003089904785,
            "Time in s": 675.394352
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8452737673658404,
            "MicroF1": 0.8452737673658404,
            "MacroF1": 0.8411086163638233,
            "Memory in Mb": 9.830622673034668,
            "Time in s": 899.024814
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8374601618043638,
            "MicroF1": 0.8374601618043638,
            "MacroF1": 0.8238000521910981,
            "Memory in Mb": 11.003908157348633,
            "Time in s": 1161.3046
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8250501448629374,
            "MicroF1": 0.8250501448629373,
            "MacroF1": 0.8343531144302688,
            "Memory in Mb": 11.974610328674316,
            "Time in s": 1461.738376
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8232890704800817,
            "MicroF1": 0.8232890704800817,
            "MacroF1": 0.8292209535545839,
            "Memory in Mb": 12.919659614562988,
            "Time in s": 1801.820426
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.8199132566471808,
            "MicroF1": 0.819913256647181,
            "MacroF1": 0.8044565992905442,
            "Memory in Mb": 13.86521053314209,
            "Time in s": 2181.861898
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7998599194536858,
            "MicroF1": 0.7998599194536857,
            "MacroF1": 0.8029484507582976,
            "Memory in Mb": 14.811628341674805,
            "Time in s": 2601.779179
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7970256577872201,
            "MicroF1": 0.7970256577872201,
            "MacroF1": 0.7783451709211457,
            "Memory in Mb": 15.75713062286377,
            "Time in s": 3063.5971010000003
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7720239007200858,
            "MicroF1": 0.7720239007200858,
            "MacroF1": 0.767005590841987,
            "Memory in Mb": 16.704151153564453,
            "Time in s": 3570.6766780000003
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7645277577505407,
            "MicroF1": 0.7645277577505407,
            "MacroF1": 0.766187831914561,
            "Memory in Mb": 17.649503707885742,
            "Time in s": 4126.519897
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.773389622769985,
            "MicroF1": 0.7733896227699851,
            "MacroF1": 0.770832075885354,
            "Memory in Mb": 18.61162567138672,
            "Time in s": 4733.5217410000005
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7737066185008385,
            "MicroF1": 0.7737066185008385,
            "MacroF1": 0.7718493223486268,
            "Memory in Mb": 19.557814598083496,
            "Time in s": 5395.069721000001
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7765657556073048,
            "MicroF1": 0.7765657556073047,
            "MacroF1": 0.7724710929560354,
            "Memory in Mb": 20.503721237182617,
            "Time in s": 6113.943535
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7730827594257033,
            "MicroF1": 0.7730827594257033,
            "MacroF1": 0.7727491763630034,
            "Memory in Mb": 21.88267517089844,
            "Time in s": 6890.839823
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7714763231197772,
            "MicroF1": 0.7714763231197772,
            "MacroF1": 0.7717207236627096,
            "Memory in Mb": 22.87528133392334,
            "Time in s": 7728.212391
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7702227432590856,
            "MicroF1": 0.7702227432590856,
            "MacroF1": 0.7694267539223918,
            "Memory in Mb": 23.822596549987797,
            "Time in s": 8626.275614
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7656010621999796,
            "MicroF1": 0.7656010621999795,
            "MacroF1": 0.7644081311179032,
            "Memory in Mb": 24.768078804016117,
            "Time in s": 9586.24664
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.757623296401608,
            "MicroF1": 0.757623296401608,
            "MacroF1": 0.749720417225094,
            "Memory in Mb": 25.71299648284912,
            "Time in s": 10618.940127
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.737154709154332,
            "MicroF1": 0.737154709154332,
            "MacroF1": 0.7245707699101513,
            "Memory in Mb": 26.660439491271973,
            "Time in s": 11726.561153
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.729822968679074,
            "MicroF1": 0.7298229686790739,
            "MacroF1": 0.7256689004292383,
            "Memory in Mb": 27.605186462402344,
            "Time in s": 12907.41343
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7229274271207213,
            "MicroF1": 0.7229274271207213,
            "MacroF1": 0.7092514304350318,
            "Memory in Mb": 28.551199913024902,
            "Time in s": 14153.769988
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7133801031189249,
            "MicroF1": 0.7133801031189249,
            "MacroF1": 0.7054771135814562,
            "Memory in Mb": 29.4963436126709,
            "Time in s": 15465.906612
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7177874009314487,
            "MicroF1": 0.7177874009314487,
            "MacroF1": 0.7138351093258007,
            "Memory in Mb": 30.441871643066406,
            "Time in s": 16835.329364
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7147149521625682,
            "MicroF1": 0.7147149521625682,
            "MacroF1": 0.7065885995198201,
            "Memory in Mb": 31.388431549072266,
            "Time in s": 18265.757575
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7031788586748372,
            "MicroF1": 0.7031788586748372,
            "MacroF1": 0.6954173783902821,
            "Memory in Mb": 32.33424186706543,
            "Time in s": 19760.458564
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7011067369828419,
            "MicroF1": 0.7011067369828419,
            "MacroF1": 0.6966368809795416,
            "Memory in Mb": 33.27959156036377,
            "Time in s": 21319.158047
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7007425564126595,
            "MicroF1": 0.7007425564126595,
            "MacroF1": 0.6971102154727419,
            "Memory in Mb": 34.22630214691162,
            "Time in s": 22941.129728
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6961972126899643,
            "MicroF1": 0.6961972126899643,
            "MacroF1": 0.691133802747568,
            "Memory in Mb": 35.17108726501465,
            "Time in s": 24623.129677
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.698781235105876,
            "MicroF1": 0.698781235105876,
            "MacroF1": 0.696592906911097,
            "Memory in Mb": 36.11711597442627,
            "Time in s": 26362.470984
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7048029148724744,
            "MicroF1": 0.7048029148724744,
            "MacroF1": 0.702773358939844,
            "Memory in Mb": 37.0643196105957,
            "Time in s": 28156.052692
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.7047668193252918,
            "MicroF1": 0.7047668193252918,
            "MacroF1": 0.7013012225519919,
            "Memory in Mb": 38.00920104980469,
            "Time in s": 30004.434818
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6956822324178241,
            "MicroF1": 0.6956822324178241,
            "MacroF1": 0.6887843659114408,
            "Memory in Mb": 38.955204010009766,
            "Time in s": 31904.325566000003
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6869906244255163,
            "MicroF1": 0.6869906244255163,
            "MacroF1": 0.6817298949676788,
            "Memory in Mb": 39.901418685913086,
            "Time in s": 33880.147234000004
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6840437615830693,
            "MicroF1": 0.6840437615830693,
            "MacroF1": 0.6809878840610977,
            "Memory in Mb": 40.84670162200928,
            "Time in s": 35894.19480500001
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6798949518529326,
            "MicroF1": 0.6798949518529326,
            "MacroF1": 0.6760668667678135,
            "Memory in Mb": 42.678324699401855,
            "Time in s": 37945.35177200001
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6725759562218548,
            "MicroF1": 0.6725759562218548,
            "MacroF1": 0.6693298574086026,
            "Memory in Mb": 43.72208595275879,
            "Time in s": 40033.19473500001
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6715503314578575,
            "MicroF1": 0.6715503314578575,
            "MacroF1": 0.6700615486077944,
            "Memory in Mb": 44.66869449615479,
            "Time in s": 42156.41544100001
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6768887194291628,
            "MicroF1": 0.6768887194291628,
            "MacroF1": 0.6760264883444682,
            "Memory in Mb": 45.61451721191406,
            "Time in s": 44306.462280000014
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6818884211648105,
            "MicroF1": 0.6818884211648105,
            "MacroF1": 0.6814185274246665,
            "Memory in Mb": 46.56109237670898,
            "Time in s": 46484.07667300002
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6739504563233377,
            "MicroF1": 0.6739504563233377,
            "MacroF1": 0.6724064481498903,
            "Memory in Mb": 47.50611400604248,
            "Time in s": 48682.185033000016
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.677883878874534,
            "MicroF1": 0.677883878874534,
            "MacroF1": 0.6774885006147249,
            "Memory in Mb": 48.45180988311768,
            "Time in s": 50904.928535000014
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6733530088539843,
            "MicroF1": 0.6733530088539843,
            "MacroF1": 0.6729949515014169,
            "Memory in Mb": 49.39821243286133,
            "Time in s": 53145.742009000016
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.6697387126819943,
            "MicroF1": 0.6697387126819943,
            "MacroF1": 0.6699810213452306,
            "Memory in Mb": 50.34487438201904,
            "Time in s": 55411.38251600001
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.3777777777777777,
            "MicroF1": 0.3777777777777777,
            "MacroF1": 0.2811210847975554,
            "Memory in Mb": 4.09740161895752,
            "Time in s": 6.997987
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5164835164835165,
            "MicroF1": 0.5164835164835165,
            "MacroF1": 0.5316649744849407,
            "Memory in Mb": 4.097981452941895,
            "Time in s": 22.017115
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.5547445255474452,
            "MicroF1": 0.5547445255474452,
            "MacroF1": 0.5804654781117263,
            "Memory in Mb": 4.0981035232543945,
            "Time in s": 44.610384
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6174863387978142,
            "MicroF1": 0.6174863387978142,
            "MacroF1": 0.6394923756219437,
            "Memory in Mb": 4.098713874816895,
            "Time in s": 74.61421299999999
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6506550218340611,
            "MicroF1": 0.6506550218340611,
            "MacroF1": 0.66859135700569,
            "Memory in Mb": 4.098713874816895,
            "Time in s": 111.653321
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6618181818181819,
            "MicroF1": 0.6618181818181819,
            "MacroF1": 0.6795855359270878,
            "Memory in Mb": 4.098832130432129,
            "Time in s": 156.076644
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.6853582554517134,
            "MicroF1": 0.6853582554517134,
            "MacroF1": 0.6872635633687633,
            "Memory in Mb": 4.099373817443848,
            "Time in s": 207.574915
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7111716621253406,
            "MicroF1": 0.7111716621253404,
            "MacroF1": 0.7098417316927395,
            "Memory in Mb": 4.099347114562988,
            "Time in s": 266.341739
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7215496368038741,
            "MicroF1": 0.7215496368038742,
            "MacroF1": 0.7201557312728714,
            "Memory in Mb": 4.09926700592041,
            "Time in s": 332.356571
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7211328976034859,
            "MicroF1": 0.721132897603486,
            "MacroF1": 0.7175330036146421,
            "Memory in Mb": 4.099320411682129,
            "Time in s": 405.380301
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7287128712871287,
            "MicroF1": 0.7287128712871287,
            "MacroF1": 0.7233455022590812,
            "Memory in Mb": 4.099320411682129,
            "Time in s": 485.520305
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7295825771324864,
            "MicroF1": 0.7295825771324864,
            "MacroF1": 0.7255599965917697,
            "Memory in Mb": 4.099240303039551,
            "Time in s": 572.983507
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7353433835845896,
            "MicroF1": 0.7353433835845896,
            "MacroF1": 0.7308494254186014,
            "Memory in Mb": 4.0992631912231445,
            "Time in s": 667.526521
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7340590979782271,
            "MicroF1": 0.7340590979782271,
            "MacroF1": 0.7314183982762247,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 768.914228
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.737300435413643,
            "MicroF1": 0.737300435413643,
            "MacroF1": 0.7343909641298695,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 877.069835
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7387755102040816,
            "MicroF1": 0.7387755102040816,
            "MacroF1": 0.7369557659594496,
            "Memory in Mb": 4.099850654602051,
            "Time in s": 992.190131
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7439180537772087,
            "MicroF1": 0.7439180537772088,
            "MacroF1": 0.7419020281650245,
            "Memory in Mb": 4.099850654602051,
            "Time in s": 1114.103609
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7436517533252721,
            "MicroF1": 0.7436517533252721,
            "MacroF1": 0.7432199627682998,
            "Memory in Mb": 4.099850654602051,
            "Time in s": 1242.576589
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7502863688430699,
            "MicroF1": 0.7502863688430699,
            "MacroF1": 0.7482089866208982,
            "Memory in Mb": 4.099850654602051,
            "Time in s": 1377.530874
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.750816104461371,
            "MicroF1": 0.750816104461371,
            "MacroF1": 0.7477650187313974,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 1518.374517
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7512953367875648,
            "MicroF1": 0.7512953367875648,
            "MacroF1": 0.747322646811651,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 1664.895359
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7507418397626113,
            "MicroF1": 0.7507418397626113,
            "MacroF1": 0.7469783619055548,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 1817.198797
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7530747398297067,
            "MicroF1": 0.7530747398297066,
            "MacroF1": 0.7482363934596314,
            "Memory in Mb": 4.099823951721191,
            "Time in s": 1975.112421
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7552130553037172,
            "MicroF1": 0.7552130553037172,
            "MacroF1": 0.750118495060715,
            "Memory in Mb": 4.0998735427856445,
            "Time in s": 2138.658016
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7571801566579635,
            "MicroF1": 0.7571801566579635,
            "MacroF1": 0.7516199800653577,
            "Memory in Mb": 4.0998735427856445,
            "Time in s": 2307.825702
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7598326359832636,
            "MicroF1": 0.7598326359832636,
            "MacroF1": 0.7548841797367702,
            "Memory in Mb": 4.0998735427856445,
            "Time in s": 2482.820129
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7598710717163578,
            "MicroF1": 0.7598710717163577,
            "MacroF1": 0.7553301531902636,
            "Memory in Mb": 4.0998735427856445,
            "Time in s": 2663.447895
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7645687645687645,
            "MicroF1": 0.7645687645687647,
            "MacroF1": 0.7590078532621816,
            "Memory in Mb": 4.1004838943481445,
            "Time in s": 2849.419913
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7644411102775694,
            "MicroF1": 0.7644411102775694,
            "MacroF1": 0.7591993978414527,
            "Memory in Mb": 4.100506782531738,
            "Time in s": 3040.9965970000003
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7650471356055112,
            "MicroF1": 0.7650471356055112,
            "MacroF1": 0.7601575050520947,
            "Memory in Mb": 4.100506782531738,
            "Time in s": 3238.5768190000003
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7670175438596492,
            "MicroF1": 0.7670175438596492,
            "MacroF1": 0.7613339877221927,
            "Memory in Mb": 4.100506782531738,
            "Time in s": 3441.4807240000005
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7715839564921821,
            "MicroF1": 0.7715839564921821,
            "MacroF1": 0.7641396475218201,
            "Memory in Mb": 4.100552558898926,
            "Time in s": 3649.5015090000006
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7732366512854317,
            "MicroF1": 0.7732366512854317,
            "MacroF1": 0.7648275341801108,
            "Memory in Mb": 4.100552558898926,
            "Time in s": 3862.69427
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7735124760076776,
            "MicroF1": 0.7735124760076776,
            "MacroF1": 0.7657569341108763,
            "Memory in Mb": 4.100552558898926,
            "Time in s": 4080.891056
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7737725295214419,
            "MicroF1": 0.7737725295214419,
            "MacroF1": 0.7651494083475014,
            "Memory in Mb": 4.10057544708252,
            "Time in s": 4304.577590000001
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7740181268882175,
            "MicroF1": 0.7740181268882175,
            "MacroF1": 0.7654813489818475,
            "Memory in Mb": 4.100529670715332,
            "Time in s": 4533.710142000001
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7730746619635509,
            "MicroF1": 0.7730746619635509,
            "MacroF1": 0.766493027961906,
            "Memory in Mb": 4.100529670715332,
            "Time in s": 4767.793233000001
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7756153405838581,
            "MicroF1": 0.7756153405838581,
            "MacroF1": 0.7686072256536652,
            "Memory in Mb": 4.100529670715332,
            "Time in s": 5007.029776000001
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7769102063580591,
            "MicroF1": 0.7769102063580591,
            "MacroF1": 0.7685414235990152,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 5251.440116000002
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7781402936378466,
            "MicroF1": 0.7781402936378466,
            "MacroF1": 0.7699957723931323,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 5500.964415000001
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7761273209549071,
            "MicroF1": 0.7761273209549071,
            "MacroF1": 0.7684985598909853,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 5755.503987000001
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7762817193164163,
            "MicroF1": 0.7762817193164163,
            "MacroF1": 0.7677434418046419,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 6014.862306000001
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7774405665149215,
            "MicroF1": 0.7774405665149215,
            "MacroF1": 0.7684788817649146,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 6279.121569000001
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7790410281759763,
            "MicroF1": 0.7790410281759763,
            "MacroF1": 0.7689103339153599,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 6548.278113000001
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7786370227162881,
            "MicroF1": 0.7786370227162881,
            "MacroF1": 0.7686288077529282,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 6822.363214000001
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7791962174940898,
            "MicroF1": 0.7791962174940898,
            "MacroF1": 0.768391950800897,
            "Memory in Mb": 4.100502967834473,
            "Time in s": 7101.096348000001
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7801943544655252,
            "MicroF1": 0.7801943544655253,
            "MacroF1": 0.768962628827985,
            "Memory in Mb": 4.100525856018066,
            "Time in s": 7384.333285000001
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7820570910738559,
            "MicroF1": 0.7820570910738559,
            "MacroF1": 0.7698068761587117,
            "Memory in Mb": 4.100499153137207,
            "Time in s": 7672.298476000001
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7789613848202397,
            "MicroF1": 0.7789613848202397,
            "MacroF1": 0.7667173742344939,
            "Memory in Mb": 4.100499153137207,
            "Time in s": 7965.117559000001
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7781644193127447,
            "MicroF1": 0.7781644193127447,
            "MacroF1": 0.7659138381656089,
            "Memory in Mb": 4.100499153137207,
            "Time in s": 8262.647904000001
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "ImageSegments",
            "Accuracy": 0.7782589865742746,
            "MicroF1": 0.7782589865742745,
            "MacroF1": 0.7660163657276376,
            "Memory in Mb": 4.100499153137207,
            "Time in s": 8561.303246000001
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6218009478672986,
            "MicroF1": 0.6218009478672986,
            "MacroF1": 0.5857016652718549,
            "Memory in Mb": 6.471495628356934,
            "Time in s": 220.837673
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6196115585030791,
            "MicroF1": 0.6196115585030791,
            "MacroF1": 0.5856756432415233,
            "Memory in Mb": 10.302834510803224,
            "Time in s": 598.297395
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.628986422481844,
            "MicroF1": 0.628986422481844,
            "MacroF1": 0.5949930595607559,
            "Memory in Mb": 19.024110794067383,
            "Time in s": 1103.516793
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6294103717736207,
            "MicroF1": 0.6294103717736207,
            "MacroF1": 0.5952675443708706,
            "Memory in Mb": 19.52926254272461,
            "Time in s": 1735.893967
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6364841826103429,
            "MicroF1": 0.6364841826103429,
            "MacroF1": 0.5994911272790603,
            "Memory in Mb": 18.82306957244873,
            "Time in s": 2497.807238
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6352012628255722,
            "MicroF1": 0.6352012628255722,
            "MacroF1": 0.5993891820807258,
            "Memory in Mb": 20.00343894958496,
            "Time in s": 3379.788115
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.638749830875389,
            "MicroF1": 0.638749830875389,
            "MacroF1": 0.6030343276880051,
            "Memory in Mb": 20.9547061920166,
            "Time in s": 4385.582643
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6405824553095774,
            "MicroF1": 0.6405824553095774,
            "MacroF1": 0.6028521616895871,
            "Memory in Mb": 23.98197650909424,
            "Time in s": 5520.259032
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6449542249815847,
            "MicroF1": 0.6449542249815847,
            "MacroF1": 0.6055705492028415,
            "Memory in Mb": 24.687146186828613,
            "Time in s": 6764.141036999999
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6485462638507434,
            "MicroF1": 0.6485462638507434,
            "MacroF1": 0.6081614166360887,
            "Memory in Mb": 28.76917839050293,
            "Time in s": 8102.806145
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6490744726646578,
            "MicroF1": 0.6490744726646578,
            "MacroF1": 0.6078786452761632,
            "Memory in Mb": 30.803756713867188,
            "Time in s": 9530.02909
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6514876489621971,
            "MicroF1": 0.6514876489621971,
            "MacroF1": 0.6111938480023122,
            "Memory in Mb": 35.14385414123535,
            "Time in s": 11044.69783
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6707947840023312,
            "MicroF1": 0.6707947840023312,
            "MacroF1": 0.6607574394823457,
            "Memory in Mb": 17.51351547241211,
            "Time in s": 12617.098737
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6821348846648176,
            "MicroF1": 0.6821348846648176,
            "MacroF1": 0.6733632096765088,
            "Memory in Mb": 9.275564193725586,
            "Time in s": 14250.678949
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6778205694803965,
            "MicroF1": 0.6778205694803965,
            "MacroF1": 0.670556396248407,
            "Memory in Mb": 11.964457511901855,
            "Time in s": 15956.730999
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6754661142349808,
            "MicroF1": 0.6754661142349808,
            "MacroF1": 0.6690281338426608,
            "Memory in Mb": 12.60369873046875,
            "Time in s": 17732.973803
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6721631106902123,
            "MicroF1": 0.6721631106902123,
            "MacroF1": 0.6660357480506892,
            "Memory in Mb": 12.93508529663086,
            "Time in s": 19577.321708
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6856947440416689,
            "MicroF1": 0.6856947440416689,
            "MacroF1": 0.6751812770122833,
            "Memory in Mb": 14.563780784606934,
            "Time in s": 21465.395048
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6926680954991776,
            "MicroF1": 0.6926680954991776,
            "MacroF1": 0.6785701715539604,
            "Memory in Mb": 23.61655616760254,
            "Time in s": 23398.659989
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6942090061082438,
            "MicroF1": 0.6942090061082438,
            "MacroF1": 0.6784920731228882,
            "Memory in Mb": 30.02095413208008,
            "Time in s": 25401.280766
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6958737316798196,
            "MicroF1": 0.6958737316798196,
            "MacroF1": 0.6784853924286285,
            "Memory in Mb": 31.29345321655273,
            "Time in s": 27443.688764
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6989798114588266,
            "MicroF1": 0.6989798114588266,
            "MacroF1": 0.6799590657327791,
            "Memory in Mb": 29.59604263305664,
            "Time in s": 29526.276677
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7011981718614897,
            "MicroF1": 0.7011981718614897,
            "MacroF1": 0.680282364066019,
            "Memory in Mb": 32.615909576416016,
            "Time in s": 31645.669428
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7031527443475516,
            "MicroF1": 0.7031527443475516,
            "MacroF1": 0.6805566439417602,
            "Memory in Mb": 33.91432285308838,
            "Time in s": 33792.819539
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7051782264479716,
            "MicroF1": 0.7051782264479716,
            "MacroF1": 0.6809495737401271,
            "Memory in Mb": 35.12977695465088,
            "Time in s": 35966.301701
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7065743944636678,
            "MicroF1": 0.7065743944636678,
            "MacroF1": 0.6805936316849747,
            "Memory in Mb": 38.84447956085205,
            "Time in s": 38159.78466
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7054820946301428,
            "MicroF1": 0.7054820946301428,
            "MacroF1": 0.681225779493031,
            "Memory in Mb": 34.570815086364746,
            "Time in s": 40377.715599
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7045692833226231,
            "MicroF1": 0.7045692833226231,
            "MacroF1": 0.6849598194839713,
            "Memory in Mb": 20.38253498077393,
            "Time in s": 42611.23284999999
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7031316330862424,
            "MicroF1": 0.7031316330862424,
            "MacroF1": 0.6877640955933652,
            "Memory in Mb": 22.55568027496338,
            "Time in s": 44864.71640799999
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7032418952618454,
            "MicroF1": 0.7032418952618454,
            "MacroF1": 0.6917227552448634,
            "Memory in Mb": 26.177990913391117,
            "Time in s": 47133.482559
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7037421719871697,
            "MicroF1": 0.7037421719871697,
            "MacroF1": 0.6952024388211077,
            "Memory in Mb": 25.7611780166626,
            "Time in s": 49415.922785
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.7002160338551685,
            "MicroF1": 0.7002160338551685,
            "MacroF1": 0.6931280234945141,
            "Memory in Mb": 25.958494186401367,
            "Time in s": 51714.47139399999
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6973627571957414,
            "MicroF1": 0.6973627571957414,
            "MacroF1": 0.6902163957562899,
            "Memory in Mb": 18.894118309021,
            "Time in s": 54032.337052
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6951786758766677,
            "MicroF1": 0.6951786758766677,
            "MacroF1": 0.6877287571005829,
            "Memory in Mb": 18.049145698547363,
            "Time in s": 56371.370632
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6919830081982737,
            "MicroF1": 0.6919830081982737,
            "MacroF1": 0.6843647347906762,
            "Memory in Mb": 22.045016288757324,
            "Time in s": 58731.919307
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6900697093252663,
            "MicroF1": 0.6900697093252663,
            "MacroF1": 0.68217396069655,
            "Memory in Mb": 25.079078674316406,
            "Time in s": 61114.705624
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.688720534411712,
            "MicroF1": 0.688720534411712,
            "MacroF1": 0.6808510434728485,
            "Memory in Mb": 19.794261932373047,
            "Time in s": 63520.517783
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6867695068158597,
            "MicroF1": 0.6867695068158597,
            "MacroF1": 0.6796002866264578,
            "Memory in Mb": 10.854747772216797,
            "Time in s": 65948.78476699999
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6843843333414273,
            "MicroF1": 0.6843843333414273,
            "MacroF1": 0.6779529807793833,
            "Memory in Mb": 10.474969863891602,
            "Time in s": 68395.63477799999
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6822131205757712,
            "MicroF1": 0.6822131205757712,
            "MacroF1": 0.6764872431583758,
            "Memory in Mb": 14.707494735717772,
            "Time in s": 70864.05938699999
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6795472918350849,
            "MicroF1": 0.6795472918350849,
            "MacroF1": 0.674587653669649,
            "Memory in Mb": 12.672552108764648,
            "Time in s": 73351.02096199998
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6769633153705666,
            "MicroF1": 0.6769633153705666,
            "MacroF1": 0.6725984110786069,
            "Memory in Mb": 13.144417762756348,
            "Time in s": 75857.66838799998
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6748959411544475,
            "MicroF1": 0.6748959411544475,
            "MacroF1": 0.6710316194917795,
            "Memory in Mb": 14.719610214233398,
            "Time in s": 78383.45415699997
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6743215031315241,
            "MicroF1": 0.6743215031315241,
            "MacroF1": 0.670959098678123,
            "Memory in Mb": 15.027325630187988,
            "Time in s": 80927.72302099997
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6765293882447021,
            "MicroF1": 0.6765293882447021,
            "MacroF1": 0.6733002712216741,
            "Memory in Mb": 17.283148765563965,
            "Time in s": 83488.02074099997
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6805970149253732,
            "MicroF1": 0.6805970149253732,
            "MacroF1": 0.6770692638556323,
            "Memory in Mb": 17.906007766723633,
            "Time in s": 86063.52222099998
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6848340754770205,
            "MicroF1": 0.6848340754770205,
            "MacroF1": 0.6808344811077705,
            "Memory in Mb": 18.8202543258667,
            "Time in s": 88653.18323199998
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6890524197525992,
            "MicroF1": 0.6890524197525992,
            "MacroF1": 0.6843657264244208,
            "Memory in Mb": 21.50714492797852,
            "Time in s": 91255.74433499998
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6932531936687089,
            "MicroF1": 0.6932531936687089,
            "MacroF1": 0.6877873898777546,
            "Memory in Mb": 23.154582023620605,
            "Time in s": 93870.637319
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6956002954601412,
            "MicroF1": 0.6956002954601412,
            "MacroF1": 0.6902433463100389,
            "Memory in Mb": 14.128369331359863,
            "Time in s": 96495.216564
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Insects",
            "Accuracy": 0.6958578538043787,
            "MicroF1": 0.6958578538043787,
            "MacroF1": 0.6905081705907102,
            "Memory in Mb": 13.83100128173828,
            "Time in s": 99120.191439
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9828009828009828,
            "MicroF1": 0.9828009828009828,
            "MacroF1": 0.6067632850241546,
            "Memory in Mb": 2.0028390884399414,
            "Time in s": 23.27864
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9521472392638036,
            "MicroF1": 0.9521472392638036,
            "MacroF1": 0.8408896590786493,
            "Memory in Mb": 4.076430320739746,
            "Time in s": 76.761208
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9533932951757972,
            "MicroF1": 0.9533932951757972,
            "MacroF1": 0.9542235338779168,
            "Memory in Mb": 5.6716413497924805,
            "Time in s": 164.877928
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9589209074187616,
            "MicroF1": 0.9589209074187616,
            "MacroF1": 0.936122253486076,
            "Memory in Mb": 8.122180938720703,
            "Time in s": 291.606081
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9573320255026974,
            "MicroF1": 0.9573320255026974,
            "MacroF1": 0.9445755787125868,
            "Memory in Mb": 10.5212984085083,
            "Time in s": 455.912148
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9607682876992236,
            "MicroF1": 0.9607682876992236,
            "MacroF1": 0.9588299190873342,
            "Memory in Mb": 9.06541347503662,
            "Time in s": 649.921126
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9618213660245184,
            "MicroF1": 0.9618213660245184,
            "MacroF1": 0.9516555143941908,
            "Memory in Mb": 13.188368797302246,
            "Time in s": 870.236672
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9589334967821024,
            "MicroF1": 0.9589334967821024,
            "MacroF1": 0.9492703335352553,
            "Memory in Mb": 13.21088695526123,
            "Time in s": 1122.958204
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9585943884500135,
            "MicroF1": 0.9585943884500135,
            "MacroF1": 0.9531276848185062,
            "Memory in Mb": 16.65507411956787,
            "Time in s": 1406.732623
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9541554302525128,
            "MicroF1": 0.9541554302525128,
            "MacroF1": 0.9416377826660955,
            "Memory in Mb": 17.091320037841797,
            "Time in s": 1722.764314
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9529752618676176,
            "MicroF1": 0.9529752618676176,
            "MacroF1": 0.9549694463549354,
            "Memory in Mb": 10.336687088012695,
            "Time in s": 2070.686487
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9550561797752808,
            "MicroF1": 0.9550561797752808,
            "MacroF1": 0.95517907029875,
            "Memory in Mb": 11.520882606506348,
            "Time in s": 2449.358224
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9568168960965492,
            "MicroF1": 0.9568168960965492,
            "MacroF1": 0.9575833276239932,
            "Memory in Mb": 13.737529754638672,
            "Time in s": 2856.6015070000003
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9574505340570828,
            "MicroF1": 0.9574505340570828,
            "MacroF1": 0.9570632809827344,
            "Memory in Mb": 15.842782020568848,
            "Time in s": 3290.691514
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9557117176009152,
            "MicroF1": 0.9557117176009152,
            "MacroF1": 0.9522483041543378,
            "Memory in Mb": 20.04281044006348,
            "Time in s": 3760.43818
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9566416424084572,
            "MicroF1": 0.9566416424084572,
            "MacroF1": 0.9568246790885272,
            "Memory in Mb": 11.687369346618652,
            "Time in s": 4258.095146
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.95746214852199,
            "MicroF1": 0.95746214852199,
            "MacroF1": 0.9579855320572276,
            "Memory in Mb": 12.48728847503662,
            "Time in s": 4780.363237
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9568296336647149,
            "MicroF1": 0.9568296336647149,
            "MacroF1": 0.9563404233689646,
            "Memory in Mb": 15.327423095703123,
            "Time in s": 5334.336646
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9565217391304348,
            "MicroF1": 0.9565217391304348,
            "MacroF1": 0.9563017119581124,
            "Memory in Mb": 18.70553493499756,
            "Time in s": 5920.99825
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.954528741267312,
            "MicroF1": 0.954528741267312,
            "MacroF1": 0.9527980459948604,
            "Memory in Mb": 24.08679676055908,
            "Time in s": 6539.621381999999
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.95459320649002,
            "MicroF1": 0.95459320649002,
            "MacroF1": 0.9549210113442088,
            "Memory in Mb": 21.21516990661621,
            "Time in s": 7187.28418
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9550974930362116,
            "MicroF1": 0.9550974930362116,
            "MacroF1": 0.955362716075958,
            "Memory in Mb": 17.566545486450195,
            "Time in s": 7867.802732999999
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9555579239049344,
            "MicroF1": 0.9555579239049344,
            "MacroF1": 0.9558253322166266,
            "Memory in Mb": 15.710055351257324,
            "Time in s": 8578.363562999999
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9552650393218262,
            "MicroF1": 0.9552650393218262,
            "MacroF1": 0.955371511778808,
            "Memory in Mb": 18.71725273132324,
            "Time in s": 9321.146736
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9533287577213452,
            "MicroF1": 0.9533287577213452,
            "MacroF1": 0.9523119157834916,
            "Memory in Mb": 15.605277061462402,
            "Time in s": 10099.276789999998
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9521070990855096,
            "MicroF1": 0.9521070990855096,
            "MacroF1": 0.9515822083565744,
            "Memory in Mb": 11.186952590942385,
            "Time in s": 10903.979313999998
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.953427144802542,
            "MicroF1": 0.953427144802542,
            "MacroF1": 0.9541201209142028,
            "Memory in Mb": 7.581887245178223,
            "Time in s": 11728.435273
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.953689923837871,
            "MicroF1": 0.953689923837871,
            "MacroF1": 0.9538275342826804,
            "Memory in Mb": 10.15964126586914,
            "Time in s": 12573.844722999998
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9535964838137098,
            "MicroF1": 0.9535964838137098,
            "MacroF1": 0.9538502960885475,
            "Memory in Mb": 11.061944961547852,
            "Time in s": 13441.174569
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9541629218073372,
            "MicroF1": 0.9541629218073372,
            "MacroF1": 0.9544632162431566,
            "Memory in Mb": 11.249642372131348,
            "Time in s": 14331.138910999998
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9548509527951292,
            "MicroF1": 0.9548509527951292,
            "MacroF1": 0.9551609875055332,
            "Memory in Mb": 13.203255653381348,
            "Time in s": 15243.410521999998
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9551895825354272,
            "MicroF1": 0.955189582535427,
            "MacroF1": 0.9553883557595892,
            "Memory in Mb": 9.36058521270752,
            "Time in s": 16176.429406999998
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.955953353635891,
            "MicroF1": 0.955953353635891,
            "MacroF1": 0.9562606797905644,
            "Memory in Mb": 11.575583457946776,
            "Time in s": 17130.275872
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9561675437964098,
            "MicroF1": 0.9561675437964098,
            "MacroF1": 0.9563487774281332,
            "Memory in Mb": 11.42638874053955,
            "Time in s": 18106.07239
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9549688353526156,
            "MicroF1": 0.9549688353526156,
            "MacroF1": 0.954852939557476,
            "Memory in Mb": 10.249165534973145,
            "Time in s": 19109.380901
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9552665622659496,
            "MicroF1": 0.9552665622659496,
            "MacroF1": 0.955472434271787,
            "Memory in Mb": 8.168793678283691,
            "Time in s": 20137.264239
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9560781715799934,
            "MicroF1": 0.9560781715799934,
            "MacroF1": 0.9563263247313608,
            "Memory in Mb": 9.020037651062012,
            "Time in s": 21191.151533
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9563955363478036,
            "MicroF1": 0.9563955363478036,
            "MacroF1": 0.9565429512012836,
            "Memory in Mb": 8.031278610229492,
            "Time in s": 22273.408126999995
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9566337753755264,
            "MicroF1": 0.9566337753755264,
            "MacroF1": 0.9567672375037608,
            "Memory in Mb": 10.967172622680664,
            "Time in s": 23379.117397999995
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9563085973405232,
            "MicroF1": 0.9563085973405232,
            "MacroF1": 0.9563585840602682,
            "Memory in Mb": 11.29026985168457,
            "Time in s": 24508.785403999995
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.955580797513003,
            "MicroF1": 0.955580797513003,
            "MacroF1": 0.9555776398983684,
            "Memory in Mb": 9.525394439697266,
            "Time in s": 25660.924918999997
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9564050189670266,
            "MicroF1": 0.9564050189670268,
            "MacroF1": 0.9565585833577668,
            "Memory in Mb": 10.421767234802246,
            "Time in s": 26839.493165999997
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9566778772159836,
            "MicroF1": 0.9566778772159836,
            "MacroF1": 0.9567660151847868,
            "Memory in Mb": 11.633780479431152,
            "Time in s": 28038.177978999996
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9564369672998718,
            "MicroF1": 0.9564369672998718,
            "MacroF1": 0.9564736297242662,
            "Memory in Mb": 8.448995590209961,
            "Time in s": 29257.620389999996
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9567514570510376,
            "MicroF1": 0.9567514570510376,
            "MacroF1": 0.9568227044222712,
            "Memory in Mb": 7.821832656860352,
            "Time in s": 30499.29393699999
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9568924175414292,
            "MicroF1": 0.9568924175414292,
            "MacroF1": 0.9569505378685396,
            "Memory in Mb": 9.859258651733398,
            "Time in s": 31763.565401999997
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9567144719687092,
            "MicroF1": 0.9567144719687092,
            "MacroF1": 0.956766336746882,
            "Memory in Mb": 11.256629943847656,
            "Time in s": 33053.804573999994
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9568503293673084,
            "MicroF1": 0.9568503293673084,
            "MacroF1": 0.9569026376832064,
            "Memory in Mb": 11.690522193908691,
            "Time in s": 34367.36625199999
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9564303936771548,
            "MicroF1": 0.9564303936771548,
            "MacroF1": 0.956465338137946,
            "Memory in Mb": 12.451186180114746,
            "Time in s": 35701.899461999994
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Leveraging Bagging",
            "dataset": "Keystroke",
            "Accuracy": 0.9566155203686456,
            "MicroF1": 0.9566155203686456,
            "MacroF1": 0.9566498206969932,
            "Memory in Mb": 7.4099931716918945,
            "Time in s": 37049.10208799999
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.4,
            "MicroF1": 0.4000000000000001,
            "MacroF1": 0.3289160825620571,
            "Memory in Mb": 1.89190673828125,
            "Time in s": 1.901401
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.5494505494505495,
            "MicroF1": 0.5494505494505495,
            "MacroF1": 0.5607526488856412,
            "Memory in Mb": 2.084074020385742,
            "Time in s": 6.467373
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.5693430656934306,
            "MicroF1": 0.5693430656934306,
            "MacroF1": 0.5872103411959265,
            "Memory in Mb": 2.357966423034668,
            "Time in s": 13.822826
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.6174863387978142,
            "MicroF1": 0.6174863387978142,
            "MacroF1": 0.6372989403156369,
            "Memory in Mb": 2.7369613647460938,
            "Time in s": 24.259991
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.6375545851528385,
            "MicroF1": 0.6375545851528385,
            "MacroF1": 0.6548159763148107,
            "Memory in Mb": 2.862431526184082,
            "Time in s": 37.817905
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.6618181818181819,
            "MicroF1": 0.6618181818181819,
            "MacroF1": 0.6802187985971371,
            "Memory in Mb": 2.982741355895996,
            "Time in s": 54.565381
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.6915887850467289,
            "MicroF1": 0.6915887850467289,
            "MacroF1": 0.6955507555363084,
            "Memory in Mb": 3.080752372741699,
            "Time in s": 74.633343
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7111716621253406,
            "MicroF1": 0.7111716621253404,
            "MacroF1": 0.7105739026832886,
            "Memory in Mb": 3.232259750366211,
            "Time in s": 98.204704
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7263922518159807,
            "MicroF1": 0.7263922518159807,
            "MacroF1": 0.7261041400072307,
            "Memory in Mb": 3.505929946899414,
            "Time in s": 125.527545
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7276688453159041,
            "MicroF1": 0.7276688453159043,
            "MacroF1": 0.72519869331257,
            "Memory in Mb": 3.787288665771485,
            "Time in s": 156.78717
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7425742574257426,
            "MicroF1": 0.7425742574257425,
            "MacroF1": 0.7379486431795568,
            "Memory in Mb": 6.240692138671875,
            "Time in s": 210.523476
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7422867513611615,
            "MicroF1": 0.7422867513611615,
            "MacroF1": 0.7388440561615693,
            "Memory in Mb": 6.313092231750488,
            "Time in s": 268.009607
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7520938023450586,
            "MicroF1": 0.7520938023450586,
            "MacroF1": 0.749839509127547,
            "Memory in Mb": 6.682056427001953,
            "Time in s": 329.26112900000004
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7573872472783826,
            "MicroF1": 0.7573872472783826,
            "MacroF1": 0.7582793237949303,
            "Memory in Mb": 7.269444465637207,
            "Time in s": 394.37227100000007
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7634252539912917,
            "MicroF1": 0.7634252539912917,
            "MacroF1": 0.7648953830992049,
            "Memory in Mb": 7.531791687011719,
            "Time in s": 463.2777280000001
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7673469387755102,
            "MicroF1": 0.7673469387755102,
            "MacroF1": 0.7694390547687558,
            "Memory in Mb": 7.987269401550293,
            "Time in s": 536.1609010000001
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7772087067861716,
            "MicroF1": 0.7772087067861717,
            "MacroF1": 0.7788980835102386,
            "Memory in Mb": 8.317158699035645,
            "Time in s": 613.0067590000001
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7823458282950423,
            "MicroF1": 0.7823458282950423,
            "MacroF1": 0.7854763667551727,
            "Memory in Mb": 8.613452911376953,
            "Time in s": 693.8523060000001
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7915234822451317,
            "MicroF1": 0.7915234822451317,
            "MacroF1": 0.7933203073280156,
            "Memory in Mb": 8.694649696350098,
            "Time in s": 778.7710210000001
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.7986942328618063,
            "MicroF1": 0.7986942328618062,
            "MacroF1": 0.7996826842527437,
            "Memory in Mb": 8.824880599975586,
            "Time in s": 867.8856220000001
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8041450777202073,
            "MicroF1": 0.8041450777202073,
            "MacroF1": 0.8044659150084363,
            "Memory in Mb": 9.089361190795898,
            "Time in s": 961.208295
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8100890207715133,
            "MicroF1": 0.8100890207715133,
            "MacroF1": 0.8093994872208631,
            "Memory in Mb": 9.280214309692385,
            "Time in s": 1058.9817440000002
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8145695364238411,
            "MicroF1": 0.814569536423841,
            "MacroF1": 0.8133421993203876,
            "Memory in Mb": 9.165953636169434,
            "Time in s": 1161.0697040000002
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8213961922030825,
            "MicroF1": 0.8213961922030824,
            "MacroF1": 0.8206569542548617,
            "Memory in Mb": 8.760258674621582,
            "Time in s": 1267.2341280000005
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.824194952132289,
            "MicroF1": 0.824194952132289,
            "MacroF1": 0.8228781271733864,
            "Memory in Mb": 8.742037773132324,
            "Time in s": 1377.3471480000003
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8292887029288702,
            "MicroF1": 0.8292887029288704,
            "MacroF1": 0.8281638601893785,
            "Memory in Mb": 8.87535572052002,
            "Time in s": 1491.4919770000004
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8340048348106366,
            "MicroF1": 0.8340048348106366,
            "MacroF1": 0.833490204478907,
            "Memory in Mb": 8.332135200500488,
            "Time in s": 1609.3898390000004
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8360528360528361,
            "MicroF1": 0.8360528360528361,
            "MacroF1": 0.8353480055004047,
            "Memory in Mb": 8.416248321533203,
            "Time in s": 1730.8650650000004
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8394598649662416,
            "MicroF1": 0.8394598649662416,
            "MacroF1": 0.8389194005130135,
            "Memory in Mb": 8.469959259033203,
            "Time in s": 1855.8596220000004
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8419144307469181,
            "MicroF1": 0.8419144307469181,
            "MacroF1": 0.8414934007209077,
            "Memory in Mb": 8.578604698181152,
            "Time in s": 1984.2269550000003
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8449122807017544,
            "MicroF1": 0.8449122807017544,
            "MacroF1": 0.8435602800871403,
            "Memory in Mb": 8.689190864562988,
            "Time in s": 2115.814455
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8484024473147519,
            "MicroF1": 0.8484024473147518,
            "MacroF1": 0.8459519552383536,
            "Memory in Mb": 8.800261497497559,
            "Time in s": 2250.613689
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8503625576796309,
            "MicroF1": 0.8503625576796308,
            "MacroF1": 0.8475723684173131,
            "Memory in Mb": 9.025433540344238,
            "Time in s": 2388.852428
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8522072936660269,
            "MicroF1": 0.8522072936660269,
            "MacroF1": 0.8497128793769615,
            "Memory in Mb": 8.811847686767578,
            "Time in s": 2530.498155
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8527035425730267,
            "MicroF1": 0.8527035425730267,
            "MacroF1": 0.8503048238231962,
            "Memory in Mb": 8.729784965515137,
            "Time in s": 2675.5358680000004
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8531722054380665,
            "MicroF1": 0.8531722054380665,
            "MacroF1": 0.8508343416398155,
            "Memory in Mb": 8.761359214782715,
            "Time in s": 2823.7565440000003
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8571428571428571,
            "MicroF1": 0.8571428571428571,
            "MacroF1": 0.8561317791292776,
            "Memory in Mb": 8.798370361328125,
            "Time in s": 2975.2442650000003
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8580423583285632,
            "MicroF1": 0.8580423583285632,
            "MacroF1": 0.8567712479140972,
            "Memory in Mb": 8.86152172088623,
            "Time in s": 3129.874549
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8611266034578918,
            "MicroF1": 0.8611266034578918,
            "MacroF1": 0.8591986188286931,
            "Memory in Mb": 8.932531356811523,
            "Time in s": 3287.541657
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8618814573137574,
            "MicroF1": 0.8618814573137574,
            "MacroF1": 0.8601172531559075,
            "Memory in Mb": 8.819746017456055,
            "Time in s": 3448.3205970000004
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8636604774535809,
            "MicroF1": 0.8636604774535809,
            "MacroF1": 0.8623243992773615,
            "Memory in Mb": 9.007128715515137,
            "Time in s": 3612.136702
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8648368720870016,
            "MicroF1": 0.8648368720870016,
            "MacroF1": 0.8630569076841595,
            "Memory in Mb": 9.368453979492188,
            "Time in s": 3779.147863
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8649468892261002,
            "MicroF1": 0.8649468892261002,
            "MacroF1": 0.8631362872103546,
            "Memory in Mb": 8.952109336853027,
            "Time in s": 3949.363777
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8665348492338112,
            "MicroF1": 0.8665348492338112,
            "MacroF1": 0.8639071890295129,
            "Memory in Mb": 9.146061897277832,
            "Time in s": 4122.536804
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8680521991300145,
            "MicroF1": 0.8680521991300145,
            "MacroF1": 0.8658036637930728,
            "Memory in Mb": 8.80567455291748,
            "Time in s": 4298.84894
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8695035460992908,
            "MicroF1": 0.8695035460992909,
            "MacroF1": 0.8667661913422944,
            "Memory in Mb": 8.892473220825195,
            "Time in s": 4478.129032
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8690421101341971,
            "MicroF1": 0.869042110134197,
            "MacroF1": 0.8663186552920692,
            "Memory in Mb": 8.910783767700195,
            "Time in s": 4660.403073
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8699592206615315,
            "MicroF1": 0.8699592206615315,
            "MacroF1": 0.8669965232275297,
            "Memory in Mb": 8.99278450012207,
            "Time in s": 4845.573407999999
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.869063470927652,
            "MicroF1": 0.8690634709276521,
            "MacroF1": 0.8666022158227548,
            "Memory in Mb": 9.09610366821289,
            "Time in s": 5033.674223999999
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8686385384949978,
            "MicroF1": 0.8686385384949978,
            "MacroF1": 0.8662053097556822,
            "Memory in Mb": 9.110825538635254,
            "Time in s": 5224.692184
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "ImageSegments",
            "Accuracy": 0.8679081853616284,
            "MicroF1": 0.8679081853616284,
            "MacroF1": 0.8656034675726049,
            "Memory in Mb": 9.181622505187988,
            "Time in s": 5416.881651
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.6511848341232227,
            "MicroF1": 0.6511848341232227,
            "MacroF1": 0.5864257754346489,
            "Memory in Mb": 12.51792049407959,
            "Time in s": 137.265242
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.6873519658929418,
            "MicroF1": 0.6873519658929418,
            "MacroF1": 0.6004104483953082,
            "Memory in Mb": 15.371862411499023,
            "Time in s": 366.367491
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.6978212819703189,
            "MicroF1": 0.6978212819703189,
            "MacroF1": 0.602242348585179,
            "Memory in Mb": 17.772335052490234,
            "Time in s": 671.574116
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7054226852948141,
            "MicroF1": 0.7054226852948141,
            "MacroF1": 0.6059831617919115,
            "Memory in Mb": 20.14197826385498,
            "Time in s": 1043.757912
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7080886531540065,
            "MicroF1": 0.7080886531540066,
            "MacroF1": 0.6082411118035554,
            "Memory in Mb": 23.246225357055664,
            "Time in s": 1476.569185
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.708602999210734,
            "MicroF1": 0.708602999210734,
            "MacroF1": 0.6091818949546898,
            "Memory in Mb": 28.13547992706299,
            "Time in s": 1970.150117
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7104586659450683,
            "MicroF1": 0.7104586659450683,
            "MacroF1": 0.6104104212994758,
            "Memory in Mb": 30.16471099853516,
            "Time in s": 2526.789716
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7130342133301764,
            "MicroF1": 0.7130342133301764,
            "MacroF1": 0.6119778058667307,
            "Memory in Mb": 27.69899654388428,
            "Time in s": 3146.1270590000004
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.717773334736399,
            "MicroF1": 0.717773334736399,
            "MacroF1": 0.6149023583636667,
            "Memory in Mb": 27.04288387298584,
            "Time in s": 3829.1831980000006
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7215645420967894,
            "MicroF1": 0.7215645420967894,
            "MacroF1": 0.617635708330779,
            "Memory in Mb": 23.96706485748291,
            "Time in s": 4572.729772000001
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7213086526043909,
            "MicroF1": 0.721308652604391,
            "MacroF1": 0.6182075626749539,
            "Memory in Mb": 26.15617847442627,
            "Time in s": 5374.612830000001
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7240943887617394,
            "MicroF1": 0.7240943887617394,
            "MacroF1": 0.6351065980046956,
            "Memory in Mb": 25.05154228210449,
            "Time in s": 6233.453892000001
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7432796678079697,
            "MicroF1": 0.7432796678079697,
            "MacroF1": 0.7402334392509421,
            "Memory in Mb": 15.30208683013916,
            "Time in s": 7142.743199000001
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7491713454643848,
            "MicroF1": 0.7491713454643848,
            "MacroF1": 0.7487081677599373,
            "Memory in Mb": 11.128735542297363,
            "Time in s": 8102.097506000001
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7424079803017867,
            "MicroF1": 0.7424079803017867,
            "MacroF1": 0.7445532404968841,
            "Memory in Mb": 16.950417518615723,
            "Time in s": 9128.379042
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7382657591003255,
            "MicroF1": 0.7382657591003255,
            "MacroF1": 0.7427378731329454,
            "Memory in Mb": 18.26229953765869,
            "Time in s": 10214.572621
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7309342097933262,
            "MicroF1": 0.7309342097933262,
            "MacroF1": 0.7368436311738037,
            "Memory in Mb": 23.77636337280273,
            "Time in s": 11358.099531000002
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7429368127531962,
            "MicroF1": 0.7429368127531962,
            "MacroF1": 0.7441354243297112,
            "Memory in Mb": 12.95803928375244,
            "Time in s": 12553.803014
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7475950755121368,
            "MicroF1": 0.7475950755121367,
            "MacroF1": 0.7439196968116685,
            "Memory in Mb": 12.612845420837402,
            "Time in s": 13796.415893
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7492305506889531,
            "MicroF1": 0.7492305506889531,
            "MacroF1": 0.7418613509588597,
            "Memory in Mb": 16.95127773284912,
            "Time in s": 15088.238885
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7509808342728298,
            "MicroF1": 0.7509808342728299,
            "MacroF1": 0.7400929587109365,
            "Memory in Mb": 17.926865577697754,
            "Time in s": 16424.025269
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7532176832680471,
            "MicroF1": 0.7532176832680472,
            "MacroF1": 0.7391930166872092,
            "Memory in Mb": 20.93969821929932,
            "Time in s": 17798.240955
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7550129699015935,
            "MicroF1": 0.7550129699015935,
            "MacroF1": 0.7379653286035112,
            "Memory in Mb": 25.43882942199707,
            "Time in s": 19212.969178
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7569743124334136,
            "MicroF1": 0.7569743124334136,
            "MacroF1": 0.7375346698329149,
            "Memory in Mb": 29.94521999359131,
            "Time in s": 20668.368585
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7580590173870222,
            "MicroF1": 0.7580590173870221,
            "MacroF1": 0.7363169253318035,
            "Memory in Mb": 34.1699275970459,
            "Time in s": 22166.950006
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7593880896011656,
            "MicroF1": 0.7593880896011656,
            "MacroF1": 0.7352131419868576,
            "Memory in Mb": 32.93678665161133,
            "Time in s": 23706.536377
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7573217354705202,
            "MicroF1": 0.7573217354705202,
            "MacroF1": 0.7350502568377754,
            "Memory in Mb": 21.273219108581543,
            "Time in s": 25286.984696
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7555382690161329,
            "MicroF1": 0.7555382690161329,
            "MacroF1": 0.7386915112539557,
            "Memory in Mb": 20.747055053710938,
            "Time in s": 26906.631088
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7544982529471312,
            "MicroF1": 0.7544982529471312,
            "MacroF1": 0.7426503125712552,
            "Memory in Mb": 24.91079425811768,
            "Time in s": 28562.795387
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7531487736355315,
            "MicroF1": 0.7531487736355315,
            "MacroF1": 0.7453200395899969,
            "Memory in Mb": 32.13512706756592,
            "Time in s": 30253.076649
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7530471971895525,
            "MicroF1": 0.7530471971895525,
            "MacroF1": 0.7484606399297139,
            "Memory in Mb": 36.17057991027832,
            "Time in s": 31977.334616
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7480986061377289,
            "MicroF1": 0.748098606137729,
            "MacroF1": 0.7448942365218528,
            "Memory in Mb": 13.298456192016602,
            "Time in s": 33736.870240000004
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7436795133010016,
            "MicroF1": 0.7436795133010016,
            "MacroF1": 0.7403442775964885,
            "Memory in Mb": 15.221885681152344,
            "Time in s": 35530.857132000005
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7404952232403977,
            "MicroF1": 0.7404952232403977,
            "MacroF1": 0.7368033013057004,
            "Memory in Mb": 16.932289123535156,
            "Time in s": 37356.72126300001
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7371411564165697,
            "MicroF1": 0.7371411564165696,
            "MacroF1": 0.7332530467261859,
            "Memory in Mb": 22.237309455871586,
            "Time in s": 39213.91358200001
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7341049585689859,
            "MicroF1": 0.7341049585689859,
            "MacroF1": 0.7299460315219516,
            "Memory in Mb": 22.86026954650879,
            "Time in s": 41100.10013700001
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7343042154027284,
            "MicroF1": 0.7343042154027284,
            "MacroF1": 0.7301016033872143,
            "Memory in Mb": 21.91624164581299,
            "Time in s": 43017.482867000006
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7327734443143021,
            "MicroF1": 0.7327734443143021,
            "MacroF1": 0.728948208474553,
            "Memory in Mb": 20.388718605041504,
            "Time in s": 44961.93393100001
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7327538061821626,
            "MicroF1": 0.7327538061821626,
            "MacroF1": 0.7292630064673854,
            "Memory in Mb": 15.630711555480955,
            "Time in s": 46951.12268600001
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7331849712351145,
            "MicroF1": 0.7331849712351144,
            "MacroF1": 0.7301128191332076,
            "Memory in Mb": 20.110919952392575,
            "Time in s": 48959.16072000001
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7337567848481349,
            "MicroF1": 0.7337567848481349,
            "MacroF1": 0.7309969621648841,
            "Memory in Mb": 24.057676315307617,
            "Time in s": 50985.068017000005
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7342111790038556,
            "MicroF1": 0.7342111790038556,
            "MacroF1": 0.731637560144403,
            "Memory in Mb": 28.52964782714844,
            "Time in s": 53028.942305
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7351289448763406,
            "MicroF1": 0.7351289448763407,
            "MacroF1": 0.7324911060941295,
            "Memory in Mb": 28.861422538757324,
            "Time in s": 55091.119898
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7357682457008803,
            "MicroF1": 0.7357682457008803,
            "MacroF1": 0.7329742877599967,
            "Memory in Mb": 33.07672500610352,
            "Time in s": 57170.52325500001
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7366947957659041,
            "MicroF1": 0.736694795765904,
            "MacroF1": 0.7341498113226347,
            "Memory in Mb": 21.3528356552124,
            "Time in s": 59267.07909500001
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7403602676273804,
            "MicroF1": 0.7403602676273804,
            "MacroF1": 0.7381372580344014,
            "Memory in Mb": 19.381468772888184,
            "Time in s": 61379.50627500001
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7442122866756664,
            "MicroF1": 0.7442122866756663,
            "MacroF1": 0.742109373234967,
            "Memory in Mb": 21.8067569732666,
            "Time in s": 63507.849119000006
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7475289521968157,
            "MicroF1": 0.7475289521968157,
            "MacroF1": 0.7453466445950636,
            "Memory in Mb": 21.65154266357422,
            "Time in s": 65647.81315
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7510581141410433,
            "MicroF1": 0.7510581141410433,
            "MacroF1": 0.7487124138061083,
            "Memory in Mb": 22.87060165405273,
            "Time in s": 67797.610737
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7545218659444307,
            "MicroF1": 0.7545218659444307,
            "MacroF1": 0.752582163258218,
            "Memory in Mb": 10.55445957183838,
            "Time in s": 69956.07865499999
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Insects",
            "Accuracy": 0.7547448294132117,
            "MicroF1": 0.7547448294132117,
            "MacroF1": 0.7528178949021433,
            "Memory in Mb": 10.58643913269043,
            "Time in s": 72115.038215
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9803439803439804,
            "MicroF1": 0.9803439803439804,
            "MacroF1": 0.4950372208436724,
            "Memory in Mb": 1.786503791809082,
            "Time in s": 20.578742
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.98159509202454,
            "MicroF1": 0.98159509202454,
            "MacroF1": 0.9278568842209168,
            "Memory in Mb": 6.9002227783203125,
            "Time in s": 101.280083
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9803761242845462,
            "MicroF1": 0.9803761242845462,
            "MacroF1": 0.9574942570636208,
            "Memory in Mb": 9.112634658813477,
            "Time in s": 223.840162
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9779276517473944,
            "MicroF1": 0.9779276517473944,
            "MacroF1": 0.9432755457272628,
            "Memory in Mb": 10.40715503692627,
            "Time in s": 381.844655
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.973516429622364,
            "MicroF1": 0.973516429622364,
            "MacroF1": 0.9361356188587968,
            "Memory in Mb": 12.656171798706056,
            "Time in s": 575.269036
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9726195341234164,
            "MicroF1": 0.9726195341234164,
            "MacroF1": 0.9612590316809274,
            "Memory in Mb": 8.745987892150879,
            "Time in s": 802.257021
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754816112084064,
            "MicroF1": 0.9754816112084064,
            "MacroF1": 0.975146989141396,
            "Memory in Mb": 9.931495666503906,
            "Time in s": 1061.688609
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754826846460312,
            "MicroF1": 0.9754826846460312,
            "MacroF1": 0.9697604489278108,
            "Memory in Mb": 10.511832237243652,
            "Time in s": 1352.298412
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9733042767638246,
            "MicroF1": 0.9733042767638246,
            "MacroF1": 0.9642745555297418,
            "Memory in Mb": 11.800049781799316,
            "Time in s": 1675.333833
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9722971316499142,
            "MicroF1": 0.9722971316499142,
            "MacroF1": 0.9666413905932107,
            "Memory in Mb": 12.42660903930664,
            "Time in s": 2030.177258
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9734789391575664,
            "MicroF1": 0.9734789391575664,
            "MacroF1": 0.9728883985144964,
            "Memory in Mb": 9.746350288391112,
            "Time in s": 2413.735444
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9740551583248211,
            "MicroF1": 0.9740551583248211,
            "MacroF1": 0.9730015599884004,
            "Memory in Mb": 10.666529655456545,
            "Time in s": 2823.505547
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9741655666603808,
            "MicroF1": 0.9741655666603808,
            "MacroF1": 0.9728266773902404,
            "Memory in Mb": 11.775634765625,
            "Time in s": 3261.739577
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9747855016634565,
            "MicroF1": 0.9747855016634565,
            "MacroF1": 0.9744326987999562,
            "Memory in Mb": 12.58005428314209,
            "Time in s": 3727.994683
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9751593397613988,
            "MicroF1": 0.9751593397613988,
            "MacroF1": 0.9747223863351728,
            "Memory in Mb": 13.55466365814209,
            "Time in s": 4223.159482999999
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9751800214493642,
            "MicroF1": 0.9751800214493642,
            "MacroF1": 0.974525548169428,
            "Memory in Mb": 11.360074043273926,
            "Time in s": 4747.988555
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9763518385003604,
            "MicroF1": 0.9763518385003604,
            "MacroF1": 0.9769458779347456,
            "Memory in Mb": 11.155635833740234,
            "Time in s": 5300.577354999999
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9765763311997822,
            "MicroF1": 0.9765763311997822,
            "MacroF1": 0.976392359672136,
            "Memory in Mb": 12.33658504486084,
            "Time in s": 5881.207234
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9771642368726616,
            "MicroF1": 0.9771642368726616,
            "MacroF1": 0.9773496343719736,
            "Memory in Mb": 13.116165161132812,
            "Time in s": 6492.775159
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.976590268415247,
            "MicroF1": 0.976590268415247,
            "MacroF1": 0.975927508407602,
            "Memory in Mb": 13.303799629211426,
            "Time in s": 7137.299991
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9768880588303958,
            "MicroF1": 0.9768880588303958,
            "MacroF1": 0.9769304999907084,
            "Memory in Mb": 13.133574485778809,
            "Time in s": 7814.540539
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9774930362116993,
            "MicroF1": 0.9774930362116993,
            "MacroF1": 0.9777587646121524,
            "Memory in Mb": 13.50635814666748,
            "Time in s": 8523.072866
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9767664925929872,
            "MicroF1": 0.9767664925929872,
            "MacroF1": 0.9763135719034828,
            "Memory in Mb": 15.166536331176758,
            "Time in s": 9263.702674
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9765090389132876,
            "MicroF1": 0.9765090389132876,
            "MacroF1": 0.9763153416047448,
            "Memory in Mb": 16.169885635375977,
            "Time in s": 10037.443626
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9758799882341406,
            "MicroF1": 0.9758799882341406,
            "MacroF1": 0.9755246287395946,
            "Memory in Mb": 14.205968856811523,
            "Time in s": 10844.068015
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9755821627227302,
            "MicroF1": 0.9755821627227302,
            "MacroF1": 0.9754319444516872,
            "Memory in Mb": 12.997503280639648,
            "Time in s": 11685.064117
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9759418974126192,
            "MicroF1": 0.9759418974126192,
            "MacroF1": 0.9761027289556774,
            "Memory in Mb": 12.962043762207031,
            "Time in s": 12559.39796
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9760133064869124,
            "MicroF1": 0.9760133064869124,
            "MacroF1": 0.9760613734021468,
            "Memory in Mb": 14.09043312072754,
            "Time in s": 13467.395857
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754881244188996,
            "MicroF1": 0.9754881244188996,
            "MacroF1": 0.9753195915858492,
            "Memory in Mb": 14.295487403869627,
            "Time in s": 14408.853786
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9759784296102624,
            "MicroF1": 0.9759784296102624,
            "MacroF1": 0.9761779987511396,
            "Memory in Mb": 15.044499397277832,
            "Time in s": 15385.688043
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9762789594370206,
            "MicroF1": 0.9762789594370206,
            "MacroF1": 0.9764127823145236,
            "Memory in Mb": 15.120206832885742,
            "Time in s": 16404.149055
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9758713136729222,
            "MicroF1": 0.975871313672922,
            "MacroF1": 0.975797420384815,
            "Memory in Mb": 15.049361228942873,
            "Time in s": 17460.942559000003
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9757112084973631,
            "MicroF1": 0.9757112084973631,
            "MacroF1": 0.9757165619520196,
            "Memory in Mb": 15.162266731262209,
            "Time in s": 18558.798501
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9759930790858626,
            "MicroF1": 0.9759930790858626,
            "MacroF1": 0.9761084708221816,
            "Memory in Mb": 15.711796760559082,
            "Time in s": 19695.838422
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754884795854052,
            "MicroF1": 0.9754884795854052,
            "MacroF1": 0.975424480421301,
            "Memory in Mb": 16.988737106323242,
            "Time in s": 20872.643227
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.975624702117519,
            "MicroF1": 0.975624702117519,
            "MacroF1": 0.9757017096421696,
            "Memory in Mb": 17.869779586791992,
            "Time in s": 22084.930025
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9757535607817158,
            "MicroF1": 0.9757535607817158,
            "MacroF1": 0.9758249143111628,
            "Memory in Mb": 17.579912185668945,
            "Time in s": 23330.568569000003
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9755531187512094,
            "MicroF1": 0.9755531187512094,
            "MacroF1": 0.9755669148190674,
            "Memory in Mb": 16.59157657623291,
            "Time in s": 24610.336028
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9756772044497516,
            "MicroF1": 0.9756772044497516,
            "MacroF1": 0.97573890775282,
            "Memory in Mb": 16.193113327026367,
            "Time in s": 25925.188427
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9759176420123782,
            "MicroF1": 0.9759176420123782,
            "MacroF1": 0.9759886766110538,
            "Memory in Mb": 16.353660583496094,
            "Time in s": 27266.573062
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9756680815448078,
            "MicroF1": 0.9756680815448078,
            "MacroF1": 0.9756766431570708,
            "Memory in Mb": 17.00908374786377,
            "Time in s": 28641.859399
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9758389261744966,
            "MicroF1": 0.9758389261744966,
            "MacroF1": 0.975891563489883,
            "Memory in Mb": 18.364989280700684,
            "Time in s": 30047.550521
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9753747933648748,
            "MicroF1": 0.9753747933648748,
            "MacroF1": 0.975363882573194,
            "Memory in Mb": 17.298136711120605,
            "Time in s": 31485.782589
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9753217090969862,
            "MicroF1": 0.9753217090969862,
            "MacroF1": 0.9753429667022142,
            "Memory in Mb": 16.72727108001709,
            "Time in s": 32956.927282000004
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754888610490768,
            "MicroF1": 0.9754888610490768,
            "MacroF1": 0.9755190387029732,
            "Memory in Mb": 17.51059913635254,
            "Time in s": 34461.639008000006
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9757553151809026,
            "MicroF1": 0.9757553151809026,
            "MacroF1": 0.9757835195290104,
            "Memory in Mb": 18.871691703796387,
            "Time in s": 35998.873267
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754367666232072,
            "MicroF1": 0.9754367666232072,
            "MacroF1": 0.9754369138844644,
            "Memory in Mb": 17.42948341369629,
            "Time in s": 37568.082084
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754889444926722,
            "MicroF1": 0.9754889444926722,
            "MacroF1": 0.9754964783302286,
            "Memory in Mb": 17.978480339050293,
            "Time in s": 39170.395427
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9756390375669052,
            "MicroF1": 0.9756390375669052,
            "MacroF1": 0.975642520227376,
            "Memory in Mb": 19.26256561279297,
            "Time in s": 40805.125646
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Stacking",
            "dataset": "Keystroke",
            "Accuracy": 0.9754889945585568,
            "MicroF1": 0.9754889945585568,
            "MacroF1": 0.9754863274548964,
            "Memory in Mb": 18.711057662963867,
            "Time in s": 42471.761869
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.4666666666666667,
            "MicroF1": 0.4666666666666667,
            "MacroF1": 0.3890768588137009,
            "Memory in Mb": 0.9137420654296876,
            "Time in s": 0.663852
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.6153846153846154,
            "MicroF1": 0.6153846153846154,
            "MacroF1": 0.617040786788686,
            "Memory in Mb": 0.9906883239746094,
            "Time in s": 2.032737
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.6715328467153284,
            "MicroF1": 0.6715328467153284,
            "MacroF1": 0.6884491245817251,
            "Memory in Mb": 1.067914962768555,
            "Time in s": 4.226265
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7049180327868853,
            "MicroF1": 0.7049180327868853,
            "MacroF1": 0.7194266051408907,
            "Memory in Mb": 1.1443958282470703,
            "Time in s": 7.386208
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7292576419213974,
            "MicroF1": 0.7292576419213974,
            "MacroF1": 0.7448338459304749,
            "Memory in Mb": 1.2214689254760742,
            "Time in s": 11.723904
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7381818181818182,
            "MicroF1": 0.7381818181818182,
            "MacroF1": 0.7559766728000937,
            "Memory in Mb": 1.2995519638061523,
            "Time in s": 17.331033
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7538940809968847,
            "MicroF1": 0.7538940809968847,
            "MacroF1": 0.7616248500949714,
            "Memory in Mb": 1.3766565322875977,
            "Time in s": 24.26159
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.773841961852861,
            "MicroF1": 0.7738419618528611,
            "MacroF1": 0.7772939373537765,
            "Memory in Mb": 1.4532833099365234,
            "Time in s": 32.770568000000004
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7820823244552058,
            "MicroF1": 0.7820823244552059,
            "MacroF1": 0.7854200812154107,
            "Memory in Mb": 1.530414581298828,
            "Time in s": 42.983195
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7777777777777778,
            "MicroF1": 0.7777777777777778,
            "MacroF1": 0.7796254955467015,
            "Memory in Mb": 1.6075658798217771,
            "Time in s": 54.886431
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7861386138613862,
            "MicroF1": 0.7861386138613862,
            "MacroF1": 0.7886239053396241,
            "Memory in Mb": 3.8640270233154297,
            "Time in s": 87.00222099999999
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7858439201451906,
            "MicroF1": 0.7858439201451906,
            "MacroF1": 0.7889431335032357,
            "Memory in Mb": 4.088808059692383,
            "Time in s": 121.00394599999998
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7906197654941374,
            "MicroF1": 0.7906197654941374,
            "MacroF1": 0.7944387660679091,
            "Memory in Mb": 4.304059028625488,
            "Time in s": 157.00397999999998
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7853810264385692,
            "MicroF1": 0.7853810264385692,
            "MacroF1": 0.7901251252871709,
            "Memory in Mb": 4.532710075378418,
            "Time in s": 195.073691
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7895500725689405,
            "MicroF1": 0.7895500725689405,
            "MacroF1": 0.7935315861788143,
            "Memory in Mb": 4.759090423583984,
            "Time in s": 235.272046
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7863945578231293,
            "MicroF1": 0.7863945578231294,
            "MacroF1": 0.7911065855691086,
            "Memory in Mb": 4.991429328918457,
            "Time in s": 277.59962
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7887323943661971,
            "MicroF1": 0.7887323943661971,
            "MacroF1": 0.792926322670609,
            "Memory in Mb": 5.219735145568848,
            "Time in s": 322.071315
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7896009673518742,
            "MicroF1": 0.7896009673518742,
            "MacroF1": 0.7950712422059908,
            "Memory in Mb": 5.452417373657227,
            "Time in s": 368.82718
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7938144329896907,
            "MicroF1": 0.7938144329896907,
            "MacroF1": 0.7979586706142276,
            "Memory in Mb": 5.699496269226074,
            "Time in s": 417.885664
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.794341675734494,
            "MicroF1": 0.794341675734494,
            "MacroF1": 0.7973145688626199,
            "Memory in Mb": 5.9376373291015625,
            "Time in s": 469.16999
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7937823834196891,
            "MicroF1": 0.7937823834196891,
            "MacroF1": 0.7958827691316667,
            "Memory in Mb": 6.182188987731934,
            "Time in s": 522.9385980000001
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7912957467853611,
            "MicroF1": 0.7912957467853611,
            "MacroF1": 0.7931630938612351,
            "Memory in Mb": 6.34267520904541,
            "Time in s": 579.2700850000001
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.793755912961211,
            "MicroF1": 0.7937559129612108,
            "MacroF1": 0.7947921362588558,
            "Memory in Mb": 6.295009613037109,
            "Time in s": 638.2805060000001
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7941976427923844,
            "MicroF1": 0.7941976427923844,
            "MacroF1": 0.7951664828862093,
            "Memory in Mb": 6.2213640213012695,
            "Time in s": 699.725726
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7954743255004352,
            "MicroF1": 0.7954743255004351,
            "MacroF1": 0.7958304956922065,
            "Memory in Mb": 6.151959419250488,
            "Time in s": 763.5071
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.796652719665272,
            "MicroF1": 0.796652719665272,
            "MacroF1": 0.7972397572733622,
            "Memory in Mb": 6.087224006652832,
            "Time in s": 829.5043310000001
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7953263497179693,
            "MicroF1": 0.7953263497179693,
            "MacroF1": 0.795947547023496,
            "Memory in Mb": 6.001987457275391,
            "Time in s": 897.6078460000001
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7995337995337995,
            "MicroF1": 0.7995337995337995,
            "MacroF1": 0.799082939294124,
            "Memory in Mb": 5.924266815185547,
            "Time in s": 967.722432
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7981995498874719,
            "MicroF1": 0.7981995498874719,
            "MacroF1": 0.7978549794399667,
            "Memory in Mb": 5.872907638549805,
            "Time in s": 1039.926656
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.7991298042059464,
            "MicroF1": 0.7991298042059464,
            "MacroF1": 0.799072028035076,
            "Memory in Mb": 5.784454345703125,
            "Time in s": 1114.0085680000002
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8007017543859649,
            "MicroF1": 0.8007017543859649,
            "MacroF1": 0.799801266098334,
            "Memory in Mb": 5.781437873840332,
            "Time in s": 1190.125915
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8042148198504419,
            "MicroF1": 0.8042148198504419,
            "MacroF1": 0.8016037490391381,
            "Memory in Mb": 5.805401802062988,
            "Time in s": 1268.322504
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8048780487804879,
            "MicroF1": 0.8048780487804877,
            "MacroF1": 0.8013581039030082,
            "Memory in Mb": 5.915700912475586,
            "Time in s": 1348.933518
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8048624440179143,
            "MicroF1": 0.8048624440179143,
            "MacroF1": 0.8017038254481382,
            "Memory in Mb": 6.069503784179688,
            "Time in s": 1431.999326
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8048477315102548,
            "MicroF1": 0.8048477315102549,
            "MacroF1": 0.8009666848419111,
            "Memory in Mb": 6.138180732727051,
            "Time in s": 1517.316045
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.804833836858006,
            "MicroF1": 0.804833836858006,
            "MacroF1": 0.8009346118743482,
            "Memory in Mb": 6.15428638458252,
            "Time in s": 1604.689641
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8048206937095826,
            "MicroF1": 0.8048206937095828,
            "MacroF1": 0.802987300619633,
            "Memory in Mb": 6.14796257019043,
            "Time in s": 1694.105126
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8065254722381225,
            "MicroF1": 0.8065254722381225,
            "MacroF1": 0.8041280306488863,
            "Memory in Mb": 6.185528755187988,
            "Time in s": 1785.64513
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8070273284997211,
            "MicroF1": 0.8070273284997211,
            "MacroF1": 0.8033862119520573,
            "Memory in Mb": 6.18717098236084,
            "Time in s": 1879.221363
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8085916258836324,
            "MicroF1": 0.8085916258836324,
            "MacroF1": 0.8051706679397826,
            "Memory in Mb": 6.228180885314941,
            "Time in s": 1974.88599
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8074270557029177,
            "MicroF1": 0.8074270557029178,
            "MacroF1": 0.8044133208197751,
            "Memory in Mb": 6.244633674621582,
            "Time in s": 2072.712055
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8073537027446919,
            "MicroF1": 0.8073537027446919,
            "MacroF1": 0.8036280810428232,
            "Memory in Mb": 6.232837677001953,
            "Time in s": 2172.610836
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.808295397066262,
            "MicroF1": 0.808295397066262,
            "MacroF1": 0.8041943782356388,
            "Memory in Mb": 6.225313186645508,
            "Time in s": 2274.502409
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8096885813148789,
            "MicroF1": 0.809688581314879,
            "MacroF1": 0.8043903689108628,
            "Memory in Mb": 6.209332466125488,
            "Time in s": 2378.336668
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8086031899468342,
            "MicroF1": 0.8086031899468342,
            "MacroF1": 0.8034099584264852,
            "Memory in Mb": 6.192641258239746,
            "Time in s": 2484.108554
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.808983451536643,
            "MicroF1": 0.808983451536643,
            "MacroF1": 0.8029929757635029,
            "Memory in Mb": 6.163993835449219,
            "Time in s": 2591.83622
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8093475242943082,
            "MicroF1": 0.8093475242943081,
            "MacroF1": 0.8028985652670257,
            "Memory in Mb": 6.160528182983398,
            "Time in s": 2701.493184
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8110557317625736,
            "MicroF1": 0.8110557317625736,
            "MacroF1": 0.8037088502350873,
            "Memory in Mb": 6.127141952514648,
            "Time in s": 2812.975729
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8078118064802485,
            "MicroF1": 0.8078118064802485,
            "MacroF1": 0.8004652010359966,
            "Memory in Mb": 6.094814300537109,
            "Time in s": 2926.384262
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8064375815571988,
            "MicroF1": 0.8064375815571988,
            "MacroF1": 0.7990276111502428,
            "Memory in Mb": 6.073050498962402,
            "Time in s": 3041.734776
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "ImageSegments",
            "Accuracy": 0.8064097011693374,
            "MicroF1": 0.8064097011693374,
            "MacroF1": 0.7989986920740723,
            "Memory in Mb": 6.073922157287598,
            "Time in s": 3157.943153
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6293838862559241,
            "MicroF1": 0.6293838862559241,
            "MacroF1": 0.5938169901557457,
            "Memory in Mb": 7.681754112243652,
            "Time in s": 78.197886
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6290857413548081,
            "MicroF1": 0.6290857413548081,
            "MacroF1": 0.5936238360694311,
            "Memory in Mb": 7.563845634460449,
            "Time in s": 217.436369
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.625197347647616,
            "MicroF1": 0.625197347647616,
            "MacroF1": 0.5890732389154221,
            "Memory in Mb": 7.54627799987793,
            "Time in s": 406.781755
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.624437603599337,
            "MicroF1": 0.624437603599337,
            "MacroF1": 0.5890978975177876,
            "Memory in Mb": 7.509035110473633,
            "Time in s": 643.136123
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6309907179390036,
            "MicroF1": 0.6309907179390036,
            "MacroF1": 0.5943307513870396,
            "Memory in Mb": 7.529419898986816,
            "Time in s": 922.055301
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6249408050513023,
            "MicroF1": 0.6249408050513023,
            "MacroF1": 0.5899587518293812,
            "Memory in Mb": 7.541637420654297,
            "Time in s": 1240.879558
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6242727641726424,
            "MicroF1": 0.6242727641726424,
            "MacroF1": 0.589208790087756,
            "Memory in Mb": 7.519943237304687,
            "Time in s": 1598.2590730000002
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6266129986977625,
            "MicroF1": 0.6266129986977625,
            "MacroF1": 0.5910042020201396,
            "Memory in Mb": 7.600367546081543,
            "Time in s": 1990.9287910000005
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6255919183415763,
            "MicroF1": 0.6255919183415763,
            "MacroF1": 0.5892477749449755,
            "Memory in Mb": 7.551809310913086,
            "Time in s": 2416.671036
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6269533099725353,
            "MicroF1": 0.6269533099725353,
            "MacroF1": 0.5906555376897765,
            "Memory in Mb": 7.57810115814209,
            "Time in s": 2875.240995
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6254842875591907,
            "MicroF1": 0.6254842875591907,
            "MacroF1": 0.5899069142128334,
            "Memory in Mb": 7.574300765991211,
            "Time in s": 3366.8452850000003
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6276536974193039,
            "MicroF1": 0.6276536974193039,
            "MacroF1": 0.5948280902959312,
            "Memory in Mb": 7.593076705932617,
            "Time in s": 3891.533291
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6419465287389816,
            "MicroF1": 0.6419465287389816,
            "MacroF1": 0.6240594787506325,
            "Memory in Mb": 7.568525314331055,
            "Time in s": 4449.097087
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6349861327200162,
            "MicroF1": 0.6349861327200162,
            "MacroF1": 0.6168664949740267,
            "Memory in Mb": 7.497129440307617,
            "Time in s": 5038.3500540000005
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6042048109097796,
            "MicroF1": 0.6042048109097796,
            "MacroF1": 0.5876183517420878,
            "Memory in Mb": 7.622871398925781,
            "Time in s": 5663.9066330000005
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5831311038768866,
            "MicroF1": 0.5831311038768866,
            "MacroF1": 0.5677288238088704,
            "Memory in Mb": 7.5406084060668945,
            "Time in s": 6323.428796
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5683805916104953,
            "MicroF1": 0.5683805916104953,
            "MacroF1": 0.5530005563922373,
            "Memory in Mb": 7.511743545532227,
            "Time in s": 7015.247243
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5655811016993739,
            "MicroF1": 0.5655811016993739,
            "MacroF1": 0.5465928919365096,
            "Memory in Mb": 7.569133758544922,
            "Time in s": 7739.601247
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5718985196630614,
            "MicroF1": 0.5718985196630614,
            "MacroF1": 0.5506497035356593,
            "Memory in Mb": 8.179316520690918,
            "Time in s": 8496.204598999999
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5817510298783086,
            "MicroF1": 0.5817510298783086,
            "MacroF1": 0.55937505855693,
            "Memory in Mb": 8.13927173614502,
            "Time in s": 9285.092110999998
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.5905298759864712,
            "MicroF1": 0.5905298759864712,
            "MacroF1": 0.5668099949242361,
            "Memory in Mb": 8.13715648651123,
            "Time in s": 10104.551326
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6004907236020834,
            "MicroF1": 0.6004907236020834,
            "MacroF1": 0.5756153967719769,
            "Memory in Mb": 8.254791259765625,
            "Time in s": 10955.282648
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6088854119487792,
            "MicroF1": 0.6088854119487792,
            "MacroF1": 0.5822871692574689,
            "Memory in Mb": 8.217899322509766,
            "Time in s": 11836.441737999998
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.617014560233595,
            "MicroF1": 0.617014560233595,
            "MacroF1": 0.5890646667396601,
            "Memory in Mb": 8.13050651550293,
            "Time in s": 12747.590801999995
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6237357475661957,
            "MicroF1": 0.6237357475661957,
            "MacroF1": 0.5942060376379845,
            "Memory in Mb": 8.178851127624512,
            "Time in s": 13688.250944999996
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6299763248952832,
            "MicroF1": 0.6299763248952832,
            "MacroF1": 0.5983574644866619,
            "Memory in Mb": 8.215079307556152,
            "Time in s": 14661.447404999995
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6312651257409421,
            "MicroF1": 0.6312651257409421,
            "MacroF1": 0.6016879522351425,
            "Memory in Mb": 8.160200119018555,
            "Time in s": 15669.084531999995
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6310751851726587,
            "MicroF1": 0.6310751851726587,
            "MacroF1": 0.6062390002054064,
            "Memory in Mb": 8.153844833374023,
            "Time in s": 16709.899933999994
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6313228619011854,
            "MicroF1": 0.6313228619011854,
            "MacroF1": 0.610710416812842,
            "Memory in Mb": 8.221953392028809,
            "Time in s": 17785.196262999994
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6320590927743931,
            "MicroF1": 0.6320590927743931,
            "MacroF1": 0.614817700164209,
            "Memory in Mb": 8.237210273742676,
            "Time in s": 18894.010558999995
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6331144035436077,
            "MicroF1": 0.6331144035436077,
            "MacroF1": 0.6184679282473909,
            "Memory in Mb": 8.208189964294434,
            "Time in s": 20033.816622999995
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6291616110798733,
            "MicroF1": 0.6291616110798733,
            "MacroF1": 0.6151628967287334,
            "Memory in Mb": 8.149331092834473,
            "Time in s": 21206.789184999998
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6245587855482538,
            "MicroF1": 0.6245587855482538,
            "MacroF1": 0.6103108800280445,
            "Memory in Mb": 8.270771980285645,
            "Time in s": 22409.569843999994
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6211737180736986,
            "MicroF1": 0.6211737180736986,
            "MacroF1": 0.6063163580543118,
            "Memory in Mb": 8.246885299682617,
            "Time in s": 23639.112909
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6171433209772992,
            "MicroF1": 0.6171433209772992,
            "MacroF1": 0.6018416894357856,
            "Memory in Mb": 8.222872734069824,
            "Time in s": 24895.212451
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6153360515585953,
            "MicroF1": 0.6153360515585953,
            "MacroF1": 0.5996210858832133,
            "Memory in Mb": 8.711487770080566,
            "Time in s": 26177.407049999994
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.613472908295155,
            "MicroF1": 0.613472908295155,
            "MacroF1": 0.5980758777202522,
            "Memory in Mb": 8.84398365020752,
            "Time in s": 27486.887242999997
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6139008647544048,
            "MicroF1": 0.6139008647544048,
            "MacroF1": 0.5993833357378361,
            "Memory in Mb": 9.00393295288086,
            "Time in s": 28821.579146999997
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6157395041643396,
            "MicroF1": 0.6157395041643396,
            "MacroF1": 0.6018873090815099,
            "Memory in Mb": 8.895415306091309,
            "Time in s": 30174.675792999995
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6179833802883591,
            "MicroF1": 0.6179833802883591,
            "MacroF1": 0.6047393094362844,
            "Memory in Mb": 8.820836067199707,
            "Time in s": 31551.592344999997
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6202101859337106,
            "MicroF1": 0.6202101859337106,
            "MacroF1": 0.60743097275183,
            "Memory in Mb": 8.80302619934082,
            "Time in s": 32950.21258099999
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6221054767648982,
            "MicroF1": 0.6221054767648982,
            "MacroF1": 0.6097047537791253,
            "Memory in Mb": 8.807188034057617,
            "Time in s": 34370.71930599999
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.623736428304006,
            "MicroF1": 0.623736428304006,
            "MacroF1": 0.6112415003179203,
            "Memory in Mb": 8.906554222106934,
            "Time in s": 35814.22252799999
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6259389191399608,
            "MicroF1": 0.6259389191399608,
            "MacroF1": 0.6133867892257391,
            "Memory in Mb": 8.822076797485352,
            "Time in s": 37279.498287
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6274542814453166,
            "MicroF1": 0.6274542814453166,
            "MacroF1": 0.6153714367024555,
            "Memory in Mb": 8.875716209411621,
            "Time in s": 38770.246246
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6317858980957283,
            "MicroF1": 0.6317858980957283,
            "MacroF1": 0.6202967225132047,
            "Memory in Mb": 8.86828327178955,
            "Time in s": 40284.403256
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6360137817090125,
            "MicroF1": 0.6360137817090125,
            "MacroF1": 0.6247992459885968,
            "Memory in Mb": 8.835649490356445,
            "Time in s": 41820.805008
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6403811628228145,
            "MicroF1": 0.6403811628228145,
            "MacroF1": 0.6293790828873279,
            "Memory in Mb": 8.924153327941895,
            "Time in s": 43378.957976
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6455559206076185,
            "MicroF1": 0.6455559206076185,
            "MacroF1": 0.6346828420183047,
            "Memory in Mb": 9.21804904937744,
            "Time in s": 44959.107881
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.648269853595712,
            "MicroF1": 0.648269853595712,
            "MacroF1": 0.6377385869395499,
            "Memory in Mb": 9.400546073913574,
            "Time in s": 46560.782
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Insects",
            "Accuracy": 0.6485325562472799,
            "MicroF1": 0.6485325562472799,
            "MacroF1": 0.637999701607352,
            "Memory in Mb": 9.406517028808594,
            "Time in s": 48163.738895
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9828009828009828,
            "MicroF1": 0.9828009828009828,
            "MacroF1": 0.6067632850241546,
            "Memory in Mb": 1.4587059020996094,
            "Time in s": 10.139614
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9496932515337424,
            "MicroF1": 0.9496932515337424,
            "MacroF1": 0.7435135353411919,
            "Memory in Mb": 6.019382476806641,
            "Time in s": 66.737739
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9149632052330336,
            "MicroF1": 0.9149632052330336,
            "MacroF1": 0.9012024099743488,
            "Memory in Mb": 7.076447486877441,
            "Time in s": 151.07716299999998
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9258123850398527,
            "MicroF1": 0.9258123850398527,
            "MacroF1": 0.913338738884437,
            "Memory in Mb": 7.232892990112305,
            "Time in s": 261.540164
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9230014713094654,
            "MicroF1": 0.9230014713094654,
            "MacroF1": 0.9086113906821328,
            "Memory in Mb": 7.553393363952637,
            "Time in s": 397.836215
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8961994278708623,
            "MicroF1": 0.8961994278708623,
            "MacroF1": 0.8992132713257572,
            "Memory in Mb": 7.640434265136719,
            "Time in s": 558.733108
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.9001751313485113,
            "MicroF1": 0.9001751313485113,
            "MacroF1": 0.8860451027148403,
            "Memory in Mb": 7.9326982498168945,
            "Time in s": 743.600486
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8924302788844621,
            "MicroF1": 0.8924302788844621,
            "MacroF1": 0.8761196773917237,
            "Memory in Mb": 8.074724197387695,
            "Time in s": 952.077233
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8874965949332607,
            "MicroF1": 0.8874965949332607,
            "MacroF1": 0.8846937712308092,
            "Memory in Mb": 8.20841121673584,
            "Time in s": 1184.393658
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8815886246629075,
            "MicroF1": 0.8815886246629075,
            "MacroF1": 0.868452721773406,
            "Memory in Mb": 8.525882720947266,
            "Time in s": 1441.208937
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8760864720303098,
            "MicroF1": 0.8760864720303098,
            "MacroF1": 0.8834419600614621,
            "Memory in Mb": 8.681946754455566,
            "Time in s": 1719.7568239999998
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8737487231869254,
            "MicroF1": 0.8737487231869254,
            "MacroF1": 0.8797220914000274,
            "Memory in Mb": 8.834684371948242,
            "Time in s": 2018.974207
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8693192532528757,
            "MicroF1": 0.8693192532528757,
            "MacroF1": 0.8538682361373632,
            "Memory in Mb": 9.067034721374512,
            "Time in s": 2339.699668
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8607949571003327,
            "MicroF1": 0.8607949571003327,
            "MacroF1": 0.8654889627515672,
            "Memory in Mb": 9.271133422851562,
            "Time in s": 2680.904224
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8561856512502043,
            "MicroF1": 0.8561856512502043,
            "MacroF1": 0.84095068957581,
            "Memory in Mb": 9.378315925598145,
            "Time in s": 3042.663698
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8434196414891987,
            "MicroF1": 0.8434196414891987,
            "MacroF1": 0.8427350578509161,
            "Memory in Mb": 9.608606338500977,
            "Time in s": 3424.478417
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8392213410237923,
            "MicroF1": 0.8392213410237923,
            "MacroF1": 0.8447429510460126,
            "Memory in Mb": 9.751982688903809,
            "Time in s": 3824.86879
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8454310227427482,
            "MicroF1": 0.8454310227427482,
            "MacroF1": 0.847842289102327,
            "Memory in Mb": 9.957889556884766,
            "Time in s": 4243.00141
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8456973293768546,
            "MicroF1": 0.8456973293768547,
            "MacroF1": 0.8480563212460421,
            "Memory in Mb": 10.19985294342041,
            "Time in s": 4680.993142
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8469175144012747,
            "MicroF1": 0.8469175144012746,
            "MacroF1": 0.8472851046009279,
            "Memory in Mb": 10.418806076049805,
            "Time in s": 5138.9878340000005
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8469709349830746,
            "MicroF1": 0.8469709349830746,
            "MacroF1": 0.8501227536717817,
            "Memory in Mb": 10.607142448425291,
            "Time in s": 5616.664707000001
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8475766016713092,
            "MicroF1": 0.8475766016713092,
            "MacroF1": 0.8507851780426926,
            "Memory in Mb": 10.772598266601562,
            "Time in s": 6113.940894000001
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8459980816370031,
            "MicroF1": 0.8459980816370031,
            "MacroF1": 0.8471668648040658,
            "Memory in Mb": 10.97368335723877,
            "Time in s": 6631.342845000001
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8418956184250843,
            "MicroF1": 0.8418956184250843,
            "MacroF1": 0.8426049398612477,
            "Memory in Mb": 11.192140579223633,
            "Time in s": 7169.901201000001
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8344935778017453,
            "MicroF1": 0.8344935778017454,
            "MacroF1": 0.8308153568434791,
            "Memory in Mb": 11.354521751403809,
            "Time in s": 7729.92345
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.817384745922504,
            "MicroF1": 0.817384745922504,
            "MacroF1": 0.8105787344487394,
            "Memory in Mb": 11.59365177154541,
            "Time in s": 8312.440227000001
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8127099409895597,
            "MicroF1": 0.8127099409895597,
            "MacroF1": 0.8142119266109252,
            "Memory in Mb": 11.793928146362305,
            "Time in s": 8918.030696000002
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8079313665411888,
            "MicroF1": 0.8079313665411888,
            "MacroF1": 0.8037472320719128,
            "Memory in Mb": 11.945178031921388,
            "Time in s": 9547.170938
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8040740427689967,
            "MicroF1": 0.8040740427689967,
            "MacroF1": 0.8039730126613296,
            "Memory in Mb": 12.203582763671877,
            "Time in s": 10200.281645
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8072554947299616,
            "MicroF1": 0.8072554947299616,
            "MacroF1": 0.8097160881214022,
            "Memory in Mb": 12.414502143859863,
            "Time in s": 10877.318664
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8043014153554202,
            "MicroF1": 0.8043014153554202,
            "MacroF1": 0.8038043720799647,
            "Memory in Mb": 12.561456680297852,
            "Time in s": 11578.515438
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7996936039831483,
            "MicroF1": 0.7996936039831483,
            "MacroF1": 0.8010057260657798,
            "Memory in Mb": 12.889472007751465,
            "Time in s": 12304.325005
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7974448488449826,
            "MicroF1": 0.7974448488449826,
            "MacroF1": 0.7996515087686575,
            "Memory in Mb": 12.99599838256836,
            "Time in s": 13054.609905
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7978516329031793,
            "MicroF1": 0.7978516329031793,
            "MacroF1": 0.8006715750629478,
            "Memory in Mb": 13.20394229888916,
            "Time in s": 13829.291085
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.797674907206387,
            "MicroF1": 0.7976749072063871,
            "MacroF1": 0.8002875748518964,
            "Memory in Mb": 13.36452293395996,
            "Time in s": 14628.347686
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8007761966364813,
            "MicroF1": 0.8007761966364813,
            "MacroF1": 0.8043248634763072,
            "Memory in Mb": 13.53370189666748,
            "Time in s": 15451.756014
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8051010268300762,
            "MicroF1": 0.8051010268300763,
            "MacroF1": 0.8085780284871096,
            "Memory in Mb": 13.774932861328123,
            "Time in s": 16299.960754
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.8052634973876024,
            "MicroF1": 0.8052634973876024,
            "MacroF1": 0.8077470357827514,
            "Memory in Mb": 13.933537483215332,
            "Time in s": 17172.988913
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7978756834894098,
            "MicroF1": 0.7978756834894098,
            "MacroF1": 0.7983136026998061,
            "Memory in Mb": 14.138628005981444,
            "Time in s": 18070.675966000003
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.793369691770329,
            "MicroF1": 0.7933696917703291,
            "MacroF1": 0.7956625263629296,
            "Memory in Mb": 14.30509090423584,
            "Time in s": 18993.33345
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7901596221677527,
            "MicroF1": 0.7901596221677527,
            "MacroF1": 0.7932579365729884,
            "Memory in Mb": 14.447582244873049,
            "Time in s": 19941.842904
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7861686606361249,
            "MicroF1": 0.7861686606361248,
            "MacroF1": 0.7888822346867281,
            "Memory in Mb": 14.767212867736816,
            "Time in s": 20916.572711
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.780425240836801,
            "MicroF1": 0.780425240836801,
            "MacroF1": 0.7838193866310822,
            "Memory in Mb": 14.989240646362305,
            "Time in s": 21922.215184
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7802907915993538,
            "MicroF1": 0.7802907915993537,
            "MacroF1": 0.7845235361146662,
            "Memory in Mb": 15.200251579284668,
            "Time in s": 22957.213951
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.783975162045863,
            "MicroF1": 0.783975162045863,
            "MacroF1": 0.7883700169311393,
            "Memory in Mb": 15.375930786132812,
            "Time in s": 24020.765336
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7869664837214259,
            "MicroF1": 0.7869664837214259,
            "MacroF1": 0.7913854757843782,
            "Memory in Mb": 15.5132417678833,
            "Time in s": 25114.453204
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7816427640156454,
            "MicroF1": 0.7816427640156454,
            "MacroF1": 0.7858184292134073,
            "Memory in Mb": 15.77665901184082,
            "Time in s": 26236.293864000003
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7846090997293571,
            "MicroF1": 0.7846090997293571,
            "MacroF1": 0.7893723685613512,
            "Memory in Mb": 15.996115684509276,
            "Time in s": 27388.205854000003
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7807013155920164,
            "MicroF1": 0.7807013155920164,
            "MacroF1": 0.785620728786203,
            "Memory in Mb": 16.12063980102539,
            "Time in s": 28569.915626
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "Voting",
            "dataset": "Keystroke",
            "Accuracy": 0.7791068189617139,
            "MicroF1": 0.7791068189617139,
            "MacroF1": 0.7841355172773921,
            "Memory in Mb": 16.39253330230713,
            "Time in s": 29779.243894000003
          },
          {
            "step": 46,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1777777777777777,
            "MicroF1": 0.1777777777777777,
            "MacroF1": 0.1526026604973973,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 0.110776
          },
          {
            "step": 92,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1318681318681318,
            "MicroF1": 0.1318681318681318,
            "MacroF1": 0.1213108980966124,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 0.225611
          },
          {
            "step": 138,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1240875912408759,
            "MicroF1": 0.1240875912408759,
            "MacroF1": 0.1187445506554449,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 0.343639
          },
          {
            "step": 184,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1256830601092896,
            "MicroF1": 0.1256830601092896,
            "MacroF1": 0.1226298342307158,
            "Memory in Mb": 0.0013647079467773,
            "Time in s": 0.484524
          },
          {
            "step": 230,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1266375545851528,
            "MicroF1": 0.1266375545851528,
            "MacroF1": 0.1250385204120806,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 0.6292090000000001
          },
          {
            "step": 276,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1272727272727272,
            "MicroF1": 0.1272727272727272,
            "MacroF1": 0.1242790791814499,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 0.7861950000000001
          },
          {
            "step": 322,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1339563862928348,
            "MicroF1": 0.1339563862928348,
            "MacroF1": 0.1321003659624602,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 1.0166240000000002
          },
          {
            "step": 368,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1389645776566757,
            "MicroF1": 0.1389645776566757,
            "MacroF1": 0.1374501146297296,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 1.2507780000000002
          },
          {
            "step": 414,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1404358353510895,
            "MicroF1": 0.1404358353510895,
            "MacroF1": 0.1403581309694754,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 1.5223060000000002
          },
          {
            "step": 460,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1459694989106753,
            "MicroF1": 0.1459694989106753,
            "MacroF1": 0.1456314871072794,
            "Memory in Mb": 0.0013656616210937,
            "Time in s": 1.7974560000000002
          },
          {
            "step": 506,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1386138613861386,
            "MicroF1": 0.1386138613861386,
            "MacroF1": 0.1383381610231494,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 2.07562
          },
          {
            "step": 552,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1397459165154265,
            "MicroF1": 0.1397459165154265,
            "MacroF1": 0.1393865249177789,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 2.402759
          },
          {
            "step": 598,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1373534338358459,
            "MicroF1": 0.1373534338358459,
            "MacroF1": 0.1372798104345861,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 2.771723
          },
          {
            "step": 644,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1399688958009331,
            "MicroF1": 0.1399688958009331,
            "MacroF1": 0.1401757170901796,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 3.149556
          },
          {
            "step": 690,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1378809869375907,
            "MicroF1": 0.1378809869375907,
            "MacroF1": 0.1380151778455332,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 3.580436
          },
          {
            "step": 736,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1401360544217687,
            "MicroF1": 0.1401360544217687,
            "MacroF1": 0.1403108892795828,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 4.0152470000000005
          },
          {
            "step": 782,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1421254801536491,
            "MicroF1": 0.1421254801536491,
            "MacroF1": 0.1420930265541123,
            "Memory in Mb": 0.0013647079467773,
            "Time in s": 4.453992
          },
          {
            "step": 828,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1426844014510278,
            "MicroF1": 0.1426844014510278,
            "MacroF1": 0.1422987455304691,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 4.959761
          },
          {
            "step": 874,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.138602520045819,
            "MicroF1": 0.138602520045819,
            "MacroF1": 0.1384535269459527,
            "Memory in Mb": 0.0013647079467773,
            "Time in s": 5.469480000000001
          },
          {
            "step": 920,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1349292709466811,
            "MicroF1": 0.1349292709466811,
            "MacroF1": 0.1348083913046733,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 6.0005820000000005
          },
          {
            "step": 966,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1336787564766839,
            "MicroF1": 0.1336787564766839,
            "MacroF1": 0.1334917777444527,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 6.535053
          },
          {
            "step": 1012,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1325420375865479,
            "MicroF1": 0.1325420375865479,
            "MacroF1": 0.1324936677659038,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 7.07275
          },
          {
            "step": 1058,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1333964049195837,
            "MicroF1": 0.1333964049195837,
            "MacroF1": 0.1331834965440007,
            "Memory in Mb": 0.0013656616210937,
            "Time in s": 7.645426
          },
          {
            "step": 1104,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1341795104261106,
            "MicroF1": 0.1341795104261106,
            "MacroF1": 0.1340282652950153,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 8.221471000000001
          },
          {
            "step": 1150,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.134029590948651,
            "MicroF1": 0.134029590948651,
            "MacroF1": 0.1340639115051912,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 8.800858000000002
          },
          {
            "step": 1196,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1364016736401673,
            "MicroF1": 0.1364016736401673,
            "MacroF1": 0.1363948420172951,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 9.430169
          },
          {
            "step": 1242,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1394037066881547,
            "MicroF1": 0.1394037066881547,
            "MacroF1": 0.1391977238389222,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 10.062783
          },
          {
            "step": 1288,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1414141414141414,
            "MicroF1": 0.1414141414141414,
            "MacroF1": 0.1411871502321015,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 10.698372
          },
          {
            "step": 1334,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1432858214553638,
            "MicroF1": 0.1432858214553638,
            "MacroF1": 0.1430255327815666,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 11.387531
          },
          {
            "step": 1380,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1435823060188542,
            "MicroF1": 0.1435823060188542,
            "MacroF1": 0.1433209000486506,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 12.080639
          },
          {
            "step": 1426,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1417543859649122,
            "MicroF1": 0.1417543859649122,
            "MacroF1": 0.1414546655929112,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 12.777602000000002
          },
          {
            "step": 1472,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1393609789259007,
            "MicroF1": 0.1393609789259007,
            "MacroF1": 0.1390762971394262,
            "Memory in Mb": 0.0013647079467773,
            "Time in s": 13.546128
          },
          {
            "step": 1518,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1397495056031641,
            "MicroF1": 0.1397495056031641,
            "MacroF1": 0.1395136668589845,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 14.318195
          },
          {
            "step": 1564,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1369161868202175,
            "MicroF1": 0.1369161868202175,
            "MacroF1": 0.1366417047439511,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 15.093811
          },
          {
            "step": 1610,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1361093847110006,
            "MicroF1": 0.1361093847110006,
            "MacroF1": 0.1359768388190307,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 15.942934
          },
          {
            "step": 1656,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1365558912386707,
            "MicroF1": 0.1365558912386707,
            "MacroF1": 0.1363322462377459,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 16.795246000000002
          },
          {
            "step": 1702,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1393298059964726,
            "MicroF1": 0.1393298059964726,
            "MacroF1": 0.1390129627439909,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 17.650687
          },
          {
            "step": 1748,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1419576416714367,
            "MicroF1": 0.1419576416714367,
            "MacroF1": 0.1414719731272364,
            "Memory in Mb": 0.0013656616210937,
            "Time in s": 18.510738
          },
          {
            "step": 1794,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1422197434467373,
            "MicroF1": 0.1422197434467373,
            "MacroF1": 0.1419410396611007,
            "Memory in Mb": 0.0013647079467773,
            "Time in s": 19.374685
          },
          {
            "step": 1840,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1413811854268624,
            "MicroF1": 0.1413811854268624,
            "MacroF1": 0.1411432976659866,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 20.24245
          },
          {
            "step": 1886,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.140053050397878,
            "MicroF1": 0.140053050397878,
            "MacroF1": 0.1397325871382075,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 21.182873
          },
          {
            "step": 1932,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1429311237700673,
            "MicroF1": 0.1429311237700673,
            "MacroF1": 0.1427522922982585,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 22.12686
          },
          {
            "step": 1978,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1461810824481537,
            "MicroF1": 0.1461810824481537,
            "MacroF1": 0.1459715815160596,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 23.074113
          },
          {
            "step": 2024,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1443400889767671,
            "MicroF1": 0.1443400889767671,
            "MacroF1": 0.1441662523776106,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 24.067371
          },
          {
            "step": 2070,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1440309328177863,
            "MicroF1": 0.1440309328177863,
            "MacroF1": 0.1438554349712762,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 25.063921
          },
          {
            "step": 2116,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1446808510638297,
            "MicroF1": 0.1446808510638297,
            "MacroF1": 0.1446036231777657,
            "Memory in Mb": 0.0013637542724609,
            "Time in s": 26.06363
          },
          {
            "step": 2162,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1453031004164738,
            "MicroF1": 0.1453031004164738,
            "MacroF1": 0.1452046591382179,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 27.083891999999995
          },
          {
            "step": 2208,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1449932034435885,
            "MicroF1": 0.1449932034435885,
            "MacroF1": 0.1449110985199169,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 28.107944
          },
          {
            "step": 2254,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1464713715046604,
            "MicroF1": 0.1464713715046604,
            "MacroF1": 0.146404255341296,
            "Memory in Mb": 0.0013666152954101,
            "Time in s": 29.207951
          },
          {
            "step": 2300,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.1478903871248368,
            "MicroF1": 0.1478903871248368,
            "MacroF1": 0.1478868852481029,
            "Memory in Mb": 0.0013675689697265,
            "Time in s": 30.311507
          },
          {
            "step": 2310,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "ImageSegments",
            "Accuracy": 0.148116067561715,
            "MicroF1": 0.148116067561715,
            "MacroF1": 0.1481156678425267,
            "Memory in Mb": 0.0013694763183593,
            "Time in s": 31.415921
          },
          {
            "step": 1056,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1582938388625592,
            "MicroF1": 0.1582938388625592,
            "MacroF1": 0.1376212379233521,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 0.57267
          },
          {
            "step": 2112,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1657981999052581,
            "MicroF1": 0.1657981999052581,
            "MacroF1": 0.1511045106411843,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 1.690872
          },
          {
            "step": 3168,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1701926113040732,
            "MicroF1": 0.1701926113040732,
            "MacroF1": 0.1568151235503963,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 3.298143
          },
          {
            "step": 4224,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1659957376272791,
            "MicroF1": 0.1659957376272791,
            "MacroF1": 0.1525443315605066,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 5.473684
          },
          {
            "step": 5280,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1708656942602765,
            "MicroF1": 0.1708656942602765,
            "MacroF1": 0.1567667911399358,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 8.202311
          },
          {
            "step": 6336,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1737963693764798,
            "MicroF1": 0.1737963693764798,
            "MacroF1": 0.1613756819597299,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 11.448991
          },
          {
            "step": 7392,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1752130970098769,
            "MicroF1": 0.1752130970098769,
            "MacroF1": 0.1618940790413477,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 15.242684
          },
          {
            "step": 8448,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1772226826092103,
            "MicroF1": 0.1772226826092103,
            "MacroF1": 0.163740045170864,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 19.537217
          },
          {
            "step": 9504,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1773124276544249,
            "MicroF1": 0.1773124276544249,
            "MacroF1": 0.1637492974453096,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 24.318802
          },
          {
            "step": 10560,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1790889288758405,
            "MicroF1": 0.1790889288758405,
            "MacroF1": 0.1656421076747495,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 29.683683
          },
          {
            "step": 11616,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1789926818768833,
            "MicroF1": 0.1789926818768833,
            "MacroF1": 0.1655925383533761,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 35.598037000000005
          },
          {
            "step": 12672,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.1853050272275274,
            "MicroF1": 0.1853050272275274,
            "MacroF1": 0.182698099884098,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 41.981502000000006
          },
          {
            "step": 13728,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2479784366576819,
            "MicroF1": 0.2479784366576819,
            "MacroF1": 0.266039368455288,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 48.94863000000001
          },
          {
            "step": 14784,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2795778935263478,
            "MicroF1": 0.2795778935263478,
            "MacroF1": 0.2822974275171512,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 56.43945000000001
          },
          {
            "step": 15840,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2761537975882315,
            "MicroF1": 0.2761537975882315,
            "MacroF1": 0.2847375853365436,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 64.48233200000001
          },
          {
            "step": 16896,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2723290914471737,
            "MicroF1": 0.2723290914471737,
            "MacroF1": 0.2859139704285301,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 73.03679300000002
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2720739791655061,
            "MicroF1": 0.2720739791655061,
            "MacroF1": 0.2880143206503878,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 82.10379000000002
          },
          {
            "step": 19008,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2825274898721523,
            "MicroF1": 0.2825274898721523,
            "MacroF1": 0.2877504429321087,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 91.70347300000002
          },
          {
            "step": 20064,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2872451776902756,
            "MicroF1": 0.2872451776902756,
            "MacroF1": 0.2866739236661926,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 101.81113500000002
          },
          {
            "step": 21120,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2830626450116009,
            "MicroF1": 0.2830626450116009,
            "MacroF1": 0.2816476602425525,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 112.42818900000002
          },
          {
            "step": 22176,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2805411499436302,
            "MicroF1": 0.2805411499436302,
            "MacroF1": 0.2786296072528009,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 123.55266000000002
          },
          {
            "step": 23232,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2797124531875511,
            "MicroF1": 0.2797124531875511,
            "MacroF1": 0.2771941975793341,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 135.22034100000002
          },
          {
            "step": 24288,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2777205912628155,
            "MicroF1": 0.2777205912628155,
            "MacroF1": 0.2745878480946635,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 147.32084400000002
          },
          {
            "step": 25344,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2756579726157124,
            "MicroF1": 0.2756579726157124,
            "MacroF1": 0.2723380305202896,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 159.88729300000003
          },
          {
            "step": 26400,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2739497708246524,
            "MicroF1": 0.2739497708246524,
            "MacroF1": 0.2699690442569991,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 172.95537600000003
          },
          {
            "step": 27456,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2718994718630486,
            "MicroF1": 0.2718994718630486,
            "MacroF1": 0.2671948532388624,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 186.52082400000003
          },
          {
            "step": 28512,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2723860965942969,
            "MicroF1": 0.2723860965942969,
            "MacroF1": 0.2686965366571337,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 200.59564800000004
          },
          {
            "step": 29568,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2738187844556431,
            "MicroF1": 0.2738187844556431,
            "MacroF1": 0.2720266804437783,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 215.16150500000003
          },
          {
            "step": 30624,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2753812493877151,
            "MicroF1": 0.2753812493877151,
            "MacroF1": 0.2748698663810351,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 230.19075300000003
          },
          {
            "step": 31680,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2780390795163989,
            "MicroF1": 0.2780390795163989,
            "MacroF1": 0.2784141751235631,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 245.71900300000004
          },
          {
            "step": 32736,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.279670077898274,
            "MicroF1": 0.279670077898274,
            "MacroF1": 0.2802192251245275,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 261.76959600000004
          },
          {
            "step": 33792,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2808440117190968,
            "MicroF1": 0.2808440117190968,
            "MacroF1": 0.2811962745371706,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 278.22772000000003
          },
          {
            "step": 34848,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2772405085086234,
            "MicroF1": 0.2772405085086234,
            "MacroF1": 0.2781905182864757,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 295.19763900000004
          },
          {
            "step": 35904,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2739325404562293,
            "MicroF1": 0.2739325404562293,
            "MacroF1": 0.2754200456137155,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 312.64260700000005
          },
          {
            "step": 36960,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.271246516410076,
            "MicroF1": 0.271246516410076,
            "MacroF1": 0.273332837678202,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 330.5037730000001
          },
          {
            "step": 38016,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2685518874128633,
            "MicroF1": 0.2685518874128633,
            "MacroF1": 0.2710722002891223,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 348.8496650000001
          },
          {
            "step": 39072,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.277034117376059,
            "MicroF1": 0.277034117376059,
            "MacroF1": 0.2770619820799866,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 367.6207990000001
          },
          {
            "step": 40128,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2761731502479627,
            "MicroF1": 0.2761731502479627,
            "MacroF1": 0.2760769006623072,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 386.8573710000001
          },
          {
            "step": 41184,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2756720005827647,
            "MicroF1": 0.2756720005827647,
            "MacroF1": 0.2754352632972116,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 406.52795400000014
          },
          {
            "step": 42240,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2740121688486943,
            "MicroF1": 0.2740121688486943,
            "MacroF1": 0.2735946193588542,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 426.69962200000015
          },
          {
            "step": 43296,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2738422450629403,
            "MicroF1": 0.2738422450629403,
            "MacroF1": 0.2731948869083578,
            "Memory in Mb": 0.0013856887817382,
            "Time in s": 447.37129900000014
          },
          {
            "step": 44352,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2729588960790061,
            "MicroF1": 0.2729588960790061,
            "MacroF1": 0.2720911653869048,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 468.49129600000015
          },
          {
            "step": 45408,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2720505648908758,
            "MicroF1": 0.2720505648908758,
            "MacroF1": 0.2708084959373003,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 490.06234300000017
          },
          {
            "step": 46464,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.271377224888621,
            "MicroF1": 0.271377224888621,
            "MacroF1": 0.2698631410415437,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 512.0778290000002
          },
          {
            "step": 47520,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2723542162082535,
            "MicroF1": 0.2723542162082535,
            "MacroF1": 0.2717062798322285,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 534.5781510000002
          },
          {
            "step": 48576,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2741327843540916,
            "MicroF1": 0.2741327843540916,
            "MacroF1": 0.2744946340974243,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 557.5265480000002
          },
          {
            "step": 49632,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2753520984868328,
            "MicroF1": 0.2753520984868328,
            "MacroF1": 0.2765036876430403,
            "Memory in Mb": 0.0013818740844726,
            "Time in s": 580.9705880000001
          },
          {
            "step": 50688,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2768362696549411,
            "MicroF1": 0.2768362696549411,
            "MacroF1": 0.2786344091273496,
            "Memory in Mb": 0.0013837814331054,
            "Time in s": 604.9012140000001
          },
          {
            "step": 51744,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2782791875229499,
            "MicroF1": 0.2782791875229499,
            "MacroF1": 0.2805971515128955,
            "Memory in Mb": 0.0013885498046875,
            "Time in s": 629.3033230000001
          },
          {
            "step": 52800,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2891153241538665,
            "MicroF1": 0.2891153241538665,
            "MacroF1": 0.2892953202729756,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 654.1512880000001
          },
          {
            "step": 52848,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Insects",
            "Accuracy": 0.2897610081934642,
            "MicroF1": 0.2897610081934642,
            "MacroF1": 0.2897627257031321,
            "Memory in Mb": 0.0013866424560546,
            "Time in s": 679.0036960000001
          },
          {
            "step": 408,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975429975429976,
            "MicroF1": 0.9975429975429976,
            "MacroF1": 0.966040884438882,
            "Memory in Mb": 0.0006122589111328,
            "Time in s": 0.255536
          },
          {
            "step": 816,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975460122699388,
            "MicroF1": 0.9975460122699388,
            "MacroF1": 0.9879967903427672,
            "Memory in Mb": 0.0006628036499023,
            "Time in s": 0.794196
          },
          {
            "step": 1224,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975470155355682,
            "MicroF1": 0.9975470155355682,
            "MacroF1": 0.9931179599499376,
            "Memory in Mb": 0.0007133483886718,
            "Time in s": 1.53447
          },
          {
            "step": 1632,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975475168608215,
            "MicroF1": 0.9975475168608215,
            "MacroF1": 0.9950750839342832,
            "Memory in Mb": 0.0012521743774414,
            "Time in s": 2.469131
          },
          {
            "step": 2040,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975478175576264,
            "MicroF1": 0.9975478175576264,
            "MacroF1": 0.9960150346160552,
            "Memory in Mb": 0.0013027191162109,
            "Time in s": 3.675833
          },
          {
            "step": 2448,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975480179812016,
            "MicroF1": 0.9975480179812016,
            "MacroF1": 0.9965317313935652,
            "Memory in Mb": 0.0013532638549804,
            "Time in s": 5.030286
          },
          {
            "step": 2856,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975481611208408,
            "MicroF1": 0.9975481611208408,
            "MacroF1": 0.996842428316928,
            "Memory in Mb": 0.00140380859375,
            "Time in s": 6.586031
          },
          {
            "step": 3264,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975482684646032,
            "MicroF1": 0.9975482684646032,
            "MacroF1": 0.9970416021996,
            "Memory in Mb": 0.0014543533325195,
            "Time in s": 8.377109
          },
          {
            "step": 3672,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975483519476982,
            "MicroF1": 0.9975483519476982,
            "MacroF1": 0.9971755428551424,
            "Memory in Mb": 0.001504898071289,
            "Time in s": 10.331252
          },
          {
            "step": 4080,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975484187300808,
            "MicroF1": 0.9975484187300808,
            "MacroF1": 0.9972690115789392,
            "Memory in Mb": 0.0015554428100585,
            "Time in s": 12.525489
          },
          {
            "step": 4488,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975484733675062,
            "MicroF1": 0.9975484733675062,
            "MacroF1": 0.9973361791525124,
            "Memory in Mb": 0.0016059875488281,
            "Time in s": 14.940819
          },
          {
            "step": 4896,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975485188968336,
            "MicroF1": 0.9975485188968336,
            "MacroF1": 0.9973856025730918,
            "Memory in Mb": 0.0016565322875976,
            "Time in s": 17.495259
          },
          {
            "step": 5304,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548557420328,
            "MicroF1": 0.997548557420328,
            "MacroF1": 0.9974226798335742,
            "Memory in Mb": 0.0017070770263671,
            "Time in s": 20.336762
          },
          {
            "step": 5712,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975485904395028,
            "MicroF1": 0.9975485904395028,
            "MacroF1": 0.99745094204078,
            "Memory in Mb": 0.0017576217651367,
            "Time in s": 23.402208
          },
          {
            "step": 6120,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975486190554012,
            "MicroF1": 0.9975486190554012,
            "MacroF1": 0.9974727709453766,
            "Memory in Mb": 0.0018081665039062,
            "Time in s": 26.661861
          },
          {
            "step": 6528,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975486440937644,
            "MicroF1": 0.9975486440937644,
            "MacroF1": 0.997489815700999,
            "Memory in Mb": 0.0018587112426757,
            "Time in s": 30.164710000000003
          },
          {
            "step": 6936,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548666186013,
            "MicroF1": 0.997548666186013,
            "MacroF1": 0.9975032443691146,
            "Memory in Mb": 0.0019092559814453,
            "Time in s": 33.838397
          },
          {
            "step": 7344,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548685823233,
            "MicroF1": 0.997548685823233,
            "MacroF1": 0.9975139007887864,
            "Memory in Mb": 0.0034246444702148,
            "Time in s": 37.738436
          },
          {
            "step": 7752,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487033931104,
            "MicroF1": 0.9975487033931104,
            "MacroF1": 0.9975224052755716,
            "Memory in Mb": 0.0034751892089843,
            "Time in s": 41.800015
          },
          {
            "step": 8160,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548719205785,
            "MicroF1": 0.997548719205785,
            "MacroF1": 0.9975292209193424,
            "Memory in Mb": 0.0035257339477539,
            "Time in s": 46.105028
          },
          {
            "step": 8568,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487335123148,
            "MicroF1": 0.9975487335123148,
            "MacroF1": 0.9975346982235258,
            "Memory in Mb": 0.0035762786865234,
            "Time in s": 50.63279300000001
          },
          {
            "step": 8976,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548746518106,
            "MicroF1": 0.997548746518106,
            "MacroF1": 0.9975391057693664,
            "Memory in Mb": 0.0036268234252929,
            "Time in s": 55.447067
          },
          {
            "step": 9384,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548758392838,
            "MicroF1": 0.997548758392838,
            "MacroF1": 0.997542651662671,
            "Memory in Mb": 0.0036773681640625,
            "Time in s": 60.387128
          },
          {
            "step": 9792,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487692779084,
            "MicroF1": 0.9975487692779084,
            "MacroF1": 0.9975454987794796,
            "Memory in Mb": 0.003727912902832,
            "Time in s": 65.547582
          },
          {
            "step": 10200,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487792920874,
            "MicroF1": 0.9975487792920874,
            "MacroF1": 0.9975477757646256,
            "Memory in Mb": 0.0037784576416015,
            "Time in s": 70.981052
          },
          {
            "step": 10608,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487885358726,
            "MicroF1": 0.9975487885358726,
            "MacroF1": 0.9975495850737114,
            "Memory in Mb": 0.003829002380371,
            "Time in s": 76.594226
          },
          {
            "step": 11016,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975487970948708,
            "MicroF1": 0.9975487970948708,
            "MacroF1": 0.9975510089260562,
            "Memory in Mb": 0.0038795471191406,
            "Time in s": 82.44596800000001
          },
          {
            "step": 11424,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488050424582,
            "MicroF1": 0.9975488050424582,
            "MacroF1": 0.9975521137613484,
            "Memory in Mb": 0.0039300918579101,
            "Time in s": 88.533094
          },
          {
            "step": 11832,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.99754881244189,
            "MicroF1": 0.99754881244189,
            "MacroF1": 0.99755295361102,
            "Memory in Mb": 0.0039806365966796,
            "Time in s": 94.818744
          },
          {
            "step": 12240,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548819347986,
            "MicroF1": 0.997548819347986,
            "MacroF1": 0.9975535726732964,
            "Memory in Mb": 0.0040311813354492,
            "Time in s": 101.331754
          },
          {
            "step": 12648,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548825808492,
            "MicroF1": 0.997548825808492,
            "MacroF1": 0.997554007297632,
            "Memory in Mb": 0.0040817260742187,
            "Time in s": 108.051678
          },
          {
            "step": 13056,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488318651856,
            "MicroF1": 0.9975488318651856,
            "MacroF1": 0.997554287526727,
            "Memory in Mb": 0.0041322708129882,
            "Time in s": 114.996681
          },
          {
            "step": 13464,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488375547796,
            "MicroF1": 0.9975488375547796,
            "MacroF1": 0.9975544383040468,
            "Memory in Mb": 0.0041828155517578,
            "Time in s": 122.1119
          },
          {
            "step": 13872,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488429096676,
            "MicroF1": 0.9975488429096676,
            "MacroF1": 0.9975544804262362,
            "Memory in Mb": 0.0042333602905273,
            "Time in s": 129.47010500000002
          },
          {
            "step": 14280,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488479585404,
            "MicroF1": 0.9975488479585404,
            "MacroF1": 0.99755443129941,
            "Memory in Mb": 0.0042839050292968,
            "Time in s": 136.988051
          },
          {
            "step": 14688,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488527269012,
            "MicroF1": 0.9975488527269012,
            "MacroF1": 0.997554305543504,
            "Memory in Mb": 0.0043344497680664,
            "Time in s": 144.742896
          },
          {
            "step": 15096,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548857237496,
            "MicroF1": 0.997548857237496,
            "MacroF1": 0.9975541154780816,
            "Memory in Mb": 0.0043849945068359,
            "Time in s": 152.648866
          },
          {
            "step": 15504,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488615106752,
            "MicroF1": 0.9975488615106752,
            "MacroF1": 0.9975538715150368,
            "Memory in Mb": 0.0044355392456054,
            "Time in s": 160.767465
          },
          {
            "step": 15912,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488655647036,
            "MicroF1": 0.9975488655647036,
            "MacroF1": 0.997553582477696,
            "Memory in Mb": 0.004486083984375,
            "Time in s": 169.09858
          },
          {
            "step": 16320,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488694160182,
            "MicroF1": 0.9975488694160182,
            "MacroF1": 0.9975532558614028,
            "Memory in Mb": 0.0045366287231445,
            "Time in s": 177.653336
          },
          {
            "step": 16728,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488730794524,
            "MicroF1": 0.9975488730794524,
            "MacroF1": 0.997552898047314,
            "Memory in Mb": 0.004587173461914,
            "Time in s": 186.438203
          },
          {
            "step": 17136,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488765684272,
            "MicroF1": 0.9975488765684272,
            "MacroF1": 0.9975525144785748,
            "Memory in Mb": 0.0046377182006835,
            "Time in s": 195.447168
          },
          {
            "step": 17544,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488798951148,
            "MicroF1": 0.9975488798951148,
            "MacroF1": 0.997552109806108,
            "Memory in Mb": 0.0046882629394531,
            "Time in s": 204.563635
          },
          {
            "step": 17952,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.997548883070581,
            "MicroF1": 0.997548883070581,
            "MacroF1": 0.9975516880097278,
            "Memory in Mb": 0.0047388076782226,
            "Time in s": 213.933058
          },
          {
            "step": 18360,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488861049076,
            "MicroF1": 0.9975488861049076,
            "MacroF1": 0.997551252499137,
            "Memory in Mb": 0.0047893524169921,
            "Time in s": 223.513668
          },
          {
            "step": 18768,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488890073,
            "MicroF1": 0.9975488890073,
            "MacroF1": 0.9975508061984416,
            "Memory in Mb": 0.0048398971557617,
            "Time in s": 233.322943
          },
          {
            "step": 19176,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.99754889178618,
            "MicroF1": 0.99754889178618,
            "MacroF1": 0.9975503516171184,
            "Memory in Mb": 0.0048904418945312,
            "Time in s": 243.357771
          },
          {
            "step": 19584,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488944492672,
            "MicroF1": 0.9975488944492672,
            "MacroF1": 0.9975498909097889,
            "Memory in Mb": 0.0049409866333007,
            "Time in s": 253.567103
          },
          {
            "step": 19992,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488970036516,
            "MicroF1": 0.9975488970036516,
            "MacroF1": 0.9975494259267256,
            "Memory in Mb": 0.0049915313720703,
            "Time in s": 264.004285
          },
          {
            "step": 20400,
            "track": "Multiclass classification",
            "model": "[baseline] Last Class",
            "dataset": "Keystroke",
            "Accuracy": 0.9975488994558556,
            "MicroF1": 0.9975488994558556,
            "MacroF1": 0.9975489582566448,
            "Memory in Mb": 0.0050420761108398,
            "Time in s": 274.675054
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
          "value": "ImageSegments",
          "bind": {
            "input": "select",
            "options": [
              "ImageSegments",
              "Insects",
              "Keystroke"
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
          "Accuracy",
          "MicroF1",
          "MacroF1",
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

???- abstract "ImageSegments"

    Image segments classification.

    This dataset contains features that describe image segments into 7 classes: brickface, sky,
    foliage, cement, window, path, and grass.

        Name  ImageSegments                                                                                               
        Task  Multi-class classification                                                                                  
     Samples  2,310                                                                                                       
    Features  18                                                                                                          
     Classes  7                                                                                                           
      Sparse  False                                                                                                       
        Path  /Users/mastelini/miniconda3/envs/river-benchmark/lib/python3.10/site-packages/river/datasets/segment.csv.zip

<span />

???- abstract "Insects"

    Insects dataset.

    This dataset has different variants, which are:

    - abrupt_balanced
    - abrupt_imbalanced
    - gradual_balanced
    - gradual_imbalanced
    - incremental-abrupt_balanced
    - incremental-abrupt_imbalanced
    - incremental-reoccurring_balanced
    - incremental-reoccurring_imbalanced
    - incremental_balanced
    - incremental_imbalanced
    - out-of-control

    The number of samples and the difficulty change from one variant to another. The number of
    classes is always the same (6), except for the last variant (24).

          Name  Insects                                                                                 
          Task  Multi-class classification                                                              
       Samples  52,848                                                                                  
      Features  33                                                                                      
       Classes  6                                                                                       
        Sparse  False                                                                                   
          Path  /Users/mastelini/river_data/Insects/INSECTS-abrupt_balanced_norm.arff                   
           URL  http://sites.labic.icmc.usp.br/vsouza/repository/creme/INSECTS-abrupt_balanced_norm.arff
          Size  15.66 MB                                                                                
    Downloaded  True                                                                                    
       Variant  abrupt_balanced                                                                         

    Parameters
    ----------
        variant
            Indicates which variant of the dataset to load.

<span />

???- abstract "Keystroke"

    CMU keystroke dataset.

    Users are tasked to type in a password. The task is to determine which user is typing in the
    password.

    The only difference with the original dataset is that the "sessionIndex" and "rep" attributes
    have been dropped.

          Name  Keystroke                                                       
          Task  Multi-class classification                                      
       Samples  20,400                                                          
      Features  31                                                              
       Classes  51                                                              
        Sparse  False                                                           
          Path  /Users/mastelini/river_data/Keystroke/DSL-StrongPasswordData.csv
           URL  http://www.cs.cmu.edu/~keystroke/DSL-StrongPasswordData.csv     
          Size  4.45 MB                                                         
    Downloaded  True                                                            

<span />

## Models

???- example "Naive Bayes"

    <pre>GaussianNB ()</pre>

<span />

???- example "Hoeffding Tree"

    <pre>HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    )</pre>

<span />

???- example "Hoeffding Adaptive Tree"

    <pre>HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=42
    )</pre>

<span />

???- example "Adaptive Random Forest"

    <pre>[]</pre>

<span />

???- example "Aggregated Mondrian Forest"

    <pre>[]</pre>

<span />

???- example "Streaming Random Patches"

    <pre>SRPClassifier (
      model=HoeffdingTreeClassifier (
        grace_period=50
        max_depth=inf
        split_criterion="info_gain"
        delta=0.01
        tau=0.05
        leaf_prediction="nba"
        nb_threshold=0
        nominal_attributes=None
        splitter=GaussianSplitter (
          n_splits=10
        )
        binary_split=False
        min_branch_fraction=0.01
        max_share_to_split=0.99
        max_size=100.
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
      disable_weighted_vote=False
      seed=None
      metric=Accuracy (
        cm=ConfusionMatrix (
          classes=[]
        )
      )
    )</pre>

<span />

???- example "k-Nearest Neighbors"

    <pre>Pipeline (
      StandardScaler (
        with_std=True
      ),
      KNNClassifier (
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
        weighted=True
        cleanup_every=0
        softmax=False
      )
    )</pre>

<span />

???- example "ADWIN Bagging"

    <pre>[HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    )]</pre>

<span />

???- example "AdaBoost"

    <pre>[HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    )]</pre>

<span />

???- example "Bagging"

    <pre>[HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    ), HoeffdingAdaptiveTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
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
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
      seed=None
    )]</pre>

<span />

???- example "Leveraging Bagging"

    <pre>[HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    )]</pre>

<span />

???- example "Stacking"

    <pre>[Pipeline (
      StandardScaler (
        with_std=True
      ),
      SoftmaxRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=CrossEntropy (
          class_weight={}
        )
        l2=0
      )
    ), GaussianNB (), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), Pipeline (
      StandardScaler (
        with_std=True
      ),
      KNNClassifier (
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
        weighted=True
        cleanup_every=0
        softmax=False
      )
    )]</pre>

<span />

???- example "Voting"

    <pre>VotingClassifier (
      models=[Pipeline (
      StandardScaler (
        with_std=True
      ),
      SoftmaxRegression (
        optimizer=SGD (
          lr=Constant (
            learning_rate=0.01
          )
        )
        loss=CrossEntropy (
          class_weight={}
        )
        l2=0
      )
    ), GaussianNB (), HoeffdingTreeClassifier (
      grace_period=200
      max_depth=inf
      split_criterion="info_gain"
      delta=1e-07
      tau=0.05
      leaf_prediction="nba"
      nb_threshold=0
      nominal_attributes=None
      splitter=GaussianSplitter (
        n_splits=10
      )
      binary_split=False
      min_branch_fraction=0.01
      max_share_to_split=0.99
      max_size=100.
      memory_estimate_period=1000000
      stop_mem_management=False
      remove_poor_attrs=False
      merit_preprune=True
    ), Pipeline (
      StandardScaler (
        with_std=True
      ),
      KNNClassifier (
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
        weighted=True
        cleanup_every=0
        softmax=False
      )
    )]
      use_probabilities=True
    )</pre>

<span />

???- example "[baseline] Last Class"

    <pre>NoChangeClassifier ()</pre>

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

