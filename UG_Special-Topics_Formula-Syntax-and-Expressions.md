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
* set(...)
* unset(...)
* isset(p1)

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

**RIDE AND INTERVAL METRICS**

* 95%_Heartrate
* aBikeScore
* Activities
* Aerobic_TISS
* Aerobic_TISS
* aIF
* Anaerobic_TISS
* Anaerobic_TISS
* aNP
* aPower_Efficiency_Factor
* aPower_Relative_Intensity
* aPower_Response_Index
* Athlete_Bodyfat
* Athlete_Bodyfat_Percent
* Athlete_Lean_Weight
* Athlete_Weight
* aTSS
* aTSS_per_hour
* Average_aPower
* Average_Cadence
* Average_Core_Temperature
* Average_Heart_Rate
* Average_Left_Peak_Power_Phase_End
* Average_Peak_Left_Power_Phase_Length
* Average_Left_Peak_Power_Phase_Start
* Average_Left_Pedal_Center_Offset
* Average_Left_Pedal_Smoothness
* Average_Left_Power_Phase_End
* Average_Left_Power_Phase_Length
* Average_Left_Power_Phase_Start
* Average_Left_Torque_Effectiveness
* Average_Power
* Average_Power_Variance
* Average_Right_Peak_Power_Phase_End
* Average_Right_Peak_Power_Phase_Length
* Average_Right_Peak_Power_Phase_Start
* Average_Right_Pedal_Center_Offset
* Average_Right_Pedal_Smoothness
* Average_Right_Power_Phase_End
* Average_Right_Power_Phase_Length
* Average_Right_Power_Phase_Start
* Average_Right_Torque_Effectiveness
* Average_SmO2
* Average_Speed
* Average_Temp
* Average_tHb
* Average_Cadence
* Average_Heart_Rate
* Average_Power
* Average_Speed
* aVI
* axPower
* Below_CP_Work
* BikeScore
* BikeScore
* Calendar_Text
* Calories
* Climb_Rating
* color
* CP
* CP_setting
* Daniels_EqP
* Daniels_Points
* Daniels_EqP
* Daniels_Points
* Data
* Date
* Device
* Device_Info
* Distance
* Distance_Swim
* Duration
* EOA
* Efficiency_Factor
* Elevation_Gain
* Elevation_Gain_Carrying
* Elevation_Loss
* Elevation_Gain
* Estimated_VO2MAX
* Fatigue_Index
* File
* GOVSS
* Gradient
* Heartbeats
* HrNp_Ratio
* HrPw_Ratio
* IF
* Interesting
* isRun
* IWF
* Left/Right_Balance
* LNP
* Max_Cadence
* Max_Core_Temperature
* Max_Heartrate
* Max_Power
* Max_Power_Variance
* Max_SmO2
* Max_Speed
* Max_Temp
* Max_tHb
* Max_W'_Expended
* Maximum_W'bal_Match
* Min_Heartrate
* Min_SmO2
* Min_tHb
* Minimum_W'bal
* MMP_Percentage
* Nonzero_Average_Power
* Notes
* NP
* Objective
* Pace
* Pace_Swim
* Pacing_Index
* path
* Pmax
* Power_Percent_of_Max
* Power_Zone
* Recording_Interval
* Relative_Intensity
* Response_Index
* Route
* RPE
* RTP
* Session_RPE
* Skiba_aVI
* Skiba_VI
* Sport
* SRI
* Start_Date
* Start_Time
* STP
* SwimScore
* Tau
* Test
* Time
* Time_Carrying
* Time_Moving
* Time_Moving
* TISS_Aerobicity
* TPace
* TRIMP_Points
* TRIMP_Zonal_Points
* TRIMP(100)_Points
* TriScore
* TSS
* TSS_per_hour
* VAM
* VDOT
* VI
* W'
* W'_Watts
* W'_Work
* W'bal_Matches_>_2KJ
* W'bal_TAU
* Watts_Per_Kilogram
* Watts_RPE_Ratio
* Weight
* Work
* Workbeat_stress
* Workout_Code
* xPace
* xPace_Swim
* xPower
* xPower_Swim

**TIME IN ZONES**

_Heartrate_
* H1_Percent_in_Zone
* H1_Time_in_Zone
* H10_Percent_in_Zone
* H10_Time_in_Zone
* H2_Percent_in_Zone
* H2_Time_in_Zone
* H3_Percent_in_Zone
* H3_Time_in_Zone
* H4_Percent_in_Zone
* H4_Time_in_Zone
* H5_Percent_in_Zone
* H5_Time_in_Zone
* H6_Percent_in_Zone
* H6_Time_in_Zone
* H7_Percent_in_Zone
* H7_Time_in_Zone
* H8_Percent_in_Zone
* H8_Time_in_Zone
* H9_Percent_in_Zone
* H9_Time_in_Zone

_Power_
* L1_Percent_in_Zone
* L1_Sustained_Time
* L1_Time_in_Zone
* L10_Percent_in_Zone
* L10_Sustained_Time
* L10_Time_in_Zone
* L2_Percent_in_Zone
* L2_Sustained_Time
* L2_Time_in_Zone
* L3_Percent_in_Zone
* L3_Sustained_Time
* L3_Time_in_Zone
* L4_Percent_in_Zone
* L4_Sustained_Time
* L4_Time_in_Zone
* L5_Percent_in_Zone
* L5_Sustained_Time
* L5_Time_in_Zone
* L6_Percent_in_Zone
* L6_Sustained_Time
* L6_Time_in_Zone
* L7_Percent_in_Zone
* L7_Sustained_Time
* L7_Time_in_Zone
* L8_Percent_in_Zone
* L8_Sustained_Time
* L8_Time_in_Zone
* L9_Percent_in_Zone
* L9_Sustained_Time
* L9_Time_in_Zone

_Pace_
* P1_Percent_in_Pace_Zone
* P1_Time_in_Pace_Zone
* P10_Percent_in_Pace_Zone
* P10_Time_in_Pace_Zone
* P2_Percent_in_Pace_Zone
* P2_Time_in_Pace_Zone
* P3_Percent_in_Pace_Zone
* P3_Time_in_Pace_Zone
* P4_Percent_in_Pace_Zone
* P4_Time_in_Pace_Zone
* P5_Percent_in_Pace_Zone
* P5_Time_in_Pace_Zone
* P6_Percent_in_Pace_Zone
* P6_Time_in_Pace_Zone
* P7_Percent_in_Pace_Zone
* P7_Time_in_Pace_Zone
* P8_Percent_in_Pace_Zone
* P8_Time_in_Pace_Zone
* P9_Percent_in_Pace_Zone
* P9_Time_in_Pace_Zone

_W'bal_

* W1_Above_CP_W'bal_Low_Fatigue
* W2_Above_CP_W'bal_Moderate_Fatigue
* W3_Above_CP_W'bal_Heavy_Fatigue
* W4_Above_CP_W'bal_Severe_Fatigue
* W1_W'bal_Low_Fatigue
* W2_W'bal_Moderate_Fatigue
* W3_W'bal_Heavy_Fatigue
* W4_W'bal_Heavy_Fatigue
* W1_W'bal_Work_Low_Fatigue
* W2_W'bal_Work_Moderate_Fatigue
* W3_W'bal_Work_Heavy_Fatigue
* W4_W'bal_Work_Severe_Fatigue

_PEAK DURATION METRICS_

* 1_min_Peak_Pace
* 1_min_Peak_Pace_Swim
* 1_min_Peak_Power
* 1_min_Peak_Power_HR
* 1_min_Peak_WPK
* 1_sec_Peak_Power
* 1_sec_Peak_WPK
* 10_min_Peak_Pace
* 10_min_Peak_Pace_Swim
* 10_min_Peak_Power
* 10_min_Peak_Power_HR
* 10_min_Peak_WPK
* 10_sec_Peak_Pace
* 10_sec_Peak_Pace_Swim
* 10_sec_Peak_Power
* 10_sec_Peak_WPK
* 15_sec_Peak_Pace
* 15_sec_Peak_Pace_Swim
* 15_sec_Peak_Power
* 15_sec_Peak_WPK
* 2_min_Peak_Pace
* 2_min_Peak_Pace_Swim
* 2_min_Peak_Power
* 20_min_Peak_Pace
* 20_min_Peak_Pace_Swim
* 20_min_Peak_Power
* 20_min_Peak_Power_HR
* 20_min_Peak_WPK
* 20_sec_Peak_Pace
* 20_sec_Peak_Pace_Swim
* 20_sec_Peak_Power
* 20_sec_Peak_WPK
* 3_min_Peak_Pace
* 3_min_Peak_Pace_Swim
* 3_min_Peak_Power
* 30_min_Peak_Pace
* 30_min_Peak_Pace_Swim
* 30_min_Peak_Power
* 30_min_Peak_Power_HR
* 30_min_Peak_WPK
* 30_sec_Peak_Pace
* 30_sec_Peak_Pace_Swim
* 30_sec_Peak_Power
* 30_sec_Peak_WPK
* 5_min_Peak_Pace
* 5_min_Peak_Pace_Swim
* 5_min_Peak_Power
* 5_min_Peak_Power_HR
* 5_min_Peak_WPK
* 5_sec_Peak_Power
* 5_sec_Peak_WPK
* 60_min_Peak_Pace
* 60_min_Peak_Pace_Swim
* 60_min_Peak_Power
* 60_min_Peak_Power_HR
* 60_min_Peak_WPK
* 8_min_Peak_Pace
* 8_min_Peak_Pace_Swim
* 8_min_Peak_Power
* 90_min_Peak_Pace
* 90_min_Peak_Pace_Swim
* 90_min_Peak_Power

**OPERATORS**

Operators are the glue to building meaningful expressions
* + - / * ^ arithmetic operators evaluate an expression to a numeric value
* && || logical operators to evaluate an expression to true or false
* < <= > >= <> = comparison evaluates to true or false. Note '=' is used to compare not assign.
* matches contains startsWith endsWith string comparison evaluates to true or false
* x ? a : b evaluates to a if x is non-zero, otherwise b
* x ?: y evaluates to y if x is non-zero otherwise x
