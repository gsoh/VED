# VED (Vehicle Energy Dataset)
A novel large-scale database for fuel and energy use of diverse vehicles in real-world.

VED captures GPS trajectories of vehicles along with their timeseries data of fuel, energy, speed, and auxiliary power usage, and the data was collected through onboard OBD-II loggers from Nov, 2017 to Nov, 2018.
The fleet consists of total 383 personal cars (264 gasoline vehicles, 92 HEVs, and 27 PHEV/EVs) in Ann Arbor, Michigan, USA. 
Driving scenarios range from highways to traffic-dense downtown area in various driving conditions and seasons. 
In total, VED accumulates approximately 374,000 miles. 

A number of examples were presented in the paper to demonstrate how VED can be utilized for vehicle energy and behavior studies. Potential research opportunities include data-driven vehicle energy consumption modeling, driver behavior modeling, machine and deep learning, calibration of traffic simulators, optimal route choice modeling, prediction of human driver behaviors, and decision making of self-driving cars.

Link to the paper: 
[Vehicle Energy Dataset (VED), A Large-scale Dataset for Vehicle Energy Consumption Research](https://doi.org/10.1109/TITS.2020.3035596), [Arxiv](https://arxiv.org/pdf/1905.02081.pdf)\
**Geunseob (GS) Oh**, David J. LeBlanc, Huei Peng\
IEEE Transactions on Intelligent Transportation Systems (T-ITS), 2020 (In press).


Contact: gsoh@umich.edu.

GS Oh, Ph.D. Candidate, University of Michigan.



## Files
VED consists of Dynamic Data (time-stamped naturalistic driving records of 383 vehicles) and Static Data (Vehicle parameters for the 383 vehicles)

Dynamic Data: "VED_DynamicData.7z" contains a number of "VED_mmddyy_week.csv" files
- Includes a week worth dynamic data, for mmddyy ~ (mmddyy + 7 days)
- Columns represent:
	DayNum,	VehId,	Trip,	Timestamp(ms),	Latitude[deg],	Longitude[deg],	Vehicle Speed[km/h],	MAF[g/sec],	Engine RPM[RPM],	Absolute Load[%],	Outside Air Temperature[DegC],	Fuel Rate[L/hr],	Air Conditioning Power[kW],	Air Conditioning Power[Watts],	Heater Power[Watts],	HV Battery Current[A],	HV Battery SOC[%],	HV Battery Voltage[V],	Short Term Fuel Trim Bank 1[%],	Short Term Fuel Trim Bank 2[%],	Long Term Fuel Trim Bank 1[%],	Long Term Fuel Trim Bank 2[%]
- Notes:
	Each combination of VehID, Trip is unique.
	DayNum represents elapsed days since a reference date. (DayNum 1 = Nov, 1st, 2017, 00:00:00, DayNum 1.5 = Nov, 1st, 2017, 12:00:00)
	For the details, refer to [the VED paper](https://arxiv.org/abs/1905.02081)
	
	
Static Data: "VED_Static_Data_ICE&HEV.xlsx", and "VED_Static_Data_PHEV&EV.xlsx"
- Includes parameters of all 383 vehicles
- Columns represent: 
	VehId,	EngineType,	Vehicle Class,	Engine Configuration & Displacement	Transmission,	Drive Wheels,	Generalized_Weight[lb]



## License

License under the [Apache License 2.0](LICENSE)
