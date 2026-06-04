Final Project
================

# Predict the average reaction time through the variables we get from the survey

    ## Warning: package 'leaps' was built under R version 4.3.3

    ## Warning: package 'olsrr' was built under R version 4.3.3

    ## Warning: package 'glmnet' was built under R version 4.3.3

    ## Warning: package 'lmtest' was built under R version 4.3.3

    ## Warning: package 'zoo' was built under R version 4.3.3

    ## Warning: package 'nlme' was built under R version 4.3.3

    ## Warning: package 'car' was built under R version 4.3.3

    ## Warning: package 'carData' was built under R version 4.3.3

    ##  [1] "First"            "Second"           "Third"            "Class"           
    ##  [5] "Age"              "AvgSleepTime"     "LastNightSleep"   "HoursAweak"      
    ##  [9] "Fatigue"          "Stress"           "Distraction"      "NoiseLevel"      
    ## [13] "Temperature"      "VideoGamePlay"    "SportsPlay"       "ShootingGames"   
    ## [17] "AvgHoursExercise" "Gamer"            "CaffeinIntake"    "AlcoholIntake"   
    ## [21] "VisualAcuity"     "PrimarilyHand"    "UsePrimaryHand"   "Cautious"        
    ## [25] "InputDevice"      "RefreshRate"      "DeviceOS"         "WiFi"

    ##      First           Second          Third                    Class   
    ##  Min.   :325.0   Min.   :338.0   Min.   :341.0   Sophomore       :45  
    ##  1st Qu.:520.0   1st Qu.:498.0   1st Qu.:490.0   Junior          :55  
    ##  Median :593.0   Median :561.0   Median :542.0   Senior          :22  
    ##  Mean   :592.5   Mean   :560.7   Mean   :547.7   Graduate student: 7  
    ##  3rd Qu.:663.0   3rd Qu.:633.0   3rd Qu.:613.0                        
    ##  Max.   :934.0   Max.   :833.0   Max.   :783.0                        
    ##       Age        AvgSleepTime    LastNightSleep     HoursAweak    
    ##  Min.   :18.0   Min.   : 5.000   Min.   : 4.000   Min.   : 0.000  
    ##  1st Qu.:20.0   1st Qu.: 6.500   1st Qu.: 6.000   1st Qu.: 4.000  
    ##  Median :20.0   Median : 7.000   Median : 7.000   Median : 6.000  
    ##  Mean   :20.9   Mean   : 7.236   Mean   : 7.264   Mean   : 7.322  
    ##  3rd Qu.:21.0   3rd Qu.: 8.000   3rd Qu.: 8.000   3rd Qu.:10.000  
    ##  Max.   :26.0   Max.   :10.000   Max.   :11.000   Max.   :18.000  
    ##                 Fatigue         Stress   Distraction          NoiseLevel    
    ##  Extremely fatigued : 1   Very High: 5   Length:129         Min.   : 1.000  
    ##  Very fatigued      :16   High     :20   Class :character   1st Qu.: 2.000  
    ##  Moderately fatigued:44   Moderate :46   Mode  :character   Median : 3.000  
    ##  Slightly Fatigued  :45   Low      :35                      Mean   : 3.287  
    ##  Not fatigued at all:23   Very Low :23                      3rd Qu.: 5.000  
    ##                                                             Max.   :10.000  
    ##     Temperature               VideoGamePlay                 SportsPlay
    ##  Very Warm: 2   Daily                :11    Daily                : 5  
    ##  Warm     :16   Several times a week :36    Several times a week :24  
    ##  Neutral  :98   Once a week          : 9    Once a week          :11  
    ##  Cold     :13   Several times a month:24    Several times a month:24  
    ##                 Rarely               :38    Rarely               :50  
    ##                 Never                :11    Never                :15  
    ##       ShootingGames AvgHoursExercise    Gamer           CaffeinIntake     
    ##  None        :19    Min.   : 0.000   Length:129         Length:129        
    ##  Beginner    :54    1st Qu.: 2.000   Class :character   Class :character  
    ##  Intermediate:35    Median : 4.000   Mode  :character   Mode  :character  
    ##  Advanced    :18    Mean   : 4.097                                        
    ##  Expert      : 3    3rd Qu.: 6.000                                        
    ##                     Max.   :12.000                                        
    ##  VisualAcuity                                 PrimarilyHand UsePrimaryHand
    ##  Length:129         Right hand                       :119   Yes:122       
    ##  Class :character   Left hand                        :  6   No :  7       
    ##  Mode  :character   Ambidextrous (both hands equally):  4                 
    ##                                                                           
    ##                                                                           
    ##                                                                           
    ##                 Cautious           InputDevice    RefreshRate
    ##  Extremely cautious : 3   Game controller: 1   High     :29  
    ##  Very cautious      :32   Mouse          :47   Mid-Range:52  
    ##  Moderately cautious:68   Keyboard       : 2   Standard :48  
    ##  Slightly cautious  :21   Trackpad       :69                 
    ##  Not cautious at all: 5   Touch screen   :10                 
    ##                                                              
    ##    DeviceOS               WiFi        avg_time    
    ##  Length:129         Unstable:  2   Min.   :345.3  
    ##  Class :character   Stable  :127   1st Qu.:511.0  
    ##  Mode  :character                  Median :574.0  
    ##                                    Mean   :567.0  
    ##                                    3rd Qu.:635.0  
    ##                                    Max.   :795.0

    ## Warning: `aes_string()` was deprecated in ggplot2 3.0.0.
    ## ℹ Please use tidy evaluation idioms with `aes()`.
    ## ℹ See also `vignette("ggplot2-in-packages")` for more information.
    ## This warning is displayed once every 8 hours.
    ## Call `lifecycle::last_lifecycle_warnings()` to see where this warning was
    ## generated.

![](Code_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-2.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-3.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-4.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-5.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-6.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-7.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-8.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-9.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-10.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-11.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-12.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-13.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-14.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-15.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-16.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-17.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-18.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-19.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-20.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-21.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-22.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-6-23.png)<!-- -->

    ## 
    ## Call:
    ## lm(formula = avg_time ~ ., data = Survey_cleaned)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -119.584  -31.677   -1.699   23.259  158.041 
    ## 
    ## Coefficients:
    ##                                                 Estimate Std. Error t value
    ## (Intercept)                                     316.7155   214.0247   1.480
    ## ClassJunior                                      36.3028    19.3107   1.880
    ## ClassSenior                                       5.9146    27.0350   0.219
    ## ClassGraduate student                           120.6718    55.3700   2.179
    ## Age                                               3.0620     8.1732   0.375
    ## AvgSleepTime                                     15.7785     8.3699   1.885
    ## LastNightSleep                                    1.7912     5.3886   0.332
    ## HoursAweak                                        0.5274     2.0285   0.260
    ## DistractionYes                                   28.4336    20.0834   1.416
    ## TemperatureWarm                                  25.1289    64.2955   0.391
    ## TemperatureNeutral                               46.3851    60.6552   0.765
    ## TemperatureCold                                  65.9307    63.1520   1.044
    ## GamerYes                                         15.4718    18.0549   0.857
    ## CaffeinIntakeYes                                 40.1718    17.9718   2.235
    ## VisualAcuityExcellent                           -58.0343    29.0626  -1.997
    ## VisualAcuityGood                                -79.1387    29.9986  -2.638
    ## VisualAcuityPoor                                -72.0108    50.5460  -1.425
    ## VisualAcuityVery Poor                          -146.9141    97.1368  -1.512
    ## PrimarilyHandLeft hand                          -54.6740    44.0925  -1.240
    ## PrimarilyHandAmbidextrous (both hands equally)   34.9272    40.1681   0.870
    ## UsePrimaryHandNo                                 65.8135    40.6695   1.618
    ## CautiousVery cautious                             3.0895    45.3541   0.068
    ## CautiousModerately cautious                      -6.5308    46.0642  -0.142
    ## CautiousSlightly cautious                         9.0990    48.4746   0.188
    ## CautiousNot cautious at all                      38.3024    64.5652   0.593
    ## InputDeviceMouse                                -45.1659    78.2158  -0.577
    ## InputDeviceKeyboard                              77.1231    96.5755   0.799
    ## InputDeviceTrackpad                              37.3924    77.5345   0.482
    ## InputDeviceTouch screen                          18.3343    85.9597   0.213
    ## RefreshRateMid-Range                             30.3461    24.3793   1.245
    ## RefreshRateStandard                              59.9600    22.9308   2.615
    ## DeviceiPad(Tablet                               -42.5427    64.8587  -0.656
    ## DeviceiPhone(Smartphone                          81.0134    83.1190   0.975
    ## DeviceLaptop                                     36.2946    24.0861   1.507
    ## WiFiStable                                      -96.2096    58.0745  -1.657
    ## Fatigue_3Moderately Fatigue                      54.4543    26.0192   2.093
    ## Fatigue_3Low Fatigue                             48.2829    26.9053   1.795
    ## Stress_3Moderately Stress                        14.0792    20.5947   0.684
    ## Stress_3Low Stress                              -29.3721    21.5548  -1.363
    ## Noise_LevelModerately Noise                     -35.7234    71.8799  -0.497
    ## Noise_LevelLow Noise                            -19.1215    71.4386  -0.268
    ## Game_FrequencyLow Frequency                      21.8759    15.1069   1.448
    ## Sports_FrequencyLow Frequency                    17.6599    18.2598   0.967
    ## Shooting_LevelsIntermediate Levels               -7.1078    24.4294  -0.291
    ## Shooting_LevelsLow Levels                        21.0557    22.7596   0.925
    ## SystemLinux                                      39.9766    67.0464   0.596
    ## SystemWindows                                    -0.8867    19.2729  -0.046
    ## logAvgHoursExercise                               3.1802    12.8470   0.248
    ##                                                Pr(>|t|)   
    ## (Intercept)                                      0.1428   
    ## ClassJunior                                      0.0637 . 
    ## ClassSenior                                      0.8274   
    ## ClassGraduate student                            0.0322 * 
    ## Age                                              0.7089   
    ## AvgSleepTime                                     0.0630 . 
    ## LastNightSleep                                   0.7404   
    ## HoursAweak                                       0.7955   
    ## DistractionYes                                   0.1607   
    ## TemperatureWarm                                  0.6969   
    ## TemperatureNeutral                               0.4467   
    ## TemperatureCold                                  0.2996   
    ## GamerYes                                         0.3940   
    ## CaffeinIntakeYes                                 0.0282 * 
    ## VisualAcuityExcellent                            0.0492 * 
    ## VisualAcuityGood                                 0.0100 **
    ## VisualAcuityPoor                                 0.1581   
    ## VisualAcuityVery Poor                            0.1343   
    ## PrimarilyHandLeft hand                           0.2186   
    ## PrimarilyHandAmbidextrous (both hands equally)   0.3871   
    ## UsePrimaryHandNo                                 0.1095   
    ## CautiousVery cautious                            0.9459   
    ## CautiousModerately cautious                      0.8876   
    ## CautiousSlightly cautious                        0.8516   
    ## CautiousNot cautious at all                      0.5547   
    ## InputDeviceMouse                                 0.5652   
    ## InputDeviceKeyboard                              0.4269   
    ## InputDeviceTrackpad                              0.6309   
    ## InputDeviceTouch screen                          0.8316   
    ## RefreshRateMid-Range                             0.2168   
    ## RefreshRateStandard                              0.0106 * 
    ## DeviceiPad(Tablet                                0.5137   
    ## DeviceiPhone(Smartphone                          0.3326   
    ## DeviceLaptop                                     0.1357   
    ## WiFiStable                                       0.1015   
    ## Fatigue_3Moderately Fatigue                      0.0395 * 
    ## Fatigue_3Low Fatigue                             0.0765 . 
    ## Stress_3Moderately Stress                        0.4962   
    ## Stress_3Low Stress                               0.1768   
    ## Noise_LevelModerately Noise                      0.6205   
    ## Noise_LevelLow Noise                             0.7896   
    ## Game_FrequencyLow Frequency                      0.1515   
    ## Sports_FrequencyLow Frequency                    0.3364   
    ## Shooting_LevelsIntermediate Levels               0.7718   
    ## Shooting_LevelsLow Levels                        0.3576   
    ## SystemLinux                                      0.5527   
    ## SystemWindows                                    0.9634   
    ## logAvgHoursExercise                              0.8051   
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 66.77 on 81 degrees of freedom
    ## Multiple R-squared:  0.6914, Adjusted R-squared:  0.5123 
    ## F-statistic: 3.861 on 47 and 81 DF,  p-value: 4.833e-08

    ## Start:  AIC=1119.88
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + Cautious + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels + System + 
    ##     logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Cautious             4      6186 367259 1114.1
    ## - System               2      1980 363052 1116.6
    ## - Noise_Level          2      5074 366147 1117.7
    ## - Temperature          3     10845 371918 1117.7
    ## - logAvgHoursExercise  1       273 361346 1118.0
    ## - HoursAweak           1       301 361374 1118.0
    ## - LastNightSleep       1       493 361565 1118.0
    ## - Age                  1       626 361699 1118.1
    ## - Gamer                1      3273 364346 1119.0
    ## - Sports_Frequency     1      4170 365243 1119.4
    ## <none>                             361073 1119.9
    ## - PrimarilyHand        2     11526 372599 1119.9
    ## - Shooting_Levels      2     11896 372969 1120.1
    ## - Distraction          1      8935 370008 1121.0
    ## - Game_Frequency       1      9347 370420 1121.2
    ## - Device               3     22755 383828 1121.8
    ## - UsePrimaryHand       1     11674 372746 1122.0
    ## - WiFi                 1     12234 373307 1122.2
    ## - Fatigue_3            2     19740 380813 1122.7
    ## - AvgSleepTime         1     15842 376915 1123.4
    ## - Stress_3             2     23328 384401 1124.0
    ## - VisualAcuity         4     37145 398218 1124.5
    ## - CaffeinIntake        1     22272 383345 1125.6
    ## - Class                3     40144 401217 1127.5
    ## - RefreshRate          2     34921 395994 1127.8
    ## - InputDevice          4     73291 434364 1135.7
    ## 
    ## Step:  AIC=1114.07
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels + System + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - System               2      3458 370717 1111.3
    ## - Temperature          3     11208 378467 1112.0
    ## - logAvgHoursExercise  1         0 367259 1112.1
    ## - Age                  1       450 367708 1112.2
    ## - LastNightSleep       1       519 367778 1112.2
    ## - HoursAweak           1       611 367869 1112.3
    ## - Noise_Level          2      8204 375463 1112.9
    ## - Gamer                1      3617 370875 1113.3
    ## - Sports_Frequency     1      4109 371368 1113.5
    ## - PrimarilyHand        2     10345 377604 1113.7
    ## <none>                             367259 1114.1
    ## - Shooting_Levels      2     14422 381681 1115.0
    ## - Distraction          1     10066 377324 1115.6
    ## - Device               3     22527 389786 1115.8
    ## - Game_Frequency       1     10895 378153 1115.8
    ## - WiFi                 1     12477 379736 1116.4
    ## - UsePrimaryHand       1     15475 382733 1117.4
    ## - Fatigue_3            2     23869 391128 1118.2
    ## - Stress_3             2     23955 391213 1118.2
    ## - VisualAcuity         4     39758 407017 1119.3
    ## - CaffeinIntake        1     22391 389650 1119.7
    ## + Cautious             4      6186 361073 1119.9
    ## - AvgSleepTime         1     26198 393457 1121.0
    ## - Class                3     40028 407286 1121.4
    ## - RefreshRate          2     36741 404000 1122.4
    ## - InputDevice          4     74330 441589 1129.8
    ## 
    ## Step:  AIC=1111.28
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - logAvgHoursExercise  1        18 370734 1109.3
    ## - HoursAweak           1        91 370807 1109.3
    ## - Temperature          3     11934 382651 1109.4
    ## - Noise_Level          2      6813 377529 1109.6
    ## - Age                  1      1077 371794 1109.7
    ## - LastNightSleep       1      1080 371797 1109.7
    ## - Gamer                1      4380 375097 1110.8
    ## - PrimarilyHand        2     10668 381384 1110.9
    ## - Sports_Frequency     1      5524 376240 1111.2
    ## <none>                             370717 1111.3
    ## - Distraction          1      9422 380139 1112.5
    ## - Shooting_Levels      2     15720 386437 1112.6
    ## - Game_Frequency       1     10570 381286 1112.9
    ## - Device               3     23286 394002 1113.1
    ## - WiFi                 1     13732 384449 1114.0
    ## + System               2      3458 367259 1114.1
    ## - Fatigue_3            2     21150 391867 1114.4
    ## - UsePrimaryHand       1     16142 386858 1114.8
    ## - Stress_3             2     26900 397616 1116.3
    ## + Cautious             4      7664 363052 1116.6
    ## - VisualAcuity         4     40603 411320 1116.7
    ## - CaffeinIntake        1     23349 394066 1117.2
    ## - AvgSleepTime         1     23564 394280 1117.2
    ## - Class                3     37904 408621 1117.8
    ## - RefreshRate          2     33438 404154 1118.4
    ## - InputDevice          4    105407 476123 1135.6
    ## 
    ## Step:  AIC=1109.28
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - HoursAweak           1        87 370821 1107.3
    ## - Temperature          3     11961 382695 1107.4
    ## - Noise_Level          2      6820 377555 1107.6
    ## - Age                  1      1060 371794 1107.7
    ## - LastNightSleep       1      1064 371798 1107.7
    ## - Gamer                1      4366 375100 1108.8
    ## - PrimarilyHand        2     10827 381561 1109.0
    ## <none>                             370734 1109.3
    ## - Sports_Frequency     1      5919 376653 1109.3
    ## - Distraction          1      9495 380229 1110.5
    ## - Shooting_Levels      2     16442 387176 1110.9
    ## - Game_Frequency       1     10647 381381 1110.9
    ## - Device               3     23274 394008 1111.1
    ## + logAvgHoursExercise  1        18 370717 1111.3
    ## - WiFi                 1     13743 384477 1112.0
    ## + System               2      3475 367259 1112.1
    ## - Fatigue_3            2     21828 392562 1112.7
    ## - UsePrimaryHand       1     16130 386865 1112.8
    ## - Stress_3             2     26889 397623 1114.3
    ## + Cautious             4      7260 363474 1114.7
    ## - VisualAcuity         4     40924 411658 1114.8
    ## - AvgSleepTime         1     23825 394559 1115.3
    ## - CaffeinIntake        1     24115 394849 1115.4
    ## - Class                3     37930 408664 1115.8
    ## - RefreshRate          2     34559 405293 1116.8
    ## - InputDevice          4    105750 476484 1133.7
    ## 
    ## Step:  AIC=1107.31
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + Distraction + 
    ##     Temperature + Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + Device + WiFi + 
    ##     Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + Sports_Frequency + 
    ##     Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Temperature          3     11970 382791 1105.4
    ## - Noise_Level          2      6813 377635 1105.7
    ## - LastNightSleep       1      1066 371888 1105.7
    ## - Age                  1      1105 371926 1105.7
    ## - Gamer                1      4474 375295 1106.9
    ## <none>                             370821 1107.3
    ## - Sports_Frequency     1      6209 377030 1107.5
    ## - PrimarilyHand        2     12830 383651 1107.7
    ## - Distraction          1      9417 380238 1108.5
    ## - Game_Frequency       1     10560 381381 1108.9
    ## - Shooting_Levels      2     16837 387659 1109.0
    ## - Device               3     23213 394034 1109.2
    ## + HoursAweak           1        87 370734 1109.3
    ## + logAvgHoursExercise  1        14 370807 1109.3
    ## - WiFi                 1     13749 384571 1110.0
    ## + System               2      2952 367870 1110.3
    ## - Fatigue_3            2     23362 394183 1111.2
    ## - UsePrimaryHand       1     17655 388477 1111.3
    ## - Stress_3             2     27142 397963 1112.4
    ## + Cautious             4      7320 363501 1112.7
    ## - VisualAcuity         4     41189 412010 1112.9
    ## - AvgSleepTime         1     23826 394648 1113.3
    ## - CaffeinIntake        1     24468 395289 1113.6
    ## - Class                3     38459 409280 1114.0
    ## - RefreshRate          2     34613 405434 1114.8
    ## - InputDevice          4    107672 478493 1132.2
    ## 
    ## Step:  AIC=1105.41
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + Distraction + 
    ##     Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + 
    ##     Noise_Level + Game_Frequency + Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Noise_Level          2      4281 387073 1102.8
    ## - LastNightSleep       1       284 383075 1103.5
    ## - Age                  1      1279 384070 1103.8
    ## - Gamer                1      1827 384618 1104.0
    ## - Sports_Frequency     1      5120 387912 1105.1
    ## <none>                             382791 1105.4
    ## - Shooting_Levels      2     12603 395394 1105.6
    ## - Distraction          1      8186 390978 1106.1
    ## - Game_Frequency       1      8210 391001 1106.2
    ## - PrimarilyHand        2     16490 399282 1106.8
    ## - Device               3     23846 406638 1107.2
    ## + Temperature          3     11970 370821 1107.3
    ## + HoursAweak           1        97 382695 1107.4
    ## + logAvgHoursExercise  1        40 382751 1107.4
    ## + System               2      3673 379119 1108.2
    ## - WiFi                 1     15089 397880 1108.4
    ## - Stress_3             2     23613 406404 1109.1
    ## - VisualAcuity         4     36566 419357 1109.2
    ## - Fatigue_3            2     28179 410971 1110.6
    ## - UsePrimaryHand       1     21981 404773 1110.6
    ## + Cautious             4      7923 374869 1110.7
    ## - AvgSleepTime         1     23256 406048 1111.0
    ## - Class                3     36590 419382 1111.2
    ## - CaffeinIntake        1     25129 407921 1111.6
    ## - RefreshRate          2     36072 418863 1113.0
    ## - InputDevice          4    100467 483258 1127.5
    ## 
    ## Step:  AIC=1102.85
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + Distraction + 
    ##     Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - LastNightSleep       1       383 387456 1101.0
    ## - Gamer                1      1318 388391 1101.3
    ## - Age                  1      1614 388687 1101.4
    ## - Shooting_Levels      2     11193 398266 1102.5
    ## <none>                             387073 1102.8
    ## - Distraction          1      6132 393205 1102.9
    ## - Sports_Frequency     1      6408 393481 1103.0
    ## - Game_Frequency       1      8205 395278 1103.5
    ## - PrimarilyHand        2     16349 403422 1104.2
    ## + HoursAweak           1        74 386999 1104.8
    ## + logAvgHoursExercise  1         1 387071 1104.8
    ## + Noise_Level          2      4281 382791 1105.4
    ## - WiFi                 1     14680 401753 1105.7
    ## + Temperature          3      9438 377635 1105.7
    ## + System               2      2576 384497 1106.0
    ## - Stress_3             2     23485 410557 1106.4
    ## - Device               3     31250 418322 1106.9
    ## - VisualAcuity         4     38848 425921 1107.2
    ## + Cautious             4      9580 377493 1107.6
    ## - Fatigue_3            2     27266 414338 1107.6
    ## - Class                3     34189 421262 1107.8
    ## - AvgSleepTime         1     23007 410080 1108.3
    ## - CaffeinIntake        1     23850 410922 1108.6
    ## - UsePrimaryHand       1     24556 411629 1108.8
    ## - RefreshRate          2     35695 422768 1110.2
    ## - InputDevice          4     98624 485696 1124.1
    ## 
    ## Step:  AIC=1100.97
    ## avg_time ~ Class + Age + AvgSleepTime + Distraction + Gamer + 
    ##     CaffeinIntake + VisualAcuity + PrimarilyHand + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Gamer                1      1334 388790 1099.4
    ## - Age                  1      1828 389284 1099.6
    ## - Shooting_Levels      2     11178 398633 1100.6
    ## - Distraction          1      5951 393406 1100.9
    ## <none>                             387456 1101.0
    ## - Sports_Frequency     1      6316 393772 1101.1
    ## - Game_Frequency       1      8139 395594 1101.7
    ## - PrimarilyHand        2     16257 403712 1102.3
    ## + LastNightSleep       1       383 387073 1102.8
    ## + HoursAweak           1        76 387380 1103.0
    ## + logAvgHoursExercise  1        17 387438 1103.0
    ## + Noise_Level          2      4380 383075 1103.5
    ## - WiFi                 1     14370 401826 1103.7
    ## + Temperature          3      8701 378754 1104.0
    ## + System               2      2691 384764 1104.1
    ## - Stress_3             2     23111 410566 1104.5
    ## - Device               3     31664 419119 1105.1
    ## - VisualAcuity         4     38508 425964 1105.2
    ## + Cautious             4      9643 377812 1105.7
    ## - Class                3     34943 422398 1106.1
    ## - CaffeinIntake        1     23961 411416 1106.7
    ## - Fatigue_3            2     30543 417998 1106.8
    ## - UsePrimaryHand       1     24445 411900 1106.9
    ## - RefreshRate          2     35509 422965 1108.3
    ## - AvgSleepTime         1     29291 416746 1108.4
    ## - InputDevice          4    100671 488127 1122.8
    ## 
    ## Step:  AIC=1099.42
    ## avg_time ~ Class + Age + AvgSleepTime + Distraction + CaffeinIntake + 
    ##     VisualAcuity + PrimarilyHand + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Age                  1      2399 391188 1098.2
    ## - Shooting_Levels      2     10171 398960 1098.8
    ## - Distraction          1      5525 394315 1099.2
    ## - Sports_Frequency     1      5816 394606 1099.3
    ## <none>                             388790 1099.4
    ## - Game_Frequency       1      6920 395710 1099.7
    ## - PrimarilyHand        2     15844 404634 1100.6
    ## + Gamer                1      1334 387456 1101.0
    ## + LastNightSleep       1       399 388391 1101.3
    ## + HoursAweak           1       123 388667 1101.4
    ## + logAvgHoursExercise  1        55 388734 1101.4
    ## - WiFi                 1     13216 402006 1101.7
    ## + Noise_Level          2      3866 384924 1102.1
    ## + System               2      2804 385985 1102.5
    ## - Stress_3             2     22081 410871 1102.5
    ## + Temperature          3      6969 381821 1103.1
    ## - VisualAcuity         4     37179 425969 1103.2
    ## - Device               3     31474 420264 1103.5
    ## + Cautious             4      9881 378909 1104.1
    ## - Class                3     33671 422461 1104.1
    ## - CaffeinIntake        1     22733 411522 1104.8
    ## - Fatigue_3            2     29498 418288 1104.8
    ## - UsePrimaryHand       1     23127 411916 1104.9
    ## - AvgSleepTime         1     28824 417614 1106.6
    ## - RefreshRate          2     35662 424452 1106.7
    ## - InputDevice          4    100536 489325 1121.1
    ## 
    ## Step:  AIC=1098.21
    ## avg_time ~ Class + AvgSleepTime + Distraction + CaffeinIntake + 
    ##     VisualAcuity + PrimarilyHand + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Shooting_Levels      2      9379 400568 1097.3
    ## - Distraction          1      5870 397058 1098.1
    ## <none>                             391188 1098.2
    ## - Sports_Frequency     1      7300 398489 1098.6
    ## - Game_Frequency       1      7549 398738 1098.7
    ## + Age                  1      2399 388790 1099.4
    ## + Gamer                1      1905 389284 1099.6
    ## - PrimarilyHand        2     17520 408708 1099.9
    ## + LastNightSleep       1       661 390527 1100.0
    ## - WiFi                 1     11941 403130 1100.1
    ## + logAvgHoursExercise  1       275 390913 1100.1
    ## + HoursAweak           1       211 390977 1100.1
    ## + Noise_Level          2      4203 386986 1100.8
    ## + System               2      3594 387594 1101.0
    ## - Stress_3             2     22189 413377 1101.3
    ## - VisualAcuity         4     35439 426628 1101.4
    ## + Temperature          3      6681 384507 1102.0
    ## - Device               3     32199 423387 1102.4
    ## + Cautious             4     10431 380757 1102.7
    ## - Fatigue_3            2     30846 422034 1104.0
    ## - UsePrimaryHand       1     25826 417014 1104.5
    ## - CaffeinIntake        1     25935 417123 1104.5
    ## - AvgSleepTime         1     26988 418176 1104.8
    ## - RefreshRate          2     35935 427124 1105.5
    ## - Class                3     80062 471250 1116.2
    ## - InputDevice          4     99795 490984 1119.5
    ## 
    ## Step:  AIC=1097.27
    ## avg_time ~ Class + AvgSleepTime + Distraction + CaffeinIntake + 
    ##     VisualAcuity + PrimarilyHand + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Distraction          1      5333 405900 1097.0
    ## <none>                             400568 1097.3
    ## - WiFi                 1      8805 409372 1098.1
    ## - PrimarilyHand        2     15495 416062 1098.2
    ## + Shooting_Levels      2      9379 391188 1098.2
    ## - Sports_Frequency     1     10001 410569 1098.5
    ## + Age                  1      1607 398960 1098.8
    ## + logAvgHoursExercise  1      1285 399283 1098.8
    ## + Gamer                1       605 399962 1099.1
    ## + LastNightSleep       1       592 399976 1099.1
    ## + HoursAweak           1       476 400092 1099.1
    ## - Game_Frequency       1     12442 413010 1099.2
    ## + System               2      4113 396455 1099.9
    ## + Noise_Level          2      2983 397584 1100.3
    ## - Stress_3             2     24562 425129 1100.9
    ## + Cautious             4     11847 388721 1101.4
    ## + Temperature          3      4947 395620 1101.7
    ## - VisualAcuity         4     40553 441121 1101.7
    ## - UsePrimaryHand       1     20795 421363 1101.8
    ## - Device               3     37731 438298 1102.9
    ## - CaffeinIntake        1     25512 426080 1103.2
    ## - AvgSleepTime         1     25819 426386 1103.3
    ## - Fatigue_3            2     39403 439970 1105.4
    ## - RefreshRate          2     40891 441458 1105.8
    ## - Class                3     94721 495289 1118.7
    ## - InputDevice          4    111509 512077 1121.0
    ## 
    ## Step:  AIC=1096.97
    ## avg_time ~ Class + AvgSleepTime + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + Sports_Frequency
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## <none>                             405900 1097.0
    ## - PrimarilyHand        2     13237 419137 1097.1
    ## + Distraction          1      5333 400568 1097.3
    ## - WiFi                 1      8406 414306 1097.6
    ## - Sports_Frequency     1      8986 414886 1097.8
    ## + Shooting_Levels      2      8842 397058 1098.1
    ## + Age                  1      1943 403957 1098.3
    ## + logAvgHoursExercise  1      1905 403995 1098.4
    ## - Game_Frequency       1     11911 417811 1098.7
    ## + LastNightSleep       1       428 405473 1098.8
    ## + HoursAweak           1       399 405501 1098.8
    ## + Gamer                1       398 405503 1098.8
    ## + System               2      3809 402091 1099.8
    ## + Noise_Level          2      1132 404768 1100.6
    ## + Cautious             4     12107 393793 1101.1
    ## + Temperature          3      4990 400910 1101.4
    ## - UsePrimaryHand       1     20798 426698 1101.4
    ## - Stress_3             2     28495 434395 1101.7
    ## - VisualAcuity         4     43516 449416 1102.1
    ## - AvgSleepTime         1     24693 430593 1102.6
    ## - Device               3     38320 444220 1102.6
    ## - CaffeinIntake        1     33563 439463 1105.2
    ## - Fatigue_3            2     41583 447483 1105.5
    ## - RefreshRate          2     42714 448614 1105.9
    ## - Class                3     93752 499652 1117.8
    ## - InputDevice          4    115093 520993 1121.2

    ## 
    ## Call:
    ## lm(formula = avg_time ~ Class + AvgSleepTime + CaffeinIntake + 
    ##     VisualAcuity + PrimarilyHand + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency, data = Survey_cleaned)
    ## 
    ## Coefficients:
    ##                                    (Intercept)  
    ##                                        438.055  
    ##                                    ClassJunior  
    ##                                         38.454  
    ##                                    ClassSenior  
    ##                                         15.073  
    ##                          ClassGraduate student  
    ##                                        129.289  
    ##                                   AvgSleepTime  
    ##                                         15.025  
    ##                               CaffeinIntakeYes  
    ##                                         43.014  
    ##                          VisualAcuityExcellent  
    ##                                        -69.927  
    ##                               VisualAcuityGood  
    ##                                        -83.490  
    ##                               VisualAcuityPoor  
    ##                                        -73.772  
    ##                          VisualAcuityVery Poor  
    ##                                       -116.392  
    ##                         PrimarilyHandLeft hand  
    ##                                        -51.238  
    ## PrimarilyHandAmbidextrous (both hands equally)  
    ##                                         31.844  
    ##                               UsePrimaryHandNo  
    ##                                         74.840  
    ##                               InputDeviceMouse  
    ##                                        -51.908  
    ##                            InputDeviceKeyboard  
    ##                                         53.504  
    ##                            InputDeviceTrackpad  
    ##                                         25.861  
    ##                        InputDeviceTouch screen  
    ##                                        -20.490  
    ##                           RefreshRateMid-Range  
    ##                                         27.233  
    ##                            RefreshRateStandard  
    ##                                         57.230  
    ##                              DeviceiPad(Tablet  
    ##                                        -24.929  
    ##                        DeviceiPhone(Smartphone  
    ##                                        142.767  
    ##                                   DeviceLaptop  
    ##                                         36.504  
    ##                                     WiFiStable  
    ##                                        -71.611  
    ##                    Fatigue_3Moderately Fatigue  
    ##                                         63.388  
    ##                           Fatigue_3Low Fatigue  
    ##                                         56.646  
    ##                      Stress_3Moderately Stress  
    ##                                          7.428  
    ##                             Stress_3Low Stress  
    ##                                        -32.981  
    ##                    Game_FrequencyLow Frequency  
    ##                                         21.879  
    ##                  Sports_FrequencyLow Frequency  
    ##                                         20.661

    ## Start:  AIC=1257.15
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + Cautious + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels + System + 
    ##     logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Cautious             4      6186 367259 1239.9
    ## - Temperature          3     10845 371918 1246.4
    ## - System               2      1980 363052 1248.1
    ## - Noise_Level          2      5074 366147 1249.2
    ## - VisualAcuity         4     37145 398218 1250.3
    ## - Device               3     22755 383828 1250.5
    ## - PrimarilyHand        2     11526 372599 1251.5
    ## - Shooting_Levels      2     11896 372969 1251.6
    ## - logAvgHoursExercise  1       273 361346 1252.4
    ## - HoursAweak           1       301 361374 1252.4
    ## - LastNightSleep       1       493 361565 1252.5
    ## - Age                  1       626 361699 1252.5
    ## - Gamer                1      3273 364346 1253.5
    ## - Sports_Frequency     1      4170 365243 1253.8
    ## - Fatigue_3            2     19740 380813 1254.3
    ## - Distraction          1      8935 370008 1255.4
    ## - Stress_3             2     23328 384401 1255.5
    ## - Game_Frequency       1      9347 370420 1255.6
    ## - Class                3     40144 401217 1256.2
    ## - UsePrimaryHand       1     11674 372746 1256.4
    ## - WiFi                 1     12234 373307 1256.6
    ## <none>                             361073 1257.2
    ## - AvgSleepTime         1     15842 376915 1257.8
    ## - RefreshRate          2     34921 395994 1259.3
    ## - CaffeinIntake        1     22272 383345 1260.0
    ## - InputDevice          4     73291 434364 1261.5
    ## 
    ## Step:  AIC=1239.9
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Temperature + Gamer + CaffeinIntake + VisualAcuity + 
    ##     PrimarilyHand + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     Device + WiFi + Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels + System + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Temperature          3     11208 378467 1229.2
    ## - System               2      3458 370717 1231.4
    ## - Device               3     22527 389786 1233.0
    ## - Noise_Level          2      8204 375463 1233.0
    ## - VisualAcuity         4     39758 407017 1233.7
    ## - PrimarilyHand        2     10345 377604 1233.8
    ## - logAvgHoursExercise  1         0 367259 1235.0
    ## - Shooting_Levels      2     14422 381681 1235.2
    ## - Age                  1       450 367708 1235.2
    ## - LastNightSleep       1       519 367778 1235.2
    ## - HoursAweak           1       611 367869 1235.2
    ## - Gamer                1      3617 370875 1236.3
    ## - Sports_Frequency     1      4109 371368 1236.5
    ## - Fatigue_3            2     23869 391128 1238.3
    ## - Stress_3             2     23955 391213 1238.3
    ## - Distraction          1     10066 377324 1238.5
    ## - Class                3     40028 407286 1238.7
    ## - Game_Frequency       1     10895 378153 1238.8
    ## - WiFi                 1     12477 379736 1239.3
    ## <none>                             367259 1239.9
    ## - UsePrimaryHand       1     15475 382733 1240.4
    ## - RefreshRate          2     36741 404000 1242.5
    ## - CaffeinIntake        1     22391 389650 1242.7
    ## - AvgSleepTime         1     26198 393457 1243.9
    ## - InputDevice          4     74330 441589 1244.2
    ## + Cautious             4      6186 361073 1257.2
    ## 
    ## Step:  AIC=1229.2
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + Device + WiFi + 
    ##     Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + Sports_Frequency + 
    ##     Shooting_Levels + System + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - System               2      4184 382651 1220.9
    ## - VisualAcuity         4     35557 414024 1221.3
    ## - Noise_Level          2      5619 384085 1221.4
    ## - Device               3     23281 401748 1222.3
    ## - Shooting_Levels      2     10787 389254 1223.1
    ## - PrimarilyHand        2     13084 391551 1223.9
    ## - logAvgHoursExercise  1         4 378471 1224.3
    ## - LastNightSleep       1        78 378545 1224.4
    ## - Age                  1       538 379005 1224.5
    ## - HoursAweak           1       650 379117 1224.6
    ## - Gamer                1      1425 379892 1224.8
    ## - Sports_Frequency     1      3391 381858 1225.5
    ## - Stress_3             2     20992 399459 1226.4
    ## - Class                3     38229 416696 1227.0
    ## - Game_Frequency       1      8495 386962 1227.2
    ## - Distraction          1      8793 387260 1227.3
    ## - Fatigue_3            2     27884 406351 1228.7
    ## - WiFi                 1     13749 392215 1228.9
    ## <none>                             378467 1229.2
    ## - UsePrimaryHand       1     19388 397855 1230.8
    ## - InputDevice          4     68310 446777 1231.2
    ## - CaffeinIntake        1     22626 401093 1231.8
    ## - RefreshRate          2     38413 416880 1232.0
    ## - AvgSleepTime         1     25529 403996 1232.8
    ## + Temperature          3     11208 367259 1239.9
    ## + Cautious             4      6549 371918 1246.4
    ## 
    ## Step:  AIC=1220.9
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + Device + WiFi + 
    ##     Fatigue_3 + Stress_3 + Noise_Level + Game_Frequency + Sports_Frequency + 
    ##     Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Noise_Level          2      4347 386998 1212.6
    ## - VisualAcuity         4     36345 418996 1213.2
    ## - Device               3     23904 406555 1214.1
    ## - Shooting_Levels      2     11863 394514 1215.1
    ## - PrimarilyHand        2     13695 396346 1215.7
    ## - logAvgHoursExercise  1        44 382695 1216.0
    ## - HoursAweak           1       101 382751 1216.1
    ## - LastNightSleep       1       309 382960 1216.1
    ## - Age                  1      1275 383925 1216.5
    ## - Gamer                1      1799 384450 1216.6
    ## - Sports_Frequency     1      4666 387317 1217.6
    ## - Class                3     36049 418700 1217.9
    ## - Game_Frequency       1      8180 390831 1218.8
    ## - Distraction          1      8254 390905 1218.8
    ## - Stress_3             2     23453 406104 1218.8
    ## - Fatigue_3            2     25061 407712 1219.4
    ## <none>                             382651 1220.9
    ## - WiFi                 1     15046 397697 1221.0
    ## - RefreshRate          2     34523 417174 1222.3
    ## - UsePrimaryHand       1     20006 402657 1222.6
    ## - AvgSleepTime         1     23174 405825 1223.6
    ## - CaffeinIntake        1     24173 406824 1223.9
    ## + System               2      4184 378467 1229.2
    ## - InputDevice          4     98241 480891 1230.9
    ## + Temperature          3     11934 370717 1231.4
    ## + Cautious             4      7997 374654 1237.6
    ## 
    ## Step:  AIC=1212.63
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + VisualAcuity + PrimarilyHand + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + Device + WiFi + 
    ##     Fatigue_3 + Stress_3 + Game_Frequency + Sports_Frequency + 
    ##     Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - VisualAcuity         4     38779 425777 1205.5
    ## - Shooting_Levels      2     10264 397262 1206.3
    ## - PrimarilyHand        2     13663 400661 1207.4
    ## - logAvgHoursExercise  1         1 386999 1207.8
    ## - HoursAweak           1        73 387071 1207.8
    ## - LastNightSleep       1       367 387365 1207.9
    ## - Device               3     31210 418208 1208.1
    ## - Gamer                1      1257 388255 1208.2
    ## - Age                  1      1519 388517 1208.3
    ## - Class                3     33787 420785 1208.8
    ## - Sports_Frequency     1      5428 392426 1209.6
    ## - Distraction          1      6008 393006 1209.8
    ## - Stress_3             2     23074 410072 1210.4
    ## - Game_Frequency       1      8251 395250 1210.5
    ## - Fatigue_3            2     23851 410849 1210.6
    ## - WiFi                 1     14667 401666 1212.6
    ## <none>                             386998 1212.6
    ## - RefreshRate          2     34545 421543 1213.9
    ## - UsePrimaryHand       1     22667 409665 1215.1
    ## - AvgSleepTime         1     23015 410013 1215.2
    ## - CaffeinIntake        1     23215 410213 1215.3
    ## + Noise_Level          2      4347 382651 1220.9
    ## + System               2      2913 384085 1221.4
    ## - InputDevice          4     96745 483743 1222.0
    ## + Temperature          3      9469 377529 1224.0
    ## + Cautious             4      9588 377410 1228.8
    ## 
    ## Step:  AIC=1205.51
    ## avg_time ~ Class + Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + PrimarilyHand + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Class                3     30472 456249 1199.8
    ## - Shooting_Levels      2     13920 439697 1199.9
    ## - Stress_3             2     14882 440659 1200.2
    ## - Gamer                1         5 425782 1200.7
    ## - logAvgHoursExercise  1        20 425797 1200.7
    ## - LastNightSleep       1        55 425832 1200.7
    ## - HoursAweak           1       126 425903 1200.7
    ## - Age                  1       547 426324 1200.8
    ## - PrimarilyHand        2     16925 442702 1200.8
    ## - Device               3     36091 461868 1201.4
    ## - Sports_Frequency     1      4645 430422 1202.0
    ## - Game_Frequency       1      6796 432573 1202.7
    ## - WiFi                 1      8600 434376 1203.2
    ## - Distraction          1      8767 434544 1203.3
    ## - Fatigue_3            2     29208 454985 1204.3
    ## - CaffeinIntake        1     14298 440074 1204.9
    ## <none>                             425777 1205.5
    ## - RefreshRate          2     36358 462134 1206.4
    ## - AvgSleepTime         1     24160 449937 1207.8
    ## - UsePrimaryHand       1     26149 451926 1208.3
    ## + VisualAcuity         4     38779 386998 1212.6
    ## + Noise_Level          2      6781 418996 1213.2
    ## + System               2      3121 422656 1214.3
    ## - InputDevice          4    111805 537582 1216.2
    ## + Temperature          3      5643 420134 1218.4
    ## + Cautious             4     12690 413087 1221.0
    ## 
    ## Step:  AIC=1199.85
    ## avg_time ~ Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + PrimarilyHand + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + 
    ##     Game_Frequency + Sports_Frequency + Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - PrimarilyHand        2     15200 471449 1194.4
    ## - Device               3     34447 490696 1194.7
    ## - logAvgHoursExercise  1       179 456428 1195.0
    ## - LastNightSleep       1       254 456503 1195.1
    ## - HoursAweak           1       318 456567 1195.1
    ## - Gamer                1       525 456774 1195.1
    ## - Sports_Frequency     1      3518 459767 1196.0
    ## - Shooting_Levels      2     21649 477898 1196.1
    ## - Game_Frequency       1      4527 460777 1196.3
    ## - Fatigue_3            2     23691 479940 1196.7
    ## - CaffeinIntake        1      7922 464172 1197.2
    ## - Distraction          1      9878 466127 1197.8
    ## - WiFi                 1     10276 466525 1197.9
    ## - Stress_3             2     31047 487296 1198.6
    ## - RefreshRate          2     32563 488812 1199.0
    ## <none>                             456249 1199.8
    ## - UsePrimaryHand       1     26461 482710 1202.3
    ## - AvgSleepTime         1     30040 486289 1203.2
    ## + Class                3     30472 425777 1205.5
    ## - InputDevice          4    102228 558477 1206.5
    ## - Age                  1     42831 499080 1206.6
    ## + Noise_Level          2      4071 452178 1208.4
    ## + VisualAcuity         4     35464 420785 1208.8
    ## + System               2      1296 454953 1209.2
    ## + Temperature          3      5658 450591 1212.8
    ## + Cautious             4     11104 445145 1216.1
    ## 
    ## Step:  AIC=1194.36
    ## avg_time ~ Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Device               3     24984 496434 1186.4
    ## - Shooting_Levels      2     17731 489180 1189.4
    ## - logAvgHoursExercise  1        35 471484 1189.5
    ## - LastNightSleep       1       138 471587 1189.5
    ## - Sports_Frequency     1       909 472359 1189.8
    ## - Gamer                1       921 472370 1189.8
    ## - HoursAweak           1      3828 475278 1190.5
    ## - Game_Frequency       1      4999 476449 1190.9
    ## - CaffeinIntake        1      6754 478203 1191.3
    ## - Distraction          1      6974 478423 1191.4
    ## - WiFi                 1      9910 481360 1192.2
    ## - RefreshRate          2     30567 502017 1192.7
    ## - Fatigue_3            2     34343 505793 1193.7
    ## - UsePrimaryHand       1     17381 488830 1194.2
    ## <none>                             471449 1194.4
    ## - Stress_3             2     41305 512754 1195.5
    ## - AvgSleepTime         1     28267 499716 1197.0
    ## + PrimarilyHand        2     15200 456249 1199.8
    ## - Age                  1     43111 514560 1200.8
    ## + Class                3     28747 442702 1200.8
    ## - InputDevice          4    110627 582077 1202.1
    ## + Noise_Level          2      5782 465667 1202.5
    ## + VisualAcuity         4     38136 433314 1202.9
    ## + System               2      2180 469269 1203.5
    ## + Temperature          3      7900 463549 1206.8
    ## + Cautious             4     13026 458423 1210.2
    ## 
    ## Step:  AIC=1186.44
    ## avg_time ~ Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels + logAvgHoursExercise
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - logAvgHoursExercise  1        17 496451 1181.6
    ## - LastNightSleep       1       482 496916 1181.7
    ## - Sports_Frequency     1       771 497205 1181.8
    ## - Gamer                1      1229 497663 1181.9
    ## - HoursAweak           1      2382 498815 1182.2
    ## - Game_Frequency       1      2441 498874 1182.2
    ## - Shooting_Levels      2     25184 521618 1183.1
    ## - CaffeinIntake        1      8974 505407 1183.9
    ## - Distraction          1     10184 506618 1184.2
    ## - Fatigue_3            2     30325 526759 1184.4
    ## - WiFi                 1     12878 509311 1184.9
    ## - UsePrimaryHand       1     15112 511545 1185.5
    ## <none>                             496434 1186.4
    ## - RefreshRate          2     43484 539917 1187.5
    ## - Stress_3             2     47521 543954 1188.5
    ## - AvgSleepTime         1     31235 527669 1189.5
    ## - Age                  1     38244 534678 1191.2
    ## + Class                3     28012 468421 1193.5
    ## + Device               3     24984 471449 1194.4
    ## + PrimarilyHand        2      5737 490696 1194.7
    ## + Noise_Level          2      5195 491238 1194.8
    ## + VisualAcuity         4     39298 457135 1195.2
    ## + System               2      1585 494848 1195.8
    ## + Temperature          3      6437 489997 1199.3
    ## - InputDevice          4    141996 638430 1199.5
    ## + Cautious             4     16082 480351 1201.6
    ## 
    ## Step:  AIC=1181.59
    ## avg_time ~ Age + AvgSleepTime + LastNightSleep + HoursAweak + 
    ##     Distraction + Gamer + CaffeinIntake + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + WiFi + Fatigue_3 + Stress_3 + Game_Frequency + 
    ##     Sports_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - LastNightSleep       1       540 496991 1176.9
    ## - Sports_Frequency     1       958 497408 1177.0
    ## - Gamer                1      1217 497668 1177.0
    ## - HoursAweak           1      2420 498871 1177.3
    ## - Game_Frequency       1      2427 498877 1177.3
    ## - Shooting_Levels      2     26592 523043 1178.6
    ## - CaffeinIntake        1      9107 505558 1179.1
    ## - Distraction          1     10562 507013 1179.4
    ## - Fatigue_3            2     31573 528023 1179.8
    ## - WiFi                 1     12865 509316 1180.0
    ## - UsePrimaryHand       1     15160 511611 1180.6
    ## <none>                             496451 1181.6
    ## - RefreshRate          2     44380 540831 1182.9
    ## - Stress_3             2     47944 544395 1183.8
    ## - AvgSleepTime         1     31500 527951 1184.7
    ## + logAvgHoursExercise  1        17 496434 1186.4
    ## - Age                  1     40034 536485 1186.7
    ## + Class                3     27886 468565 1188.7
    ## + Device               3     24967 471484 1189.5
    ## + PrimarilyHand        2      5594 490856 1189.8
    ## + Noise_Level          2      5212 491238 1189.9
    ## + VisualAcuity         4     39221 457230 1190.4
    ## + System               2      1550 494900 1190.9
    ## + Temperature          3      6451 489999 1194.5
    ## - InputDevice          4    142428 638879 1194.7
    ## + Cautious             4     16031 480419 1196.8
    ## 
    ## Step:  AIC=1176.87
    ## avg_time ~ Age + AvgSleepTime + HoursAweak + Distraction + Gamer + 
    ##     CaffeinIntake + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     WiFi + Fatigue_3 + Stress_3 + Game_Frequency + Sports_Frequency + 
    ##     Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Sports_Frequency     1       917 497908 1172.2
    ## - Gamer                1      1223 498214 1172.3
    ## - Game_Frequency       1      2348 499339 1172.6
    ## - HoursAweak           1      2452 499443 1172.6
    ## - Shooting_Levels      2     26600 523591 1173.9
    ## - CaffeinIntake        1      9098 506089 1174.3
    ## - Distraction          1     10276 507267 1174.7
    ## - WiFi                 1     12476 509467 1175.2
    ## - Fatigue_3            2     34112 531103 1175.7
    ## - UsePrimaryHand       1     15027 512017 1175.8
    ## <none>                             496991 1176.9
    ## - RefreshRate          2     44203 541193 1178.1
    ## - Stress_3             2     47405 544396 1178.9
    ## + LastNightSleep       1       540 496451 1181.6
    ## + logAvgHoursExercise  1        75 496916 1181.7
    ## - AvgSleepTime         1     39943 536934 1182.0
    ## - Age                  1     41602 538593 1182.4
    ## + Class                3     28221 468770 1183.9
    ## + Device               3     25335 471656 1184.7
    ## + PrimarilyHand        2      5551 491440 1185.1
    ## + Noise_Level          2      5306 491685 1185.2
    ## + VisualAcuity         4     38058 458933 1186.0
    ## + System               2      1434 495557 1186.2
    ## + Temperature          3      6038 490953 1189.9
    ## - InputDevice          4    146159 643150 1190.7
    ## + Cautious             4     15922 481069 1192.1
    ## 
    ## Step:  AIC=1172.24
    ## avg_time ~ Age + AvgSleepTime + HoursAweak + Distraction + Gamer + 
    ##     CaffeinIntake + UsePrimaryHand + InputDevice + RefreshRate + 
    ##     WiFi + Fatigue_3 + Stress_3 + Game_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Gamer                1      1386 499295 1167.7
    ## - HoursAweak           1      2721 500630 1168.1
    ## - Game_Frequency       1      3143 501051 1168.2
    ## - CaffeinIntake        1      8335 506243 1169.5
    ## - Shooting_Levels      2     28238 526146 1169.6
    ## - Distraction          1     10235 508143 1170.0
    ## - WiFi                 1     12099 510007 1170.5
    ## - Fatigue_3            2     33464 531372 1170.9
    ## - UsePrimaryHand       1     15333 513241 1171.3
    ## <none>                             497908 1172.2
    ## - RefreshRate          2     43934 541842 1173.4
    ## - Stress_3             2     49014 546922 1174.6
    ## + Sports_Frequency     1       917 496991 1176.9
    ## + LastNightSleep       1       500 497408 1177.0
    ## + logAvgHoursExercise  1       325 497583 1177.0
    ## - AvgSleepTime         1     39834 537743 1177.3
    ## - Age                  1     42854 540762 1178.0
    ## + Class                3     27684 470225 1179.4
    ## + Device               3     25150 472758 1180.1
    ## + Noise_Level          2      5635 492273 1180.5
    ## + PrimarilyHand        2      4831 493077 1180.7
    ## + System               2      1516 496392 1181.6
    ## + VisualAcuity         4     37485 460423 1181.6
    ## + Temperature          3      5636 492273 1185.4
    ## - InputDevice          4    145248 643156 1185.8
    ## + Cautious             4     16828 481080 1187.2
    ## 
    ## Step:  AIC=1167.74
    ## avg_time ~ Age + AvgSleepTime + HoursAweak + Distraction + CaffeinIntake + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + WiFi + Fatigue_3 + 
    ##     Stress_3 + Game_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - HoursAweak           1      2588 501882 1163.5
    ## - Game_Frequency       1      5180 504475 1164.2
    ## - CaffeinIntake        1     10350 509645 1165.5
    ## - Distraction          1     10866 510161 1165.7
    ## - Shooting_Levels      2     33060 532355 1166.3
    ## - Fatigue_3            2     33861 533156 1166.5
    ## - WiFi                 1     14221 513515 1166.5
    ## - UsePrimaryHand       1     18935 518229 1167.7
    ## <none>                             499295 1167.7
    ## - RefreshRate          2     43903 543198 1168.9
    ## - Stress_3             2     51385 550680 1170.7
    ## + Gamer                1      1386 497908 1172.2
    ## + Sports_Frequency     1      1081 498214 1172.3
    ## + LastNightSleep       1       503 498792 1172.5
    ## + logAvgHoursExercise  1       290 499005 1172.5
    ## - AvgSleepTime         1     39965 539260 1172.8
    ## - Age                  1     43453 542747 1173.7
    ## + Class                3     28805 470489 1174.7
    ## + Device               3     25513 473781 1175.6
    ## + Noise_Level          2      6074 493221 1175.9
    ## + PrimarilyHand        2      5074 494220 1176.1
    ## + VisualAcuity         4     38863 460432 1176.7
    ## + System               2      1724 497571 1177.0
    ## + Temperature          3      6500 492795 1180.6
    ## + Cautious             4     15940 483355 1183.0
    ## - InputDevice          4    155703 654997 1183.3
    ## 
    ## Step:  AIC=1163.55
    ## avg_time ~ Age + AvgSleepTime + Distraction + CaffeinIntake + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + WiFi + Fatigue_3 + 
    ##     Stress_3 + Game_Frequency + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Game_Frequency       1      4791 506674 1159.9
    ## - Distraction          1      9976 511858 1161.2
    ## - CaffeinIntake        1     10020 511902 1161.2
    ## - Fatigue_3            2     31583 533465 1161.7
    ## - WiFi                 1     13625 515507 1162.2
    ## - Shooting_Levels      2     33587 535469 1162.2
    ## <none>                             501882 1163.5
    ## - UsePrimaryHand       1     20303 522185 1163.8
    ## - RefreshRate          2     41954 543837 1164.2
    ## - Stress_3             2     49054 550936 1165.9
    ## + HoursAweak           1      2588 499295 1167.7
    ## + Sports_Frequency     1      1354 500528 1168.1
    ## + Gamer                1      1253 500630 1168.1
    ## - AvgSleepTime         1     38386 540268 1168.2
    ## + LastNightSleep       1       528 501354 1168.3
    ## + logAvgHoursExercise  1       469 501413 1168.3
    ## - Age                  1     43493 545375 1169.4
    ## + Class                3     29478 472404 1170.3
    ## + PrimarilyHand        2      6881 495002 1171.5
    ## + Noise_Level          2      5836 496046 1171.8
    ## + Device               3     23758 478124 1171.9
    ## + VisualAcuity         4     38846 463036 1172.6
    ## + System               2      2226 499657 1172.7
    ## + Temperature          3      6485 495397 1176.5
    ## + Cautious             4     16785 485098 1178.6
    ## - InputDevice          4    156592 658474 1179.1
    ## 
    ## Step:  AIC=1159.92
    ## avg_time ~ Age + AvgSleepTime + Distraction + CaffeinIntake + 
    ##     UsePrimaryHand + InputDevice + RefreshRate + WiFi + Fatigue_3 + 
    ##     Stress_3 + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Distraction          1      9399 516073 1157.4
    ## - Fatigue_3            2     30803 537476 1157.8
    ## - CaffeinIntake        1     11427 518101 1157.9
    ## - WiFi                 1     17303 523976 1159.4
    ## <none>                             506674 1159.9
    ## - Shooting_Levels      2     40965 547638 1160.2
    ## - UsePrimaryHand       1     21635 528308 1160.5
    ## - RefreshRate          2     42254 548928 1160.5
    ## - Stress_3             2     52770 559444 1163.0
    ## + Game_Frequency       1      4791 501882 1163.5
    ## + Gamer                1      3135 503539 1164.0
    ## + Sports_Frequency     1      2730 503944 1164.1
    ## - AvgSleepTime         1     36788 543462 1164.1
    ## + HoursAweak           1      2199 504475 1164.2
    ## + logAvgHoursExercise  1       480 506193 1164.7
    ## + LastNightSleep       1       393 506281 1164.7
    ## - Age                  1     47627 554301 1166.7
    ## + Class                3     28130 478544 1167.1
    ## + PrimarilyHand        2      7216 499457 1167.8
    ## + Noise_Level          2      5861 500812 1168.1
    ## + System               2      3106 503568 1168.8
    ## + VisualAcuity         4     39132 467542 1169.0
    ## + Device               3     20460 486214 1169.2
    ## + Temperature          3      5374 501300 1173.1
    ## + Cautious             4     15584 491090 1175.3
    ## - InputDevice          4    161112 667786 1176.1
    ## 
    ## Step:  AIC=1157.43
    ## avg_time ~ Age + AvgSleepTime + CaffeinIntake + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + WiFi + Fatigue_3 + Stress_3 + 
    ##     Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Fatigue_3            2     32434 548507 1155.6
    ## - WiFi                 1     16084 532157 1156.5
    ## - CaffeinIntake        1     18303 534376 1157.1
    ## <none>                             516073 1157.4
    ## - Shooting_Levels      2     40953 557026 1157.6
    ## - RefreshRate          2     44636 560709 1158.4
    ## - UsePrimaryHand       1     25136 541209 1158.7
    ## + Distraction          1      9399 506674 1159.9
    ## - AvgSleepTime         1     34735 550808 1161.0
    ## + Game_Frequency       1      4215 511858 1161.2
    ## + Gamer                1      3809 512264 1161.3
    ## + Sports_Frequency     1      2540 513533 1161.7
    ## + HoursAweak           1      1426 514647 1161.9
    ## + logAvgHoursExercise  1      1099 514974 1162.0
    ## + LastNightSleep       1       167 515906 1162.2
    ## - Stress_3             2     62638 578711 1162.5
    ## - Age                  1     45851 561924 1163.5
    ## + Class                3     29900 486173 1164.3
    ## + VisualAcuity         4     43461 472612 1165.5
    ## + PrimarilyHand        2      5354 510719 1165.8
    ## + Device               3     23544 492529 1166.0
    ## + System               2      4423 511650 1166.0
    ## + Noise_Level          2      3899 512174 1166.2
    ## + Temperature          3      5094 510979 1170.7
    ## + Cautious             4     17788 498285 1172.3
    ## - InputDevice          4    170658 686731 1174.8
    ## 
    ## Step:  AIC=1155.57
    ## avg_time ~ Age + AvgSleepTime + CaffeinIntake + UsePrimaryHand + 
    ##     InputDevice + RefreshRate + WiFi + Stress_3 + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - CaffeinIntake        1     14370 562877 1154.0
    ## - WiFi                 1     18603 567110 1155.0
    ## <none>                             548507 1155.6
    ## - RefreshRate          2     49010 597517 1156.9
    ## - Stress_3             2     50136 598643 1157.1
    ## + Fatigue_3            2     32434 516073 1157.4
    ## + Distraction          1     11031 537476 1157.8
    ## - UsePrimaryHand       1     33482 581989 1158.3
    ## - Shooting_Levels      2     57337 605844 1158.7
    ## + Gamer                1      4553 543954 1159.4
    ## + Game_Frequency       1      3318 545189 1159.7
    ## + LastNightSleep       1      2410 546097 1159.9
    ## - AvgSleepTime         1     41446 589953 1160.1
    ## + HoursAweak           1       952 547555 1160.2
    ## + Sports_Frequency     1       875 547632 1160.2
    ## - Age                  1     42449 590956 1160.3
    ## + logAvgHoursExercise  1       194 548313 1160.4
    ## + PrimarilyHand        2      7688 540819 1163.5
    ## + VisualAcuity         4     46810 501697 1163.5
    ## + Class                3     25855 522652 1163.9
    ## + System               2      4806 543701 1164.2
    ## + Device               3     23110 525397 1164.6
    ## + Noise_Level          2      1086 547421 1165.0
    ## + Temperature          3      8404 540103 1168.2
    ## + Cautious             4     23783 524724 1169.3
    ## - InputDevice          4    164875 713382 1170.0
    ## 
    ## Step:  AIC=1154.05
    ## avg_time ~ Age + AvgSleepTime + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + WiFi + Stress_3 + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - WiFi                 1     16704 579581 1153.0
    ## <none>                             562877 1154.0
    ## - RefreshRate          2     47383 610260 1154.8
    ## + Distraction          1     17472 545405 1154.8
    ## - UsePrimaryHand       1     28044 590921 1155.5
    ## + CaffeinIntake        1     14370 548507 1155.6
    ## - Stress_3             2     54950 617826 1156.3
    ## - Shooting_Levels      2     56682 619558 1156.7
    ## + Gamer                1      8444 554433 1157.0
    ## + Fatigue_3            2     28501 534376 1157.1
    ## + Game_Frequency       1      4306 558570 1157.9
    ## - AvgSleepTime         1     42193 605070 1158.5
    ## + LastNightSleep       1      1688 561188 1158.5
    ## + logAvgHoursExercise  1      1178 561698 1158.6
    ## + HoursAweak           1       909 561968 1158.7
    ## + Sports_Frequency     1        96 562781 1158.9
    ## - Age                  1     57490 620367 1161.7
    ## + System               2      6116 556760 1162.4
    ## + Device               3     26692 536185 1162.4
    ## + PrimarilyHand        2      6096 556781 1162.4
    ## + Noise_Level          2      1298 561579 1163.5
    ## + Class                3     19876 543000 1164.0
    ## + VisualAcuity         4     39616 523260 1164.1
    ## + Temperature          3     10323 552554 1166.2
    ## + Cautious             4     17666 545210 1169.4
    ## - InputDevice          4    186676 749553 1171.6
    ## 
    ## Step:  AIC=1152.96
    ## avg_time ~ Age + AvgSleepTime + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Stress_3 + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - RefreshRate          2     38588 618169 1151.5
    ## <none>                             579581 1153.0
    ## - Stress_3             2     46025 625606 1153.1
    ## - UsePrimaryHand       1     25145 604725 1153.6
    ## - Shooting_Levels      2     50150 629731 1154.0
    ## + WiFi                 1     16704 562877 1154.0
    ## + Distraction          1     15752 563829 1154.3
    ## + Gamer                1     12747 566834 1155.0
    ## + CaffeinIntake        1     12471 567110 1155.0
    ## + Fatigue_3            2     31821 547760 1155.4
    ## + Game_Frequency       1      7149 572432 1156.2
    ## - AvgSleepTime         1     39927 619508 1156.7
    ## + logAvgHoursExercise  1      1643 577938 1157.5
    ## + HoursAweak           1      1097 578484 1157.6
    ## + LastNightSleep       1       552 579029 1157.7
    ## + Sports_Frequency     1        65 579516 1157.8
    ## - Age                  1     56084 635665 1160.0
    ## + System               2      8240 571341 1160.8
    ## + Device               3     28221 551360 1161.1
    ## + PrimarilyHand        2      5849 573732 1161.4
    ## + Noise_Level          2      1237 578344 1162.4
    ## + Class                3     20137 559444 1163.0
    ## + VisualAcuity         4     37486 542095 1163.8
    ## + Temperature          3     12005 567576 1164.8
    ## + Cautious             4     17982 561599 1168.3
    ## - InputDevice          4    206012 785593 1172.8
    ## 
    ## Step:  AIC=1151.55
    ## avg_time ~ Age + AvgSleepTime + UsePrimaryHand + InputDevice + 
    ##     Stress_3 + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - Stress_3             2     31408 649578 1148.2
    ## - UsePrimaryHand       1     20059 638228 1150.8
    ## <none>                             618169 1151.5
    ## - AvgSleepTime         1     28131 646300 1152.4
    ## + Distraction          1     18466 599703 1152.5
    ## + RefreshRate          2     38588 579581 1153.0
    ## + Gamer                1     12207 605962 1153.8
    ## + CaffeinIntake        1     11635 606535 1154.0
    ## + Fatigue_3            2     32187 585983 1154.4
    ## + WiFi                 1      7909 610260 1154.8
    ## + Game_Frequency       1      6661 611508 1155.0
    ## + logAvgHoursExercise  1      5245 612925 1155.3
    ## + HoursAweak           1      3800 614370 1155.6
    ## - Shooting_Levels      2     70043 688212 1155.7
    ## + LastNightSleep       1       803 617367 1156.2
    ## + Sports_Frequency     1        16 618153 1156.4
    ## + Device               3     41828 576341 1157.1
    ## - Age                  1     58968 677138 1158.5
    ## + System               2      9841 608328 1159.2
    ## + PrimarilyHand        2      2122 616047 1160.8
    ## + Noise_Level          2       333 617836 1161.2
    ## + Class                3     17642 600527 1162.4
    ## + VisualAcuity         4     38691 579479 1162.7
    ## + Temperature          3     16185 601985 1162.7
    ## + Cautious             4     12811 605358 1168.3
    ## - InputDevice          4    271562 889731 1179.1
    ## 
    ## Step:  AIC=1148.23
    ## avg_time ~ Age + AvgSleepTime + UsePrimaryHand + InputDevice + 
    ##     Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## - UsePrimaryHand       1     11011 660588 1145.5
    ## + Distraction          1     28950 620627 1147.2
    ## - AvgSleepTime         1     24124 673701 1148.1
    ## <none>                             649578 1148.2
    ## + Gamer                1     16505 633072 1149.8
    ## + CaffeinIntake        1     15521 634056 1150.0
    ## + Game_Frequency       1      8352 641225 1151.4
    ## + Stress_3             2     31408 618169 1151.5
    ## + HoursAweak           1      4977 644601 1152.1
    ## + WiFi                 1      3966 645611 1152.3
    ## + logAvgHoursExercise  1      1322 648256 1152.8
    ## + Sports_Frequency     1       647 648930 1153.0
    ## + LastNightSleep       1        20 649558 1153.1
    ## + RefreshRate          2     23972 625606 1153.1
    ## + Device               3     45013 604564 1153.5
    ## + Fatigue_3            2     21485 628092 1153.6
    ## - Shooting_Levels      2     81570 731148 1153.8
    ## + System               2     11376 638202 1155.7
    ## + Class                3     33514 616064 1156.0
    ## + PrimarilyHand        2      3633 645945 1157.2
    ## - Age                  1     75656 725234 1157.6
    ## + Noise_Level          2      1087 648490 1157.7
    ## + Temperature          3     12004 637574 1160.4
    ## + VisualAcuity         4     28589 620989 1161.9
    ## + Cautious             4     18355 631223 1164.0
    ## - InputDevice          4    261468 911045 1172.4
    ## 
    ## Step:  AIC=1145.54
    ## avg_time ~ Age + AvgSleepTime + InputDevice + Shooting_Levels
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## + Distraction          1     29814 630774 1144.4
    ## - AvgSleepTime         1     21999 682587 1144.9
    ## <none>                             660588 1145.5
    ## + Gamer                1     21720 638869 1146.1
    ## + CaffeinIntake        1     11642 648946 1148.1
    ## + UsePrimaryHand       1     11011 649578 1148.2
    ## + Game_Frequency       1      8848 651740 1148.7
    ## - Shooting_Levels      2     73292 733880 1149.4
    ## + HoursAweak           1      4211 656378 1149.6
    ## + WiFi                 1      3701 656887 1149.7
    ## + logAvgHoursExercise  1      1219 659369 1150.2
    ## + Sports_Frequency     1       925 659663 1150.2
    ## + Fatigue_3            2     25158 635430 1150.2
    ## + LastNightSleep       1         2 660586 1150.4
    ## + RefreshRate          2     22553 638035 1150.8
    ## + Stress_3             2     22360 638228 1150.8
    ## + Device               3     38732 621856 1152.3
    ## + Class                3     35674 624914 1153.0
    ## + System               2     10872 649716 1153.1
    ## + PrimarilyHand        2      2970 657618 1154.7
    ## + Noise_Level          2       307 660281 1155.2
    ## - Age                  1     80964 741552 1155.6
    ## + Temperature          3     13189 647399 1157.5
    ## + VisualAcuity         4     31287 629301 1158.7
    ## + Cautious             4     19194 641394 1161.2
    ## - InputDevice          4    276674 937262 1171.2
    ## 
    ## Step:  AIC=1144.44
    ## avg_time ~ Age + AvgSleepTime + InputDevice + Shooting_Levels + 
    ##     Distraction
    ## 
    ##                       Df Sum of Sq    RSS    AIC
    ## <none>                             630774 1144.4
    ## - AvgSleepTime         1     26881 657655 1145.0
    ## - Distraction          1     29814 660588 1145.5
    ## + Gamer                1     16241 614533 1145.9
    ## + UsePrimaryHand       1     10147 620627 1147.2
    ## + Game_Frequency       1     10002 620772 1147.2
    ## - Shooting_Levels      2     66798 697572 1147.7
    ## + WiFi                 1      5756 625018 1148.1
    ## + CaffeinIntake        1      4188 626586 1148.4
    ## + logAvgHoursExercise  1      2644 628130 1148.8
    ## + HoursAweak           1      2039 628735 1148.9
    ## + Fatigue_3            2     24828 605946 1149.0
    ## + Sports_Frequency     1      1474 629300 1149.0
    ## + LastNightSleep       1       333 630441 1149.2
    ## + RefreshRate          2     21687 609087 1149.7
    ## + Stress_3             2     14083 616691 1151.2
    ## + Device               3     31374 599400 1152.4
    ## + Class                3     30755 600019 1152.6
    ## + Noise_Level          2      6423 624351 1152.8
    ## + System               2      6359 624415 1152.8
    ## + PrimarilyHand        2      3173 627601 1153.5
    ## - Age                  1     75201 705976 1154.1
    ## + Temperature          3     14039 616735 1156.1
    ## + VisualAcuity         4     27428 603346 1158.1
    ## + Cautious             4     14802 615972 1160.8
    ## - InputDevice          4    247894 878668 1167.8

    ## 
    ## Call:
    ## lm(formula = avg_time ~ Age + AvgSleepTime + InputDevice + Shooting_Levels + 
    ##     Distraction, data = Survey_cleaned)
    ## 
    ## Coefficients:
    ##                        (Intercept)                                 Age  
    ##                            113.638                              15.768  
    ##                       AvgSleepTime                    InputDeviceMouse  
    ##                             14.512                             -88.056  
    ##                InputDeviceKeyboard                 InputDeviceTrackpad  
    ##                             56.524                               8.402  
    ##            InputDeviceTouch screen  Shooting_LevelsIntermediate Levels  
    ##                            -28.410                              22.652  
    ##          Shooting_LevelsLow Levels                      DistractionYes  
    ##                             58.928                              37.854

![](Code_files/figure-gfm/unnamed-chunk-8-1.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-8-2.png)<!-- -->

    ## 49 x 1 sparse Matrix of class "dgCMatrix"
    ##                                                        s1
    ## (Intercept)                                    434.637178
    ## (Intercept)                                      .       
    ## ClassJunior                                      .       
    ## ClassSenior                                      .       
    ## ClassGraduate student                           38.495659
    ## Age                                              4.207794
    ## AvgSleepTime                                     4.959268
    ## LastNightSleep                                   .       
    ## HoursAweak                                       .       
    ## DistractionYes                                  13.502323
    ## TemperatureWarm                                  .       
    ## TemperatureNeutral                               .       
    ## TemperatureCold                                  .       
    ## GamerYes                                       -15.617365
    ## CaffeinIntakeYes                                 2.454916
    ## VisualAcuityExcellent                            .       
    ## VisualAcuityGood                                 .       
    ## VisualAcuityPoor                                 .       
    ## VisualAcuityVery Poor                            .       
    ## PrimarilyHandLeft hand                           .       
    ## PrimarilyHandAmbidextrous (both hands equally)   .       
    ## UsePrimaryHandNo                                 .       
    ## CautiousVery cautious                            .       
    ## CautiousModerately cautious                     -2.849909
    ## CautiousSlightly cautious                        1.386369
    ## CautiousNot cautious at all                      .       
    ## InputDeviceMouse                               -64.358406
    ## InputDeviceKeyboard                              .       
    ## InputDeviceTrackpad                              0.167877
    ## InputDeviceTouch screen                          .       
    ## RefreshRateMid-Range                             .       
    ## RefreshRateStandard                              2.010429
    ## DeviceiPad(Tablet                                .       
    ## DeviceiPhone(Smartphone                          .       
    ## DeviceLaptop                                    31.126876
    ## WiFiStable                                       .       
    ## Fatigue_3Moderately Fatigue                      .       
    ## Fatigue_3Low Fatigue                             .       
    ## Stress_3Moderately Stress                        .       
    ## Stress_3Low Stress                              -7.020384
    ## Noise_LevelModerately Noise                      .       
    ## Noise_LevelLow Noise                             .       
    ## Game_FrequencyLow Frequency                      .       
    ## Sports_FrequencyLow Frequency                    .       
    ## Shooting_LevelsIntermediate Levels               .       
    ## Shooting_LevelsLow Levels                       25.202538
    ## SystemLinux                                      .       
    ## SystemWindows                                   -5.059475
    ## logAvgHoursExercise                              .

![](Code_files/figure-gfm/unnamed-chunk-8-3.png)<!-- -->![](Code_files/figure-gfm/unnamed-chunk-8-4.png)<!-- -->

    ## 49 x 1 sparse Matrix of class "dgCMatrix"
    ##                                                         s1
    ## (Intercept)                                    368.5377698
    ## (Intercept)                                      .        
    ## ClassJunior                                      9.2179213
    ## ClassSenior                                     -4.0525003
    ## ClassGraduate student                           37.7032688
    ## Age                                              5.1690070
    ## AvgSleepTime                                     6.5175895
    ## LastNightSleep                                   3.1701663
    ## HoursAweak                                      -0.5404607
    ## DistractionYes                                  16.6195321
    ## TemperatureWarm                                 -8.2325000
    ## TemperatureNeutral                               3.5619055
    ## TemperatureCold                                  4.6298805
    ## GamerYes                                       -13.5314439
    ## CaffeinIntakeYes                                13.9420796
    ## VisualAcuityExcellent                           -4.0959600
    ## VisualAcuityGood                               -11.0979381
    ## VisualAcuityPoor                                 4.1943588
    ## VisualAcuityVery Poor                          -64.8507779
    ## PrimarilyHandLeft hand                          -8.0711916
    ## PrimarilyHandAmbidextrous (both hands equally)  13.1496551
    ## UsePrimaryHandNo                                23.8720903
    ## CautiousVery cautious                            2.9004930
    ## CautiousModerately cautious                     -7.9892714
    ## CautiousSlightly cautious                       10.2090207
    ## CautiousNot cautious at all                      7.5536393
    ## InputDeviceMouse                               -28.1947413
    ## InputDeviceKeyboard                             43.8645305
    ## InputDeviceTrackpad                             22.3201868
    ## InputDeviceTouch screen                          3.9222785
    ## RefreshRateMid-Range                             6.6727554
    ## RefreshRateStandard                             18.5185918
    ## DeviceiPad(Tablet                              -14.9492712
    ## DeviceiPhone(Smartphone                         45.4042015
    ## DeviceLaptop                                    26.9626098
    ## WiFiStable                                     -29.9684480
    ## Fatigue_3Moderately Fatigue                     10.8075295
    ## Fatigue_3Low Fatigue                             6.1120911
    ## Stress_3Moderately Stress                        7.7363361
    ## Stress_3Low Stress                             -12.1926836
    ## Noise_LevelModerately Noise                      1.0909481
    ## Noise_LevelLow Noise                             1.2814921
    ## Game_FrequencyLow Frequency                     11.0270908
    ## Sports_FrequencyLow Frequency                    4.9663124
    ## Shooting_LevelsIntermediate Levels              -3.6278837
    ## Shooting_LevelsLow Levels                       17.7413953
    ## SystemLinux                                    -27.5803947
    ## SystemWindows                                  -14.1677818
    ## logAvgHoursExercise                              0.4618736

    ## 
    ## Call:
    ## lm(formula = avg_time ~ Class + AvgSleepTime + CaffeinIntake + 
    ##     VisualAcuity + PrimarilyHand + UsePrimaryHand + InputDevice + 
    ##     RefreshRate + Device + WiFi + Fatigue_3 + Stress_3 + Game_Frequency, 
    ##     data = Survey_cleaned)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -138.894  -31.697   -6.822   33.277  192.712 
    ## 
    ## Coefficients:
    ##                                                Estimate Std. Error t value
    ## (Intercept)                                     425.317    105.952   4.014
    ## ClassJunior                                      38.217     15.069   2.536
    ## ClassSenior                                      13.981     18.142   0.771
    ## ClassGraduate student                           130.035     28.253   4.602
    ## AvgSleepTime                                     15.003      6.128   2.448
    ## CaffeinIntakeYes                                 39.404     14.849   2.654
    ## VisualAcuityExcellent                           -69.883     25.778  -2.711
    ## VisualAcuityGood                                -82.245     26.164  -3.143
    ## VisualAcuityPoor                                -80.451     42.878  -1.876
    ## VisualAcuityVery Poor                          -117.412     75.133  -1.563
    ## PrimarilyHandLeft hand                          -41.362     35.280  -1.172
    ## PrimarilyHandAmbidextrous (both hands equally)   32.110     36.761   0.873
    ## UsePrimaryHandNo                                 71.433     33.181   2.153
    ## InputDeviceMouse                                -31.564     68.331  -0.462
    ## InputDeviceKeyboard                              68.597     85.193   0.805
    ## InputDeviceTrackpad                              45.508     67.390   0.675
    ## InputDeviceTouch screen                          -3.979     75.914  -0.052
    ## RefreshRateMid-Range                             28.670     19.571   1.465
    ## RefreshRateStandard                              55.821     18.704   2.984
    ## DeviceiPad(Tablet                               -11.942     53.720  -0.222
    ## DeviceiPhone(Smartphone                         140.629     63.237   2.224
    ## DeviceLaptop                                     38.479     21.151   1.819
    ## WiFiStable                                      -65.223     49.872  -1.308
    ## Fatigue_3Moderately Fatigue                      62.065     20.502   3.027
    ## Fatigue_3Low Fatigue                             54.603     20.072   2.720
    ## Stress_3Moderately Stress                         7.351     17.207   0.427
    ## Stress_3Low Stress                              -35.489     18.291  -1.940
    ## Game_FrequencyLow Frequency                      26.502     12.463   2.127
    ##                                                Pr(>|t|)    
    ## (Intercept)                                    0.000115 ***
    ## ClassJunior                                    0.012744 *  
    ## ClassSenior                                    0.442730    
    ## ClassGraduate student                          1.22e-05 ***
    ## AvgSleepTime                                   0.016081 *  
    ## CaffeinIntakeYes                               0.009250 ** 
    ## VisualAcuityExcellent                          0.007885 ** 
    ## VisualAcuityGood                               0.002193 ** 
    ## VisualAcuityPoor                               0.063504 .  
    ## VisualAcuityVery Poor                          0.121248    
    ## PrimarilyHandLeft hand                         0.243804    
    ## PrimarilyHandAmbidextrous (both hands equally) 0.384468    
    ## UsePrimaryHandNo                               0.033711 *  
    ## InputDeviceMouse                               0.645123    
    ## InputDeviceKeyboard                            0.422595    
    ## InputDeviceTrackpad                            0.501031    
    ## InputDeviceTouch screen                        0.958303    
    ## RefreshRateMid-Range                           0.146044    
    ## RefreshRateStandard                            0.003564 ** 
    ## DeviceiPad(Tablet                              0.824536    
    ## DeviceiPhone(Smartphone                        0.028387 *  
    ## DeviceLaptop                                   0.071840 .  
    ## WiFiStable                                     0.193907    
    ## Fatigue_3Moderately Fatigue                    0.003131 ** 
    ## Fatigue_3Low Fatigue                           0.007680 ** 
    ## Stress_3Moderately Stress                      0.670124    
    ## Stress_3Low Stress                             0.055140 .  
    ## Game_FrequencyLow Frequency                    0.035894 *  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 64.09 on 101 degrees of freedom
    ## Multiple R-squared:  0.6454, Adjusted R-squared:  0.5506 
    ## F-statistic: 6.808 on 27 and 101 DF,  p-value: 4.733e-13

    ##                    GVIF Df GVIF^(1/(2*Df))
    ## Class          1.882939  3        1.111235
    ## AvgSleepTime   1.242119  1        1.114504
    ## CaffeinIntake  1.291534  1        1.136457
    ## VisualAcuity   1.918683  4        1.084864
    ## PrimarilyHand  2.157614  2        1.211974
    ## UsePrimaryHand 1.774313  1        1.332033
    ## InputDevice    6.483538  4        1.263213
    ## RefreshRate    2.266885  2        1.227036
    ## Device         6.241066  3        1.356885
    ## WiFi           1.192216  1        1.091886
    ## Fatigue_3      1.749256  2        1.150041
    ## Stress_3       1.897225  2        1.173626
    ## Game_Frequency 1.198209  1        1.094627

    ## Analysis of Variance Table
    ## 
    ## Response: avg_time
    ##                             Df Sum Sq Mean Sq F value    Pr(>F)    
    ## Class                        3  70764   23588  4.6315 0.0047165 ** 
    ## AvgSleepTime                 1  51358   51358 10.0842 0.0020692 ** 
    ## CaffeinIntake                1  44474   44474  8.7324 0.0040213 ** 
    ## VisualAcuity                 4 112552   28138  5.5249 0.0005194 ***
    ## UsePrimaryHand               1   8500    8500  1.6689 0.1998229    
    ## RefreshRate                  2 133463   66731 13.1028 1.061e-05 ***
    ## Device                       3  90243   30081  5.9064 0.0010229 ** 
    ## WiFi                         1  19165   19165  3.7631 0.0556363 .  
    ## Fatigue_3                    2  29443   14722  2.8906 0.0608947 .  
    ## Stress_3                     2  33627   16814  3.3014 0.0414977 *  
    ## Game_Frequency               1  31181   31181  6.1224 0.0152893 *  
    ## Class:AvgSleepTime           3   4805    1602  0.3145 0.8148506    
    ## AvgSleepTime:CaffeinIntake   1   2820    2820  0.5538 0.4587899    
    ## AvgSleepTime:VisualAcuity    3   4600    1533  0.3011 0.8245341    
    ## AvgSleepTime:PrimarilyHand   2  19859    9929  1.9497 0.1484902    
    ## AvgSleepTime:UsePrimaryHand  1   4988    4988  0.9794 0.3250906    
    ## AvgSleepTime:RefreshRate     2  21825   10912  2.1426 0.1234963    
    ## AvgSleepTime:Device          2  20285   10143  1.9915 0.1426606    
    ## AvgSleepTime:WiFi            1    162     162  0.0318 0.8588795    
    ## AvgSleepTime:Fatigue_3       2  13297    6648  1.3054 0.2763119    
    ## AvgSleepTime:Stress_3        2   8767    4383  0.8607 0.4264506    
    ## AvgSleepTime:Game_Frequency  1    694     694  0.1363 0.7129253    
    ## Residuals                   87 443084    5093                      
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Analysis of Variance Table
    ## 
    ## Response: avg_time
    ##                 Df Sum Sq Mean Sq F value    Pr(>F)    
    ## Class            3  70764   23588  4.6294 0.0043877 ** 
    ## AvgSleepTime     1  51358   51358 10.0797 0.0019583 ** 
    ## CaffeinIntake    1  44474   44474  8.7285 0.0038528 ** 
    ## VisualAcuity     4 112552   28138  5.5225 0.0004426 ***
    ## UsePrimaryHand   1   8500    8500  1.6682 0.1992846    
    ## RefreshRate      2 133463   66731 13.0969 8.168e-06 ***
    ## Device           3  90243   30081  5.9038 0.0009104 ***
    ## WiFi             1  19165   19165  3.7614 0.0550824 .  
    ## Fatigue_3        2  29443   14722  2.8893 0.0599655 .  
    ## Stress_3         2  33627   16814  3.2999 0.0406746 *  
    ## Game_Frequency   1  31181   31181  6.1196 0.0149411 *  
    ## Residuals      107 545186    5095                      
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Analysis of Variance Table
    ## 
    ## Response: avg_time
    ##                 Df Sum Sq Mean Sq F value    Pr(>F)    
    ## Class            3  70764   23588  4.4860 0.0052020 ** 
    ## AvgSleepTime     1  51358   51358  9.7673 0.0022721 ** 
    ## CaffeinIntake    1  44474   44474  8.4581 0.0043975 ** 
    ## VisualAcuity     4 112552   28138  5.3513 0.0005638 ***
    ## RefreshRate      2 124040   62020 11.7950 2.286e-05 ***
    ## Device           3  82181   27394  5.2098 0.0021120 ** 
    ## Fatigue_3        2  39237   19619  3.7311 0.0270521 *  
    ## Game_Frequency   1  44518   44518  8.4664 0.0043787 ** 
    ## UsePrimaryHand   1  22436   22436  4.2668 0.0412128 *  
    ## Residuals      110 578395    5258                      
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ##                     GVIF Df GVIF^(1/(2*Df))
    ## Age             1.083396  1        1.040863
    ## AvgSleepTime    1.064404  1        1.031699
    ## InputDevice     1.183969  4        1.021333
    ## Shooting_Levels 1.095841  2        1.023144
    ## Distraction     1.053618  1        1.026459

    ## 
    ## Call:
    ## lm(formula = avg_time ~ Age + AvgSleepTime + InputDevice + Shooting_Levels + 
    ##     Distraction, data = Survey_cleaned)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -128.316  -49.446   -2.732   51.405  201.703 
    ## 
    ## Coefficients:
    ##                                    Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)                         113.638    124.733   0.911 0.364110    
    ## Age                                  15.768      4.186   3.767 0.000259 ***
    ## AvgSleepTime                         14.512      6.444   2.252 0.026159 *  
    ## InputDeviceMouse                    -88.056     74.274  -1.186 0.238156    
    ## InputDeviceKeyboard                  56.524     89.861   0.629 0.530541    
    ## InputDeviceTrackpad                   8.402     73.690   0.114 0.909417    
    ## InputDeviceTouch screen             -28.410     76.999  -0.369 0.712813    
    ## Shooting_LevelsIntermediate Levels   22.652     20.549   1.102 0.272535    
    ## Shooting_LevelsLow Levels            58.928     18.504   3.185 0.001851 ** 
    ## DistractionYes                       37.854     15.961   2.372 0.019315 *  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 72.81 on 119 degrees of freedom
    ## Multiple R-squared:  0.4609, Adjusted R-squared:  0.4201 
    ## F-statistic:  11.3 on 9 and 119 DF,  p-value: 1.231e-12

    ## Analysis of Variance Table
    ## 
    ## Response: avg_time
    ##                               Df Sum Sq Mean Sq F value    Pr(>F)    
    ## Age                            1  37863   37863  5.9245 0.0164430 *  
    ## AvgSleepTime                   1  60340   60340  9.4417 0.0026391 ** 
    ## Shooting_Levels                2 134489   67245 10.5220 6.278e-05 ***
    ## Distraction                    1  58594   58594  9.1684 0.0030297 ** 
    ## Age:Shooting_Levels            2 120026   60013  9.3905 0.0001651 ***
    ## Age:Distraction                1   1556    1556  0.2435 0.6225874    
    ## AvgSleepTime:Shooting_Levels   2   9066    4533  0.7093 0.4941076    
    ## AvgSleepTime:Distraction       1    288     288  0.0451 0.8321666    
    ## Residuals                    117 747731    6391                      
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Analysis of Variance Table
    ## 
    ## Response: avg_time
    ##                      Df Sum Sq Mean Sq F value    Pr(>F)    
    ## Age                   1  37863   37863  6.0390 0.0154107 *  
    ## AvgSleepTime          1  60340   60340  9.6240 0.0023906 ** 
    ## Shooting_Levels       2 134489   67245 10.7252 5.151e-05 ***
    ## Distraction           1  58594   58594  9.3455 0.0027516 ** 
    ## Age:Shooting_Levels   2 120026   60013  9.5718 0.0001383 ***
    ## Residuals           121 758642    6270                      
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Warning: not plotting observations with leverage one:
    ##   14

![](Code_files/figure-gfm/unnamed-chunk-13-1.png)<!-- -->

    ## 
    ##  studentized Breusch-Pagan test
    ## 
    ## data:  AICmod4
    ## BP = 26.426, df = 18, p-value = 0.0904

    ## 
    ##  Shapiro-Wilk normality test
    ## 
    ## data:  residuals(AICmod4)
    ## W = 0.98837, p-value = 0.3476

    ## 
    ##  Durbin-Watson test
    ## 
    ## data:  AICmod4
    ## DW = 2.1674, p-value = 0.8238
    ## alternative hypothesis: true autocorrelation is greater than 0

![](Code_files/figure-gfm/unnamed-chunk-14-1.png)<!-- -->

    ## 
    ##  studentized Breusch-Pagan test
    ## 
    ## data:  BICmod3
    ## BP = 18.42, df = 7, p-value = 0.01021

    ## 
    ##  Shapiro-Wilk normality test
    ## 
    ## data:  residuals(BICmod3)
    ## W = 0.99066, p-value = 0.5411

    ## 
    ##  Durbin-Watson test
    ## 
    ## data:  BICmod3
    ## DW = 1.649, p-value = 0.02156
    ## alternative hypothesis: true autocorrelation is greater than 0

    ## 
    ##  studentized Breusch-Pagan test
    ## 
    ## data:  BICmod3_weighted
    ## BP = 9.2754, df = 7, p-value = 0.2335

    ## 
    ##  Shapiro-Wilk normality test
    ## 
    ## data:  residuals(BICmod3_weighted)
    ## W = 0.99034, p-value = 0.511

    ## [1] 66.96031

![](Code_files/figure-gfm/unnamed-chunk-15-1.png)<!-- -->

    ## [1] 76.78642

![](Code_files/figure-gfm/unnamed-chunk-15-2.png)<!-- -->

    ## [1] 70.01466

![](Code_files/figure-gfm/unnamed-chunk-15-3.png)<!-- -->

    ## [1] 62.5103

![](Code_files/figure-gfm/unnamed-chunk-15-4.png)<!-- -->
