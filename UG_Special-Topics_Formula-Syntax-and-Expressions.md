**MATHS FUNCTIONS**

Each of the maths functions returns a high precision value (double), where acos, atan et al return the arc cosine, tan etc and the acosh, atanh return the arc cosine of the hypoteneuse etc.

The exp() functions returns e raised to the power of p1. Lastly, isinf returns true if the expression evaluates to an infinite value and isnan if the expression evaluates to an undefined value (not a number).

* cos(p1)
* tan(p1)
* sin(p1)
* acos(p1)
* atan(p1)
* asin(p1)
* cosh(p1)
* tanh(p1)
* sinh(p1)
* acosh(p1)
* atanh(p1)
* asinh(p1)
* exp(p1)
* log(p1)
* log10(p1)
* ceil(p1)
* floor(p1)
* round(p1)
* fabs(p1)
* isinf(p1)
* isnan(p1)

**LIST / VECTOR REDUCE FUNCTIONS**

Each of the reduce functions operate on a variable list of inputs; sum(1,2,3) would return 6. You can also supply a vector or list of vectors to reduce them.

* sum(...) - evaluate a sum of all supplied values
* mean(...) - evaluate the mean average of all supplied values
* max(...) - return the maximal value in the supplied values
* min(...) - return the minimal value in the supplied values
* count(...) - return a count of values supplied
* which(cond, ...) - filter the values returning a vector containing values that meet the condition cond. The condition references 'x' to evaluate for each supplied value e.g. which(x>0, 1,2,-1) would return a vector containing the values 1 and 2, but not -1 since it is not greater than zero.

**MODEL FUNCTIONS**
* estimate(model, (cp|ftp|w'|pmax|x))
* vdottime(VDOT, distance)

**MEAN MAX and ZONE FUNCTIONS**
* best(...)
* tiz(...)

**PMC FUNCTIONS**
* lts(p1)
* sts(p1)
* sb(p1)
* rr(p1)
* ctl
* tsb
* atl

**SET/UNSET FUNCTIONS**
* set(symbol, value, filter) - set 'symbol' to 'value' for activities that match 'filter', e.g. set(Sport, "Bike", "Data contains 'P'")
* unset(symbol, filter) - clear 'symbol' for activities that match 'filter'
* isset(symbol) - if 'symbol' is set to nonzero or non-blank returns true

**CONFIGURED PARAMETERS**
* config(cranklength)
* config(cp)
* config(w)
* config(pmax)
* config(cv)
* config(scv)
* config(height)
* config(weight)
* config(lthr)
* config(maxhr)
* config(rhr)
* config(units)

**HIGH PRECISION CONSTANTS**
* const(e)
* const(pi)

**DATE RANGE SELECTION**

* daterange(start)
* daterange(stop)

**RIDE SAMPLE DATA**

* SECS
* CADENCE
* CADENCED
* HEARTRATE
* HEARTRATED
* DISTANCE
* SPEED
* SPEEDD
* TORQUE
* TORQUED
* POWER
* POWERD
* NP
* ALTITUDE
* LON
* LAT
* HEADWIND
* SLOPE
* TEMPERATURE
* BALANCE
* LEFTEFFECTIVENESS
* RIGHTEFFECTIVENESS
* LEFTSMOOTHNESS
* RIGHTSMOOTHNESS
* SMO2
* THB
* RUNVERT
* RUNCADENCE
* RUNCONTACT
* LEFTPCO
* RIGHTPCO
* LEFTPPB
* RIGHTPPB
* LEFTPPE
* RIGHTPPE
* LEFTPPPB
* RIGHTPPPB
* LEFTPPPE
* RIGHTPPPE

**BUILT-IN METRICS**

* __1_min_Peak_Pace__ -	1 min Peak Pace
* __1_min_Peak_Pace_Swim__ -	1 min Peak Pace Swim
* __1_min_Peak_Power__ -	1 min Peak Power
* __1_min_Peak_Power_HR__ -	Average Heart Rate for 1 min Peak Power interval
* __1_min_Peak_WPK__ -	1 min Peak Power relative to Athlete Weight.
* __1_sec_Peak_Power__ -	1 sec Peak Power
* __1_sec_Peak_WPK__ -	1 sec Peak Power relative to Athlete Weight.
* __10_min_Peak_Pace__ -	10 min Peak Pace
* __10_min_Peak_Pace_Swim__ -	10 min Peak Pace Swim
* __10_min_Peak_Power__ -	10 min Peak Power
* __10_min_Peak_Power_HR__ -	Average Heart Rate for 10 min Peak Power interval
* __10_min_Peak_WPK__ -	10 min Peak Power relative to Athlete Weight.
* __10_sec_Peak_Pace__ -	10 sec Peak Pace
* __10_sec_Peak_Pace_Swim__ -	10 sec Peak Pace Swim
* __10_sec_Peak_Power__ -	10 sec Peak Power
* __10_sec_Peak_WPK__ -	10 sec Peak Power relative to Athlete Weight.
* __15_sec_Peak_Pace__ -	15 sec Peak Pace
* __15_sec_Peak_Pace_Swim__ -	15 sec Peak Pace Swim
* __15_sec_Peak_Power__ -	15 sec Peak Power
* __15_sec_Peak_WPK__ -	15 sec Peak Power relative to Athlete Weight.
* __2_min_Peak_Pace__ -	2 min Peak Pace
* __2_min_Peak_Pace_Swim__ -	2 min Peak Pace Swim
* __2_min_Peak_Power__ -	2 min Peak Power
* __20_min_Peak_Pace__ -	20 min Peak Pace
* __20_min_Peak_Pace_Swim__ -	20 min Peak Pace Swim
* __20_min_Peak_Power__ -	20 min Peak Power
* __20_min_Peak_Power_HR__ -	Average Heart Rate for 20 min Peak Power interval
* __20_min_Peak_WPK__ -	20 min Peak Power relative to Athlete Weight.
* __20_sec_Peak_Pace__ -	20 sec Peak Pace
* __20_sec_Peak_Pace_Swim__ -	20 sec Peak Pace Swim
* __20_sec_Peak_Power__ -	20 sec Peak Power
* __20_sec_Peak_WPK__ -	20 sec Peak Power relative to Athlete Weight.
* __3_min_Peak_Pace__ -	3 min Peak Pace
* __3_min_Peak_Pace_Swim__ -	3 min Peak Pace Swim
* __3_min_Peak_Power__ -	3 min Peak Power
* __30_min_Peak_Pace__ -	30 min Peak Pace
* __30_min_Peak_Pace_Swim__ -	30 min Peak Pace Swim
* __30_min_Peak_Power__ -	30 min Peak Power
* __30_min_Peak_Power_HR__ -	Average Heart Rate for 30 min Peak Power interval
* __30_min_Peak_WPK__ -	30 min Peak Power relative to Athlete Weight.
* __30_sec_Peak_Pace__ -	30 sec Peak Pace
* __30_sec_Peak_Pace_Swim__ -	30 sec Peak Pace Swim
* __30_sec_Peak_Power__ -	30 sec Peak Power
* __30_sec_Peak_WPK__ -	30 sec Peak Power relative to Athlete Weight.
* __5_min_Peak_Pace__ -	5 min Peak Pace
* __5_min_Peak_Pace_Swim__ -	5 min Peak Pace Swim
* __5_min_Peak_Power__ -	5 min Peak Power
* __5_min_Peak_Power_HR__ -	Average Heart Rate for 5 min Peak Power interval
* __5_min_Peak_WPK__ -	5 min Peak Power relative to Athlete Weight.
* __5_sec_Peak_Power__ -	5 sec Peak Power
* __5_sec_Peak_WPK__ -	5 sec Peak Power relative to Athlete Weight.
* __60_min_Peak_Pace__ -	60 min Peak Pace
* __60_min_Peak_Pace_Swim__ -	60 min Peak Pace Swim
* __60_min_Peak_Power__ -	60 min Peak Power
* __60_min_Peak_Power_HR__ -	Average Heart Rate for 60 min Peak Power interval
* __60_min_Peak_WPK__ -	60 min Peak Power relative to Athlete Weight.
* __8_min_Peak_Pace__ -	8 min Peak Pace
* __8_min_Peak_Pace_Swim__ -	8 min Peak Pace Swim
* __8_min_Peak_Power__ -	8 min Peak Power
* __90_min_Peak_Pace__ -	90 min Peak Pace
* __90_min_Peak_Pace_Swim__ -	90 min Peak Pace Swim
* __90_min_Peak_Power__ -	90 min Peak Power
* __95%_Heartrate__ -	Heart Rate for which 95% of activity samples has lower HR values
* __aBikeScore__ -	Skiba's altitude adjusted stress score taking into account both the intensity and the duration of the training session plus the altitude effect, similar to aTSS it can be computed as 100 * hours * (aPower Relative Intensity)^2
* __Activities__ -	Activity Count
* __Aerobic_Decoupling__ -	Aerobic decoupling is a measure of how much heart rate rises or how much power/pace falls off during the course of a long ride/run.
* __Aerobic_TISS__ -	Aerobic Training Impact Scoring System. It's a metric to quantify the training strain or response on the aerobic system
* __aIF__ -	Altitude Adjusted Intensity Factor is the ratio between aNP and the Critical Power (CP) configured in Power Zones.
* __Anaerobic_TISS__ -	Anaerobic Training Impact Scoring System. It's a metric to quantify the training strain or response on the anaerobic system
* __aNP__ -	Altitude Adjusted Normalized Power is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant accounting for altitude.
* __aPower_Efficiency_Factor__ -	The ratio between aNP and Average HR
* __aPower_Relative_Intensity__ -	Altitude Adjusted Relative Intensity is the ratio between axPower and the Critical Power (CP) configured in Power Zones, similar to aIF.
* __aPower_Response_Index__ -	The ratio between axPower and Average HR, similar to aPower Efficiency Factor
* __Athlete_Bodyfat__ -	Bodyfat in kg or lbs from Withings data
* __Athlete_Bodyfat_Percent__ -	Bodyfat Percent from Withings data
* __Athlete_Lean_Weight__ -	Lean Weight in kg or lbs from Withings data
* __Athlete_Weight__ -	Weight in kg or lbs: first from Withings data, then from Activity metadaa and last from Athlete configuration with 75kg default
* __aTSS__ -	Altitude Adjusted Training Stress Score takes into account both the intensity and the duration of the training session plus the altitude effect, it can be computed as 100 * hours * aIF^2
* __aTSS_per_hour__ -	Altitude Adjusted Training Stress Score divided by Duration in hours
* __Average_aPower__ -	Average altitude power. Recorded power ajusted to take into account the effect of altitude on vo2max and thus power output.
* __Average_Cadence__ -	Average Cadence, computed when Cadence > 0
* __Average_Core_Temperature__ -	Average Core Temperature. The core body temperature estimate is based on HR data
* __Average_Ground_Contact_Time__ -	Average Ground Contact Time
* __Average_Heart_Rate__ -	Average Heart Rate computed for samples when hr is greater than zero
* __Average_Left_Peak_Power_Phase_End__ -	It is the left pedal stroke angle where you end producing peak power, on average.
* __Average_Left_Peak_Power_Phase_Length__ -	It is the left pedal stroke region length where you produce peak power, on average.
* __Average_Left_Peak_Power_Phase_Start__ -	It is the left pedal stroke angle where you start producing peak power, on average.
* __Average_Left_Pedal_Center_Offset__ -	Platform center offset is the location on the left pedal platform where you apply force, on average.
* __Average_Left_Pedal_Smoothness__ -	It measures how smoothly power is delivered to the left pedal throughout the revolution, on average.
* __Average_Left_Power_Phase_End__ -	It is the left pedal stroke angle where you end producing positive power, on average.
* __Average_Left_Power_Phase_Length__ -	It is the left pedal stroke region length where you produce positive power, on average.
* __Average_Left_Power_Phase_Start__ -	It is the left pedal stroke angle where you start producing positive power, on average.
* __Average_Left_Torque_Effectiveness__ -	It measures how much of the power delivered to the left pedal is pushing it forward, on average.
* __Average_Power__ -	Average Power from all samples with power greater than or equal to zero
* __Average_Power_Variance__ -	Mean Power Deviation with respect to 30sec Moving Average
* __Average_Right_Peak_Power_Phase_End__ -	It is the right pedal stroke angle where you end producing peak power, on average.
* __Average_Right_Peak_Power_Phase_Length__ -	It is the right pedal stroke region length where you produce peak power, on average.
* __Average_Right_Peak_Power_Phase_Start__ -	It is the right pedal stroke angle where you start producing peak power, on average.
* __Average_Right_Pedal_Center_Offset__ -	Platform center offset is the location on the right pedal platform where you apply force, on average.
* __Average_Right_Pedal_Smoothness__ -	It measures how smoothly power is delivered to the right pedal throughout the revolution, on average.
* __Average_Right_Power_Phase_End__ -	It is the right pedal stroke angle where you end producing positive power, on average.
* __Average_Right_Power_Phase_Length__ -	It is the right pedal stroke region length where you produce positive power, on average.
* __Average_Right_Power_Phase_Start__ -	It is the right pedal stroke angle where you start producing positive power, on average.
* __Average_Right_Torque_Effectiveness__ -	It measures how much of the power delivered to the right pedal is pushing it forward, on average.
* __Average_Running_Cadence__ -	Average Running Cadence, computed when Cadence > 0
* __Average_SmO2__ -	Average Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* __Average_Speed__ -	Average Speed in kph or mph, computed from distance over time when speed not zero
* __Average_Temp__ -	Average Temp from activity data
* __Average_tHb__ -	Average total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* __Average_Vertical_Oscillation__ -	Average Vertical Oscillation
* __aVI__ -	Altitude Adjusted Variability Index is the ratio between aNP and Average aPower.
* __axPower__ -	Altitude Adjusted xPower is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant at altitude, similar to aNP.
* __Below_CP_Work__ -	Below CP Work is the amount of kJ produced while power is below CP.
* __Best_1000m__ -	Best 1000m
* __Best_100m__ -	Best 100m
* __Best_10km__ -	Best 10km
* __Best_1500m__ -	Best 1500m
* __Best_15km__ -	Best 15km
* __Best_2000m__ -	Best 2000m
* __Best_200m__ -	Best 200m
* __Best_20km__ -	Best 20km
* __Best_3000m__ -	Best 3000m
* __Best_30km__ -	Best 30km
* __Best_4000m__ -	Best 4000m
* __Best_400m__ -	Best 400m
* __Best_40km__ -	Best 40km
* __Best_5000m__ -	Best 5000m
* __Best_500m__ -	Best 500m
* __Best_50m__ -	Best 50m
* __Best_800m__ -	Best 800m
* __Best_Half_Marathon__ -	Best Half Marathon
* __Best_Marathon__ -	Best Marathon
* __BikeScore&#8482;__ -	Skiba's stress score taking into account both the intensity and the duration of the training session, similar to TSS it can be computed as 100 * hours * (Relative Intensity)^2
* __Calories_(HR)__ -	Total Calories estimated from Time Moving, Heart Rate, Weight, Sex and Age
* __Checksum__ -	A checksum for the activity, can be used to trigger cache refresh in R scripts.
* __Climb_Rating__ -	According to Dan Conelly: Elevation Gain ^2 / Distance / 1000, 100 is HARD
* __Critical_Power__ -	Critical Power (CP) configured in Power Zones.
* __Daniels_EqP__ -	Daniels EqP is the constant power which would produce equivalent Daniels Points.
* __Daniels_Points__ -	Daniels Points adapted for cycling using power instead of pace and assuming VO2max-power=1.2*CP, normalized to assign 100 points to 1 hour at CP.
* __Distance__ -	Total Distance in km or miles
* __Distance_Swim__ -	Total Distance in meters or yards
* __Duration__ -	Total Duration
* __Effect_of_Altitude__ -	Relationship between altitude adjusted power and recorded power
* __Efficiency_Factor__ -	The ratio between NP and Average HR for Cycling and xPace (in yd/min) and Average HR for Running
* __Efficiency_Index__ -	Efficiency Index : average speed by average power
* __Elevation_Gain__ -	Elevation Gain in meters of feets
* __Elevation_Gain_Carrying_(Est)__ -	Elevation gained at low speed with no power nor cadence
* __Elevation_Loss__ -	Elevation Loss in meters of feets
* __Estimated_VO2MAX__ -	Estimated VO2max from 5 min Peak Power relative to Athlete Weight using new ACSM formula: 10.8 * Watts / KG + 7 (3.5 per leg).
* __Exhaustion_Best_R__ -	Best value for R in differential model for exhaustion point.
* __Fatigue_Index__ -	Fatigue Index is power decay from Max Power to Min Power as a percent of Max Power.
* __GOVSS__ -	Gravity Ordered Velocity Stress Score, the TSS like metric defined by Dr. Skiba for Running, accounts for variations in speed, slope and relative intensity and duration
* __Gradient__ -	Elevation Gain to Total Distance percent ratio
* __H1_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 1.
* __H1_Time_in_Zone__ -	Time in Heart Rate Zone 1.
* __H10_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 10.
* __H10_Time_in_Zone__ -	Time in Heart Rate Zone 10.
* __H2_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 2.
* __H2_Time_in_Zone__ -	Time in Heart Rate Zone 2.
* __H3_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 3.
* __H3_Time_in_Zone__ -	Time in Heart Rate Zone 3.
* __H4_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 4.
* __H4_Time_in_Zone__ -	Time in Heart Rate Zone 4.
* __H5_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 5.
* __H5_Time_in_Zone__ -	Time in Heart Rate Zone 5.
* __H6_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 6.
* __H6_Time_in_Zone__ -	Time in Heart Rate Zone 6.
* __H7_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 7.
* __H7_Time_in_Zone__ -	Time in Heart Rate Zone 7.
* __H8_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 8.
* __H8_Time_in_Zone__ -	Time in Heart Rate Zone 8.
* __H9_Percent_in_Zone__ -	Percent of Time in Heart Rate Zone 9.
* __H9_Time_in_Zone__ -	Time in Heart Rate Zone 9.
* __Heartbeats__ -	Total Heartbeats
* __HrNp_Ratio__ -	Normalized Power to Average Heart Rate ratio in watts/bpm
* __HrPw_Ratio__ -	Power to Heart Rate Ratio in watts/bpm
* __IF__ -	Intensity Factor is the ratio between NP and the Functional Threshold Power (FTP) configured in Power Zones.
* __IWF__ -	Intensity Weigthting Factor, part of GOVSS calculation, defined as LNP/RTP
* __L1_Percent_in_Zone__ -	Percent of Time in Power Zone 1.
* __L1_Sustained_Time__ -	Sustained Time in Power Zone 1, based on (sustained) EFFORT intervals.
* __L1_Time_in_Zone__ -	Time in Power Zone 1.
* __L10_Percent_in_Zone__ -	Percent of Time in Power Zone 10.
* __L10_Sustained_Time__ -	Sustained Time in Power Zone 10, based on (sustained) EFFORT intervals.
* __L10_Time_in_Zone__ -	Time in Power Zone 10.
* __L2_Percent_in_Zone__ -	Percent of Time in Power Zone 2.
* __L2_Sustained_Time__ -	Sustained Time in Power Zone 2, based on (sustained) EFFORT intervals.
* __L2_Time_in_Zone__ -	Time in Power Zone 2.
* __L3_Percent_in_Zone__ -	Percent of Time in Power Zone 3.
* __L3_Sustained_Time__ -	Sustained Time in Power Zone 3, based on (sustained) EFFORT intervals.
* __L3_Time_in_Zone__ -	Time in Power Zone 3.
* __L4_Percent_in_Zone__ -	Percent of Time in Power Zone 4.
* __L4_Sustained_Time__ -	Sustained Time in Power Zone 4, based on (sustained) EFFORT intervals.
* __L4_Time_in_Zone__ -	Time in Power Zone 4.
* __L5_Percent_in_Zone__ -	Percent of Time in Power Zone 5.
* __L5_Sustained_Time__ -	Sustained Time in Power Zone 5, based on (sustained) EFFORT intervals.
* __L5_Time_in_Zone__ -	Time in Power Zone 5.
* __L6_Percent_in_Zone__ -	Percent of Time in Power Zone 6.
* __L6_Sustained_Time__ -	Sustained Time in Power Zone 6, based on (sustained) EFFORT intervals.
* __L6_Time_in_Zone__ -	Time in Power Zone 6.
* __L7_Percent_in_Zone__ -	Percent of Time in Power Zone 7.
* __L7_Sustained_Time__ -	Sustained Time in Power Zone 7, based on (sustained) EFFORT intervals.
* __L7_Time_in_Zone__ -	Time in Power Zone 7.
* __L8_Percent_in_Zone__ -	Percent of Time in Power Zone 8.
* __L8_Sustained_Time__ -	Sustained Time in Power Zone 8, based on (sustained) EFFORT intervals.
* __L8_Time_in_Zone__ -	Time in Power Zone 8.
* __L9_Percent_in_Zone__ -	Percent of Time in Power Zone 9.
* __L9_Sustained_Time__ -	Sustained Time in Power Zone 9, based on (sustained) EFFORT intervals.
* __L9_Time_in_Zone__ -	Time in Power Zone 9.
* __Left/Right_Balance__ -	Left/Right Balance shows the proportion of power coming from each pedal.
* __LNP__ -	Lactate Normalized Power as defined by Dr. Skiba in GOVSS algorithm
* __Max_Cadence__ -	Maximum Cadence
* __Max_Core_Temperature__ -	Maximum Core Temperature. The core body temperature estimate is based on HR data
* __Max_Heartrate__ -	Maximum Heart Rate.
* __Max_Power__ -	Maximum Power
* __Max_Power_Variance__ -	Maximum Power Deviation with respect to 30sec Moving Average
* __Max_Running_Cadence__ -	Maximum Running Cadence
* __Max_SmO2__ -	Maximum Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* __Max_Speed__ -	Maximum Speed
* __Max_Temp__ -	Maximum Cadence
* __Max_tHb__ -	Maximum total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* __Max_W'_Expended__ -	Maximum W' bal Expended expressed as percentage of W', W' bal tracks the level of W' according to CP model during intermitent exercise.
* __Maximum_W'bal_Match__ -	Maximum W' bal Match, W' bal tracks the level of W' according to CP model during intermitent exercise.
* __Min_Heartrate__ -	Minimum Heart Rate.
* __Min_SmO2__ -	Minimum Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* __Min_Temp__ -	Minimum Temperature
* __Min_tHb__ -	Minimum total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* __Minimum_W'_bal__ -	Minimum W' bal, W' bal tracks the level of W' according to CP model during intermitent exercise.
* __MMP_Percentage__ -	Average Power as Percent of Mean Maximal Power for Duration.
* __Nonzero_Average_Power__ -	Average Power without zero values, it gives inflated values when frecuent coasting is present
* __NP__ -	Normalized Power is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant.
* __P1_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 1.
* __P1_Time_in_Pace_Zone__ -	Time in Pace Zone 1.
* __P10_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 10.
* __P10_Time_in_Pace_Zone__ -	Time in Pace Zone 10.
* __P2_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 2.
* __P2_Time_in_Pace_Zone__ -	Time in Pace Zone 2.
* __P3_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 3.
* __P3_Time_in_Pace_Zone__ -	Time in Pace Zone 3.
* __P4_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 4.
* __P4_Time_in_Pace_Zone__ -	Time in Pace Zone 4.
* __P5_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 5.
* __P5_Time_in_Pace_Zone__ -	Time in Pace Zone 5.
* __P6_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 6.
* __P6_Time_in_Pace_Zone__ -	Time in Pace Zone 6.
* __P7_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 7.
* __P7_Time_in_Pace_Zone__ -	Time in Pace Zone 7.
* __P8_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 8.
* __P8_Time_in_Pace_Zone__ -	Time in Pace Zone 8.
* __P9_Percent_in_Pace_Zone__ -	Percent of Time in Pace Zone 9.
* __P9_Time_in_Pace_Zone__ -	Time in Pace Zone 9.
* __Pace__ -	Average Speed expressed in pace units: min/km or min/mile
* __Pace_Swim__ -	Average Speed expressed in swim pace units: min/100m or min/100yd
* __Pacing_Index__ -	Pacing Index is Average Power as a percent of Maximal Power
* __Power_Percent_of_Max__ -	Power as percent of Pmax according to Power Zones
* __Power_Zone__ -	Power Zone fractional number determined from Average Power.
* __Relative_Intensity__ -	Relative Intensity is the ratio between xPower and the Critical Power (CP) configured in Power Zones, similar to IF.
* __Response_Index__ -	The ratio between xPower and Average HR, similar to Efficiency Factor
* __RTP__ -	Run Threshold Power, computed from Critical Velocity using the GOVSS related algorithm
* __Session_RPE__ -	Session RPE is the product of RPE * minutes, where RPE is the rate of perceived exercion (10 point modified borg scale) and minutes is Time Moving if available or Duration otherwise.
* __Skiba_aVI__ -	Skiba Altitude Adjusted Variability Index is the ratio between axPower and Average aPower.
* __Skiba_VI__ -	Skiba Variability Index is the ratio between xPower and Average Power.
* __SRI__ -	Swimming Relative Intensity, used for SwimScore calculation, defined as xPowerSwim/STP
* __STP__ -	Swimming Threshold Power based on Swimming Critical Velocity, used for SwimScore calculation
* __Stroke_Rate__ -	Stroke Rate in strokes/min, counting both arms for freestyle/backstroke, corrected by 3m push-off length for pool swims
* __Strokes_Per_Length__ -	Strokes per length, counting the arm using the watch, Pool Length defaults to 50m for open water swims
* __Swim_Pace__ -	Average Swim Pace, computed only when Cadence > 0 to avoid kick/drill lengths
* __SwimScore__ -	SwimScore swimming stress metric as defined by Dr. Skiba
* __SWolf__ -	Strokes per length, counting the arm using the watch plus time in seconds, Pool Length defaults to 50m for open water swims
* __Time_Carrying_(Est)__ -	Time with low speed and elevation gain but no power nor cadence
* __Time_Moving__ -	Time with speed or cadence different from zero
* __TISS_Aerobicity__ -	TISS Aerobicity is a percentage of Aerobic TISS of the total TISS
* __To_Exhaustion__ -	Count of exhaustion points marked by the user in an activity
* __TPace__ -	Daniels' TPace, computed as 90%vVDOT from VDOT metric, in min/km or min/mile
* __TRIMP_Points__ -	Training Impulse according to Morton/Banister with Green et al coefficient.
* __TRIMP_Zonal_Points__ -	Training Impulse with time in zones weighted according to coefficients defined in Heart Rate Zones.
* __TRIMP(100)_Points__ -	TRIMP Points normalized to assign 100 points to 1 hour at threshold heart rate.
* __TriScore__ -	TriScore combined stress metric based on Dr. Skiba stress metrics, defined as BikeScore for cycling, GOVSS for running and SwimScore for swimming
* __TSS__ -	Training Stress Score takes into account both the intensity and the duration of the training session, it can be computed as 100 * hours * IF^2
* __TSS_per_hour__ -	Training Stress Score divided by Duration in hours
* __VAM__ -	Velocita Ascensionale Media, average ascent speed in vertical meters per hour
* __VDOT__ -	Daniels' VDOT computed from best average pace for durations from 4 min 4 hr
* __VI__ -	Variability Index is the ratio between NP and Average Power.
* __W'_Power__ -	W' Power is the average power produce while power is above CP.
* __W'_Work__ -	W' Work is the amount of kJ produced while power is above CP.
* __W'bal_Matches__ -	Number of W' balance Matches higher than 2kJ, W' bal tracks the level of W' according to CP model during intermitent exercise.
* __W'bal_TAU__ -	W' bal TAU is the recovery time constant for W' bal, W' bal tracks the level of W' according to CP model during intermitent exercise.
* __W1_Above_CP_W'bal_Low_Fatigue__ -	Time expended when Power is above CP and W' bal is below 25% of W'.
* __W1_W'bal_Low_Fatigue__ -	Time expended when W' bal is below 25% of W'.
* __W1_W'bal_Work_Low_Fatigue__ -	Work produced when W' bal is below 25% of W'.
* __W2_Above_CP_W'bal_Moderate_Fatigue__ -	Time expended when Power is above CP and W' bal is between 25% and 50% of W'.
* __W2_W'bal_Moderate_Fatigue__ -	Time expended when W' bal is between 25% and 50% of W'.
* __W2_W'bal_Work_Moderate_Fatigue__ -	Work produced when W' bal is between 25% and 50% of W'.
* __W3_Above_CP_W'bal_Heavy_Fatigue__ -	Time expended when Power is above CP and W' bal is between 50% and 75% of W'.
* __W3_W'bal_Heavy_Fatigue__ -	Time expended when W' bal is between 50% and 75% of W'.
* __W3_W'bal_Work_Heavy_Fatigue__ -	Work produced when W' bal is between 50% and 75% of W'.
* __W4_W'bal_Severe_Fatigue__ -	Time expended when W' bal is above 75% of W'.
* __W4_W'bal_Severe_Fatigue__ -	Time expended when Power is above CP and W' bal is above 75% of W'.
* __W4_W'bal_Work_Severe_Fatigue__ -	Work produced when Power is above CP and W' bal is above 75% of W'.
* __Watts_Per_Kilogram__ -	Average Power relative to Athlete Weight.
* __Watts:RPE_Ratio__ -	Watts to RPE ratio
* __Work__ -	Total Work in kJ computed from power data
* __Workbeat_stress__ -	Work * Heartbeats / 100000
* __xPace__ -	Normalized pace in min/km or min/mile, defined as the constant pace in flat surface which requires the same LNP
* __xPace_Swim__ -	Normalized Swim Pace in min/100m or min/100yd, defined as the constant pace which requires the same xPowerSwim
* __xPower__ -	xPower is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant, similar to NP.
* __xPower_Swim__ -	Swimming power normalized for variations in speed as defined by Dr. Skiba in the SwimScore algorithm

**OPERATORS**

Operators are the glue to building meaningful expressions
* + - / * ^ arithmetic operators evaluate to a numeric value
* && || logical operators evaluate to true or false
* < <= > >= <> = comparison operators evaluate to true or false. _Note:_ '=' is used to compare not assign.
* matches contains startsWith endsWith string comparisons evaluate to true or false
* x ? a : b evaluates to a if x is non-zero, otherwise b

**VERSION 4 UPDATES**

*User Metrics*

We have introduced the ability to define your own metrics, by writing code to perform calculations against a workout. The user defines some named expressions (user functions) that are called on certain conditions:

* init { } is called to initialise any variables before working with the ride
* relevant { } is called to check if  this metric is relevant for the ride
* sample { } is called for every sample in the ride
* value { } is called at the end to get the metric value
* count { } is called at the end to get the count to use when aggregating averages

All the named functions are optional, but if no value { } function is defined the metric will always be zero.

*New language syntax*

* XDATA("name","series", sparse|repeat|interpolate|resample) - gets access to any xdata series.
* XDATA(..) will return true/false when filtering rides to indicate if the xdata is present in the activity.
* XDATA(..) will return the sample data value when iterating across activity samples (outer join).
* XDATA(..) repeat - repeat last observed value, sparse - only return observed points, interpolate - smooth values between observations, resample - resample the xdata to the samplerate of the activity.

__NOTE__: XDATA "name" and "series" can be specified using wildcards. such as "\*" or "[Pp][Oo][Ww][Ee][Rr]\*".
This is NOT a regular expression, it is the same format of pattern used to match filenames.

* INDEX when iterating samples (user metrics/data) its the current index
* symbol[x] treats symbol as an array and returns xth item (zero if out of bounds)
* POWER[x] when iterating samples get xth sample value for POWER
* POWER[INDEX-x] example using [] and INDEX to access the datapoint values by index
* symbol[x] <- y update xth sample in symbol with the value y (will not work on ride data like POWER)
* x ?: y evaluates to y if x is zero otherwise x (equivalent to: x ? x : y)
* !expr logical not, evaluates false if expr true, true if expr false
* symbol <- expr user symbols to hold assigned values, evaluate to the value assigned
* { expr; .. expr; } compound statements that evaluate to last expression
* if (cond) stmt; else stmt; if/else logic where statement can also be a compound statement
* name { ... } a named expression that can be called e.g. fn { p <- 1; } called as fn()
* bestime(x) returns the fastest time (seconds) to cover distance x (km)


