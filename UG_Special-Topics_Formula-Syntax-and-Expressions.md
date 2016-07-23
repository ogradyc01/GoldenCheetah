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

* 1_min_Peak_Pace	-	1 min Peak Pace
* 1_min_Peak_Pace_Swim	-	1 min Peak Pace Swim
* 1_min_Peak_Power	-	1 min Peak Power
* 1_min_Peak_Power_HR	-	Average Heart Rate for 1 min Peak Power interval
* 1_min_Peak_WPK	-	1 min Peak Power relative to Athlete Weight.
* 1_sec_Peak_Power	-	1 sec Peak Power
* 1_sec_Peak_WPK	-	1 sec Peak Power relative to Athlete Weight.
* 10_min_Peak_Pace	-	10 min Peak Pace
* 10_min_Peak_Pace_Swim	-	10 min Peak Pace Swim
* 10_min_Peak_Power	-	10 min Peak Power
* 10_min_Peak_Power_HR	-	Average Heart Rate for 10 min Peak Power interval
* 10_min_Peak_WPK	-	10 min Peak Power relative to Athlete Weight.
* 10_sec_Peak_Pace	-	10 sec Peak Pace
* 10_sec_Peak_Pace_Swim	-	10 sec Peak Pace Swim
* 10_sec_Peak_Power	-	10 sec Peak Power
* 10_sec_Peak_WPK	-	10 sec Peak Power relative to Athlete Weight.
* 15_sec_Peak_Pace	-	15 sec Peak Pace
* 15_sec_Peak_Pace_Swim	-	15 sec Peak Pace Swim
* 15_sec_Peak_Power	-	15 sec Peak Power
* 15_sec_Peak_WPK	-	15 sec Peak Power relative to Athlete Weight.
* 2_min_Peak_Pace	-	2 min Peak Pace
* 2_min_Peak_Pace_Swim	-	2 min Peak Pace Swim
* 2_min_Peak_Power	-	2 min Peak Power
* 20_min_Peak_Pace	-	20 min Peak Pace
* 20_min_Peak_Pace_Swim	-	20 min Peak Pace Swim
* 20_min_Peak_Power	-	20 min Peak Power
* 20_min_Peak_Power_HR	-	Average Heart Rate for 20 min Peak Power interval
* 20_min_Peak_WPK	-	20 min Peak Power relative to Athlete Weight.
* 20_sec_Peak_Pace	-	20 sec Peak Pace
* 20_sec_Peak_Pace_Swim	-	20 sec Peak Pace Swim
* 20_sec_Peak_Power	-	20 sec Peak Power
* 20_sec_Peak_WPK	-	20 sec Peak Power relative to Athlete Weight.
* 3_min_Peak_Pace	-	3 min Peak Pace
* 3_min_Peak_Pace_Swim	-	3 min Peak Pace Swim
* 3_min_Peak_Power	-	3 min Peak Power
* 30_min_Peak_Pace	-	30 min Peak Pace
* 30_min_Peak_Pace_Swim	-	30 min Peak Pace Swim
* 30_min_Peak_Power	-	30 min Peak Power
* 30_min_Peak_Power_HR	-	Average Heart Rate for 30 min Peak Power interval
* 30_min_Peak_WPK	-	30 min Peak Power relative to Athlete Weight.
* 30_sec_Peak_Pace	-	30 sec Peak Pace
* 30_sec_Peak_Pace_Swim	-	30 sec Peak Pace Swim
* 30_sec_Peak_Power	-	30 sec Peak Power
* 30_sec_Peak_WPK	-	30 sec Peak Power relative to Athlete Weight.
* 5_min_Peak_Pace	-	5 min Peak Pace
* 5_min_Peak_Pace_Swim	-	5 min Peak Pace Swim
* 5_min_Peak_Power	-	5 min Peak Power
* 5_min_Peak_Power_HR	-	Average Heart Rate for 5 min Peak Power interval
* 5_min_Peak_WPK	-	5 min Peak Power relative to Athlete Weight.
* 5_sec_Peak_Power	-	5 sec Peak Power
* 5_sec_Peak_WPK	-	5 sec Peak Power relative to Athlete Weight.
* 60_min_Peak_Pace	-	60 min Peak Pace
* 60_min_Peak_Pace_Swim	-	60 min Peak Pace Swim
* 60_min_Peak_Power	-	60 min Peak Power
* 60_min_Peak_Power_HR	-	Average Heart Rate for 60 min Peak Power interval
* 60_min_Peak_WPK	-	60 min Peak Power relative to Athlete Weight.
* 8_min_Peak_Pace	-	8 min Peak Pace
* 8_min_Peak_Pace_Swim	-	8 min Peak Pace Swim
* 8_min_Peak_Power	-	8 min Peak Power
* 90_min_Peak_Pace	-	90 min Peak Pace
* 90_min_Peak_Pace_Swim	-	90 min Peak Pace Swim
* 90_min_Peak_Power	-	90 min Peak Power
* 95%_Heartrate	-	Heart Rate for which 95% of activity samples has lower HR values
* aBikeScore	-	Skiba's altitude adjusted stress score taking into account both the intensity and the duration of the training session plus the altitude effect, similar to aTSS it can be computed as 100 * hours * (aPower Relative Intensity)^2
* Activities	-	Activity Count
* Aerobic_Decoupling	-	Aerobic decoupling is a measure of how much heart rate rises or how much power/pace falls off during the course of a long ride/run.
* Aerobic_TISS	-	Aerobic Training Impact Scoring System. It's a metric to quantify the training strain or response on the aerobic system
* aIF	-	Altitude Adjusted Intensity Factor is the ratio between aNP and the Critical Power (CP) configured in Power Zones.
* Anaerobic_TISS	-	Anaerobic Training Impact Scoring System. It's a metric to quantify the training strain or response on the anaerobic system
* aNP	-	Altitude Adjusted Normalized Power is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant accounting for altitude.
* aPower_Efficiency_Factor	-	The ratio between aNP and Average HR
* aPower_Relative_Intensity	-	Altitude Adjusted Relative Intensity is the ratio between axPower and the Critical Power (CP) configured in Power Zones, similar to aIF.
* aPower_Response_Index	-	The ratio between axPower and Average HR, similar to aPower Efficiency Factor
* Athlete_Bodyfat	-	Bodyfat in kg or lbs from Withings data
* Athlete_Bodyfat_Percent	-	Bodyfat Percent from Withings data
* Athlete_Lean_Weight	-	Lean Weight in kg or lbs from Withings data
* Athlete_Weight	-	Weight in kg or lbs: first from Withings data, then from Activity metadaa and last from Athlete configuration with 75kg default
* aTSS	-	Altitude Adjusted Training Stress Score takes into account both the intensity and the duration of the training session plus the altitude effect, it can be computed as 100 * hours * aIF^2
* aTSS_per_hour	-	Altitude Adjusted Training Stress Score divided by Duration in hours
* Average_aPower	-	Average altitude power. Recorded power ajusted to take into account the effect of altitude on vo2max and thus power output.
* Average_Cadence	-	Average Cadence, computed when Cadence > 0
* Average_Core_Temperature	-	Average Core Temperature. The core body temperature estimate is based on HR data
* Average_Ground_Contact_Time	-	Average Ground Contact Time
* Average_Heart_Rate	-	Average Heart Rate computed for samples when hr is greater than zero
* Average_Left_Peak_Power_Phase_End	-	It is the left pedal stroke angle where you end producing peak power, on average.
* Average_Left_Peak_Power_Phase_Length	-	It is the left pedal stroke region length where you produce peak power, on average.
* Average_Left_Peak_Power_Phase_Start	-	It is the left pedal stroke angle where you start producing peak power, on average.
* Average_Left_Pedal_Center_Offset	-	Platform center offset is the location on the left pedal platform where you apply force, on average.
* Average_Left_Pedal_Smoothness	-	It measures how smoothly power is delivered to the left pedal throughout the revolution, on average.
* Average_Left_Power_Phase_End	-	It is the left pedal stroke angle where you end producing positive power, on average.
* Average_Left_Power_Phase_Length	-	It is the left pedal stroke region length where you produce positive power, on average.
* Average_Left_Power_Phase_Start	-	It is the left pedal stroke angle where you start producing positive power, on average.
* Average_Left_Torque_Effectiveness	-	It measures how much of the power delivered to the left pedal is pushing it forward, on average.
* Average_Power	-	Average Power from all samples with power greater than or equal to zero
* Average_Power_Variance	-	Mean Power Deviation with respect to 30sec Moving Average
* Average_Right_Peak_Power_Phase_End	-	It is the right pedal stroke angle where you end producing peak power, on average.
* Average_Right_Peak_Power_Phase_Length	-	It is the right pedal stroke region length where you produce peak power, on average.
* Average_Right_Peak_Power_Phase_Start	-	It is the right pedal stroke angle where you start producing peak power, on average.
* Average_Right_Pedal_Center_Offset	-	Platform center offset is the location on the right pedal platform where you apply force, on average.
* Average_Right_Pedal_Smoothness	-	It measures how smoothly power is delivered to the right pedal throughout the revolution, on average.
* Average_Right_Power_Phase_End	-	It is the right pedal stroke angle where you end producing positive power, on average.
* Average_Right_Power_Phase_Length	-	It is the right pedal stroke region length where you produce positive power, on average.
* Average_Right_Power_Phase_Start	-	It is the right pedal stroke angle where you start producing positive power, on average.
* Average_Right_Torque_Effectiveness	-	It measures how much of the power delivered to the right pedal is pushing it forward, on average.
* Average_Running_Cadence	-	Average Running Cadence, computed when Cadence > 0
* Average_SmO2	-	Average Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* Average_Speed	-	Average Speed in kph or mph, computed from distance over time when speed not zero
* Average_Temp	-	Average Temp from activity data
* Average_tHb	-	Average total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* Average_Vertical_Oscillation	-	Average Vertical Oscillation
* aVI	-	Altitude Adjusted Variability Index is the ratio between aNP and Average aPower.
* axPower	-	Altitude Adjusted xPower is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant at altitude, similar to aNP.
* Below_CP_Work	-	Below CP Work is the amount of kJ produced while power is below CP.
* Best_1000m	-	Best 1000m
* Best_100m	-	Best 100m
* Best_10km	-	Best 10km
* Best_1500m	-	Best 1500m
* Best_15km	-	Best 15km
* Best_2000m	-	Best 2000m
* Best_200m	-	Best 200m
* Best_20km	-	Best 20km
* Best_3000m	-	Best 3000m
* Best_30km	-	Best 30km
* Best_4000m	-	Best 4000m
* Best_400m	-	Best 400m
* Best_40km	-	Best 40km
* Best_5000m	-	Best 5000m
* Best_500m	-	Best 500m
* Best_50m	-	Best 50m
* Best_800m	-	Best 800m
* Best_Half_Marathon	-	Best Half Marathon
* Best_Marathon	-	Best Marathon
* BikeScore&#8482;	-	Skiba's stress score taking into account both the intensity and the duration of the training session, similar to TSS it can be computed as 100 * hours * (Relative Intensity)^2
* Calories_(HR)	-	Total Calories estimated from Time Moving, Heart Rate, Weight, Sex and Age
* Checksum	-	A checksum for the activity, can be used to trigger cache refresh in R scripts.
* Climb_Rating	-	According to Dan Conelly: Elevation Gain ^2 / Distance / 1000, 100 is HARD
* Critical_Power	-	Critical Power (CP) configured in Power Zones.
* Daniels_EqP	-	Daniels EqP is the constant power which would produce equivalent Daniels Points.
* Daniels_Points	-	Daniels Points adapted for cycling using power instead of pace and assuming VO2max-power=1.2*CP, normalized to assign 100 points to 1 hour at CP.
* Distance	-	Total Distance in km or miles
* Distance_Swim	-	Total Distance in meters or yards
* Duration	-	Total Duration
* Effect_of_Altitude	-	Relationship between altitude adjusted power and recorded power
* Efficiency_Factor	-	The ratio between NP and Average HR for Cycling and xPace (in yd/min) and Average HR for Running
* Efficiency_Index	-	Efficiency Index : average speed by average power
* Elevation_Gain	-	Elevation Gain in meters of feets
* Elevation_Gain_Carrying_(Est)	-	Elevation gained at low speed with no power nor cadence
* Elevation_Loss	-	Elevation Loss in meters of feets
* Estimated_VO2MAX	-	Estimated VO2max from 5 min Peak Power relative to Athlete Weight using new ACSM formula: 10.8 * Watts / KG + 7 (3.5 per leg).
* Exhaustion_Best_R	-	Best value for R in differential model for exhaustion point.
* Fatigue_Index	-	Fatigue Index is power decay from Max Power to Min Power as a percent of Max Power.
* GOVSS	-	Gravity Ordered Velocity Stress Score, the TSS like metric defined by Dr. Skiba for Running, accounts for variations in speed, slope and relative intensity and duration
* Gradient	-	Elevation Gain to Total Distance percent ratio
* H1_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 1.
* H1_Time_in_Zone	-	Time in Heart Rate Zone 1.
* H10_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 10.
* H10_Time_in_Zone	-	Time in Heart Rate Zone 10.
* H2_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 2.
* H2_Time_in_Zone	-	Time in Heart Rate Zone 2.
* H3_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 3.
* H3_Time_in_Zone	-	Time in Heart Rate Zone 3.
* H4_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 4.
* H4_Time_in_Zone	-	Time in Heart Rate Zone 4.
* H5_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 5.
* H5_Time_in_Zone	-	Time in Heart Rate Zone 5.
* H6_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 6.
* H6_Time_in_Zone	-	Time in Heart Rate Zone 6.
* H7_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 7.
* H7_Time_in_Zone	-	Time in Heart Rate Zone 7.
* H8_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 8.
* H8_Time_in_Zone	-	Time in Heart Rate Zone 8.
* H9_Percent_in_Zone	-	Percent of Time in Heart Rate Zone 9.
* H9_Time_in_Zone	-	Time in Heart Rate Zone 9.
* Heartbeats	-	Total Heartbeats
* HrNp_Ratio	-	Normalized Power to Average Heart Rate ratio in watts/bpm
* HrPw_Ratio	-	Power to Heart Rate Ratio in watts/bpm
* IF	-	Intensity Factor is the ratio between NP and the Functional Threshold Power (FTP) configured in Power Zones.
* IWF	-	Intensity Weigthting Factor, part of GOVSS calculation, defined as LNP/RTP
* L1_Percent_in_Zone	-	Percent of Time in Power Zone 1.
* L1_Sustained_Time	-	Sustained Time in Power Zone 1, based on (sustained) EFFORT intervals.
* L1_Time_in_Zone	-	Time in Power Zone 1.
* L10_Percent_in_Zone	-	Percent of Time in Power Zone 10.
* L10_Sustained_Time	-	Sustained Time in Power Zone 10, based on (sustained) EFFORT intervals.
* L10_Time_in_Zone	-	Time in Power Zone 10.
* L2_Percent_in_Zone	-	Percent of Time in Power Zone 2.
* L2_Sustained_Time	-	Sustained Time in Power Zone 2, based on (sustained) EFFORT intervals.
* L2_Time_in_Zone	-	Time in Power Zone 2.
* L3_Percent_in_Zone	-	Percent of Time in Power Zone 3.
* L3_Sustained_Time	-	Sustained Time in Power Zone 3, based on (sustained) EFFORT intervals.
* L3_Time_in_Zone	-	Time in Power Zone 3.
* L4_Percent_in_Zone	-	Percent of Time in Power Zone 4.
* L4_Sustained_Time	-	Sustained Time in Power Zone 4, based on (sustained) EFFORT intervals.
* L4_Time_in_Zone	-	Time in Power Zone 4.
* L5_Percent_in_Zone	-	Percent of Time in Power Zone 5.
* L5_Sustained_Time	-	Sustained Time in Power Zone 5, based on (sustained) EFFORT intervals.
* L5_Time_in_Zone	-	Time in Power Zone 5.
* L6_Percent_in_Zone	-	Percent of Time in Power Zone 6.
* L6_Sustained_Time	-	Sustained Time in Power Zone 6, based on (sustained) EFFORT intervals.
* L6_Time_in_Zone	-	Time in Power Zone 6.
* L7_Percent_in_Zone	-	Percent of Time in Power Zone 7.
* L7_Sustained_Time	-	Sustained Time in Power Zone 7, based on (sustained) EFFORT intervals.
* L7_Time_in_Zone	-	Time in Power Zone 7.
* L8_Percent_in_Zone	-	Percent of Time in Power Zone 8.
* L8_Sustained_Time	-	Sustained Time in Power Zone 8, based on (sustained) EFFORT intervals.
* L8_Time_in_Zone	-	Time in Power Zone 8.
* L9_Percent_in_Zone	-	Percent of Time in Power Zone 9.
* L9_Sustained_Time	-	Sustained Time in Power Zone 9, based on (sustained) EFFORT intervals.
* L9_Time_in_Zone	-	Time in Power Zone 9.
* Left/Right_Balance	-	Left/Right Balance shows the proportion of power coming from each pedal.
* LNP	-	Lactate Normalized Power as defined by Dr. Skiba in GOVSS algorithm
* Max_Cadence	-	Maximum Cadence
* Max_Core_Temperature	-	Maximum Core Temperature. The core body temperature estimate is based on HR data
* Max_Heartrate	-	Maximum Heart Rate.
* Max_Power	-	Maximum Power
* Max_Power_Variance	-	Maximum Power Deviation with respect to 30sec Moving Average
* Max_Running_Cadence	-	Maximum Running Cadence
* Max_SmO2	-	Maximum Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* Max_Speed	-	Maximum Speed
* Max_Temp	-	Maximum Cadence
* Max_tHb	-	Maximum total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* Max_W'_Expended	-	Maximum W' bal Expended expressed as percentage of W', W' bal tracks the level of W' according to CP model during intermitent exercise.
* Maximum_W'bal_Match	-	Maximum W' bal Match, W' bal tracks the level of W' according to CP model during intermitent exercise.
* Min_Heartrate	-	Minimum Heart Rate.
* Min_SmO2	-	Minimum Muscle Oxygen Saturation, the percentage of hemoglobin that is carrying oxygen.
* Min_Temp	-	Minimum Temperature
* Min_tHb	-	Minimum total hemoglobin concentration. The total grams of hemoglobin per deciliter.
* Minimum_W'_bal	-	Minimum W' bal, W' bal tracks the level of W' according to CP model during intermitent exercise.
* MMP_Percentage	-	Average Power as Percent of Mean Maximal Power for Duration.
* Nonzero_Average_Power	-	Average Power without zero values, it gives inflated values when frecuent coasting is present
* NP	-	Normalized Power is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant.
* P1_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 1.
* P1_Time_in_Pace_Zone	-	Time in Pace Zone 1.
* P10_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 10.
* P10_Time_in_Pace_Zone	-	Time in Pace Zone 10.
* P2_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 2.
* P2_Time_in_Pace_Zone	-	Time in Pace Zone 2.
* P3_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 3.
* P3_Time_in_Pace_Zone	-	Time in Pace Zone 3.
* P4_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 4.
* P4_Time_in_Pace_Zone	-	Time in Pace Zone 4.
* P5_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 5.
* P5_Time_in_Pace_Zone	-	Time in Pace Zone 5.
* P6_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 6.
* P6_Time_in_Pace_Zone	-	Time in Pace Zone 6.
* P7_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 7.
* P7_Time_in_Pace_Zone	-	Time in Pace Zone 7.
* P8_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 8.
* P8_Time_in_Pace_Zone	-	Time in Pace Zone 8.
* P9_Percent_in_Pace_Zone	-	Percent of Time in Pace Zone 9.
* P9_Time_in_Pace_Zone	-	Time in Pace Zone 9.
* Pace	-	Average Speed expressed in pace units: min/km or min/mile
* Pace_Swim	-	Average Speed expressed in swim pace units: min/100m or min/100yd
* Pacing_Index	-	Pacing Index is Average Power as a percent of Maximal Power
* Power_Percent_of_Max	-	Power as percent of Pmax according to Power Zones
* Power_Zone	-	Power Zone fractional number determined from Average Power.
* Relative_Intensity	-	Relative Intensity is the ratio between xPower and the Critical Power (CP) configured in Power Zones, similar to IF.
* Response_Index	-	The ratio between xPower and Average HR, similar to Efficiency Factor
* RTP	-	Run Threshold Power, computed from Critical Velocity using the GOVSS related algorithm
* Session_RPE	-	Session RPE is the product of RPE * minutes, where RPE is the rate of perceived exercion (10 point modified borg scale) and minutes is Time Moving if available or Duration otherwise.
* Skiba_aVI	-	Skiba Altitude Adjusted Variability Index is the ratio between axPower and Average aPower.
* Skiba_VI	-	Skiba Variability Index is the ratio between xPower and Average Power.
* SRI	-	Swimming Relative Intensity, used for SwimScore calculation, defined as xPowerSwim/STP
* STP	-	Swimming Threshold Power based on Swimming Critical Velocity, used for SwimScore calculation
* Stroke_Rate	-	Stroke Rate in strokes/min, counting both arms for freestyle/backstroke, corrected by 3m push-off length for pool swims
* Strokes_Per_Length	-	Strokes per length, counting the arm using the watch, Pool Length defaults to 50m for open water swims
* Swim_Pace	-	Average Swim Pace, computed only when Cadence > 0 to avoid kick/drill lengths
* SwimScore	-	SwimScore swimming stress metric as defined by Dr. Skiba
* SWolf	-	Strokes per length, counting the arm using the watch plus time in seconds, Pool Length defaults to 50m for open water swims
* Time_Carrying_(Est)	-	Time with low speed and elevation gain but no power nor cadence
* Time_Moving	-	Time with speed or cadence different from zero
* TISS_Aerobicity	-	TISS Aerobicity is a percentage of Aerobic TISS of the total TISS
* To_Exhaustion	-	Count of exhaustion points marked by the user in an activity
* TPace	-	Daniels' TPace, computed as 90%vVDOT from VDOT metric, in min/km or min/mile
* TRIMP_Points	-	Training Impulse according to Morton/Banister with Green et al coefficient.
* TRIMP_Zonal_Points	-	Training Impulse with time in zones weighted according to coefficients defined in Heart Rate Zones.
* TRIMP(100)_Points	-	TRIMP Points normalized to assign 100 points to 1 hour at threshold heart rate.
* TriScore	-	TriScore combined stress metric based on Dr. Skiba stress metrics, defined as BikeScore for cycling, GOVSS for running and SwimScore for swimming
* TSS	-	Training Stress Score takes into account both the intensity and the duration of the training session, it can be computed as 100 * hours * IF^2
* TSS_per_hour	-	Training Stress Score divided by Duration in hours
* VAM	-	Velocita Ascensionale Media, average ascent speed in vertical meters per hour
* VDOT	-	Daniels' VDOT computed from best average pace for durations from 4 min 4 hr
* VI	-	Variability Index is the ratio between NP and Average Power.
* W'_Power	-	W' Power is the average power produce while power is above CP.
* W'_Work	-	W' Work is the amount of kJ produced while power is above CP.
* W'bal_Matches	-	Number of W' balance Matches higher than 2kJ, W' bal tracks the level of W' according to CP model during intermitent exercise.
* W'bal_TAU	-	W' bal TAU is the recovery time constant for W' bal, W' bal tracks the level of W' according to CP model during intermitent exercise.
* W1_Above_CP_W'bal_Low_Fatigue	-	Time expended when Power is above CP and W' bal is below 25% of W'.
* W1_W'bal_Low_Fatigue	-	Time expended when W' bal is below 25% of W'.
* W1_W'bal_Work_Low_Fatigue	-	Work produced when W' bal is below 25% of W'.
* W2_Above_CP_W'bal_Moderate_Fatigue	-	Time expended when Power is above CP and W' bal is between 25% and 50% of W'.
* W2_W'bal_Moderate_Fatigue	-	Time expended when W' bal is between 25% and 50% of W'.
* W2_W'bal_Work_Moderate_Fatigue	-	Work produced when W' bal is between 25% and 50% of W'.
* W3_Above_CP_W'bal_Heavy_Fatigue	-	Time expended when Power is above CP and W' bal is between 50% and 75% of W'.
* W3_W'bal_Heavy_Fatigue	-	Time expended when W' bal is between 50% and 75% of W'.
* W3_W'bal_Work_Heavy_Fatigue	-	Work produced when W' bal is between 50% and 75% of W'.
* W4_W'bal_Severe_Fatigue	-	Time expended when W' bal is above 75% of W'.
* W4_W'bal_Severe_Fatigue	-	Time expended when Power is above CP and W' bal is above 75% of W'.
* W4_W'bal_Work_Severe_Fatigue	-	Work produced when Power is above CP and W' bal is above 75% of W'.
* Watts_Per_Kilogram	-	Average Power relative to Athlete Weight.
* Watts:RPE_Ratio	-	Watts to RPE ratio
* Work	-	Total Work in kJ computed from power data
* Workbeat_stress	-	Work * Heartbeats / 100000
* xPace	-	Normalized pace in min/km or min/mile, defined as the constant pace in flat surface which requires the same LNP
* xPace_Swim	-	Normalized Swim Pace in min/100m or min/100yd, defined as the constant pace which requires the same xPowerSwim
* xPower	-	xPower is an estimate of the power that you could have maintained for the same physiological 'cost' if your power output had been perfectly constant, similar to NP.
* xPower_Swim	-	Swimming power normalized for variations in speed as defined by Dr. Skiba in the SwimScore algorithm

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


