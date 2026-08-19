
# airfoil_self_noise
## 1. Variables
| Variable Name | Role | Type | Units
| -------- | -------- | -------- | -------- |
| `frequency` | Feature |	Integer	| Hz |
| `attack_angle` | Feature | 	Binary | deg |
| `chord_length` | Feature |	Continuous | m |
| `free_stream_velocity` | Feature | Continuous | m/s |
| `suction_side_displacement_thickness` | Feature | Continuous | m | 
| `scaled_sound_pressure` | Target | Continuous | dB | no |

## 2. Additional Variable Information

This problem has the following inputs:
1. Frequency, in Hertzs. 
2. Angle of attack, in degrees. 
3. Chord length, in meters.
4. Free-stream velocity, in meters per second. 
5. Suction side displacement thickness, in meters. 

The only output is:
6. Scaled sound pressure level, in decibels. 


# student_performance
## 1. Variables

| Variable Name | Role | Type | Units |
| -------- | -------- | -------- | -------- |
| `student_id` | Identifier | Categorical / Identifier | None |
| `gender` | Predictor / Factor | Categorical | None |
| `study_time_hours` | Predictor | Continuous | Hours/week |
| `attendance_percent` | Predictor | Continuous | Percentage (%) |
| `sleep_hours` | Predictor | Continuous | Hours/night |
| `parental_education` | Predictor / Factor | Categorical | None |
| `internet_access` | Predictor / Factor | Categorical | Yes/No |
| `extracurricular_activities` | Predictor / Factor | Categorical | Yes/No |
| `part_time_job` | Predictor / Factor | Categorical | Yes/No |
| `previous_grade` | Predictor | Continuous | Score |
| `final_exam_score` | **Response** | Continuous | Score |
| `final_grade` | Derived outcome / Category | Categorical | Grade category |


## 2. Experimental Design Analysis (DRAFT)
Factors -> Response

1. `extracurricular_activities` x `part_time_job` -> `final_exam_score` : Do ex_activity + part_time job affect the final student score?
2. `parental_education` + `interness_access` -> `final_exam_score`: Any interaction between Parent education base and student interness access? 